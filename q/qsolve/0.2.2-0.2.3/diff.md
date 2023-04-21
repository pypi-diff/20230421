# Comparing `tmp/qsolve-0.2.2.tar.gz` & `tmp/qsolve-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsolve-0.2.2.tar", last modified: Wed Apr  5 08:01:44 2023, max compression
+gzip compressed data, was "qsolve-0.2.3.tar", last modified: Fri Apr 21 08:05:23 2023, max compression
```

## Comparing `qsolve-0.2.2.tar` & `qsolve-0.2.3.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.783773 qsolve-0.2.2/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       31 2023-04-05 07:22:00.000000 qsolve-0.2.2/MANIFEST.in
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      723 2023-04-05 08:01:44.783773 qsolve-0.2.2/PKG-INFO
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      239 2023-04-03 09:09:18.000000 qsolve-0.2.2/README.md
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       38 2023-04-05 08:01:44.783773 qsolve-0.2.2/setup.cfg
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1078 2023-04-05 08:01:41.000000 qsolve-0.2.2/setup.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.763773 qsolve-0.2.2/src/
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 07:39:04.000000 qsolve-0.2.2/src/qsolve/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve/core/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       71 2023-04-05 07:10:32.000000 qsolve-0.2.2/src/qsolve/core/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    24232 2023-04-04 15:00:29.000000 qsolve-0.2.2/src/qsolve/core/qsolve_core_gpe_3d_obfs_cpython_310.pyc
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve/examples/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-03-22 10:17:33.000000 qsolve-0.2.2/src/qsolve/examples/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve/examples/examples_3d/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     9301 2023-04-03 13:29:40.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/evaluation.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.771773 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        2 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/__init__.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1527 2023-04-03 12:23:49.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_control_inputs.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_x.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1093 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xy.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1120 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xz.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1609 2023-04-03 12:20:00.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_y.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1517 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_z.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1260 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_global_phase_difference.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1235 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_number_imbalance.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)      905 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xy.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)      982 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xz.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1205 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_z_x1_x2.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1785 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_x.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1516 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_y.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1880 2023-04-03 12:23:22.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_z.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)    11931 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/figure_main.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.771773 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mystyle.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.771773 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/frames/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/frames/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11991 2023-04-05 07:41:30.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/main_ground_state_computation.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      695 2023-04-03 09:18:05.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/potential_harmonic.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.771773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     8374 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/evaluation.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.771773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.771773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        2 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/__init__.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1527 2023-04-03 12:18:30.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_control_inputs.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_x.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1101 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xy.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1128 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xz.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1609 2023-04-03 12:18:15.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_y.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1841 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_z.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1260 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_global_phase_difference.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1247 2023-04-03 12:18:45.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_number_imbalance.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)      905 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xy.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)      982 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xz.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1205 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_z_x1_x2.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)    12277 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/figure_main.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.775773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        1 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/__init__.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1212 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_mask_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_final.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1160 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1228 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_mask_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_final.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1172 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     9121 2023-03-08 11:14:48.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/figure_tof.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.775773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        1 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/__init__.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1212 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_mask_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_final.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1160 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1228 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_mask_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_final.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1172 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1263 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_mask_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1259 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1299 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_mask_tof_gpe.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1259 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_tof_gpe.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)    10384 2023-03-21 08:39:57.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/figure_tof_extended.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.775773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mystyle.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.775773 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/frames/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/frames/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    21115 2023-04-05 07:47:35.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    17753 2023-04-05 07:48:21.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    17874 2023-04-05 07:48:42.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x_box_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2138 2023-04-03 09:13:56.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1961 2023-04-03 09:22:06.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2371 2023-04-03 09:30:04.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x_box_z.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.775773 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4566 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/evaluation.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.775773 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        2 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/__init__.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     2247 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_control_inputs.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_x.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1105 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xy.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1064 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xz.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1670 2023-04-03 12:24:58.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_y.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1404 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1535 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z_eff.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1663 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1884 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z_eff.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1785 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_x.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1033 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xy.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)      940 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xz.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1516 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_y.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1880 2023-04-03 12:25:15.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_z.py
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)    11597 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/figure_main.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/colors.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/hex2rgb.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/make_cmap.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mpl_settings.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2022-06-21 06:10:24.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mystyle.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/frames/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/frames/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    13033 2023-04-05 07:48:58.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_gaussian_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12883 2023-04-05 07:49:12.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_lattice_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1369 2023-04-03 09:30:51.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_gaussian_z.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1325 2023-04-03 09:40:27.000000 qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_lattice_z.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/potentials/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-03-22 10:17:33.000000 qsolve-0.2.2/src/qsolve/potentials/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/potentials/components_3d/
--rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/box_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/gaussian_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/gaussian_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/harmonic_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/harmonic_x_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/harmonic_y_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/harmonic_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/lattice_z_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/lesanovsky_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/potentials/components_3d/tilt_x_3d.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/solvers/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       36 2023-04-05 07:40:24.000000 qsolve-0.2.2/src/qsolve/solvers/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.779773 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-04-05 07:42:19.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/__init__.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.783773 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-05 07:34:52.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      398 2023-04-04 12:58:08.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/check_python_version.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1054 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      884 2023-04-05 07:10:32.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3952 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6584 2022-06-20 07:58:38.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2022-06-03 13:20:46.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1980 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      637 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      159 2022-06-13 07:38:04.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_seed.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-04-04 12:22:35.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_time_evolution.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1897 2022-06-13 07:38:04.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      489 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/n_atoms.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2022-06-03 14:12:07.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_V.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2022-06-13 07:38:04.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_psi.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3308 2023-04-05 07:46:54.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1531 2023-04-03 09:09:18.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1110 2022-03-22 10:17:33.000000 qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.783773 qsolve-0.2.2/src/qsolve/utils/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2022-03-22 10:17:33.000000 qsolve-0.2.2/src/qsolve/utils/__init__.py
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      843 2022-03-22 10:17:33.000000 qsolve-0.2.2/src/qsolve/utils/primes.py
-drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-05 08:01:44.767773 qsolve-0.2.2/src/qsolve.egg-info/
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      723 2023-04-05 08:01:44.000000 qsolve-0.2.2/src/qsolve.egg-info/PKG-INFO
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11786 2023-04-05 08:01:44.000000 qsolve-0.2.2/src/qsolve.egg-info/SOURCES.txt
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-05 08:01:44.000000 qsolve-0.2.2/src/qsolve.egg-info/dependency_links.txt
--rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        7 2023-04-05 08:01:44.000000 qsolve-0.2.2/src/qsolve.egg-info/top_level.txt
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.830443 qsolve-0.2.3/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       30 2023-04-21 08:03:18.000000 qsolve-0.2.3/MANIFEST.in
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      674 2023-04-21 08:05:23.830443 qsolve-0.2.3/PKG-INFO
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      190 2023-04-05 08:16:01.000000 qsolve-0.2.3/README.md
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       38 2023-04-21 08:05:23.830443 qsolve-0.2.3/setup.cfg
+-rwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)     1078 2023-04-21 08:03:36.000000 qsolve-0.2.3/setup.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.810443 qsolve-0.2.3/src/
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.810443 qsolve-0.2.3/src/qsolve/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.814443 qsolve-0.2.3/src/qsolve/core/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      108 2023-04-21 07:31:36.000000 qsolve-0.2.3/src/qsolve/core/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)  1085248 2023-04-21 07:30:52.000000 qsolve-0.2.3/src/qsolve/core/qsolve_core_gpe_3d.cpython-310-x86_64-linux-gnu.so
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.814443 qsolve-0.2.3/src/qsolve/examples/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.814443 qsolve-0.2.3/src/qsolve/examples/examples_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.814443 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     9301 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/evaluation.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.814443 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.818443 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        2 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1527 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_control_inputs.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1093 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xy.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1120 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xz.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1609 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_y.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1517 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1260 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_global_phase_difference.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1235 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_number_imbalance.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      905 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xy.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      982 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xz.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1205 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_z_x1_x2.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1785 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1516 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_y.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1880 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11931 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/figure_main.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.818443 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/colors.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/hex2rgb.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/make_cmap.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mpl_settings.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mystyle.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.818443 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/frames/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/frames/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12111 2023-04-21 07:30:52.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/main_ground_state_computation.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      695 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/potential_harmonic.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.818443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     8374 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/evaluation.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.818443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.822443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        2 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1527 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_control_inputs.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1101 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xy.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1128 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xz.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1609 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_y.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1841 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1260 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_global_phase_difference.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1247 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_number_imbalance.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      905 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xy.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      982 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xz.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1205 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_z_x1_x2.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12277 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/figure_main.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.822443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1212 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_mask_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_final.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1160 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1228 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_mask_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_final.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1172 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     9121 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/figure_tof.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.822443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1212 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_mask_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_final.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1160 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1228 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_mask_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1216 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_final.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1172 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1263 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_mask_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1259 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1299 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_mask_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1259 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_tof_gpe.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    10384 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/figure_tof_extended.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.822443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/colors.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/hex2rgb.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/make_cmap.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mpl_settings.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mystyle.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.822443 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/frames/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/frames/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    21115 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_tilt_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    17753 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    17874 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x_box_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2138 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_tilt_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1961 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2371 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x_box_z.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.826443 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4566 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/evaluation.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.826443 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.826443 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        2 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2247 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_control_inputs.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1466 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1105 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xy.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1064 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xz.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1670 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_y.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1404 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1535 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z_eff.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1663 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1884 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z_eff.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1785 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_x.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1033 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xy.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      940 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xz.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1516 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_y.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1880 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11597 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/figure_main.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.826443 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4527 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/colors.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      225 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/hex2rgb.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1502 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/make_cmap.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1279 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mpl_settings.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     4727 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mystyle.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.826443 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/frames/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/frames/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    13033 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_gaussian_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    12883 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_lattice_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1369 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_gaussian_z.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1325 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_lattice_z.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.826443 qsolve-0.2.3/src/qsolve/potentials/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.830443 qsolve-0.2.3/src/qsolve/potentials/components_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      194 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/box_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      285 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/gaussian_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      126 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/gaussian_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      192 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/harmonic_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/harmonic_x_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/harmonic_y_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      116 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/harmonic_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      160 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/lattice_z_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     2746 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/lesanovsky_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3134 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       64 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/potentials/components_3d/tilt_x_3d.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.830443 qsolve-0.2.3/src/qsolve/solvers/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       36 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.830443 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       53 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/__init__.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.830443 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      398 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/check_python_version.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1054 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      884 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1985 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3952 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     6584 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      537 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1980 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      637 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      159 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_seed.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      461 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_time_evolution.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1897 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      489 2023-04-19 10:18:35.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/n_atoms.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)       83 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_V.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      374 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/set_psi.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     3308 2023-04-19 10:17:25.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1531 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)     1110 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.830443 qsolve-0.2.3/src/qsolve/utils/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/utils/__init__.py
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      843 2023-04-06 16:50:20.000000 qsolve-0.2.3/src/qsolve/utils/primes.py
+drwxrwxr-x   0 jfmennemann  (1000) jfmennemann  (1000)        0 2023-04-21 08:05:23.814443 qsolve-0.2.3/src/qsolve.egg-info/
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)      674 2023-04-21 08:05:23.000000 qsolve-0.2.3/src/qsolve.egg-info/PKG-INFO
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)    11797 2023-04-21 08:05:23.000000 qsolve-0.2.3/src/qsolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        1 2023-04-21 08:05:23.000000 qsolve-0.2.3/src/qsolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 jfmennemann  (1000) jfmennemann  (1000)        7 2023-04-21 08:05:23.000000 qsolve-0.2.3/src/qsolve.egg-info/top_level.txt
```

### Comparing `qsolve-0.2.2/PKG-INFO` & `qsolve-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: qsolve
-Version: 0.2.2
+Version: 0.2.3
 Summary: Numerical methods for the simulation of ultracold atom experiments
 Home-page: https://github.com/jfmennemann/qsolve
 Author: Jan-Frederik Mennemann
 Author-email: jfmennemann@gmx.de
 Keywords: ultracold atoms,simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 
 # QSolve
 
 QSolve provides numerical methods for the simulation of ultracold quantum gases
 at zero and finite temperature.
-Qsolve is written in the Python programming language and makes heavy use of the
-PyTorch machine learning framework.
 
+# Requirements
+
+Python 3.10
+
+# Getting Started
+
+pip install qsolve
```

### Comparing `qsolve-0.2.2/setup.py` & `qsolve-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     
     long_description = fh.read()
 
 
 setuptools.setup(
     name="qsolve",
-    version="0.2.2",
+    version="0.2.3",
     url = "https://github.com/jfmennemann/qsolve",
     author="Jan-Frederik Mennemann",
     author_email="jfmennemann@gmx.de",
     description="Numerical methods for the simulation of ultracold atom experiments",
     # long_description=read('README.md'),
     long_description=long_description,
     # long_description_content_type='text/markdown',
```

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/evaluation.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_control_inputs.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_control_inputs.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xy.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xy.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xz.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_xz.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_y.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_y.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_density_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_global_phase_difference.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_global_phase_difference.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_number_imbalance.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_number_imbalance.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xy.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xy.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xz.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_xz.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_z_x1_x2.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_phase_difference_z_x1_x2.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_y.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_y.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/fig_real_part_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/figure_main.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/figure_main/figure_main.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/colors.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/colors.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/make_cmap.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/make_cmap.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mpl_settings.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mpl_settings.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mystyle.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/figures/style/mystyle.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/main_ground_state_computation.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/main_ground_state_computation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 from figures.figure_main.figure_main import FigureMain
 
 from potential_harmonic import Potential
 
 from evaluation import eval_data
 
+from time import time
+
 
 # -------------------------------------------------------------------------------------------------
 num_threads_cpu = 8
 
 os.environ["OMP_NUM_THREADS"] = str(num_threads_cpu)
 os.environ["MKL_NUM_THREADS"] = str(num_threads_cpu)
 
@@ -205,16 +207,24 @@
 u2_0 = u2_of_times[0]
 
 solver.set_V(u=[u1_0, u2_0])
 # -------------------------------------------------------------------------------------------------
 
 
 # -------------------------------------------------------------------------------------------------
+time_1 = time()
+
 solver.compute_ground_state_solution(N=N, n_iter=20000, tau=0.001e-3, adaptive_tau=True)
 
+time_2 = time()
+
+print('elapsed time: {0:f}'.format(time_2 - time_1))
+
+input()
+
 psi_0 = solver.get('psi_0')
 
 N_psi_0 = solver.compute_n_atoms('psi_0')
 mue_psi_0 = solver.compute_chemical_potential('psi_0')
 E_psi_0 = solver.compute_E_total('psi_0')
 
 vec_res = solver.get('vec_res_ground_state_computation')
```

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/ground_state_computation/potential_harmonic.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/ground_state_computation/potential_harmonic.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/evaluation.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/evaluation.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_control_inputs.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_control_inputs.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xy.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xy.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xz.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_xz.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_y.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_y.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_density_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_global_phase_difference.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_global_phase_difference.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_number_imbalance.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_number_imbalance.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xy.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xy.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xz.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_xz.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_z_x1_x2.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/fig_phase_difference_z_x1_x2.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/figure_main.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_main/figure_main.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_mask_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_mask_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_final.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_final.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xy_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_mask_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_mask_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_final.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_final.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/fig_density_xz_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/figure_tof.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof/figure_tof.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_mask_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_mask_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_final.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_final.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xy_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_mask_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_mask_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_final.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_final.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_density_xz_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_mask_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_mask_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xy_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_mask_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_mask_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_tof_gpe.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/fig_spectrum_abs_xz_tof_gpe.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/figure_tof_extended.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/figure_tof_extended/figure_tof_extended.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/colors.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/colors.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/make_cmap.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/make_cmap.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mpl_settings.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mpl_settings.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mystyle.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/figures/style/mystyle.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_tilt_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_tilt_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x_box_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/main_lesanovsky_xy_tilt_x_box_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_tilt_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_tilt_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x_box_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/josephson_junctions/potential_lesanovsky_xy_tilt_x_box_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/evaluation.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/evaluation.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_control_inputs.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_control_inputs.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xy.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xy.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xz.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_xz.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_y.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_y.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z_eff.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_density_z_eff.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z_eff.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_phase_z_eff.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_x.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_x.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xy.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xy.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xz.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_xz.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_y.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_y.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/fig_real_part_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/figure_main.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/figure_main/figure_main.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/colors.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/colors.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/make_cmap.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/make_cmap.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mpl_settings.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mpl_settings.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mystyle.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/figures/style/mystyle.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_gaussian_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_gaussian_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_lattice_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/main_harmonic_xy_lattice_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_gaussian_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_gaussian_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_lattice_z.py` & `qsolve-0.2.3/src/qsolve/examples/examples_3d/quasi_1d_problems/potential_harmonic_xy_lattice_z.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/potentials/components_3d/lesanovsky_3d.py` & `qsolve-0.2.3/src/qsolve/potentials/components_3d/lesanovsky_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py` & `qsolve-0.2.3/src/qsolve/potentials/components_3d/lesanovsky_xy_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/chemical_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/compute_ground_state_solution.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/densities.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/energies.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/getter_functions.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_device.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_grid_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_potential.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/init_units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/solver_gpe_3d.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/spectrum.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py` & `qsolve-0.2.3/src/qsolve/solvers/solvers_3d/solver_gpe_3d/units.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve/utils/primes.py` & `qsolve-0.2.3/src/qsolve/utils/primes.py`

 * *Files identical despite different names*

### Comparing `qsolve-0.2.2/src/qsolve.egg-info/PKG-INFO` & `qsolve-0.2.3/src/qsolve.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: qsolve
-Version: 0.2.2
+Version: 0.2.3
 Summary: Numerical methods for the simulation of ultracold atom experiments
 Home-page: https://github.com/jfmennemann/qsolve
 Author: Jan-Frederik Mennemann
 Author-email: jfmennemann@gmx.de
 Keywords: ultracold atoms,simulations,Gross-Pitaevskii equation,thermal state sampling,time of flight
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 
 # QSolve
 
 QSolve provides numerical methods for the simulation of ultracold quantum gases
 at zero and finite temperature.
-Qsolve is written in the Python programming language and makes heavy use of the
-PyTorch machine learning framework.
 
+# Requirements
+
+Python 3.10
+
+# Getting Started
+
+pip install qsolve
```

### Comparing `qsolve-0.2.2/src/qsolve.egg-info/SOURCES.txt` & `qsolve-0.2.3/src/qsolve.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup.py
 src/qsolve/__init__.py
 src/qsolve.egg-info/PKG-INFO
 src/qsolve.egg-info/SOURCES.txt
 src/qsolve.egg-info/dependency_links.txt
 src/qsolve.egg-info/top_level.txt
 src/qsolve/core/__init__.py
-src/qsolve/core/qsolve_core_gpe_3d_obfs_cpython_310.pyc
+src/qsolve/core/qsolve_core_gpe_3d.cpython-310-x86_64-linux-gnu.so
 src/qsolve/examples/__init__.py
 src/qsolve/examples/examples_3d/__init__.py
 src/qsolve/examples/examples_3d/ground_state_computation/__init__.py
 src/qsolve/examples/examples_3d/ground_state_computation/evaluation.py
 src/qsolve/examples/examples_3d/ground_state_computation/main_ground_state_computation.py
 src/qsolve/examples/examples_3d/ground_state_computation/potential_harmonic.py
 src/qsolve/examples/examples_3d/ground_state_computation/figures/__init__.py
```

