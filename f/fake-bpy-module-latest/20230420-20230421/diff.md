# Comparing `tmp/fake-bpy-module-latest-20230420.tar.gz` & `tmp/fake-bpy-module-latest-20230421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230420.tar", last modified: Thu Apr 20 06:22:18 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230421.tar", last modified: Fri Apr 21 06:21:47 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230420.tar` & `fake-bpy-module-latest-20230421.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-20 06:22:17.000000 fake-bpy-module-latest-20230420/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-20 06:20:13.000000 fake-bpy-module-latest-20230420/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-20 06:22:16.000000 fake-bpy-module-latest-20230420/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 06:22:16.000000 fake-bpy-module-latest-20230420/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-20 06:22:17.000000 fake-bpy-module-latest-20230420/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-20 06:22:14.000000 fake-bpy-module-latest-20230420/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-20 06:22:12.000000 fake-bpy-module-latest-20230420/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-20 06:22:14.000000 fake-bpy-module-latest-20230420/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-20 06:22:16.000000 fake-bpy-module-latest-20230420/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-20 06:22:17.000000 fake-bpy-module-latest-20230420/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-20 06:22:16.000000 fake-bpy-module-latest-20230420/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-20 06:22:14.000000 fake-bpy-module-latest-20230420/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-20 06:22:14.000000 fake-bpy-module-latest-20230420/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-20 06:22:17.000000 fake-bpy-module-latest-20230420/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-20 06:22:14.000000 fake-bpy-module-latest-20230420/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-20 06:22:16.000000 fake-bpy-module-latest-20230420/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-20 06:22:15.000000 fake-bpy-module-latest-20230420/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97820 2023-04-20 06:22:14.000000 fake-bpy-module-latest-20230420/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-20 06:21:29.000000 fake-bpy-module-latest-20230420/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-20 06:20:22.000000 fake-bpy-module-latest-20230420/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-20 06:21:34.000000 fake-bpy-module-latest-20230420/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-20 06:21:57.000000 fake-bpy-module-latest-20230420/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-20 06:21:57.000000 fake-bpy-module-latest-20230420/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-20 06:21:46.000000 fake-bpy-module-latest-20230420/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-20 06:21:24.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-20 06:22:02.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-20 06:21:52.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-20 06:21:55.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-20 06:21:29.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-20 06:20:24.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-20 06:20:24.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-20 06:21:35.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-20 06:21:13.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-20 06:21:55.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-20 06:22:10.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-20 06:20:25.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-20 06:21:52.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-20 06:21:54.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-20 06:21:52.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-20 06:21:51.000000 fake-bpy-module-latest-20230420/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-20 06:21:30.000000 fake-bpy-module-latest-20230420/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-20 06:21:16.000000 fake-bpy-module-latest-20230420/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-20 06:21:58.000000 fake-bpy-module-latest-20230420/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-20 06:21:32.000000 fake-bpy-module-latest-20230420/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-20 06:21:58.000000 fake-bpy-module-latest-20230420/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-20 06:21:32.000000 fake-bpy-module-latest-20230420/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-20 06:20:22.000000 fake-bpy-module-latest-20230420/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-20 06:21:23.000000 fake-bpy-module-latest-20230420/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-20 06:21:57.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-20 06:21:23.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-20 06:20:23.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-20 06:21:55.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-20 06:21:32.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-20 06:22:10.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-20 06:21:51.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-20 06:21:16.000000 fake-bpy-module-latest-20230420/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-20 06:21:13.000000 fake-bpy-module-latest-20230420/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-20 06:21:13.000000 fake-bpy-module-latest-20230420/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-20 06:21:54.000000 fake-bpy-module-latest-20230420/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-20 06:20:22.000000 fake-bpy-module-latest-20230420/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-20 06:20:25.000000 fake-bpy-module-latest-20230420/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-20 06:21:12.000000 fake-bpy-module-latest-20230420/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-20 06:21:51.000000 fake-bpy-module-latest-20230420/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-20 06:21:53.000000 fake-bpy-module-latest-20230420/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-20 06:20:25.000000 fake-bpy-module-latest-20230420/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-20 06:21:57.000000 fake-bpy-module-latest-20230420/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-20 06:21:29.000000 fake-bpy-module-latest-20230420/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-20 06:21:20.000000 fake-bpy-module-latest-20230420/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-20 06:21:52.000000 fake-bpy-module-latest-20230420/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-20 06:21:15.000000 fake-bpy-module-latest-20230420/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-20 06:20:24.000000 fake-bpy-module-latest-20230420/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-20 06:21:35.000000 fake-bpy-module-latest-20230420/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-20 06:21:54.000000 fake-bpy-module-latest-20230420/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-20 06:22:02.000000 fake-bpy-module-latest-20230420/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-20 06:21:15.000000 fake-bpy-module-latest-20230420/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-20 06:20:25.000000 fake-bpy-module-latest-20230420/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-20 06:21:16.000000 fake-bpy-module-latest-20230420/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-20 06:22:03.000000 fake-bpy-module-latest-20230420/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-20 06:21:11.000000 fake-bpy-module-latest-20230420/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-04-20 06:21:16.000000 fake-bpy-module-latest-20230420/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-20 06:21:47.000000 fake-bpy-module-latest-20230420/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-20 06:21:28.000000 fake-bpy-module-latest-20230420/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-20 06:21:11.000000 fake-bpy-module-latest-20230420/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   234684 2023-04-20 06:22:10.000000 fake-bpy-module-latest-20230420/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 06:22:11.000000 fake-bpy-module-latest-20230420/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-20 06:20:13.000000 fake-bpy-module-latest-20230420/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-20 06:19:31.000000 fake-bpy-module-latest-20230420/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-20 06:19:43.000000 fake-bpy-module-latest-20230420/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-20 06:19:52.000000 fake-bpy-module-latest-20230420/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-20 06:19:39.000000 fake-bpy-module-latest-20230420/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-20 06:19:44.000000 fake-bpy-module-latest-20230420/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-20 06:19:52.000000 fake-bpy-module-latest-20230420/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-20 06:19:58.000000 fake-bpy-module-latest-20230420/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-20 06:19:39.000000 fake-bpy-module-latest-20230420/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-20 06:19:36.000000 fake-bpy-module-latest-20230420/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-20 06:19:43.000000 fake-bpy-module-latest-20230420/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-20 06:19:31.000000 fake-bpy-module-latest-20230420/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-20 06:19:36.000000 fake-bpy-module-latest-20230420/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-20 06:19:33.000000 fake-bpy-module-latest-20230420/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-20 06:19:34.000000 fake-bpy-module-latest-20230420/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-20 06:20:05.000000 fake-bpy-module-latest-20230420/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-20 06:19:48.000000 fake-bpy-module-latest-20230420/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-20 06:19:31.000000 fake-bpy-module-latest-20230420/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-20 06:19:59.000000 fake-bpy-module-latest-20230420/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-20 06:20:09.000000 fake-bpy-module-latest-20230420/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-20 06:19:48.000000 fake-bpy-module-latest-20230420/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-20 06:19:48.000000 fake-bpy-module-latest-20230420/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-04-20 06:19:45.000000 fake-bpy-module-latest-20230420/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-20 06:19:48.000000 fake-bpy-module-latest-20230420/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-20 06:19:39.000000 fake-bpy-module-latest-20230420/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   131531 2023-04-20 06:20:07.000000 fake-bpy-module-latest-20230420/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-20 06:19:34.000000 fake-bpy-module-latest-20230420/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-20 06:19:45.000000 fake-bpy-module-latest-20230420/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-20 06:19:33.000000 fake-bpy-module-latest-20230420/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-20 06:19:32.000000 fake-bpy-module-latest-20230420/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-20 06:19:51.000000 fake-bpy-module-latest-20230420/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-20 06:19:51.000000 fake-bpy-module-latest-20230420/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-20 06:19:33.000000 fake-bpy-module-latest-20230420/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-20 06:19:59.000000 fake-bpy-module-latest-20230420/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-20 06:19:34.000000 fake-bpy-module-latest-20230420/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-20 06:19:59.000000 fake-bpy-module-latest-20230420/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-20 06:19:43.000000 fake-bpy-module-latest-20230420/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-20 06:19:34.000000 fake-bpy-module-latest-20230420/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-20 06:19:43.000000 fake-bpy-module-latest-20230420/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-20 06:19:40.000000 fake-bpy-module-latest-20230420/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-20 06:19:49.000000 fake-bpy-module-latest-20230420/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-20 06:20:02.000000 fake-bpy-module-latest-20230420/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-20 06:19:33.000000 fake-bpy-module-latest-20230420/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-20 06:19:50.000000 fake-bpy-module-latest-20230420/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-20 06:20:03.000000 fake-bpy-module-latest-20230420/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-20 06:20:05.000000 fake-bpy-module-latest-20230420/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-20 06:19:40.000000 fake-bpy-module-latest-20230420/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-20 06:19:44.000000 fake-bpy-module-latest-20230420/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-20 06:19:32.000000 fake-bpy-module-latest-20230420/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-20 06:19:32.000000 fake-bpy-module-latest-20230420/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-20 06:19:34.000000 fake-bpy-module-latest-20230420/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-20 06:19:36.000000 fake-bpy-module-latest-20230420/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-20 06:19:46.000000 fake-bpy-module-latest-20230420/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-20 06:19:32.000000 fake-bpy-module-latest-20230420/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-20 06:19:44.000000 fake-bpy-module-latest-20230420/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-20 06:19:47.000000 fake-bpy-module-latest-20230420/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-20 06:19:35.000000 fake-bpy-module-latest-20230420/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-20 06:20:07.000000 fake-bpy-module-latest-20230420/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-20 06:19:52.000000 fake-bpy-module-latest-20230420/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-20 06:20:03.000000 fake-bpy-module-latest-20230420/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-20 06:19:43.000000 fake-bpy-module-latest-20230420/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-20 06:19:31.000000 fake-bpy-module-latest-20230420/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    56151 2023-04-20 06:20:04.000000 fake-bpy-module-latest-20230420/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-20 06:19:35.000000 fake-bpy-module-latest-20230420/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-20 06:19:51.000000 fake-bpy-module-latest-20230420/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   245978 2023-04-20 06:19:58.000000 fake-bpy-module-latest-20230420/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-20 06:19:44.000000 fake-bpy-module-latest-20230420/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-20 06:19:48.000000 fake-bpy-module-latest-20230420/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3485780 2023-04-20 06:19:31.000000 fake-bpy-module-latest-20230420/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 06:20:11.000000 fake-bpy-module-latest-20230420/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 06:22:17.000000 fake-bpy-module-latest-20230420/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-20 06:20:20.000000 fake-bpy-module-latest-20230420/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-20 06:20:15.000000 fake-bpy-module-latest-20230420/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-20 06:20:15.000000 fake-bpy-module-latest-20230420/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-20 06:20:15.000000 fake-bpy-module-latest-20230420/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-20 06:20:15.000000 fake-bpy-module-latest-20230420/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-20 06:20:16.000000 fake-bpy-module-latest-20230420/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-20 06:20:15.000000 fake-bpy-module-latest-20230420/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-20 06:20:15.000000 fake-bpy-module-latest-20230420/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-20 06:20:14.000000 fake-bpy-module-latest-20230420/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:12:59.000000 fake-bpy-module-latest-20230420/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 06:20:19.000000 fake-bpy-module-latest-20230420/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:22:18.000000 fake-bpy-module-latest-20230420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-20 06:22:17.000000 fake-bpy-module-latest-20230420/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 06:20:21.000000 fake-bpy-module-latest-20230420/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-21 06:19:53.000000 fake-bpy-module-latest-20230421/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-21 06:19:50.000000 fake-bpy-module-latest-20230421/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-21 06:21:42.000000 fake-bpy-module-latest-20230421/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-21 06:21:42.000000 fake-bpy-module-latest-20230421/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-21 06:21:44.000000 fake-bpy-module-latest-20230421/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-21 06:21:44.000000 fake-bpy-module-latest-20230421/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-21 06:21:42.000000 fake-bpy-module-latest-20230421/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-21 06:21:42.000000 fake-bpy-module-latest-20230421/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-21 06:21:41.000000 fake-bpy-module-latest-20230421/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-21 06:21:44.000000 fake-bpy-module-latest-20230421/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-21 06:21:42.000000 fake-bpy-module-latest-20230421/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-21 06:21:43.000000 fake-bpy-module-latest-20230421/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-21 06:21:43.000000 fake-bpy-module-latest-20230421/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-21 06:21:44.000000 fake-bpy-module-latest-20230421/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-21 06:21:43.000000 fake-bpy-module-latest-20230421/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-21 06:21:41.000000 fake-bpy-module-latest-20230421/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-21 06:21:45.000000 fake-bpy-module-latest-20230421/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-21 06:21:43.000000 fake-bpy-module-latest-20230421/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-21 06:21:41.000000 fake-bpy-module-latest-20230421/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97820 2023-04-21 06:21:44.000000 fake-bpy-module-latest-20230421/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-21 06:19:56.000000 fake-bpy-module-latest-20230421/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-21 06:20:09.000000 fake-bpy-module-latest-20230421/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 06:20:17.000000 fake-bpy-module-latest-20230421/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-21 06:19:58.000000 fake-bpy-module-latest-20230421/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-21 06:20:33.000000 fake-bpy-module-latest-20230421/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-21 06:20:08.000000 fake-bpy-module-latest-20230421/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-21 06:20:49.000000 fake-bpy-module-latest-20230421/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-21 06:19:58.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-21 06:20:26.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-21 06:20:06.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-21 06:19:59.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-21 06:19:59.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-21 06:20:31.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-21 06:20:16.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-21 06:20:12.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-21 06:20:08.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-21 06:20:07.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-21 06:20:08.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-21 06:20:12.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-21 06:20:06.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-21 06:20:18.000000 fake-bpy-module-latest-20230421/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-21 06:20:49.000000 fake-bpy-module-latest-20230421/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-21 06:20:08.000000 fake-bpy-module-latest-20230421/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-21 06:20:05.000000 fake-bpy-module-latest-20230421/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-21 06:20:06.000000 fake-bpy-module-latest-20230421/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-21 06:20:09.000000 fake-bpy-module-latest-20230421/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-21 06:20:07.000000 fake-bpy-module-latest-20230421/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-21 06:20:09.000000 fake-bpy-module-latest-20230421/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-21 06:20:16.000000 fake-bpy-module-latest-20230421/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-21 06:20:53.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-21 06:20:30.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-21 06:20:12.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-21 06:20:25.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-21 06:20:11.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-21 06:20:09.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-21 06:20:37.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-21 06:20:38.000000 fake-bpy-module-latest-20230421/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-21 06:20:51.000000 fake-bpy-module-latest-20230421/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-21 06:20:32.000000 fake-bpy-module-latest-20230421/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-21 06:20:31.000000 fake-bpy-module-latest-20230421/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-21 06:20:32.000000 fake-bpy-module-latest-20230421/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-21 06:20:26.000000 fake-bpy-module-latest-20230421/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-21 06:20:52.000000 fake-bpy-module-latest-20230421/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-21 06:20:05.000000 fake-bpy-module-latest-20230421/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-21 06:20:53.000000 fake-bpy-module-latest-20230421/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-21 06:20:17.000000 fake-bpy-module-latest-20230421/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-21 06:20:18.000000 fake-bpy-module-latest-20230421/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-21 06:20:37.000000 fake-bpy-module-latest-20230421/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-21 06:20:38.000000 fake-bpy-module-latest-20230421/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-21 06:20:37.000000 fake-bpy-module-latest-20230421/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-21 06:20:02.000000 fake-bpy-module-latest-20230421/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-21 06:20:08.000000 fake-bpy-module-latest-20230421/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-21 06:20:18.000000 fake-bpy-module-latest-20230421/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-21 06:21:40.000000 fake-bpy-module-latest-20230421/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-21 06:20:30.000000 fake-bpy-module-latest-20230421/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-21 06:20:13.000000 fake-bpy-module-latest-20230421/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-21 06:20:08.000000 fake-bpy-module-latest-20230421/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-21 06:19:59.000000 fake-bpy-module-latest-20230421/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-04-21 06:20:33.000000 fake-bpy-module-latest-20230421/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-21 06:20:52.000000 fake-bpy-module-latest-20230421/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-21 06:20:30.000000 fake-bpy-module-latest-20230421/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-21 06:21:36.000000 fake-bpy-module-latest-20230421/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-04-21 06:20:25.000000 fake-bpy-module-latest-20230421/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 06:20:00.000000 fake-bpy-module-latest-20230421/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-21 06:19:50.000000 fake-bpy-module-latest-20230421/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-21 06:19:53.000000 fake-bpy-module-latest-20230421/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-21 06:19:53.000000 fake-bpy-module-latest-20230421/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-21 06:19:53.000000 fake-bpy-module-latest-20230421/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-21 06:19:10.000000 fake-bpy-module-latest-20230421/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-21 06:19:21.000000 fake-bpy-module-latest-20230421/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-21 06:19:13.000000 fake-bpy-module-latest-20230421/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-21 06:19:37.000000 fake-bpy-module-latest-20230421/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-21 06:19:21.000000 fake-bpy-module-latest-20230421/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-21 06:19:34.000000 fake-bpy-module-latest-20230421/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-21 06:19:39.000000 fake-bpy-module-latest-20230421/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-21 06:19:28.000000 fake-bpy-module-latest-20230421/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-21 06:19:45.000000 fake-bpy-module-latest-20230421/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-21 06:19:22.000000 fake-bpy-module-latest-20230421/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-21 06:19:35.000000 fake-bpy-module-latest-20230421/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-21 06:19:40.000000 fake-bpy-module-latest-20230421/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-21 06:19:23.000000 fake-bpy-module-latest-20230421/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-21 06:19:34.000000 fake-bpy-module-latest-20230421/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-21 06:19:38.000000 fake-bpy-module-latest-20230421/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-21 06:19:28.000000 fake-bpy-module-latest-20230421/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-21 06:19:40.000000 fake-bpy-module-latest-20230421/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-21 06:19:37.000000 fake-bpy-module-latest-20230421/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-21 06:19:14.000000 fake-bpy-module-latest-20230421/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-04-21 06:19:41.000000 fake-bpy-module-latest-20230421/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-21 06:19:13.000000 fake-bpy-module-latest-20230421/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-21 06:19:13.000000 fake-bpy-module-latest-20230421/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-04-21 06:19:20.000000 fake-bpy-module-latest-20230421/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-21 06:19:38.000000 fake-bpy-module-latest-20230421/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-21 06:19:14.000000 fake-bpy-module-latest-20230421/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-21 06:19:45.000000 fake-bpy-module-latest-20230421/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-21 06:19:21.000000 fake-bpy-module-latest-20230421/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-21 06:19:14.000000 fake-bpy-module-latest-20230421/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-21 06:19:45.000000 fake-bpy-module-latest-20230421/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-21 06:19:35.000000 fake-bpy-module-latest-20230421/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-21 06:19:39.000000 fake-bpy-module-latest-20230421/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-21 06:19:43.000000 fake-bpy-module-latest-20230421/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-21 06:19:15.000000 fake-bpy-module-latest-20230421/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-21 06:19:13.000000 fake-bpy-module-latest-20230421/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-21 06:19:44.000000 fake-bpy-module-latest-20230421/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-21 06:19:36.000000 fake-bpy-module-latest-20230421/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-21 06:19:13.000000 fake-bpy-module-latest-20230421/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-21 06:19:13.000000 fake-bpy-module-latest-20230421/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-21 06:19:35.000000 fake-bpy-module-latest-20230421/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-21 06:19:45.000000 fake-bpy-module-latest-20230421/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-21 06:19:34.000000 fake-bpy-module-latest-20230421/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-21 06:19:22.000000 fake-bpy-module-latest-20230421/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-21 06:19:10.000000 fake-bpy-module-latest-20230421/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-21 06:19:25.000000 fake-bpy-module-latest-20230421/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-21 06:19:44.000000 fake-bpy-module-latest-20230421/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-21 06:19:21.000000 fake-bpy-module-latest-20230421/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-21 06:19:46.000000 fake-bpy-module-latest-20230421/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-21 06:19:21.000000 fake-bpy-module-latest-20230421/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-21 06:19:27.000000 fake-bpy-module-latest-20230421/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-21 06:19:23.000000 fake-bpy-module-latest-20230421/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-21 06:19:22.000000 fake-bpy-module-latest-20230421/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-21 06:19:37.000000 fake-bpy-module-latest-20230421/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-21 06:19:34.000000 fake-bpy-module-latest-20230421/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-21 06:19:34.000000 fake-bpy-module-latest-20230421/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-21 06:19:25.000000 fake-bpy-module-latest-20230421/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-21 06:19:38.000000 fake-bpy-module-latest-20230421/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56151 2023-04-21 06:19:24.000000 fake-bpy-module-latest-20230421/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-21 06:19:18.000000 fake-bpy-module-latest-20230421/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-21 06:19:28.000000 fake-bpy-module-latest-20230421/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245978 2023-04-21 06:19:34.000000 fake-bpy-module-latest-20230421/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-21 06:19:35.000000 fake-bpy-module-latest-20230421/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-21 06:19:37.000000 fake-bpy-module-latest-20230421/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-21 06:19:48.000000 fake-bpy-module-latest-20230421/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3485908 2023-04-21 06:19:10.000000 fake-bpy-module-latest-20230421/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-21 06:19:47.000000 fake-bpy-module-latest-20230421/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-21 06:19:56.000000 fake-bpy-module-latest-20230421/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-21 06:19:52.000000 fake-bpy-module-latest-20230421/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-21 06:19:51.000000 fake-bpy-module-latest-20230421/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:12:57.000000 fake-bpy-module-latest-20230421/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 06:21:46.000000 fake-bpy-module-latest-20230421/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-21 06:21:47.000000 fake-bpy-module-latest-20230421/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 06:19:55.000000 fake-bpy-module-latest-20230421/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230420/PKG-INFO` & `fake-bpy-module-latest-20230421/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230420
+Version: 20230421
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230420/README.rst` & `fake-bpy-module-latest-20230421/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/addon_utils.py` & `fake-bpy-module-latest-20230421/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/animsys_refactor.py` & `fake-bpy-module-latest-20230421/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/aud.py` & `fake-bpy-module-latest-20230421/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bgl.py` & `fake-bpy-module-latest-20230421/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230421/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230421/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230421/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230421/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230421/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_math.py` & `fake-bpy-module-latest-20230421/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/__init__.py` & `fake-bpy-module-latest-20230421/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
 import typing
-from . import image
-from . import presets
+from . import uvcalc_lightmap
 from . import uvcalc_transform
-from . import console
-from . import wm
-from . import spreadsheet
-from . import freestyle
-from . import clip
+from . import sequencer
 from . import object_quick_effects
-from . import rigidbody
-from . import userpref
-from . import file
-from . import assets
 from . import view3d
-from . import geometry_nodes
-from . import object_align
-from . import anim
-from . import screen_play_rendered_anim
+from . import freestyle
+from . import presets
 from . import vertexpaint_dirt
 from . import constraint
+from . import clip
+from . import console
+from . import geometry_nodes
+from . import assets
+from . import anim
+from . import object
 from . import object_randomize_transform
 from . import uvcalc_follow_active
-from . import object
-from . import uvcalc_lightmap
+from . import node
+from . import wm
+from . import file
+from . import object_align
+from . import bmesh
 from . import mesh
+from . import screen_play_rendered_anim
+from . import rigidbody
+from . import image
+from . import userpref
 from . import add_mesh_torus
-from . import bmesh
-from . import sequencer
-from . import node
+from . import spreadsheet
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230420/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230421/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/anim.py` & `fake-bpy-module-latest-20230421/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/assets.py` & `fake-bpy-module-latest-20230421/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230421/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/clip.py` & `fake-bpy-module-latest-20230421/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/console.py` & `fake-bpy-module-latest-20230421/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/constraint.py` & `fake-bpy-module-latest-20230421/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/file.py` & `fake-bpy-module-latest-20230421/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230421/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230421/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/image.py` & `fake-bpy-module-latest-20230421/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/mesh.py` & `fake-bpy-module-latest-20230421/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/node.py` & `fake-bpy-module-latest-20230421/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/object.py` & `fake-bpy-module-latest-20230421/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/object_align.py` & `fake-bpy-module-latest-20230421/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230421/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230421/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/presets.py` & `fake-bpy-module-latest-20230421/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230421/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230421/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230421/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230421/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/userpref.py` & `fake-bpy-module-latest-20230421/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230421/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230421/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230421/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230421/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/view3d.py` & `fake-bpy-module-latest-20230421/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_operators/wm.py` & `fake-bpy-module-latest-20230421/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230421/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/__init__.py` & `fake-bpy-module-latest-20230421/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_grease_pencil_common
-from . import properties_view_layer
-from . import properties_paint_common
-from . import node_add_menu
-from . import properties_physics_dynamicpaint
-from . import space_node
+from . import node_add_menu_geometry
+from . import properties_data_armature
 from . import properties_data_gpencil
-from . import properties_data_lattice
-from . import properties_data_modifier
-from . import properties_workspace
-from . import space_statusbar
-from . import space_dopesheet
-from . import space_view3d
 from . import space_toolsystem_common
-from . import properties_world
-from . import properties_render
-from . import properties_scene
-from . import properties_data_lightprobe
-from . import space_nla
-from . import space_spreadsheet
-from . import properties_physics_softbody
-from . import space_text
-from . import properties_mask_common
-from . import space_toolsystem_toolbar
-from . import space_image
-from . import properties_particle
-from . import properties_physics_common
-from . import properties_data_bone
-from . import space_userpref
-from . import space_graph
-from . import generic_ui_list
 from . import properties_data_empty
-from . import properties_freestyle
-from . import properties_physics_fluid
+from . import space_dopesheet
+from . import utils
+from . import space_statusbar
+from . import properties_object
+from . import properties_data_bone
+from . import properties_data_curves
+from . import properties_data_lattice
+from . import space_node
+from . import space_clip
+from . import properties_mask_common
+from . import properties_data_curve
+from . import properties_material
+from . import properties_data_speaker
 from . import properties_output
-from . import properties_material_gpencil
-from . import node_add_menu_geometry
+from . import properties_data_modifier
 from . import space_outliner
-from . import properties_data_light
-from . import properties_constraint
-from . import space_topbar
-from . import space_clip
-from . import properties_data_volume
-from . import properties_physics_rigidbody_constraint
-from . import space_info
+from . import properties_collection
+from . import properties_data_metaball
+from . import space_time
 from . import properties_data_pointcloud
-from . import properties_data_speaker
-from . import properties_data_curve
-from . import space_console
-from . import properties_texture
+from . import properties_grease_pencil_common
+from . import properties_material_gpencil
+from . import properties_paint_common
+from . import generic_ui_list
+from . import properties_physics_rigidbody
+from . import properties_physics_fluid
+from . import properties_physics_dynamicpaint
 from . import properties_data_shaderfx
-from . import space_properties
 from . import properties_data_mesh
-from . import properties_data_curves
-from . import properties_physics_field
+from . import space_text
+from . import properties_particle
+from . import properties_data_lightprobe
 from . import space_filebrowser
-from . import properties_physics_cloth
+from . import node_add_menu
+from . import space_graph
+from . import properties_data_volume
+from . import space_properties
+from . import space_view3d_toolbar
+from . import properties_physics_field
+from . import properties_data_camera
+from . import properties_workspace
+from . import space_userpref
+from . import properties_physics_common
+from . import space_spreadsheet
+from . import properties_data_light
+from . import properties_texture
+from . import properties_view_layer
+from . import properties_scene
+from . import space_toolsystem_toolbar
 from . import properties_animviz
-from . import properties_collection
-from . import properties_material
-from . import properties_object
+from . import space_image
+from . import space_nla
+from . import properties_physics_rigidbody_constraint
+from . import properties_physics_softbody
+from . import space_info
+from . import properties_constraint
+from . import properties_freestyle
+from . import properties_render
+from . import space_topbar
+from . import properties_world
+from . import properties_physics_cloth
+from . import space_console
+from . import space_view3d
 from . import space_sequencer
-from . import properties_data_camera
-from . import space_time
-from . import space_view3d_toolbar
-from . import properties_physics_rigidbody
-from . import properties_data_metaball
-from . import utils
-from . import properties_data_armature
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230420/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230421/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230421/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230421/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230421/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_console.py` & `fake-bpy-module-latest-20230421/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230421/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230421/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230421/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_image.py` & `fake-bpy-module-latest-20230421/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_info.py` & `fake-bpy-module-latest-20230421/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230421/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_node.py` & `fake-bpy-module-latest-20230421/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230421/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230421/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230421/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230421/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230421/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_text.py` & `fake-bpy-module-latest-20230421/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_time.py` & `fake-bpy-module-latest-20230421/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230421/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230421/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230421/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230421/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230421/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230421/bl_ui/space_view3d_toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -7771,14 +7771,222 @@
     def values(self):
         ''' 
 
         '''
         pass
 
 
+class VIEW3D_PT_tools_grease_pencil_weight_options(
+        View3DPanel, GreasePencilWeightPanel, bpy_types.Panel,
+        bpy_types._GenericUI):
+    bl_category = None
+    ''' '''
+
+    bl_context = None
+    ''' '''
+
+    bl_label = None
+    ''' '''
+
+    bl_options = None
+    ''' '''
+
+    bl_region_type = None
+    ''' '''
+
+    bl_rna = None
+    ''' '''
+
+    bl_space_type = None
+    ''' '''
+
+    id_data = None
+    ''' '''
+
+    def append(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def as_pointer(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass_py(self):
+        ''' 
+
+        '''
+        pass
+
+    def draw(self, context):
+        ''' 
+
+        '''
+        pass
+
+    def driver_add(self):
+        ''' 
+
+        '''
+        pass
+
+    def driver_remove(self):
+        ''' 
+
+        '''
+        pass
+
+    def get(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_clear(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ensure(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ui(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_extended(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_hidden(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_overridable_library(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_readonly(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def items(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_delete(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_insert(self):
+        ''' 
+
+        '''
+        pass
+
+    def keys(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_from_id(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_resolve(self):
+        ''' 
+
+        '''
+        pass
+
+    def poll(self, context):
+        ''' 
+
+        '''
+        pass
+
+    def pop(self):
+        ''' 
+
+        '''
+        pass
+
+    def prepend(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def property_overridable_library_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def property_unset(self):
+        ''' 
+
+        '''
+        pass
+
+    def remove(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def type_recast(self):
+        ''' 
+
+        '''
+        pass
+
+    def values(self):
+        ''' 
+
+        '''
+        pass
+
+
 class VIEW3D_PT_tools_grease_pencil_weight_paint_select(
         View3DPanel, GreasePencilWeightPanel, bpy_types.Panel,
         bpy_types._GenericUI):
     bl_category = None
     ''' '''
 
     bl_context = None
@@ -14329,14 +14537,17 @@
 
     bl_label = None
     ''' '''
 
     bl_options = None
     ''' '''
 
+    bl_parent_id = None
+    ''' '''
+
     bl_region_type = None
     ''' '''
 
     bl_rna = None
     ''' '''
 
     bl_space_type = None
```

### Comparing `fake-bpy-module-latest-20230420/bl_ui/utils.py` & `fake-bpy-module-latest-20230421/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/blf.py` & `fake-bpy-module-latest-20230421/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bmesh/__init__.py` & `fake-bpy-module-latest-20230421/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bmesh/geometry.py` & `fake-bpy-module-latest-20230421/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bmesh/ops.py` & `fake-bpy-module-latest-20230421/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bmesh/types.py` & `fake-bpy-module-latest-20230421/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bmesh/utils.py` & `fake-bpy-module-latest-20230421/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/app/__init__.py` & `fake-bpy-module-latest-20230421/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import typing
+from . import handlers
 from . import icons
 from . import translations
-from . import handlers
 from . import timers
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def is_job_running(job_type: typing.Optional[str]) -> typing.Any:
     ''' Check whether a job of the given type is running.
```

### Comparing `fake-bpy-module-latest-20230420/bpy/app/handlers.py` & `fake-bpy-module-latest-20230421/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/app/icons.py` & `fake-bpy-module-latest-20230421/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/app/timers.py` & `fake-bpy-module-latest-20230421/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/app/translations.py` & `fake-bpy-module-latest-20230421/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/msgbus.py` & `fake-bpy-module-latest-20230421/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230421/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import sys
 import typing
+from . import render
+from . import object
+from . import anim
+from . import paintcurve
+from . import gizmogroup
+from . import palette
+from . import geometry
+from . import image
+from . import fluid
+from . import info
+from . import nla
+from . import node
 from . import uilist
-from . import export_anim
-from . import console
-from . import sculpt
-from . import preferences
+from . import material
 from . import import_curve
-from . import ptcache
-from . import curve
-from . import info
-from . import import_anim
-from . import outliner
-from . import graph
-from . import mball
-from . import rigidbody
-from . import marker
-from . import curves
 from . import view2d
-from . import sound
-from . import clip
-from . import scene
+from . import curves
 from . import constraint
-from . import armature
-from . import gizmogroup
-from . import camera
-from . import pose
-from . import nla
-from . import mesh
+from . import poselib
+from . import cycles
+from . import gpencil
 from . import action
-from . import collection
-from . import material
-from . import texture
+from . import script
 from . import boid
 from . import sculpt_curves
-from . import poselib
-from . import workspace
-from . import image
-from . import font
-from . import screen
-from . import sequencer
-from . import file
-from . import ed
-from . import fluid
-from . import world
-from . import geometry
-from . import node
-from . import paint
 from . import import_scene
+from . import clip
+from . import spreadsheet
+from . import ptcache
+from . import sound
+from . import console
+from . import uv
+from . import transform
+from . import rigidbody
+from . import sequencer
 from . import view3d
-from . import import_mesh
-from . import buttons
-from . import surface
-from . import anim
-from . import wm
 from . import cachefile
-from . import mask
 from . import export_mesh
-from . import lattice
-from . import object
+from . import wm
+from . import brush
+from . import texture
 from . import text
-from . import palette
-from . import uv
-from . import paintcurve
-from . import ui
-from . import asset
-from . import script
-from . import render
 from . import dpaint
-from . import brush
-from . import cloth
+from . import preferences
 from . import particle
-from . import cycles
-from . import gpencil
-from . import spreadsheet
+from . import cloth
+from . import mask
+from . import workspace
+from . import paint
+from . import armature
+from . import surface
+from . import file
+from . import world
+from . import graph
+from . import ui
+from . import ed
+from . import mball
+from . import buttons
 from . import export_scene
-from . import transform
+from . import collection
+from . import font
+from . import mesh
+from . import screen
+from . import outliner
+from . import pose
+from . import camera
+from . import marker
+from . import import_anim
+from . import sculpt
+from . import curve
+from . import scene
+from . import lattice
+from . import asset
+from . import export_anim
+from . import import_mesh
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/action.py` & `fake-bpy-module-latest-20230421/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/anim.py` & `fake-bpy-module-latest-20230421/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/armature.py` & `fake-bpy-module-latest-20230421/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/asset.py` & `fake-bpy-module-latest-20230421/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/boid.py` & `fake-bpy-module-latest-20230421/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/brush.py` & `fake-bpy-module-latest-20230421/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230421/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230421/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/camera.py` & `fake-bpy-module-latest-20230421/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/clip.py` & `fake-bpy-module-latest-20230421/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230421/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/collection.py` & `fake-bpy-module-latest-20230421/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/console.py` & `fake-bpy-module-latest-20230421/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230421/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/curve.py` & `fake-bpy-module-latest-20230421/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/curves.py` & `fake-bpy-module-latest-20230421/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230421/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230421/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/ed.py` & `fake-bpy-module-latest-20230421/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230421/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230421/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230421/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/file.py` & `fake-bpy-module-latest-20230421/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230421/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/font.py` & `fake-bpy-module-latest-20230421/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230421/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230421/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230421/bpy/ops/gpencil.py`

 * *Files 0% similar despite different names*

```diff
@@ -3014,28 +3014,56 @@
                  Union[typing.Dict, 'bpy.types.Context'] = None,
                  execution_context: typing.Union[str, int] = None,
                  undo: typing.Optional[bool] = None,
                  *,
                  stroke: typing.Optional[bpy.types.bpy_prop_collection[
                      'bpy.types.OperatorStrokeElement']] = None,
                  wait_for_input: typing.Union[bool, typing.Any] = True):
-    ''' Paint stroke points with a color
+    ''' Draw weight on stroke points
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param stroke: Stroke
     :type stroke: typing.Optional[bpy.types.bpy_prop_collection['bpy.types.OperatorStrokeElement']]
     :param wait_for_input: Wait for Input
     :type wait_for_input: typing.Union[bool, typing.Any]
     '''
 
     pass
 
 
+def weight_sample(override_context: typing.
+                  Union[typing.Dict, 'bpy.types.Context'] = None,
+                  execution_context: typing.Union[str, int] = None,
+                  undo: typing.Optional[bool] = None):
+    ''' Use the mouse to sample a weight in the 3D view
+
+    :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
+    :type execution_context: typing.Union[str, int]
+    :type undo: typing.Optional[bool]
+    '''
+
+    pass
+
+
+def weight_toggle_direction(override_context: typing.
+                            Union[typing.Dict, 'bpy.types.Context'] = None,
+                            execution_context: typing.Union[str, int] = None,
+                            undo: typing.Optional[bool] = None):
+    ''' Toggle Add/Subtract for the weight paint draw tool
+
+    :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
+    :type execution_context: typing.Union[str, int]
+    :type undo: typing.Optional[bool]
+    '''
+
+    pass
+
+
 def weightmode_toggle(override_context: typing.
                       Union[typing.Dict, 'bpy.types.Context'] = None,
                       execution_context: typing.Union[str, int] = None,
                       undo: typing.Optional[bool] = None,
                       *,
                       back: typing.Union[bool, typing.Any] = False):
     ''' Enter/Exit weight paint mode for Grease Pencil strokes
```

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/graph.py` & `fake-bpy-module-latest-20230421/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/image.py` & `fake-bpy-module-latest-20230421/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230421/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230421/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230421/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230421/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/info.py` & `fake-bpy-module-latest-20230421/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230421/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/marker.py` & `fake-bpy-module-latest-20230421/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/mask.py` & `fake-bpy-module-latest-20230421/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/material.py` & `fake-bpy-module-latest-20230421/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/mball.py` & `fake-bpy-module-latest-20230421/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230421/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/nla.py` & `fake-bpy-module-latest-20230421/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/node.py` & `fake-bpy-module-latest-20230421/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/object.py` & `fake-bpy-module-latest-20230421/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230421/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/paint.py` & `fake-bpy-module-latest-20230421/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230421/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/palette.py` & `fake-bpy-module-latest-20230421/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/particle.py` & `fake-bpy-module-latest-20230421/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/pose.py` & `fake-bpy-module-latest-20230421/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230421/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230421/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230421/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/render.py` & `fake-bpy-module-latest-20230421/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230421/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/scene.py` & `fake-bpy-module-latest-20230421/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/screen.py` & `fake-bpy-module-latest-20230421/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/script.py` & `fake-bpy-module-latest-20230421/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230421/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230421/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230421/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/sound.py` & `fake-bpy-module-latest-20230421/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230421/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/surface.py` & `fake-bpy-module-latest-20230421/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/text.py` & `fake-bpy-module-latest-20230421/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/texture.py` & `fake-bpy-module-latest-20230421/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/transform.py` & `fake-bpy-module-latest-20230421/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/ui.py` & `fake-bpy-module-latest-20230421/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230421/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/uv.py` & `fake-bpy-module-latest-20230421/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230421/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230421/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/wm.py` & `fake-bpy-module-latest-20230421/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230421/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/ops/world.py` & `fake-bpy-module-latest-20230421/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/path.py` & `fake-bpy-module-latest-20230421/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/props.py` & `fake-bpy-module-latest-20230421/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/types.py` & `fake-bpy-module-latest-20230421/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,173 +1,173 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7072 6f70 6572 7469 6573 5f67 7265  i.properties_gre
-00000050: 6173 655f 7065 6e63 696c 5f63 6f6d 6d6f  ase_pencil_commo
-00000060: 6e0a 696d 706f 7274 2062 6c5f 7569 2e70  n.import bl_ui.p
-00000070: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
-00000080: 6179 6572 0a69 6d70 6f72 7420 626c 5f75  ayer.import bl_u
-00000090: 692e 7072 6f70 6572 7469 6573 5f70 6169  i.properties_pai
-000000a0: 6e74 5f63 6f6d 6d6f 6e0a 696d 706f 7274  nt_common.import
-000000b0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000000c0: 735f 7068 7973 6963 735f 6479 6e61 6d69  s_physics_dynami
-000000d0: 6370 6169 6e74 0a69 6d70 6f72 7420 626c  cpaint.import bl
-000000e0: 5f75 692e 7370 6163 655f 6e6f 6465 0a69  _ui.space_node.i
-000000f0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000100: 6572 7469 6573 5f64 6174 615f 6770 656e  erties_data_gpen
-00000110: 6369 6c0a 696d 706f 7274 2062 6c5f 7569  cil.import bl_ui
-00000120: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-00000130: 5f6c 6174 7469 6365 0a69 6d70 6f72 7420  _lattice.import 
-00000140: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000150: 5f64 6174 615f 6d6f 6469 6669 6572 0a69  _data_modifier.i
-00000160: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000170: 6572 7469 6573 5f77 6f72 6b73 7061 6365  erties_workspace
-00000180: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000190: 746f 7273 2e70 7265 7365 7473 0a69 6d70  tors.presets.imp
-000001a0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-000001b0: 7374 6174 7573 6261 720a 696d 706f 7274  statusbar.import
-000001c0: 2062 6c5f 6f70 6572 6174 6f72 732e 776d   bl_operators.wm
-000001d0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000001e0: 746f 7273 2e73 7072 6561 6473 6865 6574  tors.spreadsheet
-000001f0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000200: 6163 655f 646f 7065 7368 6565 740a 696d  ace_dopesheet.im
-00000210: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
-00000220: 732e 6672 6565 7374 796c 650a 696d 706f  s.freestyle.impo
-00000230: 7274 2062 6c5f 7569 2e73 7061 6365 5f76  rt bl_ui.space_v
-00000240: 6965 7733 640a 696d 706f 7274 2062 6c5f  iew3d.import bl_
-00000250: 7569 2e73 7061 6365 5f74 6f6f 6c73 7973  ui.space_toolsys
-00000260: 7465 6d5f 636f 6d6d 6f6e 0a69 6d70 6f72  tem_common.impor
-00000270: 7420 626c 5f6f 7065 7261 746f 7273 2e63  t bl_operators.c
-00000280: 6c69 700a 696d 706f 7274 2062 6c5f 7569  lip.import bl_ui
-00000290: 2e70 726f 7065 7274 6965 735f 776f 726c  .properties_worl
-000002a0: 640a 696d 706f 7274 2062 6c5f 7569 2e70  d.import bl_ui.p
-000002b0: 726f 7065 7274 6965 735f 7265 6e64 6572  roperties_render
-000002c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000002d0: 6f70 6572 7469 6573 5f73 6365 6e65 0a69  operties_scene.i
-000002e0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000002f0: 6572 7469 6573 5f64 6174 615f 6c69 6768  erties_data_ligh
-00000300: 7470 726f 6265 0a69 6d70 6f72 7420 626c  tprobe.import bl
-00000310: 5f75 692e 7370 6163 655f 6e6c 610a 696d  _ui.space_nla.im
-00000320: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000330: 5f73 7072 6561 6473 6865 6574 0a69 6d70  _spreadsheet.imp
-00000340: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000350: 7469 6573 5f70 6879 7369 6373 5f73 6f66  ties_physics_sof
-00000360: 7462 6f64 790a 696d 706f 7274 2062 6c5f  tbody.import bl_
-00000370: 7569 2e73 7061 6365 5f74 6578 740a 696d  ui.space_text.im
-00000380: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000390: 7274 6965 735f 6d61 736b 5f63 6f6d 6d6f  rties_mask_commo
-000003a0: 6e0a 696d 706f 7274 2062 6c5f 7569 2e73  n.import bl_ui.s
-000003b0: 7061 6365 5f74 6f6f 6c73 7973 7465 6d5f  pace_toolsystem_
-000003c0: 746f 6f6c 6261 720a 696d 706f 7274 2062  toolbar.import b
-000003d0: 6c5f 7569 2e73 7061 6365 5f69 6d61 6765  l_ui.space_image
-000003e0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000003f0: 6f70 6572 7469 6573 5f70 6172 7469 636c  operties_particl
-00000400: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
-00000410: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
-00000420: 735f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  s_common.import 
-00000430: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000440: 5f64 6174 615f 626f 6e65 0a69 6d70 6f72  _data_bone.impor
-00000450: 7420 626c 5f6f 7065 7261 746f 7273 2e75  t bl_operators.u
-00000460: 7365 7270 7265 660a 696d 706f 7274 2062  serpref.import b
-00000470: 6c5f 7569 2e73 7061 6365 5f75 7365 7270  l_ui.space_userp
-00000480: 7265 660a 696d 706f 7274 2062 6c5f 7569  ref.import bl_ui
-00000490: 2e73 7061 6365 5f67 7261 7068 0a69 6d70  .space_graph.imp
-000004a0: 6f72 7420 626c 5f75 690a 696d 706f 7274  ort bl_ui.import
-000004b0: 2062 6c5f 7569 2e67 656e 6572 6963 5f75   bl_ui.generic_u
-000004c0: 695f 6c69 7374 0a69 6d70 6f72 7420 626c  i_list.import bl
-000004d0: 5f6f 7065 7261 746f 7273 2e66 696c 650a  _operators.file.
-000004e0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000004f0: 7065 7274 6965 735f 6461 7461 5f65 6d70  perties_data_emp
-00000500: 7479 0a69 6d70 6f72 7420 626c 5f75 692e  ty.import bl_ui.
-00000510: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00000520: 7479 6c65 0a69 6d70 6f72 7420 626c 5f75  tyle.import bl_u
-00000530: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-00000540: 7369 6373 5f66 6c75 6964 0a69 6d70 6f72  sics_fluid.impor
-00000550: 7420 626c 5f6f 7065 7261 746f 7273 2e61  t bl_operators.a
-00000560: 7373 6574 730a 696d 706f 7274 2062 6c5f  ssets.import bl_
-00000570: 6f70 6572 6174 6f72 732e 7669 6577 3364  operators.view3d
-00000580: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000590: 6f70 6572 7469 6573 5f6f 7574 7075 740a  operties_output.
-000005a0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000005b0: 7065 7274 6965 735f 6d61 7465 7269 616c  perties_material
-000005c0: 5f67 7065 6e63 696c 0a69 6d70 6f72 7420  _gpencil.import 
-000005d0: 626c 5f75 692e 6e6f 6465 5f61 6464 5f6d  bl_ui.node_add_m
-000005e0: 656e 755f 6765 6f6d 6574 7279 0a69 6d70  enu_geometry.imp
-000005f0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000600: 6f75 746c 696e 6572 0a69 6d70 6f72 7420  outliner.import 
-00000610: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000620: 5f64 6174 615f 6c69 6768 740a 696d 706f  _data_light.impo
-00000630: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000640: 6965 735f 636f 6e73 7472 6169 6e74 0a69  ies_constraint.i
-00000650: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000660: 655f 746f 7062 6172 0a69 6d70 6f72 7420  e_topbar.import 
-00000670: 626c 5f75 692e 7370 6163 655f 636c 6970  bl_ui.space_clip
-00000680: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000690: 6f70 6572 7469 6573 5f64 6174 615f 766f  operties_data_vo
-000006a0: 6c75 6d65 0a69 6d70 6f72 7420 626c 5f75  lume.import bl_u
-000006b0: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-000006c0: 7369 6373 5f72 6967 6964 626f 6479 5f63  sics_rigidbody_c
-000006d0: 6f6e 7374 7261 696e 740a 696d 706f 7274  onstraint.import
-000006e0: 2062 6c5f 7569 2e73 7061 6365 5f69 6e66   bl_ui.space_inf
-000006f0: 6f0a 696d 706f 7274 2062 6c5f 7569 2e70  o.import bl_ui.p
-00000700: 726f 7065 7274 6965 735f 6461 7461 5f70  roperties_data_p
-00000710: 6f69 6e74 636c 6f75 640a 696d 706f 7274  ointcloud.import
-00000720: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000730: 735f 6461 7461 5f73 7065 616b 6572 0a69  s_data_speaker.i
-00000740: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000750: 6572 7469 6573 5f64 6174 615f 6375 7276  erties_data_curv
-00000760: 650a 696d 706f 7274 2062 6c5f 7569 2e73  e.import bl_ui.s
-00000770: 7061 6365 5f63 6f6e 736f 6c65 0a69 6d70  pace_console.imp
-00000780: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000790: 7469 6573 5f74 6578 7475 7265 0a69 6d70  ties_texture.imp
-000007a0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000007b0: 7469 6573 5f64 6174 615f 7368 6164 6572  ties_data_shader
-000007c0: 6678 0a69 6d70 6f72 7420 626c 5f75 692e  fx.import bl_ui.
-000007d0: 7370 6163 655f 7072 6f70 6572 7469 6573  space_properties
-000007e0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000007f0: 6f70 6572 7469 6573 5f64 6174 615f 6d65  operties_data_me
-00000800: 7368 0a69 6d70 6f72 7420 626c 5f75 692e  sh.import bl_ui.
-00000810: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-00000820: 6375 7276 6573 0a69 6d70 6f72 7420 626c  curves.import bl
-00000830: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
-00000840: 6879 7369 6373 5f66 6965 6c64 0a69 6d70  hysics_field.imp
-00000850: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000860: 2e61 6e69 6d0a 696d 706f 7274 2062 6c5f  .anim.import bl_
-00000870: 7569 2e73 7061 6365 5f66 696c 6562 726f  ui.space_filebro
-00000880: 7773 6572 0a69 6d70 6f72 7420 626c 5f75  wser.import bl_u
-00000890: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-000008a0: 7369 6373 5f63 6c6f 7468 0a69 6d70 6f72  sics_cloth.impor
-000008b0: 7420 626c 5f6f 7065 7261 746f 7273 2e63  t bl_operators.c
-000008c0: 6f6e 7374 7261 696e 740a 696d 706f 7274  onstraint.import
-000008d0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000008e0: 735f 636f 6c6c 6563 7469 6f6e 0a69 6d70  s_collection.imp
-000008f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000900: 7469 6573 5f6d 6174 6572 6961 6c0a 696d  ties_material.im
-00000910: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000920: 7274 6965 735f 6f62 6a65 6374 0a69 6d70  rties_object.imp
-00000930: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000940: 7365 7175 656e 6365 720a 696d 706f 7274  sequencer.import
-00000950: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000960: 735f 6461 7461 5f63 616d 6572 610a 696d  s_data_camera.im
-00000970: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000980: 5f74 696d 650a 696d 706f 7274 2062 6c5f  _time.import bl_
-00000990: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-000009a0: 746f 6f6c 6261 720a 696d 706f 7274 2062  toolbar.import b
-000009b0: 6c5f 6f70 6572 6174 6f72 732e 6f62 6a65  l_operators.obje
-000009c0: 6374 0a69 6d70 6f72 7420 626c 5f75 692e  ct.import bl_ui.
-000009d0: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-000009e0: 6373 5f72 6967 6964 626f 6479 0a69 6d70  cs_rigidbody.imp
-000009f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000a00: 7469 6573 5f64 6174 615f 6d65 7461 6261  ties_data_metaba
-00000a10: 6c6c 0a69 6d70 6f72 7420 626c 5f6f 7065  ll.import bl_ope
-00000a20: 7261 746f 7273 2e6e 6f64 650a 696d 706f  rators.node.impo
-00000a30: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000a40: 6965 735f 6461 7461 5f61 726d 6174 7572  ies_data_armatur
-00000a50: 650a 0a47 656e 6572 6963 5479 7065 203d  e..GenericType =
+00000040: 692e 6e6f 6465 5f61 6464 5f6d 656e 755f  i.node_add_menu_
+00000050: 6765 6f6d 6574 7279 0a69 6d70 6f72 7420  geometry.import 
+00000060: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000070: 5f64 6174 615f 6172 6d61 7475 7265 0a69  _data_armature.i
+00000080: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000090: 6572 7469 6573 5f64 6174 615f 6770 656e  erties_data_gpen
+000000a0: 6369 6c0a 696d 706f 7274 2062 6c5f 7569  cil.import bl_ui
+000000b0: 2e73 7061 6365 5f74 6f6f 6c73 7973 7465  .space_toolsyste
+000000c0: 6d5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  m_common.import 
+000000d0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000000e0: 5f64 6174 615f 656d 7074 790a 696d 706f  _data_empty.impo
+000000f0: 7274 2062 6c5f 7569 2e73 7061 6365 5f64  rt bl_ui.space_d
+00000100: 6f70 6573 6865 6574 0a69 6d70 6f72 7420  opesheet.import 
+00000110: 626c 5f75 692e 7370 6163 655f 7374 6174  bl_ui.space_stat
+00000120: 7573 6261 720a 696d 706f 7274 2062 6c5f  usbar.import bl_
+00000130: 7569 2e70 726f 7065 7274 6965 735f 6f62  ui.properties_ob
+00000140: 6a65 6374 0a69 6d70 6f72 7420 626c 5f75  ject.import bl_u
+00000150: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000160: 615f 626f 6e65 0a69 6d70 6f72 7420 626c  a_bone.import bl
+00000170: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000180: 6174 615f 6375 7276 6573 0a69 6d70 6f72  ata_curves.impor
+00000190: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000001a0: 6573 5f64 6174 615f 6c61 7474 6963 650a  es_data_lattice.
+000001b0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000001c0: 6365 5f6e 6f64 650a 696d 706f 7274 2062  ce_node.import b
+000001d0: 6c5f 7569 2e73 7061 6365 5f63 6c69 700a  l_ui.space_clip.
+000001e0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+000001f0: 7065 7274 6965 735f 6d61 736b 5f63 6f6d  perties_mask_com
+00000200: 6d6f 6e0a 696d 706f 7274 2062 6c5f 7569  mon.import bl_ui
+00000210: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+00000220: 5f63 7572 7665 0a69 6d70 6f72 7420 626c  _curve.import bl
+00000230: 5f75 692e 7072 6f70 6572 7469 6573 5f6d  _ui.properties_m
+00000240: 6174 6572 6961 6c0a 696d 706f 7274 2062  aterial.import b
+00000250: 6c5f 6f70 6572 6174 6f72 732e 7669 6577  l_operators.view
+00000260: 3364 0a69 6d70 6f72 7420 626c 5f6f 7065  3d.import bl_ope
+00000270: 7261 746f 7273 2e66 7265 6573 7479 6c65  rators.freestyle
+00000280: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000290: 6f70 6572 7469 6573 5f64 6174 615f 7370  operties_data_sp
+000002a0: 6561 6b65 720a 696d 706f 7274 2062 6c5f  eaker.import bl_
+000002b0: 7569 2e70 726f 7065 7274 6965 735f 6f75  ui.properties_ou
+000002c0: 7470 7574 0a69 6d70 6f72 7420 626c 5f75  tput.import bl_u
+000002d0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+000002e0: 615f 6d6f 6469 6669 6572 0a69 6d70 6f72  a_modifier.impor
+000002f0: 7420 626c 5f75 692e 7370 6163 655f 6f75  t bl_ui.space_ou
+00000300: 746c 696e 6572 0a69 6d70 6f72 7420 626c  tliner.import bl
+00000310: 5f75 692e 7072 6f70 6572 7469 6573 5f63  _ui.properties_c
+00000320: 6f6c 6c65 6374 696f 6e0a 696d 706f 7274  ollection.import
+00000330: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000340: 735f 6461 7461 5f6d 6574 6162 616c 6c0a  s_data_metaball.
+00000350: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000360: 6365 5f74 696d 650a 696d 706f 7274 2062  ce_time.import b
+00000370: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000380: 6461 7461 5f70 6f69 6e74 636c 6f75 640a  data_pointcloud.
+00000390: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000003a0: 6f72 732e 7072 6573 6574 730a 696d 706f  ors.presets.impo
+000003b0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000003c0: 6965 735f 6772 6561 7365 5f70 656e 6369  ies_grease_penci
+000003d0: 6c5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  l_common.import 
+000003e0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000003f0: 5f6d 6174 6572 6961 6c5f 6770 656e 6369  _material_gpenci
+00000400: 6c0a 696d 706f 7274 2062 6c5f 7569 2e70  l.import bl_ui.p
+00000410: 726f 7065 7274 6965 735f 7061 696e 745f  roperties_paint_
+00000420: 636f 6d6d 6f6e 0a69 6d70 6f72 7420 626c  common.import bl
+00000430: 5f75 692e 6765 6e65 7269 635f 7569 5f6c  _ui.generic_ui_l
+00000440: 6973 740a 696d 706f 7274 2062 6c5f 7569  ist.import bl_ui
+00000450: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
+00000460: 6963 735f 7269 6769 6462 6f64 790a 696d  ics_rigidbody.im
+00000470: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000480: 7274 6965 735f 7068 7973 6963 735f 666c  rties_physics_fl
+00000490: 7569 640a 696d 706f 7274 2062 6c5f 7569  uid.import bl_ui
+000004a0: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
+000004b0: 6963 735f 6479 6e61 6d69 6370 6169 6e74  ics_dynamicpaint
+000004c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000004d0: 6f70 6572 7469 6573 5f64 6174 615f 7368  operties_data_sh
+000004e0: 6164 6572 6678 0a69 6d70 6f72 7420 626c  aderfx.import bl
+000004f0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000500: 6174 615f 6d65 7368 0a69 6d70 6f72 7420  ata_mesh.import 
+00000510: 626c 5f75 692e 7370 6163 655f 7465 7874  bl_ui.space_text
+00000520: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000530: 6f70 6572 7469 6573 5f70 6172 7469 636c  operties_particl
+00000540: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
+00000550: 726f 7065 7274 6965 735f 6461 7461 5f6c  roperties_data_l
+00000560: 6967 6874 7072 6f62 650a 696d 706f 7274  ightprobe.import
+00000570: 2062 6c5f 6f70 6572 6174 6f72 732e 636f   bl_operators.co
+00000580: 6e73 7472 6169 6e74 0a69 6d70 6f72 7420  nstraint.import 
+00000590: 626c 5f75 692e 7370 6163 655f 6669 6c65  bl_ui.space_file
+000005a0: 6272 6f77 7365 720a 696d 706f 7274 2062  browser.import b
+000005b0: 6c5f 6f70 6572 6174 6f72 732e 636c 6970  l_operators.clip
+000005c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+000005d0: 6163 655f 6772 6170 680a 696d 706f 7274  ace_graph.import
+000005e0: 2062 6c5f 6f70 6572 6174 6f72 732e 6173   bl_operators.as
+000005f0: 7365 7473 0a69 6d70 6f72 7420 626c 5f75  sets.import bl_u
+00000600: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000610: 615f 766f 6c75 6d65 0a69 6d70 6f72 7420  a_volume.import 
+00000620: 626c 5f75 692e 7370 6163 655f 7072 6f70  bl_ui.space_prop
+00000630: 6572 7469 6573 0a69 6d70 6f72 7420 626c  erties.import bl
+00000640: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00000650: 5f74 6f6f 6c62 6172 0a69 6d70 6f72 7420  _toolbar.import 
+00000660: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000670: 5f70 6879 7369 6373 5f66 6965 6c64 0a69  _physics_field.i
+00000680: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000690: 7273 2e61 6e69 6d0a 696d 706f 7274 2062  rs.anim.import b
+000006a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000006b0: 6461 7461 5f63 616d 6572 610a 696d 706f  data_camera.impo
+000006c0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000006d0: 6965 735f 776f 726b 7370 6163 650a 696d  ies_workspace.im
+000006e0: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
+000006f0: 732e 6f62 6a65 6374 0a69 6d70 6f72 7420  s.object.import 
+00000700: 626c 5f75 692e 7370 6163 655f 7573 6572  bl_ui.space_user
+00000710: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
+00000720: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000730: 7369 6373 5f63 6f6d 6d6f 6e0a 696d 706f  sics_common.impo
+00000740: 7274 2062 6c5f 7569 2e73 7061 6365 5f73  rt bl_ui.space_s
+00000750: 7072 6561 6473 6865 6574 0a69 6d70 6f72  preadsheet.impor
+00000760: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000770: 6573 5f64 6174 615f 6c69 6768 740a 696d  es_data_light.im
+00000780: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000790: 7274 6965 735f 7465 7874 7572 650a 696d  rties_texture.im
+000007a0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000007b0: 7274 6965 735f 7669 6577 5f6c 6179 6572  rties_view_layer
+000007c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000007d0: 6f70 6572 7469 6573 5f73 6365 6e65 0a69  operties_scene.i
+000007e0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+000007f0: 655f 746f 6f6c 7379 7374 656d 5f74 6f6f  e_toolsystem_too
+00000800: 6c62 6172 0a69 6d70 6f72 7420 626c 5f6f  lbar.import bl_o
+00000810: 7065 7261 746f 7273 2e6e 6f64 650a 696d  perators.node.im
+00000820: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
+00000830: 732e 776d 0a69 6d70 6f72 7420 626c 5f75  s.wm.import bl_u
+00000840: 692e 7370 6163 655f 696d 6167 650a 696d  i.space_image.im
+00000850: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000860: 5f6e 6c61 0a69 6d70 6f72 7420 626c 5f6f  _nla.import bl_o
+00000870: 7065 7261 746f 7273 2e66 696c 650a 696d  perators.file.im
+00000880: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000890: 7274 6965 735f 7068 7973 6963 735f 7269  rties_physics_ri
+000008a0: 6769 6462 6f64 795f 636f 6e73 7472 6169  gidbody_constrai
+000008b0: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
+000008c0: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
+000008d0: 6373 5f73 6f66 7462 6f64 790a 696d 706f  cs_softbody.impo
+000008e0: 7274 2062 6c5f 7569 2e73 7061 6365 5f69  rt bl_ui.space_i
+000008f0: 6e66 6f0a 696d 706f 7274 2062 6c5f 7569  nfo.import bl_ui
+00000900: 2e70 726f 7065 7274 6965 735f 636f 6e73  .properties_cons
+00000910: 7472 6169 6e74 0a69 6d70 6f72 7420 626c  traint.import bl
+00000920: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+00000930: 7265 6573 7479 6c65 0a69 6d70 6f72 7420  reestyle.import 
+00000940: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000950: 5f72 656e 6465 720a 696d 706f 7274 2062  _render.import b
+00000960: 6c5f 6f70 6572 6174 6f72 732e 7573 6572  l_operators.user
+00000970: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
+00000980: 692e 7370 6163 655f 746f 7062 6172 0a69  i.space_topbar.i
+00000990: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000009a0: 6572 7469 6573 5f77 6f72 6c64 0a69 6d70  erties_world.imp
+000009b0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000009c0: 7469 6573 5f70 6879 7369 6373 5f63 6c6f  ties_physics_clo
+000009d0: 7468 0a69 6d70 6f72 7420 626c 5f75 692e  th.import bl_ui.
+000009e0: 7370 6163 655f 636f 6e73 6f6c 650a 696d  space_console.im
+000009f0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000a00: 5f76 6965 7733 640a 696d 706f 7274 2062  _view3d.import b
+00000a10: 6c5f 7569 2e73 7061 6365 5f73 6571 7565  l_ui.space_seque
+00000a20: 6e63 6572 0a69 6d70 6f72 7420 626c 5f6f  ncer.import bl_o
+00000a30: 7065 7261 746f 7273 2e73 7072 6561 6473  perators.spreads
+00000a40: 6865 6574 0a69 6d70 6f72 7420 626c 5f75  heet.import bl_u
+00000a50: 690a 0a47 656e 6572 6963 5479 7065 203d  i..GenericType =
 00000a60: 2074 7970 696e 672e 5479 7065 5661 7228   typing.TypeVar(
 00000a70: 2247 656e 6572 6963 5479 7065 2229 0a0a  "GenericType")..
 00000a80: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
 00000a90: 743a 0a20 2020 2027 2727 2062 7569 6c74  t:.    ''' built
 00000aa0: 2d69 6e20 6261 7365 2063 6c61 7373 2066  -in base class f
 00000ab0: 6f72 2061 6c6c 2063 6c61 7373 6573 2069  or all classes i
 00000ac0: 6e20 6270 792e 7479 7065 732e 0a20 2020  n bpy.types..   
@@ -217166,697 +217166,705 @@
 003504d0: 6e63 653a 2027 626c 5f75 692e 7370 6163  nce: 'bl_ui.spac
 003504e0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
 003504f0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
 00350500: 5f67 7265 6173 655f 7065 6e63 696c 5f77  _grease_pencil_w
 00350510: 6569 6768 745f 6170 7065 6172 616e 6365  eight_appearance
 00350520: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
 00350530: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00350540: 5f70 656e 6369 6c5f 7765 6967 6874 5f70  _pencil_weight_p
-00350550: 6169 6e74 5f73 656c 6563 743a 2027 626c  aint_select: 'bl
-00350560: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350570: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00350580: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00350590: 7065 6e63 696c 5f77 6569 6768 745f 7061  pencil_weight_pa
-003505a0: 696e 745f 7365 6c65 6374 2720 3d20 4e6f  int_select' = No
-003505b0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003505c0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-003505d0: 6c5f 7765 6967 6874 5f70 6169 6e74 5f73  l_weight_paint_s
-003505e0: 6574 7469 6e67 733a 2027 626c 5f75 692e  ettings: 'bl_ui.
-003505f0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00350600: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00350610: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00350620: 696c 5f77 6569 6768 745f 7061 696e 745f  il_weight_paint_
-00350630: 7365 7474 696e 6773 2720 3d20 4e6f 6e65  settings' = None
-00350640: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00350650: 735f 696d 6167 6570 6169 6e74 5f6f 7074  s_imagepaint_opt
-00350660: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
-00350670: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00350680: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00350690: 735f 696d 6167 6570 6169 6e74 5f6f 7074  s_imagepaint_opt
-003506a0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-003506b0: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
-003506c0: 6167 6570 6169 6e74 5f6f 7074 696f 6e73  agepaint_options
-003506d0: 5f63 6176 6974 793a 2027 626c 5f75 692e  _cavity: 'bl_ui.
-003506e0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-003506f0: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00350700: 6f6f 6c73 5f69 6d61 6765 7061 696e 745f  ools_imagepaint_
-00350710: 6f70 7469 6f6e 735f 6361 7669 7479 2720  options_cavity' 
-00350720: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350730: 545f 746f 6f6c 735f 696d 6167 6570 6169  T_tools_imagepai
-00350740: 6e74 5f6f 7074 696f 6e73 5f65 7874 6572  nt_options_exter
-00350750: 6e61 6c3a 2027 626c 5f75 692e 7370 6163  nal: 'bl_ui.spac
-00350760: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00350770: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00350780: 5f69 6d61 6765 7061 696e 745f 6f70 7469  _imagepaint_opti
-00350790: 6f6e 735f 6578 7465 726e 616c 2720 3d20  ons_external' = 
-003507a0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003507b0: 746f 6f6c 735f 696d 6167 6570 6169 6e74  tools_imagepaint
-003507c0: 5f73 796d 6d65 7472 793a 2027 626c 5f75  _symmetry: 'bl_u
-003507d0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-003507e0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-003507f0: 5f74 6f6f 6c73 5f69 6d61 6765 7061 696e  _tools_imagepain
-00350800: 745f 7379 6d6d 6574 7279 2720 3d20 4e6f  t_symmetry' = No
-00350810: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350820: 6f6c 735f 6d61 736b 5f74 6578 7475 7265  ols_mask_texture
-00350830: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350840: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00350850: 4557 3344 5f50 545f 746f 6f6c 735f 6d61  EW3D_PT_tools_ma
-00350860: 736b 5f74 6578 7475 7265 2720 3d20 4e6f  sk_texture' = No
-00350870: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350880: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
-00350890: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
-003508a0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-003508b0: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-003508c0: 735f 6d65 7368 6564 6974 5f6f 7074 696f  s_meshedit_optio
-003508d0: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-003508e0: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
-003508f0: 6564 6974 5f6f 7074 696f 6e73 5f61 7574  edit_options_aut
-00350900: 6f6d 6572 6765 3a20 2762 6c5f 7569 2e73  omerge: 'bl_ui.s
-00350910: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00350920: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00350930: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
-00350940: 696f 6e73 5f61 7574 6f6d 6572 6765 2720  ions_automerge' 
-00350950: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350960: 545f 746f 6f6c 735f 6f62 6a65 6374 5f6f  T_tools_object_o
-00350970: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
-00350980: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00350990: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003509a0: 6f6c 735f 6f62 6a65 6374 5f6f 7074 696f  ols_object_optio
-003509b0: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-003509c0: 3344 5f50 545f 746f 6f6c 735f 6f62 6a65  3D_PT_tools_obje
-003509d0: 6374 5f6f 7074 696f 6e73 5f74 7261 6e73  ct_options_trans
-003509e0: 666f 726d 3a20 2762 6c5f 7569 2e73 7061  form: 'bl_ui.spa
-003509f0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00350a00: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00350a10: 735f 6f62 6a65 6374 5f6f 7074 696f 6e73  s_object_options
-00350a20: 5f74 7261 6e73 666f 726d 2720 3d20 4e6f  _transform' = No
-00350a30: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350a40: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
-00350a50: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350a60: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00350a70: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
-00350a80: 7274 6963 6c65 6d6f 6465 2720 3d20 4e6f  rticlemode' = No
-00350a90: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350aa0: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
-00350ab0: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
-00350ac0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00350ad0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00350ae0: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-00350af0: 6465 5f6f 7074 696f 6e73 2720 3d20 4e6f  de_options' = No
-00350b00: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350b10: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
-00350b20: 5f6f 7074 696f 6e73 5f64 6973 706c 6179  _options_display
-00350b30: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350b40: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00350b50: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
-00350b60: 7274 6963 6c65 6d6f 6465 5f6f 7074 696f  rticlemode_optio
-00350b70: 6e73 5f64 6973 706c 6179 2720 3d20 4e6f  ns_display' = No
+00350540: 5f70 656e 6369 6c5f 7765 6967 6874 5f6f  _pencil_weight_o
+00350550: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
+00350560: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00350570: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00350580: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00350590: 6c5f 7765 6967 6874 5f6f 7074 696f 6e73  l_weight_options
+003505a0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003505b0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+003505c0: 5f70 656e 6369 6c5f 7765 6967 6874 5f70  _pencil_weight_p
+003505d0: 6169 6e74 5f73 656c 6563 743a 2027 626c  aint_select: 'bl
+003505e0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+003505f0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00350600: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
+00350610: 7065 6e63 696c 5f77 6569 6768 745f 7061  pencil_weight_pa
+00350620: 696e 745f 7365 6c65 6374 2720 3d20 4e6f  int_select' = No
+00350630: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350640: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00350650: 6c5f 7765 6967 6874 5f70 6169 6e74 5f73  l_weight_paint_s
+00350660: 6574 7469 6e67 733a 2027 626c 5f75 692e  ettings: 'bl_ui.
+00350670: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00350680: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00350690: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
+003506a0: 696c 5f77 6569 6768 745f 7061 696e 745f  il_weight_paint_
+003506b0: 7365 7474 696e 6773 2720 3d20 4e6f 6e65  settings' = None
+003506c0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+003506d0: 735f 696d 6167 6570 6169 6e74 5f6f 7074  s_imagepaint_opt
+003506e0: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
+003506f0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00350700: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00350710: 735f 696d 6167 6570 6169 6e74 5f6f 7074  s_imagepaint_opt
+00350720: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
+00350730: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
+00350740: 6167 6570 6169 6e74 5f6f 7074 696f 6e73  agepaint_options
+00350750: 5f63 6176 6974 793a 2027 626c 5f75 692e  _cavity: 'bl_ui.
+00350760: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00350770: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00350780: 6f6f 6c73 5f69 6d61 6765 7061 696e 745f  ools_imagepaint_
+00350790: 6f70 7469 6f6e 735f 6361 7669 7479 2720  options_cavity' 
+003507a0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003507b0: 545f 746f 6f6c 735f 696d 6167 6570 6169  T_tools_imagepai
+003507c0: 6e74 5f6f 7074 696f 6e73 5f65 7874 6572  nt_options_exter
+003507d0: 6e61 6c3a 2027 626c 5f75 692e 7370 6163  nal: 'bl_ui.spac
+003507e0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+003507f0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00350800: 5f69 6d61 6765 7061 696e 745f 6f70 7469  _imagepaint_opti
+00350810: 6f6e 735f 6578 7465 726e 616c 2720 3d20  ons_external' = 
+00350820: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00350830: 746f 6f6c 735f 696d 6167 6570 6169 6e74  tools_imagepaint
+00350840: 5f73 796d 6d65 7472 793a 2027 626c 5f75  _symmetry: 'bl_u
+00350850: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00350860: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00350870: 5f74 6f6f 6c73 5f69 6d61 6765 7061 696e  _tools_imagepain
+00350880: 745f 7379 6d6d 6574 7279 2720 3d20 4e6f  t_symmetry' = No
+00350890: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+003508a0: 6f6c 735f 6d61 736b 5f74 6578 7475 7265  ols_mask_texture
+003508b0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003508c0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+003508d0: 4557 3344 5f50 545f 746f 6f6c 735f 6d61  EW3D_PT_tools_ma
+003508e0: 736b 5f74 6578 7475 7265 2720 3d20 4e6f  sk_texture' = No
+003508f0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350900: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
+00350910: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
+00350920: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00350930: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00350940: 735f 6d65 7368 6564 6974 5f6f 7074 696f  s_meshedit_optio
+00350950: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+00350960: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
+00350970: 6564 6974 5f6f 7074 696f 6e73 5f61 7574  edit_options_aut
+00350980: 6f6d 6572 6765 3a20 2762 6c5f 7569 2e73  omerge: 'bl_ui.s
+00350990: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+003509a0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+003509b0: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
+003509c0: 696f 6e73 5f61 7574 6f6d 6572 6765 2720  ions_automerge' 
+003509d0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003509e0: 545f 746f 6f6c 735f 6f62 6a65 6374 5f6f  T_tools_object_o
+003509f0: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
+00350a00: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00350a10: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00350a20: 6f6c 735f 6f62 6a65 6374 5f6f 7074 696f  ols_object_optio
+00350a30: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+00350a40: 3344 5f50 545f 746f 6f6c 735f 6f62 6a65  3D_PT_tools_obje
+00350a50: 6374 5f6f 7074 696f 6e73 5f74 7261 6e73  ct_options_trans
+00350a60: 666f 726d 3a20 2762 6c5f 7569 2e73 7061  form: 'bl_ui.spa
+00350a70: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00350a80: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00350a90: 735f 6f62 6a65 6374 5f6f 7074 696f 6e73  s_object_options
+00350aa0: 5f74 7261 6e73 666f 726d 2720 3d20 4e6f  _transform' = No
+00350ab0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350ac0: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
+00350ad0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350ae0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00350af0: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
+00350b00: 7274 6963 6c65 6d6f 6465 2720 3d20 4e6f  rticlemode' = No
+00350b10: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350b20: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
+00350b30: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
+00350b40: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00350b50: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00350b60: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
+00350b70: 6465 5f6f 7074 696f 6e73 2720 3d20 4e6f  de_options' = No
 00350b80: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
 00350b90: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
-00350ba0: 5f6f 7074 696f 6e73 5f73 6861 7065 6375  _options_shapecu
-00350bb0: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
-00350bc0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-00350bd0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f70  IEW3D_PT_tools_p
-00350be0: 6172 7469 636c 656d 6f64 655f 6f70 7469  articlemode_opti
-00350bf0: 6f6e 735f 7368 6170 6563 7574 2720 3d20  ons_shapecut' = 
-00350c00: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350c10: 746f 6f6c 735f 706f 7365 6d6f 6465 5f6f  tools_posemode_o
-00350c20: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
-00350c30: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00350c40: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00350c50: 6f6c 735f 706f 7365 6d6f 6465 5f6f 7074  ols_posemode_opt
-00350c60: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-00350c70: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
-00350c80: 7274 6578 7061 696e 745f 6f70 7469 6f6e  rtexpaint_option
-00350c90: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-00350ca0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-00350cb0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f76  IEW3D_PT_tools_v
-00350cc0: 6572 7465 7870 6169 6e74 5f6f 7074 696f  ertexpaint_optio
-00350cd0: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-00350ce0: 3344 5f50 545f 746f 6f6c 735f 7665 7274  3D_PT_tools_vert
-00350cf0: 6578 7061 696e 745f 7379 6d6d 6574 7279  expaint_symmetry
-00350d00: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350d10: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00350d20: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
-00350d30: 7274 6578 7061 696e 745f 7379 6d6d 6574  rtexpaint_symmet
-00350d40: 7279 2720 3d20 4e6f 6e65 0a0a 5649 4557  ry' = None..VIEW
-00350d50: 3344 5f50 545f 746f 6f6c 735f 7665 7274  3D_PT_tools_vert
-00350d60: 6578 7061 696e 745f 7379 6d6d 6574 7279  expaint_symmetry
-00350d70: 5f66 6f72 5f74 6f70 6261 723a 2027 626c  _for_topbar: 'bl
-00350d80: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350d90: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00350da0: 5054 5f74 6f6f 6c73 5f76 6572 7465 7870  PT_tools_vertexp
-00350db0: 6169 6e74 5f73 796d 6d65 7472 795f 666f  aint_symmetry_fo
-00350dc0: 725f 746f 7062 6172 2720 3d20 4e6f 6e65  r_topbar' = None
-00350dd0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00350de0: 735f 7765 6967 6874 5f67 7261 6469 656e  s_weight_gradien
-00350df0: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
-00350e00: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-00350e10: 4945 5733 445f 5054 5f74 6f6f 6c73 5f77  IEW3D_PT_tools_w
-00350e20: 6569 6768 745f 6772 6164 6965 6e74 2720  eight_gradient' 
-00350e30: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350e40: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
-00350e50: 696e 745f 6f70 7469 6f6e 733a 2027 626c  int_options: 'bl
-00350e60: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350e70: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00350e80: 5054 5f74 6f6f 6c73 5f77 6569 6768 7470  PT_tools_weightp
-00350e90: 6169 6e74 5f6f 7074 696f 6e73 2720 3d20  aint_options' = 
-00350ea0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350eb0: 746f 6f6c 735f 7765 6967 6874 7061 696e  tools_weightpain
-00350ec0: 745f 7379 6d6d 6574 7279 3a20 2762 6c5f  t_symmetry: 'bl_
-00350ed0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00350ee0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00350ef0: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
-00350f00: 696e 745f 7379 6d6d 6574 7279 2720 3d20  int_symmetry' = 
-00350f10: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350f20: 746f 6f6c 735f 7765 6967 6874 7061 696e  tools_weightpain
-00350f30: 745f 7379 6d6d 6574 7279 5f66 6f72 5f74  t_symmetry_for_t
-00350f40: 6f70 6261 723a 2027 626c 5f75 692e 7370  opbar: 'bl_ui.sp
-00350f50: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00350f60: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00350f70: 6c73 5f77 6569 6768 7470 6169 6e74 5f73  ls_weightpaint_s
-00350f80: 796d 6d65 7472 795f 666f 725f 746f 7062  ymmetry_for_topb
-00350f90: 6172 2720 3d20 4e6f 6e65 0a0a 5649 4557  ar' = None..VIEW
-00350fa0: 3344 5f50 545f 7472 616e 7366 6f72 6d5f  3D_PT_transform_
-00350fb0: 6f72 6965 6e74 6174 696f 6e73 3a20 2762  orientations: 'b
-00350fc0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350fd0: 642e 5649 4557 3344 5f50 545f 7472 616e  d.VIEW3D_PT_tran
-00350fe0: 7366 6f72 6d5f 6f72 6965 6e74 6174 696f  sform_orientatio
-00350ff0: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-00351000: 3344 5f50 545f 7669 6577 3364 5f63 7572  3D_PT_view3d_cur
-00351010: 736f 723a 2027 626c 5f75 692e 7370 6163  sor: 'bl_ui.spac
-00351020: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351030: 5054 5f76 6965 7733 645f 6375 7273 6f72  PT_view3d_cursor
-00351040: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351050: 5f50 545f 7669 6577 3364 5f6c 6f63 6b3a  _PT_view3d_lock:
-00351060: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351070: 6577 3364 2e56 4945 5733 445f 5054 5f76  ew3d.VIEW3D_PT_v
-00351080: 6965 7733 645f 6c6f 636b 2720 3d20 4e6f  iew3d_lock' = No
-00351090: 6e65 0a0a 5649 4557 3344 5f50 545f 7669  ne..VIEW3D_PT_vi
-003510a0: 6577 3364 5f70 726f 7065 7274 6965 733a  ew3d_properties:
-003510b0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003510c0: 6577 3364 2e56 4945 5733 445f 5054 5f76  ew3d.VIEW3D_PT_v
-003510d0: 6965 7733 645f 7072 6f70 6572 7469 6573  iew3d_properties
-003510e0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003510f0: 5f50 545f 7669 6577 3364 5f73 7465 7265  _PT_view3d_stere
-00351100: 6f3a 2027 626c 5f75 692e 7370 6163 655f  o: 'bl_ui.space_
-00351110: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-00351120: 5f76 6965 7733 645f 7374 6572 656f 2720  _view3d_stereo' 
-00351130: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351140: 545f 7669 6577 706f 7274 5f64 6562 7567  T_viewport_debug
-00351150: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00351160: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-00351170: 7669 6577 706f 7274 5f64 6562 7567 2720  viewport_debug' 
-00351180: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00351190: 525f 4d54 5f6c 6967 6874 6772 6f75 705f  R_MT_lightgroup_
-003511a0: 7379 6e63 3a20 2762 6c5f 7569 2e70 726f  sync: 'bl_ui.pro
-003511b0: 7065 7274 6965 735f 7669 6577 5f6c 6179  perties_view_lay
-003511c0: 6572 2e56 4945 574c 4159 4552 5f4d 545f  er.VIEWLAYER_MT_
-003511d0: 6c69 6768 7467 726f 7570 5f73 796e 6327  lightgroup_sync'
-003511e0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-003511f0: 4552 5f50 545f 6565 7665 655f 6c61 7965  ER_PT_eevee_laye
-00351200: 725f 7061 7373 6573 5f64 6174 613a 2027  r_passes_data: '
-00351210: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00351220: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
-00351230: 4c41 5945 525f 5054 5f65 6576 6565 5f6c  LAYER_PT_eevee_l
-00351240: 6179 6572 5f70 6173 7365 735f 6461 7461  ayer_passes_data
-00351250: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00351260: 5945 525f 5054 5f65 6576 6565 5f6c 6179  YER_PT_eevee_lay
-00351270: 6572 5f70 6173 7365 735f 6566 6665 6374  er_passes_effect
-00351280: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
-00351290: 7469 6573 5f76 6965 775f 6c61 7965 722e  ties_view_layer.
-003512a0: 5649 4557 4c41 5945 525f 5054 5f65 6576  VIEWLAYER_PT_eev
-003512b0: 6565 5f6c 6179 6572 5f70 6173 7365 735f  ee_layer_passes_
-003512c0: 6566 6665 6374 7327 203d 204e 6f6e 650a  effects' = None.
-003512d0: 0a56 4945 574c 4159 4552 5f50 545f 6565  .VIEWLAYER_PT_ee
-003512e0: 7665 655f 6c61 7965 725f 7061 7373 6573  vee_layer_passes
-003512f0: 5f6c 6967 6874 3a20 2762 6c5f 7569 2e70  _light: 'bl_ui.p
-00351300: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
-00351310: 6179 6572 2e56 4945 574c 4159 4552 5f50  ayer.VIEWLAYER_P
-00351320: 545f 6565 7665 655f 6c61 7965 725f 7061  T_eevee_layer_pa
-00351330: 7373 6573 5f6c 6967 6874 2720 3d20 4e6f  sses_light' = No
-00351340: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
-00351350: 5f65 6576 6565 5f6e 6578 745f 6c61 7965  _eevee_next_laye
-00351360: 725f 7061 7373 6573 5f64 6174 613a 2027  r_passes_data: '
-00351370: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00351380: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
-00351390: 4c41 5945 525f 5054 5f65 6576 6565 5f6e  LAYER_PT_eevee_n
-003513a0: 6578 745f 6c61 7965 725f 7061 7373 6573  ext_layer_passes
-003513b0: 5f64 6174 6127 203d 204e 6f6e 650a 0a56  _data' = None..V
-003513c0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-003513d0: 7374 796c 653a 2027 626c 5f75 692e 7072  style: 'bl_ui.pr
-003513e0: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-003513f0: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
-00351400: 6672 6565 7374 796c 6527 203d 204e 6f6e  freestyle' = Non
-00351410: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00351420: 6672 6565 7374 796c 655f 6564 6765 5f64  freestyle_edge_d
-00351430: 6574 6563 7469 6f6e 3a20 2762 6c5f 7569  etection: 'bl_ui
-00351440: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
-00351450: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
-00351460: 5054 5f66 7265 6573 7479 6c65 5f65 6467  PT_freestyle_edg
-00351470: 655f 6465 7465 6374 696f 6e27 203d 204e  e_detection' = N
-00351480: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-00351490: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-003514a0: 7365 743a 2027 626c 5f75 692e 7072 6f70  set: 'bl_ui.prop
-003514b0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-003514c0: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-003514d0: 6565 7374 796c 655f 6c69 6e65 7365 7427  eestyle_lineset'
-003514e0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-003514f0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-00351500: 6c69 6e65 7365 745f 636f 6c6c 6563 7469  lineset_collecti
-00351510: 6f6e 3a20 2762 6c5f 7569 2e70 726f 7065  on: 'bl_ui.prope
-00351520: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-00351530: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-00351540: 6573 7479 6c65 5f6c 696e 6573 6574 5f63  estyle_lineset_c
-00351550: 6f6c 6c65 6374 696f 6e27 203d 204e 6f6e  ollection' = Non
-00351560: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00351570: 6672 6565 7374 796c 655f 6c69 6e65 7365  freestyle_linese
-00351580: 745f 6564 6765 7479 7065 3a20 2762 6c5f  t_edgetype: 'bl_
-00351590: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
-003515a0: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
-003515b0: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
-003515c0: 696e 6573 6574 5f65 6467 6574 7970 6527  ineset_edgetype'
-003515d0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-003515e0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003515f0: 6c69 6e65 7365 745f 6661 6365 6d61 726b  lineset_facemark
-00351600: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
-00351610: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00351620: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00351630: 7374 796c 655f 6c69 6e65 7365 745f 6661  style_lineset_fa
-00351640: 6365 6d61 726b 7327 203d 204e 6f6e 650a  cemarks' = None.
-00351650: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00351660: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
-00351670: 7669 7369 6269 6c74 793a 2027 626c 5f75  visibilty: 'bl_u
-00351680: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00351690: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-003516a0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-003516b0: 6e65 7365 745f 7669 7369 6269 6c74 7927  neset_visibilty'
-003516c0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-003516d0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003516e0: 6c69 6e65 7374 796c 655f 616c 7068 613a  linestyle_alpha:
-003516f0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00351700: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
-00351710: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00351720: 796c 655f 6c69 6e65 7374 796c 655f 616c  yle_linestyle_al
-00351730: 7068 6127 203d 204e 6f6e 650a 0a56 4945  pha' = None..VIE
-00351740: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00351750: 796c 655f 6c69 6e65 7374 796c 655f 636f  yle_linestyle_co
-00351760: 6c6f 723a 2027 626c 5f75 692e 7072 6f70  lor: 'bl_ui.prop
-00351770: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-00351780: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00351790: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-003517a0: 655f 636f 6c6f 7227 203d 204e 6f6e 650a  e_color' = None.
-003517b0: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-003517c0: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-003517d0: 655f 6765 6f6d 6574 7279 3a20 2762 6c5f  e_geometry: 'bl_
-003517e0: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
-003517f0: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
-00351800: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
-00351810: 696e 6573 7479 6c65 5f67 656f 6d65 7472  inestyle_geometr
-00351820: 7927 203d 204e 6f6e 650a 0a56 4945 574c  y' = None..VIEWL
-00351830: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00351840: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
-00351850: 6b65 733a 2027 626c 5f75 692e 7072 6f70  kes: 'bl_ui.prop
-00351860: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-00351870: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00351880: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-00351890: 655f 7374 726f 6b65 7327 203d 204e 6f6e  e_strokes' = Non
-003518a0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-003518b0: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-003518c0: 796c 655f 7374 726f 6b65 735f 6368 6169  yle_strokes_chai
-003518d0: 6e69 6e67 3a20 2762 6c5f 7569 2e70 726f  ning: 'bl_ui.pro
-003518e0: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
-003518f0: 652e 5649 4557 4c41 5945 525f 5054 5f66  e.VIEWLAYER_PT_f
-00351900: 7265 6573 7479 6c65 5f6c 696e 6573 7479  reestyle_linesty
-00351910: 6c65 5f73 7472 6f6b 6573 5f63 6861 696e  le_strokes_chain
-00351920: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
-00351930: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00351940: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-00351950: 726f 6b65 735f 6461 7368 6564 6c69 6e65  rokes_dashedline
-00351960: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00351970: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
-00351980: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00351990: 7479 6c65 5f6c 696e 6573 7479 6c65 5f73  tyle_linestyle_s
-003519a0: 7472 6f6b 6573 5f64 6173 6865 646c 696e  trokes_dashedlin
-003519b0: 6527 203d 204e 6f6e 650a 0a56 4945 574c  e' = None..VIEWL
-003519c0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-003519d0: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
-003519e0: 6b65 735f 7365 6c65 6374 696f 6e3a 2027  kes_selection: '
-003519f0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00351a00: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
-00351a10: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00351a20: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
-00351a30: 6b65 735f 7365 6c65 6374 696f 6e27 203d  kes_selection' =
-00351a40: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00351a50: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00351a60: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
-00351a70: 736f 7274 696e 673a 2027 626c 5f75 692e  sorting: 'bl_ui.
-00351a80: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00351a90: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-00351aa0: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-00351ab0: 7374 796c 655f 7374 726f 6b65 735f 736f  style_strokes_so
-00351ac0: 7274 696e 6727 203d 204e 6f6e 650a 0a56  rting' = None..V
-00351ad0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00351ae0: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00351af0: 7374 726f 6b65 735f 7370 6c69 7474 696e  strokes_splittin
-00351b00: 673a 2027 626c 5f75 692e 7072 6f70 6572  g: 'bl_ui.proper
-00351b10: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00351b20: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00351b30: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00351b40: 7374 726f 6b65 735f 7370 6c69 7474 696e  strokes_splittin
-00351b50: 6727 203d 204e 6f6e 650a 0a56 4945 574c  g' = None..VIEWL
-00351b60: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00351b70: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
-00351b80: 6b65 735f 7370 6c69 7474 696e 675f 7061  kes_splitting_pa
-00351b90: 7474 6572 6e3a 2027 626c 5f75 692e 7072  ttern: 'bl_ui.pr
-00351ba0: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-00351bb0: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
-00351bc0: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-00351bd0: 796c 655f 7374 726f 6b65 735f 7370 6c69  yle_strokes_spli
-00351be0: 7474 696e 675f 7061 7474 6572 6e27 203d  tting_pattern' =
-00351bf0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00351c00: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00351c10: 6e65 7374 796c 655f 7465 7874 7572 653a  nestyle_texture:
-00351c20: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00351c30: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
-00351c40: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00351c50: 796c 655f 6c69 6e65 7374 796c 655f 7465  yle_linestyle_te
-00351c60: 7874 7572 6527 203d 204e 6f6e 650a 0a56  xture' = None..V
-00351c70: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00351c80: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00351c90: 7468 6963 6b6e 6573 733a 2027 626c 5f75  thickness: 'bl_u
-00351ca0: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00351cb0: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-00351cc0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00351cd0: 6e65 7374 796c 655f 7468 6963 6b6e 6573  nestyle_thicknes
-00351ce0: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
-00351cf0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00351d00: 655f 7374 796c 655f 6d6f 6475 6c65 733a  e_style_modules:
-00351d10: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00351d20: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
-00351d30: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00351d40: 796c 655f 7374 796c 655f 6d6f 6475 6c65  yle_style_module
-00351d50: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
-00351d60: 4159 4552 5f50 545f 6c61 7965 723a 2027  AYER_PT_layer: '
-00351d70: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00351d80: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
-00351d90: 4c41 5945 525f 5054 5f6c 6179 6572 2720  LAYER_PT_layer' 
-00351da0: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00351db0: 525f 5054 5f6c 6179 6572 5f63 7573 746f  R_PT_layer_custo
-00351dc0: 6d5f 7072 6f70 733a 2027 626c 5f75 692e  m_props: 'bl_ui.
-00351dd0: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
-00351de0: 6c61 7965 722e 5649 4557 4c41 5945 525f  layer.VIEWLAYER_
-00351df0: 5054 5f6c 6179 6572 5f63 7573 746f 6d5f  PT_layer_custom_
-00351e00: 7072 6f70 7327 203d 204e 6f6e 650a 0a56  props' = None..V
-00351e10: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
-00351e20: 725f 7061 7373 6573 3a20 2762 6c5f 7569  r_passes: 'bl_ui
-00351e30: 2e70 726f 7065 7274 6965 735f 7669 6577  .properties_view
-00351e40: 5f6c 6179 6572 2e56 4945 574c 4159 4552  _layer.VIEWLAYER
-00351e50: 5f50 545f 6c61 7965 725f 7061 7373 6573  _PT_layer_passes
-00351e60: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00351e70: 5945 525f 5054 5f6c 6179 6572 5f70 6173  YER_PT_layer_pas
-00351e80: 7365 735f 616f 763a 2027 626c 5f75 692e  ses_aov: 'bl_ui.
-00351e90: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
-00351ea0: 6c61 7965 722e 5649 4557 4c41 5945 525f  layer.VIEWLAYER_
-00351eb0: 5054 5f6c 6179 6572 5f70 6173 7365 735f  PT_layer_passes_
-00351ec0: 616f 7627 203d 204e 6f6e 650a 0a56 4945  aov' = None..VIE
-00351ed0: 574c 4159 4552 5f50 545f 6c61 7965 725f  WLAYER_PT_layer_
-00351ee0: 7061 7373 6573 5f63 7279 7074 6f6d 6174  passes_cryptomat
-00351ef0: 7465 3a20 2762 6c5f 7569 2e70 726f 7065  te: 'bl_ui.prope
-00351f00: 7274 6965 735f 7669 6577 5f6c 6179 6572  rties_view_layer
-00351f10: 2e56 4945 574c 4159 4552 5f50 545f 6c61  .VIEWLAYER_PT_la
-00351f20: 7965 725f 7061 7373 6573 5f63 7279 7074  yer_passes_crypt
-00351f30: 6f6d 6174 7465 2720 3d20 4e6f 6e65 0a0a  omatte' = None..
-00351f40: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
-00351f50: 6572 5f70 6173 7365 735f 6c69 6768 7467  er_passes_lightg
-00351f60: 726f 7570 733a 2027 626c 5f75 692e 7072  roups: 'bl_ui.pr
-00351f70: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
-00351f80: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
-00351f90: 5f6c 6179 6572 5f70 6173 7365 735f 6c69  _layer_passes_li
-00351fa0: 6768 7467 726f 7570 7327 203d 204e 6f6e  ghtgroups' = Non
-00351fb0: 650a 0a56 4945 574c 4159 4552 5f55 4c5f  e..VIEWLAYER_UL_
-00351fc0: 616f 763a 2027 626c 5f75 692e 7072 6f70  aov: 'bl_ui.prop
-00351fd0: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
-00351fe0: 722e 5649 4557 4c41 5945 525f 554c 5f61  r.VIEWLAYER_UL_a
-00351ff0: 6f76 2720 3d20 4e6f 6e65 0a0a 5649 4557  ov' = None..VIEW
-00352000: 4c41 5945 525f 554c 5f6c 696e 6573 6574  LAYER_UL_lineset
-00352010: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
-00352020: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00352030: 4945 574c 4159 4552 5f55 4c5f 6c69 6e65  IEWLAYER_UL_line
-00352040: 7365 7473 2720 3d20 4e6f 6e65 0a0a 564f  sets' = None..VO
-00352050: 4c55 4d45 5f55 4c5f 6772 6964 733a 2027  LUME_UL_grids: '
-00352060: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00352070: 5f64 6174 615f 766f 6c75 6d65 2e56 4f4c  _data_volume.VOL
-00352080: 554d 455f 554c 5f67 7269 6473 2720 3d20  UME_UL_grids' = 
-00352090: 4e6f 6e65 0a0a 574d 5f4d 545f 6f70 6572  None..WM_MT_oper
-003520a0: 6174 6f72 5f70 7265 7365 7473 3a20 2762  ator_presets: 'b
-003520b0: 6c5f 6f70 6572 6174 6f72 732e 7072 6573  l_operators.pres
-003520c0: 6574 732e 574d 5f4d 545f 6f70 6572 6174  ets.WM_MT_operat
-003520d0: 6f72 5f70 7265 7365 7473 2720 3d20 4e6f  or_presets' = No
-003520e0: 6e65 0a0a 574d 5f4d 545f 7370 6c61 7368  ne..WM_MT_splash
-003520f0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-00352100: 776d 2e57 4d5f 4d54 5f73 706c 6173 6827  wm.WM_MT_splash'
-00352110: 203d 204e 6f6e 650a 0a57 4d5f 4d54 5f73   = None..WM_MT_s
-00352120: 706c 6173 685f 6162 6f75 743a 2027 626c  plash_about: 'bl
-00352130: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-00352140: 5f4d 545f 7370 6c61 7368 5f61 626f 7574  _MT_splash_about
-00352150: 2720 3d20 4e6f 6e65 0a0a 574d 5f4d 545f  ' = None..WM_MT_
-00352160: 7370 6c61 7368 5f71 7569 636b 5f73 6574  splash_quick_set
-00352170: 7570 3a20 2762 6c5f 6f70 6572 6174 6f72  up: 'bl_operator
-00352180: 732e 776d 2e57 4d5f 4d54 5f73 706c 6173  s.wm.WM_MT_splas
-00352190: 685f 7175 6963 6b5f 7365 7475 7027 203d  h_quick_setup' =
-003521a0: 204e 6f6e 650a 0a57 4d5f 4d54 5f74 6f6f   None..WM_MT_too
-003521b0: 6c73 7973 7465 6d5f 7375 626d 656e 753a  lsystem_submenu:
-003521c0: 2027 626c 5f75 692e 7370 6163 655f 746f   'bl_ui.space_to
-003521d0: 6f6c 7379 7374 656d 5f63 6f6d 6d6f 6e2e  olsystem_common.
-003521e0: 574d 5f4d 545f 746f 6f6c 7379 7374 656d  WM_MT_toolsystem
-003521f0: 5f73 7562 6d65 6e75 2720 3d20 4e6f 6e65  _submenu' = None
-00352200: 0a0a 574d 5f4f 545f 6261 7463 685f 7265  ..WM_OT_batch_re
-00352210: 6e61 6d65 3a20 2762 6c5f 6f70 6572 6174  name: 'bl_operat
-00352220: 6f72 732e 776d 2e57 4d5f 4f54 5f62 6174  ors.wm.WM_OT_bat
-00352230: 6368 5f72 656e 616d 6527 203d 204e 6f6e  ch_rename' = Non
-00352240: 650a 0a57 4d5f 4f54 5f62 6c65 6e64 5f73  e..WM_OT_blend_s
-00352250: 7472 696e 6773 5f75 7466 385f 7661 6c69  trings_utf8_vali
-00352260: 6461 7465 3a20 2762 6c5f 6f70 6572 6174  date: 'bl_operat
-00352270: 6f72 732e 6669 6c65 2e57 4d5f 4f54 5f62  ors.file.WM_OT_b
-00352280: 6c65 6e64 5f73 7472 696e 6773 5f75 7466  lend_strings_utf
-00352290: 385f 7661 6c69 6461 7465 2720 3d20 4e6f  8_validate' = No
-003522a0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-003522b0: 745f 636f 6c6c 6563 7469 6f6e 5f62 6f6f  t_collection_boo
-003522c0: 6c65 616e 5f73 6574 3a20 2762 6c5f 6f70  lean_set: 'bl_op
-003522d0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-003522e0: 5f63 6f6e 7465 7874 5f63 6f6c 6c65 6374  _context_collect
-003522f0: 696f 6e5f 626f 6f6c 6561 6e5f 7365 7427  ion_boolean_set'
-00352300: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
-00352310: 6f6e 7465 7874 5f63 7963 6c65 5f61 7272  ontext_cycle_arr
-00352320: 6179 3a20 2762 6c5f 6f70 6572 6174 6f72  ay: 'bl_operator
-00352330: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-00352340: 7874 5f63 7963 6c65 5f61 7272 6179 2720  xt_cycle_array' 
-00352350: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
-00352360: 6e74 6578 745f 6379 636c 655f 656e 756d  ntext_cycle_enum
-00352370: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-00352380: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
-00352390: 5f63 7963 6c65 5f65 6e75 6d27 203d 204e  _cycle_enum' = N
-003523a0: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
-003523b0: 7874 5f63 7963 6c65 5f69 6e74 3a20 2762  xt_cycle_int: 'b
-003523c0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-003523d0: 4d5f 4f54 5f63 6f6e 7465 7874 5f63 7963  M_OT_context_cyc
-003523e0: 6c65 5f69 6e74 2720 3d20 4e6f 6e65 0a0a  le_int' = None..
-003523f0: 574d 5f4f 545f 636f 6e74 6578 745f 6d65  WM_OT_context_me
-00352400: 6e75 5f65 6e75 6d3a 2027 626c 5f6f 7065  nu_enum: 'bl_ope
-00352410: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-00352420: 636f 6e74 6578 745f 6d65 6e75 5f65 6e75  context_menu_enu
-00352430: 6d27 203d 204e 6f6e 650a 0a57 4d5f 4f54  m' = None..WM_OT
-00352440: 5f63 6f6e 7465 7874 5f6d 6f64 616c 5f6d  _context_modal_m
-00352450: 6f75 7365 3a20 2762 6c5f 6f70 6572 6174  ouse: 'bl_operat
-00352460: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00352470: 7465 7874 5f6d 6f64 616c 5f6d 6f75 7365  text_modal_mouse
-00352480: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00352490: 636f 6e74 6578 745f 7069 655f 656e 756d  context_pie_enum
-003524a0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003524b0: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
-003524c0: 5f70 6965 5f65 6e75 6d27 203d 204e 6f6e  _pie_enum' = Non
-003524d0: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
-003524e0: 5f73 6361 6c65 5f66 6c6f 6174 3a20 2762  _scale_float: 'b
-003524f0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00352500: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6361  M_OT_context_sca
-00352510: 6c65 5f66 6c6f 6174 2720 3d20 4e6f 6e65  le_float' = None
-00352520: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
-00352530: 7363 616c 655f 696e 743a 2027 626c 5f6f  scale_int: 'bl_o
-00352540: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00352550: 545f 636f 6e74 6578 745f 7363 616c 655f  T_context_scale_
-00352560: 696e 7427 203d 204e 6f6e 650a 0a57 4d5f  int' = None..WM_
-00352570: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f62  OT_context_set_b
-00352580: 6f6f 6c65 616e 3a20 2762 6c5f 6f70 6572  oolean: 'bl_oper
-00352590: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
-003525a0: 6f6e 7465 7874 5f73 6574 5f62 6f6f 6c65  ontext_set_boole
-003525b0: 616e 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  an' = None..WM_O
-003525c0: 545f 636f 6e74 6578 745f 7365 745f 656e  T_context_set_en
-003525d0: 756d 3a20 2762 6c5f 6f70 6572 6174 6f72  um: 'bl_operator
-003525e0: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-003525f0: 7874 5f73 6574 5f65 6e75 6d27 203d 204e  xt_set_enum' = N
-00352600: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
-00352610: 7874 5f73 6574 5f66 6c6f 6174 3a20 2762  xt_set_float: 'b
-00352620: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00352630: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
-00352640: 5f66 6c6f 6174 2720 3d20 4e6f 6e65 0a0a  _float' = None..
-00352650: 574d 5f4f 545f 636f 6e74 6578 745f 7365  WM_OT_context_se
-00352660: 745f 6964 3a20 2762 6c5f 6f70 6572 6174  t_id: 'bl_operat
-00352670: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00352680: 7465 7874 5f73 6574 5f69 6427 203d 204e  text_set_id' = N
-00352690: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
-003526a0: 7874 5f73 6574 5f69 6e74 3a20 2762 6c5f  xt_set_int: 'bl_
-003526b0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-003526c0: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f69  OT_context_set_i
-003526d0: 6e74 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  nt' = None..WM_O
-003526e0: 545f 636f 6e74 6578 745f 7365 745f 7374  T_context_set_st
-003526f0: 7269 6e67 3a20 2762 6c5f 6f70 6572 6174  ring: 'bl_operat
-00352700: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00352710: 7465 7874 5f73 6574 5f73 7472 696e 6727  text_set_string'
-00352720: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
-00352730: 6f6e 7465 7874 5f73 6574 5f76 616c 7565  ontext_set_value
-00352740: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-00352750: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
-00352760: 5f73 6574 5f76 616c 7565 2720 3d20 4e6f  _set_value' = No
-00352770: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-00352780: 745f 746f 6767 6c65 3a20 2762 6c5f 6f70  t_toggle: 'bl_op
-00352790: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-003527a0: 5f63 6f6e 7465 7874 5f74 6f67 676c 6527  _context_toggle'
-003527b0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
-003527c0: 6f6e 7465 7874 5f74 6f67 676c 655f 656e  ontext_toggle_en
-003527d0: 756d 3a20 2762 6c5f 6f70 6572 6174 6f72  um: 'bl_operator
-003527e0: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-003527f0: 7874 5f74 6f67 676c 655f 656e 756d 2720  xt_toggle_enum' 
-00352800: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 646f  = None..WM_OT_do
-00352810: 635f 7669 6577 3a20 2762 6c5f 6f70 6572  c_view: 'bl_oper
-00352820: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f64  ators.wm.WM_OT_d
-00352830: 6f63 5f76 6965 7727 203d 204e 6f6e 650a  oc_view' = None.
-00352840: 0a57 4d5f 4f54 5f64 6f63 5f76 6965 775f  .WM_OT_doc_view_
-00352850: 6d61 6e75 616c 3a20 2762 6c5f 6f70 6572  manual: 'bl_oper
-00352860: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f64  ators.wm.WM_OT_d
-00352870: 6f63 5f76 6965 775f 6d61 6e75 616c 2720  oc_view_manual' 
-00352880: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 6472  = None..WM_OT_dr
-00352890: 6f70 5f62 6c65 6e64 5f66 696c 653a 2027  op_blend_file: '
-003528a0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-003528b0: 574d 5f4f 545f 6472 6f70 5f62 6c65 6e64  WM_OT_drop_blend
-003528c0: 5f66 696c 6527 203d 204e 6f6e 650a 0a57  _file' = None..W
-003528d0: 4d5f 4f54 5f6f 7065 7261 746f 725f 6368  M_OT_operator_ch
-003528e0: 6561 745f 7368 6565 743a 2027 626c 5f6f  eat_sheet: 'bl_o
-003528f0: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00352900: 545f 6f70 6572 6174 6f72 5f63 6865 6174  T_operator_cheat
-00352910: 5f73 6865 6574 2720 3d20 4e6f 6e65 0a0a  _sheet' = None..
-00352920: 574d 5f4f 545f 6f70 6572 6174 6f72 5f70  WM_OT_operator_p
-00352930: 6965 5f65 6e75 6d3a 2027 626c 5f6f 7065  ie_enum: 'bl_ope
-00352940: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-00352950: 6f70 6572 6174 6f72 5f70 6965 5f65 6e75  operator_pie_enu
-00352960: 6d27 203d 204e 6f6e 650a 0a57 4d5f 4f54  m' = None..WM_OT
-00352970: 5f6f 776e 6572 5f64 6973 6162 6c65 3a20  _owner_disable: 
-00352980: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00352990: 2e57 4d5f 4f54 5f6f 776e 6572 5f64 6973  .WM_OT_owner_dis
-003529a0: 6162 6c65 2720 3d20 4e6f 6e65 0a0a 574d  able' = None..WM
-003529b0: 5f4f 545f 6f77 6e65 725f 656e 6162 6c65  _OT_owner_enable
-003529c0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003529d0: 776d 2e57 4d5f 4f54 5f6f 776e 6572 5f65  wm.WM_OT_owner_e
-003529e0: 6e61 626c 6527 203d 204e 6f6e 650a 0a57  nable' = None..W
-003529f0: 4d5f 4f54 5f70 6174 685f 6f70 656e 3a20  M_OT_path_open: 
+00350ba0: 5f6f 7074 696f 6e73 5f64 6973 706c 6179  _options_display
+00350bb0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350bc0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00350bd0: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
+00350be0: 7274 6963 6c65 6d6f 6465 5f6f 7074 696f  rticlemode_optio
+00350bf0: 6e73 5f64 6973 706c 6179 2720 3d20 4e6f  ns_display' = No
+00350c00: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350c10: 6f6c 735f 7061 7274 6963 6c65 6d6f 6465  ols_particlemode
+00350c20: 5f6f 7074 696f 6e73 5f73 6861 7065 6375  _options_shapecu
+00350c30: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
+00350c40: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00350c50: 4945 5733 445f 5054 5f74 6f6f 6c73 5f70  IEW3D_PT_tools_p
+00350c60: 6172 7469 636c 656d 6f64 655f 6f70 7469  articlemode_opti
+00350c70: 6f6e 735f 7368 6170 6563 7574 2720 3d20  ons_shapecut' = 
+00350c80: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00350c90: 746f 6f6c 735f 706f 7365 6d6f 6465 5f6f  tools_posemode_o
+00350ca0: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
+00350cb0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00350cc0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00350cd0: 6f6c 735f 706f 7365 6d6f 6465 5f6f 7074  ols_posemode_opt
+00350ce0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
+00350cf0: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
+00350d00: 7274 6578 7061 696e 745f 6f70 7469 6f6e  rtexpaint_option
+00350d10: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
+00350d20: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00350d30: 4945 5733 445f 5054 5f74 6f6f 6c73 5f76  IEW3D_PT_tools_v
+00350d40: 6572 7465 7870 6169 6e74 5f6f 7074 696f  ertexpaint_optio
+00350d50: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+00350d60: 3344 5f50 545f 746f 6f6c 735f 7665 7274  3D_PT_tools_vert
+00350d70: 6578 7061 696e 745f 7379 6d6d 6574 7279  expaint_symmetry
+00350d80: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350d90: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00350da0: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
+00350db0: 7274 6578 7061 696e 745f 7379 6d6d 6574  rtexpaint_symmet
+00350dc0: 7279 2720 3d20 4e6f 6e65 0a0a 5649 4557  ry' = None..VIEW
+00350dd0: 3344 5f50 545f 746f 6f6c 735f 7665 7274  3D_PT_tools_vert
+00350de0: 6578 7061 696e 745f 7379 6d6d 6574 7279  expaint_symmetry
+00350df0: 5f66 6f72 5f74 6f70 6261 723a 2027 626c  _for_topbar: 'bl
+00350e00: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00350e10: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00350e20: 5054 5f74 6f6f 6c73 5f76 6572 7465 7870  PT_tools_vertexp
+00350e30: 6169 6e74 5f73 796d 6d65 7472 795f 666f  aint_symmetry_fo
+00350e40: 725f 746f 7062 6172 2720 3d20 4e6f 6e65  r_topbar' = None
+00350e50: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00350e60: 735f 7765 6967 6874 5f67 7261 6469 656e  s_weight_gradien
+00350e70: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
+00350e80: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00350e90: 4945 5733 445f 5054 5f74 6f6f 6c73 5f77  IEW3D_PT_tools_w
+00350ea0: 6569 6768 745f 6772 6164 6965 6e74 2720  eight_gradient' 
+00350eb0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00350ec0: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
+00350ed0: 696e 745f 6f70 7469 6f6e 733a 2027 626c  int_options: 'bl
+00350ee0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00350ef0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00350f00: 5054 5f74 6f6f 6c73 5f77 6569 6768 7470  PT_tools_weightp
+00350f10: 6169 6e74 5f6f 7074 696f 6e73 2720 3d20  aint_options' = 
+00350f20: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00350f30: 746f 6f6c 735f 7765 6967 6874 7061 696e  tools_weightpain
+00350f40: 745f 7379 6d6d 6574 7279 3a20 2762 6c5f  t_symmetry: 'bl_
+00350f50: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00350f60: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00350f70: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
+00350f80: 696e 745f 7379 6d6d 6574 7279 2720 3d20  int_symmetry' = 
+00350f90: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00350fa0: 746f 6f6c 735f 7765 6967 6874 7061 696e  tools_weightpain
+00350fb0: 745f 7379 6d6d 6574 7279 5f66 6f72 5f74  t_symmetry_for_t
+00350fc0: 6f70 6261 723a 2027 626c 5f75 692e 7370  opbar: 'bl_ui.sp
+00350fd0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00350fe0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00350ff0: 6c73 5f77 6569 6768 7470 6169 6e74 5f73  ls_weightpaint_s
+00351000: 796d 6d65 7472 795f 666f 725f 746f 7062  ymmetry_for_topb
+00351010: 6172 2720 3d20 4e6f 6e65 0a0a 5649 4557  ar' = None..VIEW
+00351020: 3344 5f50 545f 7472 616e 7366 6f72 6d5f  3D_PT_transform_
+00351030: 6f72 6965 6e74 6174 696f 6e73 3a20 2762  orientations: 'b
+00351040: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351050: 642e 5649 4557 3344 5f50 545f 7472 616e  d.VIEW3D_PT_tran
+00351060: 7366 6f72 6d5f 6f72 6965 6e74 6174 696f  sform_orientatio
+00351070: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+00351080: 3344 5f50 545f 7669 6577 3364 5f63 7572  3D_PT_view3d_cur
+00351090: 736f 723a 2027 626c 5f75 692e 7370 6163  sor: 'bl_ui.spac
+003510a0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+003510b0: 5054 5f76 6965 7733 645f 6375 7273 6f72  PT_view3d_cursor
+003510c0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003510d0: 5f50 545f 7669 6577 3364 5f6c 6f63 6b3a  _PT_view3d_lock:
+003510e0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003510f0: 6577 3364 2e56 4945 5733 445f 5054 5f76  ew3d.VIEW3D_PT_v
+00351100: 6965 7733 645f 6c6f 636b 2720 3d20 4e6f  iew3d_lock' = No
+00351110: 6e65 0a0a 5649 4557 3344 5f50 545f 7669  ne..VIEW3D_PT_vi
+00351120: 6577 3364 5f70 726f 7065 7274 6965 733a  ew3d_properties:
+00351130: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351140: 6577 3364 2e56 4945 5733 445f 5054 5f76  ew3d.VIEW3D_PT_v
+00351150: 6965 7733 645f 7072 6f70 6572 7469 6573  iew3d_properties
+00351160: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00351170: 5f50 545f 7669 6577 3364 5f73 7465 7265  _PT_view3d_stere
+00351180: 6f3a 2027 626c 5f75 692e 7370 6163 655f  o: 'bl_ui.space_
+00351190: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+003511a0: 5f76 6965 7733 645f 7374 6572 656f 2720  _view3d_stereo' 
+003511b0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003511c0: 545f 7669 6577 706f 7274 5f64 6562 7567  T_viewport_debug
+003511d0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003511e0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+003511f0: 7669 6577 706f 7274 5f64 6562 7567 2720  viewport_debug' 
+00351200: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00351210: 525f 4d54 5f6c 6967 6874 6772 6f75 705f  R_MT_lightgroup_
+00351220: 7379 6e63 3a20 2762 6c5f 7569 2e70 726f  sync: 'bl_ui.pro
+00351230: 7065 7274 6965 735f 7669 6577 5f6c 6179  perties_view_lay
+00351240: 6572 2e56 4945 574c 4159 4552 5f4d 545f  er.VIEWLAYER_MT_
+00351250: 6c69 6768 7467 726f 7570 5f73 796e 6327  lightgroup_sync'
+00351260: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00351270: 4552 5f50 545f 6565 7665 655f 6c61 7965  ER_PT_eevee_laye
+00351280: 725f 7061 7373 6573 5f64 6174 613a 2027  r_passes_data: '
+00351290: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+003512a0: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
+003512b0: 4c41 5945 525f 5054 5f65 6576 6565 5f6c  LAYER_PT_eevee_l
+003512c0: 6179 6572 5f70 6173 7365 735f 6461 7461  ayer_passes_data
+003512d0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
+003512e0: 5945 525f 5054 5f65 6576 6565 5f6c 6179  YER_PT_eevee_lay
+003512f0: 6572 5f70 6173 7365 735f 6566 6665 6374  er_passes_effect
+00351300: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
+00351310: 7469 6573 5f76 6965 775f 6c61 7965 722e  ties_view_layer.
+00351320: 5649 4557 4c41 5945 525f 5054 5f65 6576  VIEWLAYER_PT_eev
+00351330: 6565 5f6c 6179 6572 5f70 6173 7365 735f  ee_layer_passes_
+00351340: 6566 6665 6374 7327 203d 204e 6f6e 650a  effects' = None.
+00351350: 0a56 4945 574c 4159 4552 5f50 545f 6565  .VIEWLAYER_PT_ee
+00351360: 7665 655f 6c61 7965 725f 7061 7373 6573  vee_layer_passes
+00351370: 5f6c 6967 6874 3a20 2762 6c5f 7569 2e70  _light: 'bl_ui.p
+00351380: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
+00351390: 6179 6572 2e56 4945 574c 4159 4552 5f50  ayer.VIEWLAYER_P
+003513a0: 545f 6565 7665 655f 6c61 7965 725f 7061  T_eevee_layer_pa
+003513b0: 7373 6573 5f6c 6967 6874 2720 3d20 4e6f  sses_light' = No
+003513c0: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+003513d0: 5f65 6576 6565 5f6e 6578 745f 6c61 7965  _eevee_next_laye
+003513e0: 725f 7061 7373 6573 5f64 6174 613a 2027  r_passes_data: '
+003513f0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00351400: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
+00351410: 4c41 5945 525f 5054 5f65 6576 6565 5f6e  LAYER_PT_eevee_n
+00351420: 6578 745f 6c61 7965 725f 7061 7373 6573  ext_layer_passes
+00351430: 5f64 6174 6127 203d 204e 6f6e 650a 0a56  _data' = None..V
+00351440: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00351450: 7374 796c 653a 2027 626c 5f75 692e 7072  style: 'bl_ui.pr
+00351460: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
+00351470: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
+00351480: 6672 6565 7374 796c 6527 203d 204e 6f6e  freestyle' = Non
+00351490: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+003514a0: 6672 6565 7374 796c 655f 6564 6765 5f64  freestyle_edge_d
+003514b0: 6574 6563 7469 6f6e 3a20 2762 6c5f 7569  etection: 'bl_ui
+003514c0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+003514d0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
+003514e0: 5054 5f66 7265 6573 7479 6c65 5f65 6467  PT_freestyle_edg
+003514f0: 655f 6465 7465 6374 696f 6e27 203d 204e  e_detection' = N
+00351500: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+00351510: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00351520: 7365 743a 2027 626c 5f75 692e 7072 6f70  set: 'bl_ui.prop
+00351530: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
+00351540: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00351550: 6565 7374 796c 655f 6c69 6e65 7365 7427  eestyle_lineset'
+00351560: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00351570: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00351580: 6c69 6e65 7365 745f 636f 6c6c 6563 7469  lineset_collecti
+00351590: 6f6e 3a20 2762 6c5f 7569 2e70 726f 7065  on: 'bl_ui.prope
+003515a0: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
+003515b0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+003515c0: 6573 7479 6c65 5f6c 696e 6573 6574 5f63  estyle_lineset_c
+003515d0: 6f6c 6c65 6374 696f 6e27 203d 204e 6f6e  ollection' = Non
+003515e0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+003515f0: 6672 6565 7374 796c 655f 6c69 6e65 7365  freestyle_linese
+00351600: 745f 6564 6765 7479 7065 3a20 2762 6c5f  t_edgetype: 'bl_
+00351610: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
+00351620: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
+00351630: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+00351640: 696e 6573 6574 5f65 6467 6574 7970 6527  ineset_edgetype'
+00351650: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00351660: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00351670: 6c69 6e65 7365 745f 6661 6365 6d61 726b  lineset_facemark
+00351680: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
+00351690: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+003516a0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+003516b0: 7374 796c 655f 6c69 6e65 7365 745f 6661  style_lineset_fa
+003516c0: 6365 6d61 726b 7327 203d 204e 6f6e 650a  cemarks' = None.
+003516d0: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+003516e0: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
+003516f0: 7669 7369 6269 6c74 793a 2027 626c 5f75  visibilty: 'bl_u
+00351700: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00351710: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00351720: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00351730: 6e65 7365 745f 7669 7369 6269 6c74 7927  neset_visibilty'
+00351740: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00351750: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00351760: 6c69 6e65 7374 796c 655f 616c 7068 613a  linestyle_alpha:
+00351770: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00351780: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+00351790: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003517a0: 796c 655f 6c69 6e65 7374 796c 655f 616c  yle_linestyle_al
+003517b0: 7068 6127 203d 204e 6f6e 650a 0a56 4945  pha' = None..VIE
+003517c0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003517d0: 796c 655f 6c69 6e65 7374 796c 655f 636f  yle_linestyle_co
+003517e0: 6c6f 723a 2027 626c 5f75 692e 7072 6f70  lor: 'bl_ui.prop
+003517f0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
+00351800: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00351810: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
+00351820: 655f 636f 6c6f 7227 203d 204e 6f6e 650a  e_color' = None.
+00351830: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00351840: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
+00351850: 655f 6765 6f6d 6574 7279 3a20 2762 6c5f  e_geometry: 'bl_
+00351860: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
+00351870: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
+00351880: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+00351890: 696e 6573 7479 6c65 5f67 656f 6d65 7472  inestyle_geometr
+003518a0: 7927 203d 204e 6f6e 650a 0a56 4945 574c  y' = None..VIEWL
+003518b0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+003518c0: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+003518d0: 6b65 733a 2027 626c 5f75 692e 7072 6f70  kes: 'bl_ui.prop
+003518e0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
+003518f0: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00351900: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
+00351910: 655f 7374 726f 6b65 7327 203d 204e 6f6e  e_strokes' = Non
+00351920: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00351930: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00351940: 796c 655f 7374 726f 6b65 735f 6368 6169  yle_strokes_chai
+00351950: 6e69 6e67 3a20 2762 6c5f 7569 2e70 726f  ning: 'bl_ui.pro
+00351960: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
+00351970: 652e 5649 4557 4c41 5945 525f 5054 5f66  e.VIEWLAYER_PT_f
+00351980: 7265 6573 7479 6c65 5f6c 696e 6573 7479  reestyle_linesty
+00351990: 6c65 5f73 7472 6f6b 6573 5f63 6861 696e  le_strokes_chain
+003519a0: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
+003519b0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003519c0: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
+003519d0: 726f 6b65 735f 6461 7368 6564 6c69 6e65  rokes_dashedline
+003519e0: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+003519f0: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
+00351a00: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
+00351a10: 7479 6c65 5f6c 696e 6573 7479 6c65 5f73  tyle_linestyle_s
+00351a20: 7472 6f6b 6573 5f64 6173 6865 646c 696e  trokes_dashedlin
+00351a30: 6527 203d 204e 6f6e 650a 0a56 4945 574c  e' = None..VIEWL
+00351a40: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00351a50: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00351a60: 6b65 735f 7365 6c65 6374 696f 6e3a 2027  kes_selection: '
+00351a70: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00351a80: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+00351a90: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00351aa0: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00351ab0: 6b65 735f 7365 6c65 6374 696f 6e27 203d  kes_selection' =
+00351ac0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00351ad0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00351ae0: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+00351af0: 736f 7274 696e 673a 2027 626c 5f75 692e  sorting: 'bl_ui.
+00351b00: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
+00351b10: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
+00351b20: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00351b30: 7374 796c 655f 7374 726f 6b65 735f 736f  style_strokes_so
+00351b40: 7274 696e 6727 203d 204e 6f6e 650a 0a56  rting' = None..V
+00351b50: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00351b60: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+00351b70: 7374 726f 6b65 735f 7370 6c69 7474 696e  strokes_splittin
+00351b80: 673a 2027 626c 5f75 692e 7072 6f70 6572  g: 'bl_ui.proper
+00351b90: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+00351ba0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00351bb0: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+00351bc0: 7374 726f 6b65 735f 7370 6c69 7474 696e  strokes_splittin
+00351bd0: 6727 203d 204e 6f6e 650a 0a56 4945 574c  g' = None..VIEWL
+00351be0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00351bf0: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00351c00: 6b65 735f 7370 6c69 7474 696e 675f 7061  kes_splitting_pa
+00351c10: 7474 6572 6e3a 2027 626c 5f75 692e 7072  ttern: 'bl_ui.pr
+00351c20: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
+00351c30: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
+00351c40: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00351c50: 796c 655f 7374 726f 6b65 735f 7370 6c69  yle_strokes_spli
+00351c60: 7474 696e 675f 7061 7474 6572 6e27 203d  tting_pattern' =
+00351c70: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00351c80: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00351c90: 6e65 7374 796c 655f 7465 7874 7572 653a  nestyle_texture:
+00351ca0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00351cb0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+00351cc0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+00351cd0: 796c 655f 6c69 6e65 7374 796c 655f 7465  yle_linestyle_te
+00351ce0: 7874 7572 6527 203d 204e 6f6e 650a 0a56  xture' = None..V
+00351cf0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00351d00: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+00351d10: 7468 6963 6b6e 6573 733a 2027 626c 5f75  thickness: 'bl_u
+00351d20: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00351d30: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00351d40: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00351d50: 6e65 7374 796c 655f 7468 6963 6b6e 6573  nestyle_thicknes
+00351d60: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
+00351d70: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00351d80: 655f 7374 796c 655f 6d6f 6475 6c65 733a  e_style_modules:
+00351d90: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00351da0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+00351db0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+00351dc0: 796c 655f 7374 796c 655f 6d6f 6475 6c65  yle_style_module
+00351dd0: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
+00351de0: 4159 4552 5f50 545f 6c61 7965 723a 2027  AYER_PT_layer: '
+00351df0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00351e00: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
+00351e10: 4c41 5945 525f 5054 5f6c 6179 6572 2720  LAYER_PT_layer' 
+00351e20: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00351e30: 525f 5054 5f6c 6179 6572 5f63 7573 746f  R_PT_layer_custo
+00351e40: 6d5f 7072 6f70 733a 2027 626c 5f75 692e  m_props: 'bl_ui.
+00351e50: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
+00351e60: 6c61 7965 722e 5649 4557 4c41 5945 525f  layer.VIEWLAYER_
+00351e70: 5054 5f6c 6179 6572 5f63 7573 746f 6d5f  PT_layer_custom_
+00351e80: 7072 6f70 7327 203d 204e 6f6e 650a 0a56  props' = None..V
+00351e90: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
+00351ea0: 725f 7061 7373 6573 3a20 2762 6c5f 7569  r_passes: 'bl_ui
+00351eb0: 2e70 726f 7065 7274 6965 735f 7669 6577  .properties_view
+00351ec0: 5f6c 6179 6572 2e56 4945 574c 4159 4552  _layer.VIEWLAYER
+00351ed0: 5f50 545f 6c61 7965 725f 7061 7373 6573  _PT_layer_passes
+00351ee0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
+00351ef0: 5945 525f 5054 5f6c 6179 6572 5f70 6173  YER_PT_layer_pas
+00351f00: 7365 735f 616f 763a 2027 626c 5f75 692e  ses_aov: 'bl_ui.
+00351f10: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
+00351f20: 6c61 7965 722e 5649 4557 4c41 5945 525f  layer.VIEWLAYER_
+00351f30: 5054 5f6c 6179 6572 5f70 6173 7365 735f  PT_layer_passes_
+00351f40: 616f 7627 203d 204e 6f6e 650a 0a56 4945  aov' = None..VIE
+00351f50: 574c 4159 4552 5f50 545f 6c61 7965 725f  WLAYER_PT_layer_
+00351f60: 7061 7373 6573 5f63 7279 7074 6f6d 6174  passes_cryptomat
+00351f70: 7465 3a20 2762 6c5f 7569 2e70 726f 7065  te: 'bl_ui.prope
+00351f80: 7274 6965 735f 7669 6577 5f6c 6179 6572  rties_view_layer
+00351f90: 2e56 4945 574c 4159 4552 5f50 545f 6c61  .VIEWLAYER_PT_la
+00351fa0: 7965 725f 7061 7373 6573 5f63 7279 7074  yer_passes_crypt
+00351fb0: 6f6d 6174 7465 2720 3d20 4e6f 6e65 0a0a  omatte' = None..
+00351fc0: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
+00351fd0: 6572 5f70 6173 7365 735f 6c69 6768 7467  er_passes_lightg
+00351fe0: 726f 7570 733a 2027 626c 5f75 692e 7072  roups: 'bl_ui.pr
+00351ff0: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
+00352000: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
+00352010: 5f6c 6179 6572 5f70 6173 7365 735f 6c69  _layer_passes_li
+00352020: 6768 7467 726f 7570 7327 203d 204e 6f6e  ghtgroups' = Non
+00352030: 650a 0a56 4945 574c 4159 4552 5f55 4c5f  e..VIEWLAYER_UL_
+00352040: 616f 763a 2027 626c 5f75 692e 7072 6f70  aov: 'bl_ui.prop
+00352050: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
+00352060: 722e 5649 4557 4c41 5945 525f 554c 5f61  r.VIEWLAYER_UL_a
+00352070: 6f76 2720 3d20 4e6f 6e65 0a0a 5649 4557  ov' = None..VIEW
+00352080: 4c41 5945 525f 554c 5f6c 696e 6573 6574  LAYER_UL_lineset
+00352090: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
+003520a0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+003520b0: 4945 574c 4159 4552 5f55 4c5f 6c69 6e65  IEWLAYER_UL_line
+003520c0: 7365 7473 2720 3d20 4e6f 6e65 0a0a 564f  sets' = None..VO
+003520d0: 4c55 4d45 5f55 4c5f 6772 6964 733a 2027  LUME_UL_grids: '
+003520e0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+003520f0: 5f64 6174 615f 766f 6c75 6d65 2e56 4f4c  _data_volume.VOL
+00352100: 554d 455f 554c 5f67 7269 6473 2720 3d20  UME_UL_grids' = 
+00352110: 4e6f 6e65 0a0a 574d 5f4d 545f 6f70 6572  None..WM_MT_oper
+00352120: 6174 6f72 5f70 7265 7365 7473 3a20 2762  ator_presets: 'b
+00352130: 6c5f 6f70 6572 6174 6f72 732e 7072 6573  l_operators.pres
+00352140: 6574 732e 574d 5f4d 545f 6f70 6572 6174  ets.WM_MT_operat
+00352150: 6f72 5f70 7265 7365 7473 2720 3d20 4e6f  or_presets' = No
+00352160: 6e65 0a0a 574d 5f4d 545f 7370 6c61 7368  ne..WM_MT_splash
+00352170: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00352180: 776d 2e57 4d5f 4d54 5f73 706c 6173 6827  wm.WM_MT_splash'
+00352190: 203d 204e 6f6e 650a 0a57 4d5f 4d54 5f73   = None..WM_MT_s
+003521a0: 706c 6173 685f 6162 6f75 743a 2027 626c  plash_about: 'bl
+003521b0: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+003521c0: 5f4d 545f 7370 6c61 7368 5f61 626f 7574  _MT_splash_about
+003521d0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4d 545f  ' = None..WM_MT_
+003521e0: 7370 6c61 7368 5f71 7569 636b 5f73 6574  splash_quick_set
+003521f0: 7570 3a20 2762 6c5f 6f70 6572 6174 6f72  up: 'bl_operator
+00352200: 732e 776d 2e57 4d5f 4d54 5f73 706c 6173  s.wm.WM_MT_splas
+00352210: 685f 7175 6963 6b5f 7365 7475 7027 203d  h_quick_setup' =
+00352220: 204e 6f6e 650a 0a57 4d5f 4d54 5f74 6f6f   None..WM_MT_too
+00352230: 6c73 7973 7465 6d5f 7375 626d 656e 753a  lsystem_submenu:
+00352240: 2027 626c 5f75 692e 7370 6163 655f 746f   'bl_ui.space_to
+00352250: 6f6c 7379 7374 656d 5f63 6f6d 6d6f 6e2e  olsystem_common.
+00352260: 574d 5f4d 545f 746f 6f6c 7379 7374 656d  WM_MT_toolsystem
+00352270: 5f73 7562 6d65 6e75 2720 3d20 4e6f 6e65  _submenu' = None
+00352280: 0a0a 574d 5f4f 545f 6261 7463 685f 7265  ..WM_OT_batch_re
+00352290: 6e61 6d65 3a20 2762 6c5f 6f70 6572 6174  name: 'bl_operat
+003522a0: 6f72 732e 776d 2e57 4d5f 4f54 5f62 6174  ors.wm.WM_OT_bat
+003522b0: 6368 5f72 656e 616d 6527 203d 204e 6f6e  ch_rename' = Non
+003522c0: 650a 0a57 4d5f 4f54 5f62 6c65 6e64 5f73  e..WM_OT_blend_s
+003522d0: 7472 696e 6773 5f75 7466 385f 7661 6c69  trings_utf8_vali
+003522e0: 6461 7465 3a20 2762 6c5f 6f70 6572 6174  date: 'bl_operat
+003522f0: 6f72 732e 6669 6c65 2e57 4d5f 4f54 5f62  ors.file.WM_OT_b
+00352300: 6c65 6e64 5f73 7472 696e 6773 5f75 7466  lend_strings_utf
+00352310: 385f 7661 6c69 6461 7465 2720 3d20 4e6f  8_validate' = No
+00352320: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
+00352330: 745f 636f 6c6c 6563 7469 6f6e 5f62 6f6f  t_collection_boo
+00352340: 6c65 616e 5f73 6574 3a20 2762 6c5f 6f70  lean_set: 'bl_op
+00352350: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00352360: 5f63 6f6e 7465 7874 5f63 6f6c 6c65 6374  _context_collect
+00352370: 696f 6e5f 626f 6f6c 6561 6e5f 7365 7427  ion_boolean_set'
+00352380: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
+00352390: 6f6e 7465 7874 5f63 7963 6c65 5f61 7272  ontext_cycle_arr
+003523a0: 6179 3a20 2762 6c5f 6f70 6572 6174 6f72  ay: 'bl_operator
+003523b0: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
+003523c0: 7874 5f63 7963 6c65 5f61 7272 6179 2720  xt_cycle_array' 
+003523d0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
+003523e0: 6e74 6578 745f 6379 636c 655f 656e 756d  ntext_cycle_enum
+003523f0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00352400: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+00352410: 5f63 7963 6c65 5f65 6e75 6d27 203d 204e  _cycle_enum' = N
+00352420: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00352430: 7874 5f63 7963 6c65 5f69 6e74 3a20 2762  xt_cycle_int: 'b
+00352440: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00352450: 4d5f 4f54 5f63 6f6e 7465 7874 5f63 7963  M_OT_context_cyc
+00352460: 6c65 5f69 6e74 2720 3d20 4e6f 6e65 0a0a  le_int' = None..
+00352470: 574d 5f4f 545f 636f 6e74 6578 745f 6d65  WM_OT_context_me
+00352480: 6e75 5f65 6e75 6d3a 2027 626c 5f6f 7065  nu_enum: 'bl_ope
+00352490: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+003524a0: 636f 6e74 6578 745f 6d65 6e75 5f65 6e75  context_menu_enu
+003524b0: 6d27 203d 204e 6f6e 650a 0a57 4d5f 4f54  m' = None..WM_OT
+003524c0: 5f63 6f6e 7465 7874 5f6d 6f64 616c 5f6d  _context_modal_m
+003524d0: 6f75 7365 3a20 2762 6c5f 6f70 6572 6174  ouse: 'bl_operat
+003524e0: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+003524f0: 7465 7874 5f6d 6f64 616c 5f6d 6f75 7365  text_modal_mouse
+00352500: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+00352510: 636f 6e74 6578 745f 7069 655f 656e 756d  context_pie_enum
+00352520: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00352530: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+00352540: 5f70 6965 5f65 6e75 6d27 203d 204e 6f6e  _pie_enum' = Non
+00352550: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
+00352560: 5f73 6361 6c65 5f66 6c6f 6174 3a20 2762  _scale_float: 'b
+00352570: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00352580: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6361  M_OT_context_sca
+00352590: 6c65 5f66 6c6f 6174 2720 3d20 4e6f 6e65  le_float' = None
+003525a0: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
+003525b0: 7363 616c 655f 696e 743a 2027 626c 5f6f  scale_int: 'bl_o
+003525c0: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+003525d0: 545f 636f 6e74 6578 745f 7363 616c 655f  T_context_scale_
+003525e0: 696e 7427 203d 204e 6f6e 650a 0a57 4d5f  int' = None..WM_
+003525f0: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f62  OT_context_set_b
+00352600: 6f6f 6c65 616e 3a20 2762 6c5f 6f70 6572  oolean: 'bl_oper
+00352610: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
+00352620: 6f6e 7465 7874 5f73 6574 5f62 6f6f 6c65  ontext_set_boole
+00352630: 616e 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  an' = None..WM_O
+00352640: 545f 636f 6e74 6578 745f 7365 745f 656e  T_context_set_en
+00352650: 756d 3a20 2762 6c5f 6f70 6572 6174 6f72  um: 'bl_operator
+00352660: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
+00352670: 7874 5f73 6574 5f65 6e75 6d27 203d 204e  xt_set_enum' = N
+00352680: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00352690: 7874 5f73 6574 5f66 6c6f 6174 3a20 2762  xt_set_float: 'b
+003526a0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+003526b0: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
+003526c0: 5f66 6c6f 6174 2720 3d20 4e6f 6e65 0a0a  _float' = None..
+003526d0: 574d 5f4f 545f 636f 6e74 6578 745f 7365  WM_OT_context_se
+003526e0: 745f 6964 3a20 2762 6c5f 6f70 6572 6174  t_id: 'bl_operat
+003526f0: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+00352700: 7465 7874 5f73 6574 5f69 6427 203d 204e  text_set_id' = N
+00352710: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00352720: 7874 5f73 6574 5f69 6e74 3a20 2762 6c5f  xt_set_int: 'bl_
+00352730: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00352740: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f69  OT_context_set_i
+00352750: 6e74 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  nt' = None..WM_O
+00352760: 545f 636f 6e74 6578 745f 7365 745f 7374  T_context_set_st
+00352770: 7269 6e67 3a20 2762 6c5f 6f70 6572 6174  ring: 'bl_operat
+00352780: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+00352790: 7465 7874 5f73 6574 5f73 7472 696e 6727  text_set_string'
+003527a0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
+003527b0: 6f6e 7465 7874 5f73 6574 5f76 616c 7565  ontext_set_value
+003527c0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+003527d0: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+003527e0: 5f73 6574 5f76 616c 7565 2720 3d20 4e6f  _set_value' = No
+003527f0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
+00352800: 745f 746f 6767 6c65 3a20 2762 6c5f 6f70  t_toggle: 'bl_op
+00352810: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00352820: 5f63 6f6e 7465 7874 5f74 6f67 676c 6527  _context_toggle'
+00352830: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
+00352840: 6f6e 7465 7874 5f74 6f67 676c 655f 656e  ontext_toggle_en
+00352850: 756d 3a20 2762 6c5f 6f70 6572 6174 6f72  um: 'bl_operator
+00352860: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
+00352870: 7874 5f74 6f67 676c 655f 656e 756d 2720  xt_toggle_enum' 
+00352880: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 646f  = None..WM_OT_do
+00352890: 635f 7669 6577 3a20 2762 6c5f 6f70 6572  c_view: 'bl_oper
+003528a0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f64  ators.wm.WM_OT_d
+003528b0: 6f63 5f76 6965 7727 203d 204e 6f6e 650a  oc_view' = None.
+003528c0: 0a57 4d5f 4f54 5f64 6f63 5f76 6965 775f  .WM_OT_doc_view_
+003528d0: 6d61 6e75 616c 3a20 2762 6c5f 6f70 6572  manual: 'bl_oper
+003528e0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f64  ators.wm.WM_OT_d
+003528f0: 6f63 5f76 6965 775f 6d61 6e75 616c 2720  oc_view_manual' 
+00352900: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 6472  = None..WM_OT_dr
+00352910: 6f70 5f62 6c65 6e64 5f66 696c 653a 2027  op_blend_file: '
+00352920: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+00352930: 574d 5f4f 545f 6472 6f70 5f62 6c65 6e64  WM_OT_drop_blend
+00352940: 5f66 696c 6527 203d 204e 6f6e 650a 0a57  _file' = None..W
+00352950: 4d5f 4f54 5f6f 7065 7261 746f 725f 6368  M_OT_operator_ch
+00352960: 6561 745f 7368 6565 743a 2027 626c 5f6f  eat_sheet: 'bl_o
+00352970: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+00352980: 545f 6f70 6572 6174 6f72 5f63 6865 6174  T_operator_cheat
+00352990: 5f73 6865 6574 2720 3d20 4e6f 6e65 0a0a  _sheet' = None..
+003529a0: 574d 5f4f 545f 6f70 6572 6174 6f72 5f70  WM_OT_operator_p
+003529b0: 6965 5f65 6e75 6d3a 2027 626c 5f6f 7065  ie_enum: 'bl_ope
+003529c0: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+003529d0: 6f70 6572 6174 6f72 5f70 6965 5f65 6e75  operator_pie_enu
+003529e0: 6d27 203d 204e 6f6e 650a 0a57 4d5f 4f54  m' = None..WM_OT
+003529f0: 5f6f 776e 6572 5f64 6973 6162 6c65 3a20  _owner_disable: 
 00352a00: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00352a10: 2e57 4d5f 4f54 5f70 6174 685f 6f70 656e  .WM_OT_path_open
-00352a20: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00352a30: 7072 6576 6965 7773 5f62 6174 6368 5f63  previews_batch_c
-00352a40: 6c65 6172 3a20 2762 6c5f 6f70 6572 6174  lear: 'bl_operat
-00352a50: 6f72 732e 6669 6c65 2e57 4d5f 4f54 5f70  ors.file.WM_OT_p
-00352a60: 7265 7669 6577 735f 6261 7463 685f 636c  reviews_batch_cl
-00352a70: 6561 7227 203d 204e 6f6e 650a 0a57 4d5f  ear' = None..WM_
-00352a80: 4f54 5f70 7265 7669 6577 735f 6261 7463  OT_previews_batc
-00352a90: 685f 6765 6e65 7261 7465 3a20 2762 6c5f  h_generate: 'bl_
-00352aa0: 6f70 6572 6174 6f72 732e 6669 6c65 2e57  operators.file.W
-00352ab0: 4d5f 4f54 5f70 7265 7669 6577 735f 6261  M_OT_previews_ba
-00352ac0: 7463 685f 6765 6e65 7261 7465 2720 3d20  tch_generate' = 
-00352ad0: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6f70  None..WM_OT_prop
-00352ae0: 6572 7469 6573 5f61 6464 3a20 2762 6c5f  erties_add: 'bl_
-00352af0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00352b00: 4f54 5f70 726f 7065 7274 6965 735f 6164  OT_properties_ad
-00352b10: 6427 203d 204e 6f6e 650a 0a57 4d5f 4f54  d' = None..WM_OT
-00352b20: 5f70 726f 7065 7274 6965 735f 636f 6e74  _properties_cont
-00352b30: 6578 745f 6368 616e 6765 3a20 2762 6c5f  ext_change: 'bl_
-00352b40: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00352b50: 4f54 5f70 726f 7065 7274 6965 735f 636f  OT_properties_co
-00352b60: 6e74 6578 745f 6368 616e 6765 2720 3d20  ntext_change' = 
-00352b70: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6f70  None..WM_OT_prop
-00352b80: 6572 7469 6573 5f65 6469 743a 2027 626c  erties_edit: 'bl
-00352b90: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-00352ba0: 5f4f 545f 7072 6f70 6572 7469 6573 5f65  _OT_properties_e
-00352bb0: 6469 7427 203d 204e 6f6e 650a 0a57 4d5f  dit' = None..WM_
-00352bc0: 4f54 5f70 726f 7065 7274 6965 735f 6564  OT_properties_ed
-00352bd0: 6974 5f76 616c 7565 3a20 2762 6c5f 6f70  it_value: 'bl_op
-00352be0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00352bf0: 5f70 726f 7065 7274 6965 735f 6564 6974  _properties_edit
-00352c00: 5f76 616c 7565 2720 3d20 4e6f 6e65 0a0a  _value' = None..
-00352c10: 574d 5f4f 545f 7072 6f70 6572 7469 6573  WM_OT_properties
-00352c20: 5f72 656d 6f76 653a 2027 626c 5f6f 7065  _remove: 'bl_ope
-00352c30: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-00352c40: 7072 6f70 6572 7469 6573 5f72 656d 6f76  properties_remov
-00352c50: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
-00352c60: 5f73 7973 696e 666f 3a20 2762 6c5f 6f70  _sysinfo: 'bl_op
-00352c70: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00352c80: 5f73 7973 696e 666f 2720 3d20 4e6f 6e65  _sysinfo' = None
-00352c90: 0a0a 574d 5f4f 545f 746f 6f6c 5f73 6574  ..WM_OT_tool_set
-00352ca0: 5f62 795f 6964 3a20 2762 6c5f 6f70 6572  _by_id: 'bl_oper
-00352cb0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f74  ators.wm.WM_OT_t
-00352cc0: 6f6f 6c5f 7365 745f 6279 5f69 6427 203d  ool_set_by_id' =
-00352cd0: 204e 6f6e 650a 0a57 4d5f 4f54 5f74 6f6f   None..WM_OT_too
-00352ce0: 6c5f 7365 745f 6279 5f69 6e64 6578 3a20  l_set_by_index: 
-00352cf0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00352d00: 2e57 4d5f 4f54 5f74 6f6f 6c5f 7365 745f  .WM_OT_tool_set_
-00352d10: 6279 5f69 6e64 6578 2720 3d20 4e6f 6e65  by_index' = None
-00352d20: 0a0a 574d 5f4f 545f 746f 6f6c 6261 723a  ..WM_OT_toolbar:
-00352d30: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00352d40: 6d2e 574d 5f4f 545f 746f 6f6c 6261 7227  m.WM_OT_toolbar'
-00352d50: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f74   = None..WM_OT_t
-00352d60: 6f6f 6c62 6172 5f66 616c 6c62 6163 6b5f  oolbar_fallback_
-00352d70: 7069 653a 2027 626c 5f6f 7065 7261 746f  pie: 'bl_operato
-00352d80: 7273 2e77 6d2e 574d 5f4f 545f 746f 6f6c  rs.wm.WM_OT_tool
-00352d90: 6261 725f 6661 6c6c 6261 636b 5f70 6965  bar_fallback_pie
-00352da0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00352db0: 746f 6f6c 6261 725f 7072 6f6d 7074 3a20  toolbar_prompt: 
-00352dc0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00352dd0: 2e57 4d5f 4f54 5f74 6f6f 6c62 6172 5f70  .WM_OT_toolbar_p
-00352de0: 726f 6d70 7427 203d 204e 6f6e 650a 0a57  rompt' = None..W
-00352df0: 4d5f 4f54 5f75 726c 5f6f 7065 6e3a 2027  M_OT_url_open: '
-00352e00: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00352e10: 574d 5f4f 545f 7572 6c5f 6f70 656e 2720  WM_OT_url_open' 
-00352e20: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7572  = None..WM_OT_ur
-00352e30: 6c5f 6f70 656e 5f70 7265 7365 743a 2027  l_open_preset: '
-00352e40: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00352e50: 574d 5f4f 545f 7572 6c5f 6f70 656e 5f70  WM_OT_url_open_p
-00352e60: 7265 7365 7427 203d 204e 6f6e 650a 0a57  reset' = None..W
-00352e70: 4f52 4b53 5041 4345 5f50 545f 6164 646f  ORKSPACE_PT_addo
-00352e80: 6e73 3a20 2762 6c5f 7569 2e70 726f 7065  ns: 'bl_ui.prope
-00352e90: 7274 6965 735f 776f 726b 7370 6163 652e  rties_workspace.
-00352ea0: 574f 524b 5350 4143 455f 5054 5f61 6464  WORKSPACE_PT_add
-00352eb0: 6f6e 7327 203d 204e 6f6e 650a 0a57 4f52  ons' = None..WOR
-00352ec0: 4b53 5041 4345 5f50 545f 6375 7374 6f6d  KSPACE_PT_custom
-00352ed0: 5f70 726f 7073 3a20 2762 6c5f 7569 2e70  _props: 'bl_ui.p
-00352ee0: 726f 7065 7274 6965 735f 776f 726b 7370  roperties_worksp
-00352ef0: 6163 652e 574f 524b 5350 4143 455f 5054  ace.WORKSPACE_PT
-00352f00: 5f63 7573 746f 6d5f 7072 6f70 7327 203d  _custom_props' =
-00352f10: 204e 6f6e 650a 0a57 4f52 4b53 5041 4345   None..WORKSPACE
-00352f20: 5f50 545f 6d61 696e 3a20 2762 6c5f 7569  _PT_main: 'bl_ui
-00352f30: 2e70 726f 7065 7274 6965 735f 776f 726b  .properties_work
-00352f40: 7370 6163 652e 574f 524b 5350 4143 455f  space.WORKSPACE_
-00352f50: 5054 5f6d 6169 6e27 203d 204e 6f6e 650a  PT_main' = None.
-00352f60: 0a57 4f52 4c44 5f50 545f 636f 6e74 6578  .WORLD_PT_contex
-00352f70: 745f 776f 726c 643a 2027 626c 5f75 692e  t_world: 'bl_ui.
-00352f80: 7072 6f70 6572 7469 6573 5f77 6f72 6c64  properties_world
-00352f90: 2e57 4f52 4c44 5f50 545f 636f 6e74 6578  .WORLD_PT_contex
-00352fa0: 745f 776f 726c 6427 203d 204e 6f6e 650a  t_world' = None.
-00352fb0: 0a57 4f52 4c44 5f50 545f 6375 7374 6f6d  .WORLD_PT_custom
-00352fc0: 5f70 726f 7073 3a20 2762 6c5f 7569 2e70  _props: 'bl_ui.p
-00352fd0: 726f 7065 7274 6965 735f 776f 726c 642e  roperties_world.
-00352fe0: 574f 524c 445f 5054 5f63 7573 746f 6d5f  WORLD_PT_custom_
-00352ff0: 7072 6f70 7327 203d 204e 6f6e 650a 0a57  props' = None..W
-00353000: 4f52 4c44 5f50 545f 7669 6577 706f 7274  ORLD_PT_viewport
-00353010: 5f64 6973 706c 6179 3a20 2762 6c5f 7569  _display: 'bl_ui
-00353020: 2e70 726f 7065 7274 6965 735f 776f 726c  .properties_worl
-00353030: 642e 574f 524c 445f 5054 5f76 6965 7770  d.WORLD_PT_viewp
-00353040: 6f72 745f 6469 7370 6c61 7927 203d 204e  ort_display' = N
-00353050: 6f6e 650a                                one.
+00352a10: 2e57 4d5f 4f54 5f6f 776e 6572 5f64 6973  .WM_OT_owner_dis
+00352a20: 6162 6c65 2720 3d20 4e6f 6e65 0a0a 574d  able' = None..WM
+00352a30: 5f4f 545f 6f77 6e65 725f 656e 6162 6c65  _OT_owner_enable
+00352a40: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00352a50: 776d 2e57 4d5f 4f54 5f6f 776e 6572 5f65  wm.WM_OT_owner_e
+00352a60: 6e61 626c 6527 203d 204e 6f6e 650a 0a57  nable' = None..W
+00352a70: 4d5f 4f54 5f70 6174 685f 6f70 656e 3a20  M_OT_path_open: 
+00352a80: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00352a90: 2e57 4d5f 4f54 5f70 6174 685f 6f70 656e  .WM_OT_path_open
+00352aa0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+00352ab0: 7072 6576 6965 7773 5f62 6174 6368 5f63  previews_batch_c
+00352ac0: 6c65 6172 3a20 2762 6c5f 6f70 6572 6174  lear: 'bl_operat
+00352ad0: 6f72 732e 6669 6c65 2e57 4d5f 4f54 5f70  ors.file.WM_OT_p
+00352ae0: 7265 7669 6577 735f 6261 7463 685f 636c  reviews_batch_cl
+00352af0: 6561 7227 203d 204e 6f6e 650a 0a57 4d5f  ear' = None..WM_
+00352b00: 4f54 5f70 7265 7669 6577 735f 6261 7463  OT_previews_batc
+00352b10: 685f 6765 6e65 7261 7465 3a20 2762 6c5f  h_generate: 'bl_
+00352b20: 6f70 6572 6174 6f72 732e 6669 6c65 2e57  operators.file.W
+00352b30: 4d5f 4f54 5f70 7265 7669 6577 735f 6261  M_OT_previews_ba
+00352b40: 7463 685f 6765 6e65 7261 7465 2720 3d20  tch_generate' = 
+00352b50: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6f70  None..WM_OT_prop
+00352b60: 6572 7469 6573 5f61 6464 3a20 2762 6c5f  erties_add: 'bl_
+00352b70: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00352b80: 4f54 5f70 726f 7065 7274 6965 735f 6164  OT_properties_ad
+00352b90: 6427 203d 204e 6f6e 650a 0a57 4d5f 4f54  d' = None..WM_OT
+00352ba0: 5f70 726f 7065 7274 6965 735f 636f 6e74  _properties_cont
+00352bb0: 6578 745f 6368 616e 6765 3a20 2762 6c5f  ext_change: 'bl_
+00352bc0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00352bd0: 4f54 5f70 726f 7065 7274 6965 735f 636f  OT_properties_co
+00352be0: 6e74 6578 745f 6368 616e 6765 2720 3d20  ntext_change' = 
+00352bf0: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6f70  None..WM_OT_prop
+00352c00: 6572 7469 6573 5f65 6469 743a 2027 626c  erties_edit: 'bl
+00352c10: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+00352c20: 5f4f 545f 7072 6f70 6572 7469 6573 5f65  _OT_properties_e
+00352c30: 6469 7427 203d 204e 6f6e 650a 0a57 4d5f  dit' = None..WM_
+00352c40: 4f54 5f70 726f 7065 7274 6965 735f 6564  OT_properties_ed
+00352c50: 6974 5f76 616c 7565 3a20 2762 6c5f 6f70  it_value: 'bl_op
+00352c60: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00352c70: 5f70 726f 7065 7274 6965 735f 6564 6974  _properties_edit
+00352c80: 5f76 616c 7565 2720 3d20 4e6f 6e65 0a0a  _value' = None..
+00352c90: 574d 5f4f 545f 7072 6f70 6572 7469 6573  WM_OT_properties
+00352ca0: 5f72 656d 6f76 653a 2027 626c 5f6f 7065  _remove: 'bl_ope
+00352cb0: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+00352cc0: 7072 6f70 6572 7469 6573 5f72 656d 6f76  properties_remov
+00352cd0: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
+00352ce0: 5f73 7973 696e 666f 3a20 2762 6c5f 6f70  _sysinfo: 'bl_op
+00352cf0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00352d00: 5f73 7973 696e 666f 2720 3d20 4e6f 6e65  _sysinfo' = None
+00352d10: 0a0a 574d 5f4f 545f 746f 6f6c 5f73 6574  ..WM_OT_tool_set
+00352d20: 5f62 795f 6964 3a20 2762 6c5f 6f70 6572  _by_id: 'bl_oper
+00352d30: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f74  ators.wm.WM_OT_t
+00352d40: 6f6f 6c5f 7365 745f 6279 5f69 6427 203d  ool_set_by_id' =
+00352d50: 204e 6f6e 650a 0a57 4d5f 4f54 5f74 6f6f   None..WM_OT_too
+00352d60: 6c5f 7365 745f 6279 5f69 6e64 6578 3a20  l_set_by_index: 
+00352d70: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00352d80: 2e57 4d5f 4f54 5f74 6f6f 6c5f 7365 745f  .WM_OT_tool_set_
+00352d90: 6279 5f69 6e64 6578 2720 3d20 4e6f 6e65  by_index' = None
+00352da0: 0a0a 574d 5f4f 545f 746f 6f6c 6261 723a  ..WM_OT_toolbar:
+00352db0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00352dc0: 6d2e 574d 5f4f 545f 746f 6f6c 6261 7227  m.WM_OT_toolbar'
+00352dd0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f74   = None..WM_OT_t
+00352de0: 6f6f 6c62 6172 5f66 616c 6c62 6163 6b5f  oolbar_fallback_
+00352df0: 7069 653a 2027 626c 5f6f 7065 7261 746f  pie: 'bl_operato
+00352e00: 7273 2e77 6d2e 574d 5f4f 545f 746f 6f6c  rs.wm.WM_OT_tool
+00352e10: 6261 725f 6661 6c6c 6261 636b 5f70 6965  bar_fallback_pie
+00352e20: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+00352e30: 746f 6f6c 6261 725f 7072 6f6d 7074 3a20  toolbar_prompt: 
+00352e40: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00352e50: 2e57 4d5f 4f54 5f74 6f6f 6c62 6172 5f70  .WM_OT_toolbar_p
+00352e60: 726f 6d70 7427 203d 204e 6f6e 650a 0a57  rompt' = None..W
+00352e70: 4d5f 4f54 5f75 726c 5f6f 7065 6e3a 2027  M_OT_url_open: '
+00352e80: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+00352e90: 574d 5f4f 545f 7572 6c5f 6f70 656e 2720  WM_OT_url_open' 
+00352ea0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7572  = None..WM_OT_ur
+00352eb0: 6c5f 6f70 656e 5f70 7265 7365 743a 2027  l_open_preset: '
+00352ec0: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
+00352ed0: 574d 5f4f 545f 7572 6c5f 6f70 656e 5f70  WM_OT_url_open_p
+00352ee0: 7265 7365 7427 203d 204e 6f6e 650a 0a57  reset' = None..W
+00352ef0: 4f52 4b53 5041 4345 5f50 545f 6164 646f  ORKSPACE_PT_addo
+00352f00: 6e73 3a20 2762 6c5f 7569 2e70 726f 7065  ns: 'bl_ui.prope
+00352f10: 7274 6965 735f 776f 726b 7370 6163 652e  rties_workspace.
+00352f20: 574f 524b 5350 4143 455f 5054 5f61 6464  WORKSPACE_PT_add
+00352f30: 6f6e 7327 203d 204e 6f6e 650a 0a57 4f52  ons' = None..WOR
+00352f40: 4b53 5041 4345 5f50 545f 6375 7374 6f6d  KSPACE_PT_custom
+00352f50: 5f70 726f 7073 3a20 2762 6c5f 7569 2e70  _props: 'bl_ui.p
+00352f60: 726f 7065 7274 6965 735f 776f 726b 7370  roperties_worksp
+00352f70: 6163 652e 574f 524b 5350 4143 455f 5054  ace.WORKSPACE_PT
+00352f80: 5f63 7573 746f 6d5f 7072 6f70 7327 203d  _custom_props' =
+00352f90: 204e 6f6e 650a 0a57 4f52 4b53 5041 4345   None..WORKSPACE
+00352fa0: 5f50 545f 6d61 696e 3a20 2762 6c5f 7569  _PT_main: 'bl_ui
+00352fb0: 2e70 726f 7065 7274 6965 735f 776f 726b  .properties_work
+00352fc0: 7370 6163 652e 574f 524b 5350 4143 455f  space.WORKSPACE_
+00352fd0: 5054 5f6d 6169 6e27 203d 204e 6f6e 650a  PT_main' = None.
+00352fe0: 0a57 4f52 4c44 5f50 545f 636f 6e74 6578  .WORLD_PT_contex
+00352ff0: 745f 776f 726c 643a 2027 626c 5f75 692e  t_world: 'bl_ui.
+00353000: 7072 6f70 6572 7469 6573 5f77 6f72 6c64  properties_world
+00353010: 2e57 4f52 4c44 5f50 545f 636f 6e74 6578  .WORLD_PT_contex
+00353020: 745f 776f 726c 6427 203d 204e 6f6e 650a  t_world' = None.
+00353030: 0a57 4f52 4c44 5f50 545f 6375 7374 6f6d  .WORLD_PT_custom
+00353040: 5f70 726f 7073 3a20 2762 6c5f 7569 2e70  _props: 'bl_ui.p
+00353050: 726f 7065 7274 6965 735f 776f 726c 642e  roperties_world.
+00353060: 574f 524c 445f 5054 5f63 7573 746f 6d5f  WORLD_PT_custom_
+00353070: 7072 6f70 7327 203d 204e 6f6e 650a 0a57  props' = None..W
+00353080: 4f52 4c44 5f50 545f 7669 6577 706f 7274  ORLD_PT_viewport
+00353090: 5f64 6973 706c 6179 3a20 2762 6c5f 7569  _display: 'bl_ui
+003530a0: 2e70 726f 7065 7274 6965 735f 776f 726c  .properties_worl
+003530b0: 642e 574f 524c 445f 5054 5f76 6965 7770  d.WORLD_PT_viewp
+003530c0: 6f72 745f 6469 7370 6c61 7927 203d 204e  ort_display' = N
+003530d0: 6f6e 650a                                one.
```

### Comparing `fake-bpy-module-latest-20230420/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230421/bpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/utils/previews.py` & `fake-bpy-module-latest-20230421/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy/utils/units.py` & `fake-bpy-module-latest-20230421/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Sequence', 'bpy.types.Object', 'bpy.types.Action'],
+        Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Sequence', 'bpy.types.Object', 'bpy.types.Action']
+    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230421/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230421/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/bpy_types.py` & `fake-bpy-module-latest-20230421/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230420
+Version: 20230421
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230420/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230421/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230421/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/functions.py` & `fake-bpy-module-latest-20230421/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/predicates.py` & `fake-bpy-module-latest-20230421/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/shaders.py` & `fake-bpy-module-latest-20230421/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/types.py` & `fake-bpy-module-latest-20230421/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230421/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230421/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/capabilities.py` & `fake-bpy-module-latest-20230421/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/matrix.py` & `fake-bpy-module-latest-20230421/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/platform.py` & `fake-bpy-module-latest-20230421/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/shader.py` & `fake-bpy-module-latest-20230421/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/state.py` & `fake-bpy-module-latest-20230421/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/texture.py` & `fake-bpy-module-latest-20230421/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu/types.py` & `fake-bpy-module-latest-20230421/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu_extras/batch.py` & `fake-bpy-module-latest-20230421/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/gpu_extras/presets.py` & `fake-bpy-module-latest-20230421/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/idprop/types.py` & `fake-bpy-module-latest-20230421/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/imbuf/__init__.py` & `fake-bpy-module-latest-20230421/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/imbuf/types.py` & `fake-bpy-module-latest-20230421/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/keyingsets_builtins.py` & `fake-bpy-module-latest-20230421/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/keyingsets_utils.py` & `fake-bpy-module-latest-20230421/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/mathutils/__init__.py` & `fake-bpy-module-latest-20230421/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230421/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/mathutils/geometry.py` & `fake-bpy-module-latest-20230421/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/mathutils/kdtree.py` & `fake-bpy-module-latest-20230421/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/mathutils/noise.py` & `fake-bpy-module-latest-20230421/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/nodeitems_builtins.py` & `fake-bpy-module-latest-20230421/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/nodeitems_utils.py` & `fake-bpy-module-latest-20230421/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/rna_info.py` & `fake-bpy-module-latest-20230421/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/rna_keymap_ui.py` & `fake-bpy-module-latest-20230421/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/rna_prop_ui.py` & `fake-bpy-module-latest-20230421/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/rna_xml.py` & `fake-bpy-module-latest-20230421/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230420/setup.py` & `fake-bpy-module-latest-20230421/setup.py`

 * *Files identical despite different names*

