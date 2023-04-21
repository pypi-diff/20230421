# Comparing `tmp/theseus-ai-nightly-2023.4.12.tar.gz` & `tmp/theseus-ai-nightly-2023.4.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theseus-ai-nightly-2023.4.12.tar", last modified: Wed Apr 12 22:35:58 2023, max compression
+gzip compressed data, was "theseus-ai-nightly-2023.4.21.tar", last modified: Fri Apr 21 20:16:07 2023, max compression
```

## Comparing `theseus-ai-nightly-2023.4.12.tar` & `theseus-ai-nightly-2023.4.21.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11642 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11035 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.756432 theseus-ai-nightly-2023.4.12/examples/
--rw-r--r--   0 root         (0) root         (0)      179 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/examples/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7193 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/backward_modes.py
--rw-r--r--   0 root         (0) root         (0)     8158 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/bundle_adjustment.py
--rw-r--r--   0 root         (0) root         (0)    19017 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/homography_estimation.py
--rw-r--r--   0 root         (0) root         (0)     9181 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/examples/motion_planning_2d.py
--rw-r--r--   0 root         (0) root         (0)     2352 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/se2_inverse.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/examples/se2_planning.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/simple_example.py
--rw-r--r--   0 root         (0) root         (0)    12290 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/state_estimation_2d.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/examples/tactile_pose_estimation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.756432 theseus-ai-nightly-2023.4.12/requirements/
--rw-r--r--   0 root         (0) root         (0)      192 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/requirements/main.txt
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6284 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.760433 theseus-ai-nightly-2023.4.12/tests/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.760433 theseus-ai-nightly-2023.4.12/tests/core/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/common.py
--rw-r--r--   0 root         (0) root         (0)    13514 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_cost_weight.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_manifold.py
--rw-r--r--   0 root         (0) root         (0)    19419 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_objective.py
--rw-r--r--   0 root         (0) root         (0)     5416 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_robust_cost.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_variable.py
--rw-r--r--   0 root         (0) root         (0)    14670 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/core/test_vectorizer.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.764433 theseus-ai-nightly-2023.4.12/tests/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho_simple.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_cusolver_lu_solver.py
--rw-r--r--   0 root         (0) root         (0)     4409 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/extlib/test_mat_mult.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.764433 theseus-ai-nightly-2023.4.12/tests/geometry/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19548 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/common.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/point_types_mypy_check.py
--rw-r--r--   0 root         (0) root         (0)     4561 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_point_types.py
--rw-r--r--   0 root         (0) root         (0)     8862 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_se2.py
--rw-r--r--   0 root         (0) root         (0)    12861 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_se3.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_so2.py
--rw-r--r--   0 root         (0) root         (0)    10391 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_so3.py
--rw-r--r--   0 root         (0) root         (0)     7443 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/geometry/test_vector.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/tests/test_dlm_perturbation.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/tests/test_pgo_benchmark.py
--rw-r--r--   0 root         (0) root         (0)    21069 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/tests/test_theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.764433 theseus-ai-nightly-2023.4.12/theseus/
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/core/
--rw-r--r--   0 root         (0) root         (0)      624 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15935 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/cost_function.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/cost_weight.py
--rw-r--r--   0 root         (0) root         (0)    30933 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/core/objective.py
--rw-r--r--   0 root         (0) root         (0)     6131 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/robust_cost_function.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/robust_loss.py
--rw-r--r--   0 root         (0) root         (0)     6417 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/theseus_function.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/variable.py
--rw-r--r--   0 root         (0) root         (0)    20067 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/core/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/
--rw-r--r--   0 root         (0) root         (0)      581 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/
--rw-r--r--   0 root         (0) root         (0)      329 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3616 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/collision.py
--rw-r--r--   0 root         (0) root         (0)     4906 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/eff_obj_contact.py
--rw-r--r--   0 root         (0) root         (0)     9043 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/collision/signed_distance_field.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/
--rw-r--r--   0 root         (0) root         (0)      257 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/kinematics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.768433 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/
--rw-r--r--   0 root         (0) root         (0)      301 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/between.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/moving_frame_between.py
--rw-r--r--   0 root         (0) root         (0)     4090 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/reprojection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.772433 theseus-ai-nightly-2023.4.12/theseus/embodied/misc/
--rw-r--r--   0 root         (0) root         (0)      213 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/misc/local_cost_fn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.772433 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/
--rw-r--r--   0 root         (0) root         (0)      365 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7715 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/double_integrator.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/misc.py
--rw-r--r--   0 root         (0) root         (0)    11526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.772433 theseus-ai-nightly-2023.4.12/theseus/extlib/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3751 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.h
--rw-r--r--   0 root         (0) root         (0)    12381 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver_cuda.cu
--rw-r--r--   0 root         (0) root         (0)    16013 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_lu_solver.cpp
--rw-r--r--   0 root         (0) root         (0)     3140 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.cpp
--rw-r--r--   0 root         (0) root         (0)      744 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.h
--rw-r--r--   0 root         (0) root         (0)    14555 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/mat_mult.cu
--rw-r--r--   0 root         (0) root         (0)     1186 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/extlib/utils.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.776433 theseus-ai-nightly-2023.4.12/theseus/geometry/
--rw-r--r--   0 root         (0) root         (0)      911 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group_check.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/manifold.py
--rw-r--r--   0 root         (0) root         (0)     7322 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/point_types.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/se2.py
--rw-r--r--   0 root         (0) root         (0)    29506 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/se3.py
--rw-r--r--   0 root         (0) root         (0)    11359 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/so2.py
--rw-r--r--   0 root         (0) root         (0)    25233 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/so3.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/utils.py
--rw-r--r--   0 root         (0) root         (0)     9405 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/geometry/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.776433 theseus-ai-nightly-2023.4.12/theseus/labs/
--rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.776433 theseus-ai-nightly-2023.4.12/theseus/labs/lie/
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.780433 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/
--rw-r--r--   0 root         (0) root         (0)      247 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/constants.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/lie_group.py
--rw-r--r--   0 root         (0) root         (0)    34776 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/se3_impl.py
--rw-r--r--   0 root         (0) root         (0)    30196 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/so3_impl.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/utils.py
--rw-r--r--   0 root         (0) root         (0)    17619 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/lie_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/labs/lie/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.780433 theseus-ai-nightly-2023.4.12/theseus/optimizer/
--rw-r--r--   0 root         (0) root         (0)      505 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.780433 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/
--rw-r--r--   0 root         (0) root         (0)      454 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/baspacho_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/cholmod_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/common.py
--rw-r--r--   0 root         (0) root         (0)     7572 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
--rw-r--r--   0 root         (0) root         (0)     2691 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/dense_linearization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.784433 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/
--rw-r--r--   0 root         (0) root         (0)      520 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5161 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/baspacho_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/cholmod_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     5681 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/dense_solver.py
--rw-r--r--   0 root         (0) root         (0)     2630 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_solver.py
--rw-r--r--   0 root         (0) root         (0)     6892 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/lu_cuda_sparse_solver.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/utils.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linear_system.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/linearization.py
--rw-r--r--   0 root         (0) root         (0)     6184 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/manifold_gaussian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.784433 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/
--rw-r--r--   0 root         (0) root         (0)      584 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8241 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dcem.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dogleg.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/gauss_newton.py
--rw-r--r--   0 root         (0) root         (0)     7009 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/levenberg_marquardt.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_least_squares.py
--rw-r--r--   0 root         (0) root         (0)    10762 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/trust_region.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     8226 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/sparse_linearization.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/optimizer/variable_ordering.py
--rw-r--r--   0 root         (0) root         (0)    12958 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/theseus_layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.784433 theseus-ai-nightly-2023.4.12/theseus/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28031 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/easyaug.py
--rwxr-xr-x   0 root         (0) root         (0)     6703 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/lml.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/third_party/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/
--rw-r--r--   0 root         (0) root         (0)      244 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12392 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/data.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/
--rw-r--r--   0 root         (0) root         (0)      435 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9168 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/misc.py
--rw-r--r--   0 root         (0) root         (0)     9771 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/models.py
--rw-r--r--   0 root         (0) root         (0)    19745 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/motion_planner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/
--rw-r--r--   0 root         (0) root         (0)      308 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16407 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.788433 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/
--rw-r--r--   0 root         (0) root         (0)      510 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/misc.py
--rw-r--r--   0 root         (0) root         (0)    10050 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/models.py
--rw-r--r--   0 root         (0) root         (0)     9304 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
--rw-r--r--   0 root         (0) root         (0)    12465 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/trainer.py
--rw-r--r--   0 root         (0) root         (0)     8649 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.12/theseus/utils/sparse_matrix_utils.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-04-12 22:35:53.000000 theseus-ai-nightly-2023.4.12/theseus/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:35:58.792434 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11642 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5682 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      406 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 22:35:58.000000 theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.232204 theseus-ai-nightly-2023.4.21/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11642 2023-04-21 20:16:07.232204 theseus-ai-nightly-2023.4.21/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11035 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.200203 theseus-ai-nightly-2023.4.21/examples/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/examples/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7193 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/backward_modes.py
+-rw-r--r--   0 root         (0) root         (0)     8158 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/bundle_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)    19017 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/homography_estimation.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/examples/motion_planning_2d.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/se2_inverse.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/examples/se2_planning.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/simple_example.py
+-rw-r--r--   0 root         (0) root         (0)    12290 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/state_estimation_2d.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/examples/tactile_pose_estimation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.200203 theseus-ai-nightly-2023.4.21/requirements/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/requirements/main.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-21 20:16:07.232204 theseus-ai-nightly-2023.4.21/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6284 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.200203 theseus-ai-nightly-2023.4.21/tests/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.204203 theseus-ai-nightly-2023.4.21/tests/core/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/common.py
+-rw-r--r--   0 root         (0) root         (0)    13514 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_cost_weight.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_manifold.py
+-rw-r--r--   0 root         (0) root         (0)    19419 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_robust_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_theseus_function.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_variable.py
+-rw-r--r--   0 root         (0) root         (0)    14670 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/core/test_vectorizer.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.204203 theseus-ai-nightly-2023.4.21/tests/extlib/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/extlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/extlib/test_baspacho.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/extlib/test_baspacho_simple.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/extlib/test_cusolver_lu_solver.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/extlib/test_mat_mult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.204203 theseus-ai-nightly-2023.4.21/tests/geometry/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19548 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/common.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/point_types_mypy_check.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/test_point_types.py
+-rw-r--r--   0 root         (0) root         (0)     8862 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/test_se2.py
+-rw-r--r--   0 root         (0) root         (0)    12861 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/test_se3.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/test_so2.py
+-rw-r--r--   0 root         (0) root         (0)    10391 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/test_so3.py
+-rw-r--r--   0 root         (0) root         (0)     7443 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/geometry/test_vector.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/tests/test_dlm_perturbation.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/tests/test_pgo_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    21069 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/tests/test_theseus_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.208203 theseus-ai-nightly-2023.4.21/theseus/
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.208203 theseus-ai-nightly-2023.4.21/theseus/core/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15935 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/cost_weight.py
+-rw-r--r--   0 root         (0) root         (0)    30933 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/core/objective.py
+-rw-r--r--   0 root         (0) root         (0)     6131 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/robust_cost_function.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/robust_loss.py
+-rw-r--r--   0 root         (0) root         (0)     6417 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/theseus_function.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/variable.py
+-rw-r--r--   0 root         (0) root         (0)    20067 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/core/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.208203 theseus-ai-nightly-2023.4.21/theseus/embodied/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.208203 theseus-ai-nightly-2023.4.21/theseus/embodied/collision/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/collision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/collision/collision.py
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/collision/eff_obj_contact.py
+-rw-r--r--   0 root         (0) root         (0)     9043 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/collision/signed_distance_field.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.212203 theseus-ai-nightly-2023.4.21/theseus/embodied/kinematics/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/kinematics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/kinematics/kinematics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.212203 theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/between.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/moving_frame_between.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/reprojection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.212203 theseus-ai-nightly-2023.4.21/theseus/embodied/misc/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/misc/local_cost_fn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.212203 theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/double_integrator.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/misc.py
+-rw-r--r--   0 root         (0) root         (0)    11526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/quasi_static_pushing_planar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.216204 theseus-ai-nightly-2023.4.21/theseus/extlib/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/baspacho_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/baspacho_solver.h
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/baspacho_solver_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)    16013 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/cusolver_lu_solver.cpp
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/cusolver_sp_defs.cpp
+-rw-r--r--   0 root         (0) root         (0)      744 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/cusolver_sp_defs.h
+-rw-r--r--   0 root         (0) root         (0)    14555 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/mat_mult.cu
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/extlib/utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.216204 theseus-ai-nightly-2023.4.21/theseus/geometry/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/lie_group.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/lie_group_check.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/manifold.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/point_types.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/se2.py
+-rw-r--r--   0 root         (0) root         (0)    29506 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/se3.py
+-rw-r--r--   0 root         (0) root         (0)    11359 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/so2.py
+-rw-r--r--   0 root         (0) root         (0)    25233 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/so3.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9405 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/geometry/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.216204 theseus-ai-nightly-2023.4.21/theseus/labs/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/labs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.216204 theseus-ai-nightly-2023.4.21/theseus/labs/lie/
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.220204 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/lie_group.py
+-rw-r--r--   0 root         (0) root         (0)    35277 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/se3_impl.py
+-rw-r--r--   0 root         (0) root         (0)    30733 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/so3_impl.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/utils.py
+-rw-r--r--   0 root         (0) root         (0)    20240 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/lie_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/labs/lie/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.220204 theseus-ai-nightly-2023.4.21/theseus/optimizer/
+-rw-r--r--   0 root         (0) root         (0)      505 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.220204 theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/baspacho_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/cholmod_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/common.py
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/dense_linearization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.224204 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/baspacho_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/cholmod_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/dense_solver.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/linear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/linear_solver.py
+-rw-r--r--   0 root         (0) root         (0)     6892 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/lu_cuda_sparse_solver.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linear_system.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/linearization.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/manifold_gaussian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.224204 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8421 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/dcem.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/dogleg.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/gauss_newton.py
+-rw-r--r--   0 root         (0) root         (0)     7009 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/levenberg_marquardt.py
+-rw-r--r--   0 root         (0) root         (0)    16237 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/nonlinear_least_squares.py
+-rw-r--r--   0 root         (0) root         (0)    10762 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/nonlinear_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/trust_region.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/sparse_linearization.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/optimizer/variable_ordering.py
+-rw-r--r--   0 root         (0) root         (0)    12958 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/theseus_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.224204 theseus-ai-nightly-2023.4.21/theseus/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/third_party/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28031 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/third_party/easyaug.py
+-rwxr-xr-x   0 root         (0) root         (0)     6703 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/third_party/lml.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/third_party/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.228204 theseus-ai-nightly-2023.4.21/theseus/utils/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.228204 theseus-ai-nightly-2023.4.21/theseus/utils/examples/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.228204 theseus-ai-nightly-2023.4.21/theseus/utils/examples/bundle_adjustment/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/bundle_adjustment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12392 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/bundle_adjustment/data.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/bundle_adjustment/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.228204 theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9168 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/misc.py
+-rw-r--r--   0 root         (0) root         (0)     9771 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/models.py
+-rw-r--r--   0 root         (0) root         (0)    19745 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/motion_planner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.228204 theseus-ai-nightly-2023.4.21/theseus/utils/examples/pose_graph/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/pose_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16407 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/pose_graph/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.228204 theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/
+-rw-r--r--   0 root         (0) root         (0)      510 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10221 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/misc.py
+-rw-r--r--   0 root         (0) root         (0)    10050 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/models.py
+-rw-r--r--   0 root         (0) root         (0)     9304 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    12465 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/trainer.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2023-02-21 22:38:05.000000 theseus-ai-nightly-2023.4.21/theseus/utils/sparse_matrix_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-04-21 20:16:01.000000 theseus-ai-nightly-2023.4.21/theseus/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:16:07.232204 theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11642 2023-04-21 20:16:07.000000 theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-04-21 20:16:07.000000 theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 20:16:07.000000 theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2023-04-21 20:16:07.000000 theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-21 20:16:07.000000 theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/top_level.txt
```

### Comparing `theseus-ai-nightly-2023.4.12/LICENSE` & `theseus-ai-nightly-2023.4.21/LICENSE`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/PKG-INFO` & `theseus-ai-nightly-2023.4.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai-nightly
-Version: 2023.4.12
+Version: 2023.4.21
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.12 Summary: A
+Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.21 Summary: A
 library for differentiable nonlinear optimization. Home-page: https://
 github.com/facebookresearch/theseus Author: Meta Research Keywords:
 differentiable optimization,nonlinear least squares,factor graphs Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `theseus-ai-nightly-2023.4.12/README.md` & `theseus-ai-nightly-2023.4.21/README.md`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/backward_modes.py` & `theseus-ai-nightly-2023.4.21/examples/backward_modes.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/bundle_adjustment.py` & `theseus-ai-nightly-2023.4.21/examples/bundle_adjustment.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/homography_estimation.py` & `theseus-ai-nightly-2023.4.21/examples/homography_estimation.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/motion_planning_2d.py` & `theseus-ai-nightly-2023.4.21/examples/motion_planning_2d.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/se2_inverse.py` & `theseus-ai-nightly-2023.4.21/examples/se2_inverse.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/se2_planning.py` & `theseus-ai-nightly-2023.4.21/examples/se2_planning.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/simple_example.py` & `theseus-ai-nightly-2023.4.21/examples/simple_example.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/state_estimation_2d.py` & `theseus-ai-nightly-2023.4.21/examples/state_estimation_2d.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/examples/tactile_pose_estimation.py` & `theseus-ai-nightly-2023.4.21/examples/tactile_pose_estimation.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/setup.py` & `theseus-ai-nightly-2023.4.21/setup.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/common.py` & `theseus-ai-nightly-2023.4.21/tests/core/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_cost_function.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_cost_weight.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_cost_weight.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_manifold.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_manifold.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_objective.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_objective.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_robust_cost.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_robust_cost.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_theseus_function.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_theseus_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_variable.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_variable.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/core/test_vectorizer.py` & `theseus-ai-nightly-2023.4.21/tests/core/test_vectorizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/decorators.py` & `theseus-ai-nightly-2023.4.21/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho.py` & `theseus-ai-nightly-2023.4.21/tests/extlib/test_baspacho.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/extlib/test_baspacho_simple.py` & `theseus-ai-nightly-2023.4.21/tests/extlib/test_baspacho_simple.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/extlib/test_cusolver_lu_solver.py` & `theseus-ai-nightly-2023.4.21/tests/extlib/test_cusolver_lu_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/extlib/test_mat_mult.py` & `theseus-ai-nightly-2023.4.21/tests/extlib/test_mat_mult.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/common.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/point_types_mypy_check.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/point_types_mypy_check.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/test_point_types.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/test_point_types.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/test_se2.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/test_se2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/test_se3.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/test_se3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/test_so2.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/test_so2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/test_so3.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/test_so3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/geometry/test_vector.py` & `theseus-ai-nightly-2023.4.21/tests/geometry/test_vector.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/test_dlm_perturbation.py` & `theseus-ai-nightly-2023.4.21/tests/test_dlm_perturbation.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/test_pgo_benchmark.py` & `theseus-ai-nightly-2023.4.21/tests/test_pgo_benchmark.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/tests/test_theseus_layer.py` & `theseus-ai-nightly-2023.4.21/tests/test_theseus_layer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/constants.py` & `theseus-ai-nightly-2023.4.21/theseus/constants.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/cost_function.py` & `theseus-ai-nightly-2023.4.21/theseus/core/cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/cost_weight.py` & `theseus-ai-nightly-2023.4.21/theseus/core/cost_weight.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/objective.py` & `theseus-ai-nightly-2023.4.21/theseus/core/objective.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/robust_cost_function.py` & `theseus-ai-nightly-2023.4.21/theseus/core/robust_cost_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/robust_loss.py` & `theseus-ai-nightly-2023.4.21/theseus/core/robust_loss.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/theseus_function.py` & `theseus-ai-nightly-2023.4.21/theseus/core/theseus_function.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/variable.py` & `theseus-ai-nightly-2023.4.21/theseus/core/variable.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/core/vectorizer.py` & `theseus-ai-nightly-2023.4.21/theseus/core/vectorizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/collision/collision.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/collision/collision.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/collision/eff_obj_contact.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/collision/eff_obj_contact.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/collision/signed_distance_field.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/collision/signed_distance_field.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/kinematics/kinematics_model.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/kinematics/kinematics_model.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/between.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/moving_frame_between.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/moving_frame_between.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/measurements/reprojection.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/measurements/reprojection.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/misc/local_cost_fn.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/misc/local_cost_fn.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/double_integrator.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/double_integrator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/misc.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/embodied/motionmodel/quasi_static_pushing_planar.py` & `theseus-ai-nightly-2023.4.21/theseus/embodied/motionmodel/quasi_static_pushing_planar.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.cpp` & `theseus-ai-nightly-2023.4.21/theseus/extlib/baspacho_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver.h` & `theseus-ai-nightly-2023.4.21/theseus/extlib/baspacho_solver.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/baspacho_solver_cuda.cu` & `theseus-ai-nightly-2023.4.21/theseus/extlib/baspacho_solver_cuda.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_lu_solver.cpp` & `theseus-ai-nightly-2023.4.21/theseus/extlib/cusolver_lu_solver.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.cpp` & `theseus-ai-nightly-2023.4.21/theseus/extlib/cusolver_sp_defs.cpp`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/cusolver_sp_defs.h` & `theseus-ai-nightly-2023.4.21/theseus/extlib/cusolver_sp_defs.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/mat_mult.cu` & `theseus-ai-nightly-2023.4.21/theseus/extlib/mat_mult.cu`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/extlib/utils.h` & `theseus-ai-nightly-2023.4.21/theseus/extlib/utils.h`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/lie_group.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/lie_group_check.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/lie_group_check.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/manifold.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/manifold.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/point_types.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/point_types.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/se2.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/se2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/se3.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/se3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/so2.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/so2.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/so3.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/so3.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/utils.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/geometry/vector.py` & `theseus-ai-nightly-2023.4.21/theseus/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/constants.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/constants.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/lie_group.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/lie_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,14 +165,24 @@
         dtype: Optional[torch.dtype] = None,
         device: DeviceType = None,
         requires_grad: bool = False,
     ) -> torch.Tensor:
         pass
 
 
+class _IdentityFnType(Protocol):
+    def __call__(
+        *size: int,
+        dtype: Optional[torch.dtype] = None,
+        device: DeviceType = None,
+        requires_grad: bool = False,
+    ) -> torch.Tensor:
+        pass
+
+
 # Namespace to facilitate type-checking downstream
 class LieGroupFns:
     def __init__(self, module):
         self.exp, self.jexp = UnaryOperatorFactory(module, "exp")
         self.log, self.jlog = UnaryOperatorFactory(module, "log")
         self.adj = UnaryOperatorFactory(module, "adjoint")[0]
         self.inv, self.jinv = UnaryOperatorFactory(module, "inverse")
@@ -195,7 +205,8 @@
             self.check_lift_matrix: _CheckFnType = module.check_lift_matrix
         if hasattr(module, "check_project_matrix"):
             self.check_project_matrix: _CheckFnType = module.check_project_matrix
         self.check_left_act_matrix: _CheckFnType = module.check_left_act_matrix
         self.check_left_project_matrix: _CheckFnType = module.check_left_project_matrix
         self.rand: _RandFnType = module.rand
         self.randn: _RandFnType = module.randn
+        self.identity: _IdentityFnType = module.identity
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/se3_impl.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/se3_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 from typing import cast, List, Tuple, Optional
 
 from . import constants
-from . import lie_group, so3_impl as so3
+from . import lie_group, so3_impl as SO3
 from .utils import get_module
 
 
 NAME: str = "SE3"
 DIM: int = 6
 
 
@@ -20,19 +20,19 @@
 
 def check_group_tensor(tensor: torch.Tensor):
     with torch.no_grad():
         if tensor.ndim != 3 or tensor.shape[1:] != (3, 4):
             raise ValueError(
                 f"SE3 data tensors can only be 3x4 matrices, but got shape {tensor.shape}."
             )
-    so3.check_group_tensor(tensor[:, :, :3])
+    SO3.check_group_tensor(tensor[:, :, :3])
 
 
 def check_transform_tensor(tensor: torch.Tensor):
-    so3.check_transform_tensor(tensor)
+    SO3.check_transform_tensor(tensor)
 
 
 def check_tangent_vector(tangent_vector: torch.Tensor):
     _check = tangent_vector.ndim == 3 and tangent_vector.shape[1:] == (6, 1)
     _check |= tangent_vector.ndim == 2 and tangent_vector.shape[1] == 6
     if not _check:
         raise ValueError(
@@ -43,15 +43,15 @@
 def check_hat_matrix(matrix: torch.Tensor):
     if matrix.ndim != 3 or matrix.shape[1:] != (4, 4):
         raise ValueError("Hat matrices of SE(3) can only be 3x4 matrices")
 
     if matrix[:, -1].abs().max() > constants._SE3_NEAR_ZERO_EPS[matrix.dtype]:
         raise ValueError("The last row for hat matrices of SE(3) must be zero")
 
-    so3.check_hat_matrix(matrix[:, :3, :3])
+    SO3.check_hat_matrix(matrix[:, :3, :3])
 
 
 def check_lift_matrix(matrix: torch.Tensor):
     return matrix.shape[-1] == 6
 
 
 def check_project_matrix(matrix: torch.Tensor):
@@ -77,27 +77,17 @@
     generator: Optional[torch.Generator] = None,
     dtype: Optional[torch.dtype] = None,
     device: constants.DeviceType = None,
     requires_grad: bool = False,
 ) -> torch.Tensor:
     if len(size) != 1:
         raise ValueError("The size should be 1D.")
-    rotation = so3.rand(
-        size[0],
-        generator=generator,
-        dtype=dtype,
-        device=device,
-    )
+    rotation = SO3.rand(size[0], generator=generator, dtype=dtype, device=device)
     translation = torch.rand(
-        size[0],
-        3,
-        1,
-        generator=generator,
-        dtype=dtype,
-        device=device,
+        size[0], 3, 1, generator=generator, dtype=dtype, device=device
     )
     ret = torch.cat((rotation, translation), dim=2)
     ret.requires_grad_(requires_grad)
     return ret
 
 
 # -----------------------------------------------------------------------------
@@ -108,34 +98,45 @@
     generator: Optional[torch.Generator] = None,
     dtype: Optional[torch.dtype] = None,
     device: constants.DeviceType = None,
     requires_grad: bool = False,
 ) -> torch.Tensor:
     if len(size) != 1:
         raise ValueError("The size should be 1D.")
-    rotation = so3.randn(
-        size[0],
-        generator=generator,
-        dtype=dtype,
-        device=device,
-    )
+    rotation = SO3.randn(size[0], generator=generator, dtype=dtype, device=device)
     translation = torch.randn(
-        size[0],
-        3,
-        1,
-        generator=generator,
-        dtype=dtype,
-        device=device,
+        size[0], 3, 1, generator=generator, dtype=dtype, device=device
     )
     ret = torch.cat((rotation, translation), dim=2)
     ret.requires_grad_(requires_grad)
     return ret
 
 
 # -----------------------------------------------------------------------------
+# Identity
+# -----------------------------------------------------------------------------
+_BASE_IDENTITY_SE3 = [[1.0, 0.0, 0.0, 0.0], [0.0, 1.0, 0.0, 0.0], [0.0, 0.0, 1.0, 0.0]]
+
+
+def identity(
+    *size: int,
+    dtype: Optional[torch.dtype] = None,
+    device: constants.DeviceType = None,
+    requires_grad: bool = False,
+) -> torch.Tensor:
+    if len(size) != 1:
+        raise ValueError("The size should be 1D.")
+    ret = torch.tensor(_BASE_IDENTITY_SE3, dtype=dtype, device=device).repeat(
+        size[0], 1, 1
+    )
+    ret.requires_grad_(requires_grad)
+    return ret
+
+
+# -----------------------------------------------------------------------------
 # Exponential Map
 # -----------------------------------------------------------------------------
 def _exp_impl(tangent_vector: torch.Tensor) -> torch.Tensor:
     check_tangent_vector(tangent_vector)
     tangent_vector_lin = tangent_vector[:, :3].view(-1, 3, 1)
     tangent_vector_ang = tangent_vector[:, 3:].view(-1, 3, 1)
 
@@ -316,15 +317,15 @@
         + d_theta_minus_sine_by_theta3.view(-1, 1) * wwv
     ).view(-1, 3, 1) @ w.view(-1, 1, 3)
     jac_temp_t -= v.view(-1, 3, 1) @ sw.view(-1, 1, 3)
     jac_temp_v = (
         -one_minus_cosine_by_theta2.view(-1, 1) * v
         - theta_minus_sine_by_theta3_t.view(-1, 1) * wv
     )
-    jac_temp_t += so3._hat_autograd_fn(jac_temp_v)
+    jac_temp_t += SO3._hat_autograd_fn(jac_temp_v)
     diag_jac_t = torch.diagonal(jac_temp_t, dim1=1, dim2=2)
     diag_jac_t += (sw.view(-1, 1, 3) @ v.view(-1, 3, 1)).view(-1, 1)
 
     jac[:, :3, 3:] = ret[:, :, :3].transpose(1, 2) @ jac_temp_t
 
     return [jac], ret
 
@@ -590,15 +591,15 @@
 # Adjoint Transformation
 # -----------------------------------------------------------------------------
 def _adjoint_impl(group: torch.Tensor) -> torch.Tensor:
     check_group_tensor(group)
     ret = group.new_zeros(group.shape[0], 6, 6)
     ret[:, :3, :3] = group[:, :3, :3]
     ret[:, 3:, 3:] = group[:, :3, :3]
-    ret[:, :3, 3:] = so3._hat_impl(group[:, :3, 3]) @ group[:, :3, :3]
+    ret[:, :3, 3:] = SO3._hat_impl(group[:, :3, 3]) @ group[:, :3, :3]
     return ret
 
 
 # NOTE: No jacobian is defined for the adjoint transformation
 _jadjoint_impl = None
 
 
@@ -611,17 +612,17 @@
 
     @classmethod
     def backward(cls, ctx, grad_output):
         group: torch.Tensor = ctx.saved_tensors[0]
         grad_input_rot = (
             grad_output[:, :3, :3]
             + grad_output[:, 3:, 3:]
-            - so3._hat_impl(group[:, :, 3]) @ grad_output[:, :3, 3:]
+            - SO3._hat_impl(group[:, :, 3]) @ grad_output[:, :3, 3:]
         )
-        grad_input_t = so3._project_impl(
+        grad_input_t = SO3._project_impl(
             grad_output[:, :3, 3:] @ group[:, :, :3].transpose(1, 2)
         ).view(-1, 3, 1)
 
         return torch.cat((grad_input_rot, grad_input_t), dim=2)
 
 
 _adjoint_autograd_fn = Adjoint.apply
@@ -664,15 +665,15 @@
 # -----------------------------------------------------------------------------
 # Hat
 # -----------------------------------------------------------------------------
 def _hat_impl(tangent_vector: torch.Tensor) -> torch.Tensor:
     check_tangent_vector(tangent_vector)
     tangent_vector = tangent_vector.view(-1, 6)
     matrix = tangent_vector.new_zeros(tangent_vector.shape[0], 4, 4)
-    matrix[:, :3, :3] = so3._hat_impl(tangent_vector[:, 3:])
+    matrix[:, :3, :3] = SO3._hat_impl(tangent_vector[:, 3:])
     matrix[:, :3, 3] = tangent_vector[:, :3]
 
     return matrix
 
 
 # NOTE: No jacobian is defined for the hat operator
 _jhat_impl = None
@@ -735,15 +736,15 @@
         return ret
 
     @classmethod
     def backward(cls, ctx, grad_output):
         grad_output: torch.Tensor = cast(torch.Tensor, grad_output)
         grad_input = grad_output.new_zeros(grad_output.shape[0], 4, 4)
         grad_input[:, :3, 3] = grad_output[:, :3]
-        grad_input[:, :3, :3] = 0.5 * so3._hat_impl(grad_output[:, 3:])
+        grad_input[:, :3, :3] = 0.5 * SO3._hat_impl(grad_output[:, 3:])
         return grad_input
 
 
 _vee_autograd_fn = Vee.apply
 _jvee_autograd_fn = None
 
 
@@ -811,16 +812,16 @@
 
 def _jtransform_from_impl(
     group: torch.Tensor, tensor: torch.Tensor
 ) -> Tuple[List[torch.Tensor], torch.Tensor]:
     check_group_tensor(group)
     check_transform_tensor(tensor)
     jacobian_g = group.new_empty(group.shape[0], 3, 6)
-    jacobian_g[:, :, :3] = so3._hat_autograd_fn(tensor) @ group[:, :, :3]
-    jacobian_g[:, :, 3:] = -group[:, :, :3] @ so3._hat_autograd_fn(tensor)
+    jacobian_g[:, :, :3] = SO3._hat_autograd_fn(tensor) @ group[:, :, :3]
+    jacobian_g[:, :, 3:] = -group[:, :, :3] @ SO3._hat_autograd_fn(tensor)
     jacobian_p = group[:, :, :3].view(tensor.shape[:-1] + (3, 3))
     jacobians = []
     jacobians.append(jacobian_g)
     jacobians.append(jacobian_p)
     return jacobians, _transform_from_impl(group, tensor)
 
 
@@ -852,15 +853,15 @@
 # -----------------------------------------------------------------------------
 # Lift
 # -----------------------------------------------------------------------------
 def _lift_impl(matrix: torch.Tensor) -> torch.Tensor:
     if not check_lift_matrix(matrix):
         raise ValueError("Inconsistent shape for the matrix to lift.")
     ret = matrix.new_zeros(matrix.shape[:-1] + (3, 4))
-    ret[..., :, :3] = so3._lift_impl(matrix[..., 3:])
+    ret[..., :, :3] = SO3._lift_impl(matrix[..., 3:])
     ret[..., :, 3] = matrix[..., :3]
 
     return ret
 
 
 # NOTE: No jacobian is defined for the project operator
 _jlift_impl = None
@@ -930,15 +931,15 @@
 
 # -----------------------------------------------------------------------------
 # Left Act
 # -----------------------------------------------------------------------------
 def _left_act_impl(group: torch.Tensor, matrix: torch.Tensor) -> torch.Tensor:
     check_group_tensor(group)
     check_left_act_matrix(matrix)
-    ret = so3._left_act_impl(group[:, :, :3], matrix)
+    ret = SO3._left_act_impl(group[:, :, :3], matrix)
     return ret
 
 
 def _left_act_backward_helper(group, matrix, grad_output) -> torch.Tensor:
     jac_rot = torch.einsum("n...ij,n...kj->n...ik", grad_output, matrix)
     if matrix.ndim > 3:
         dims = list(range(1, matrix.ndim - 2))
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/so3_impl.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/so3_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,30 @@
         )
     )
     ret.requires_grad_(requires_grad)
     return ret
 
 
 # -----------------------------------------------------------------------------
+# Identity
+# -----------------------------------------------------------------------------
+def identity(
+    *size: int,
+    dtype: Optional[torch.dtype] = None,
+    device: constants.DeviceType = None,
+    requires_grad: bool = False,
+) -> torch.Tensor:
+    if len(size) != 1:
+        raise ValueError("The size should be 1D.")
+    ret = torch.eye(3, device=device, dtype=dtype).repeat(size[0], 1, 1)
+    ret.requires_grad_(requires_grad)
+    return ret
+
+
+# -----------------------------------------------------------------------------
 # Exponential Map
 # -----------------------------------------------------------------------------
 def _exp_impl(tangent_vector: torch.Tensor) -> torch.Tensor:
     check_tangent_vector(tangent_vector)
     tangent_vector = tangent_vector.view(-1, 3)
     theta = torch.linalg.norm(tangent_vector, dim=1, keepdim=True).unsqueeze(1)
     theta2 = theta**2
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/functional/utils.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/functional/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/lie_tensor.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/lie_tensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 import threading
 import warnings
-from typing import Any, Callable, List, Optional, Tuple, Union
+from typing import Any, Callable, List, Optional, Tuple
 from typing import cast as type_cast
 
 import torch
 from torch.utils._pytree import tree_flatten, tree_map_only
 from torch.types import Number
 
 from theseus.labs.lie.functional.constants import DeviceType
 from theseus.labs.lie.functional.lie_group import UnaryOperatorOpFnType
 from .types import (
     ltype as _ltype,
     Device,
     SE3,
     SO3,
     TensorType,
+    _IdentityFnType,
     _JFnReturnType,
     _RandFnType,
 )
 
 
 class _LieAsEuclideanContext:
     contexts = threading.local()
@@ -51,34 +52,49 @@
 
 
 def euclidean_enabled() -> bool:
     return _LieAsEuclideanContext.get_context()
 
 
 class _LieTensorBase(torch.Tensor):
-    def __new__(cls, data: torch.Tensor, ltype: _ltype, requires_grad=False):
-        return cls._make_subclass(cls, data, requires_grad)  # type: ignore
+    def __new__(
+        cls,
+        data: torch.Tensor,
+        ltype: _ltype,
+        requires_grad: bool = False,
+        _shared_memory: bool = False,
+    ):
+        return cls._make_subclass(
+            cls, data if _shared_memory else data.clone(), requires_grad  # type: ignore
+        )
 
     @property
     def _t(self) -> torch.Tensor:
         return self.as_subclass(torch.Tensor)
 
-    def __init__(self, data: Any, ltype: _ltype, requires_grad=None):
+    def __init__(
+        self,
+        data: Any,
+        ltype: _ltype,
+        requires_grad: Optional[bool] = None,
+        _shared_memory: bool = False,
+    ):
         self.ltype = ltype
+        self.ltype._fn_lib.check_group_tensor(self.as_subclass(torch.Tensor))
 
     def __repr__(self) -> str:  # type: ignore
         return f"LieTensor({self._t}, ltype=lie.{self.ltype})"
 
     @classmethod
     def to_torch(cls, args: Any):
         return tree_map_only(cls, lambda x: x._t, args)
 
-    @classmethod
-    def resolve_ltype(cls, t: Any):
-        return t.ltype if isinstance(t, cls) else None
+    @staticmethod
+    def resolve_ltype(t: Any):
+        return t.ltype if hasattr(t, "ltype") else None
 
     @classmethod
     def get_ltype(cls, args):
         ltypes = [cls.resolve_ltype(a) for a in tree_flatten(args)[0]]
         ltypes = set(x for x in ltypes if x is not None)
         if len(ltypes) > 1:
             raise ValueError(
@@ -139,15 +155,16 @@
         torch.Tensor.is_mps.__get__,  # type: ignore
         torch.Tensor.is_sparse.__get__,  # type: ignore
         torch.Tensor.is_quantized.__get__,  # type: ignore
         torch.Tensor.grad.__get__,  # type: ignore
         torch.Tensor.layout.__get__,  # type: ignore
         torch.Tensor.requires_grad.__get__,  # type: ignore
         torch.Tensor.retains_grad.__get__,  # type: ignore
-        torch.Tensor.shape.__get__,  # type: ignore
+        torch.Tensor.storage,  # type: ignore
+        torch.Tensor.__getitem__,  # type: ignore
         torch.Tensor.clone,
         torch.Tensor.__format__,
         torch.Tensor.new_tensor,
         torch.Tensor.to,
         torch.cat,
         torch.is_complex,
         # torch.stack  # requires arbitrary batch support
@@ -159,19 +176,32 @@
     _SAFE_AS_EUCL_OPS: List[Callable] = [
         torch.zeros_like,
         torch.ones_like,
         torch.Tensor.new_zeros,
         torch.Tensor.new_ones,
         torch.allclose,
         torch.isclose,
+        torch.Tensor.grad_fn.__get__,  # type: ignore
+        torch.Tensor.shape.__get__,  # type: ignore
+        torch.Tensor.ndim.__get__,  # type: ignore
     ]
 
-    def __init__(self, tensor: torch.Tensor, ltype: _ltype, requires_grad=None):
-        super().__init__(tensor, ltype, requires_grad=requires_grad)
-        self.ltype._fn_lib.check_group_tensor(self.as_subclass(torch.Tensor))
+    def __init__(
+        self,
+        tensor: torch.Tensor,
+        ltype: _ltype,
+        requires_grad: Optional[bool] = None,
+        _shared_memory: bool = False,
+    ):
+        super().__init__(
+            tensor,
+            ltype,
+            requires_grad=requires_grad,
+            _shared_memory=_shared_memory,
+        )
 
     @staticmethod
     def from_tensor(tensor: torch.Tensor, ltype: _ltype) -> "LieTensor":
         return _FromTensor.apply(tensor, ltype)
 
     @classmethod
     def _torch_function_impl_lie(cls, func, types, args=(), kwargs=None):
@@ -181,15 +211,23 @@
             )
         if func in LieTensor._SAFE_SUPER_OPS:
             ltype = cls.get_ltype(args)
             ret = super().__torch_function__(func, types, args, kwargs or {})
             if func == torch.Tensor.grad.__get__:
                 return _EuclideanGrad(ret) if ret is not None else ret
             # tree-map to set the ltypes correctly
-            return tree_map_only(LieTensor, lambda x: LieTensor(ret, ltype), ret)
+            if func == torch.Tensor.__getitem__:
+                if isinstance(args[1], tuple):
+                    raise NotImplementedError(
+                        "LieTensor currently only supports slicing the batch dimension."
+                    )
+                assert ret.ndim in [2, 3]
+                if ret.ndim == 2:
+                    ret = ret._t.unsqueeze(0)
+            return tree_map_only(torch.Tensor, lambda x: from_tensor(x, ltype), ret)
         raise NotImplementedError(
             "Tried to call a torch function not supported by LieTensor. "
             "If trying to operate on the raw tensor data, please use group._t, "
             "or run inside the context lie.as_euclidean()."
         )
 
     @classmethod
@@ -202,52 +240,51 @@
             return cls._torch_function_impl_lie(func, types, args, kwargs)
 
     def _check_ltype(self, other: "LieTensor", op_name: str):
         if other.ltype != self.ltype:
             raise ValueError("f{op_name} requires both tensors to have same ltype.")
 
     # Returns a new LieTensor with the given data and the same ltype as self
-    def new(  # type: ignore
+    def new_lietensor(  # type: ignore
         self, args: Any, device: Device = None, dtype: Optional[torch.dtype] = None
     ) -> "LieTensor":
         if isinstance(args, LieTensor):
             warnings.warn(
-                "Calling new() on a LieTensor results in shared data storage. "
                 "To copy construct from a LieTensor, it is recommended to use "
-                "lie_tensor.clone().",
+                "lie_tensor.clone().detach() instead of lie_tensor.new_lietensor(t)",
                 UserWarning,
             )
             tensor_arg = args._t
             dtype = dtype or self.dtype
         elif isinstance(args, torch.Tensor):
             tensor_arg = args
             dtype = dtype or args.dtype
         else:
             tensor_arg = torch.as_tensor(args)
             dtype = dtype or torch.get_default_dtype()
-        return LieTensor.from_tensor(
-            tensor_arg.to(device=device, dtype=dtype), ltype=self.ltype
-        )
+        return LieTensor(tensor_arg.to(device=device, dtype=dtype), ltype=self.ltype)
 
     # ------------------------------------------------------
     # ------ Operators
     # ------------------------------------------------------
     # For the next ones the output also depends on self's data
     def log(self) -> torch.Tensor:
         return self.ltype._fn_lib.log(self._t)
 
     def adj(self) -> torch.Tensor:
         return self.ltype._fn_lib.adj(self._t)
 
     def inv(self) -> "LieTensor":
-        return self.new(self.ltype._fn_lib.inv(self._t))
+        return self.from_tensor(self.ltype._fn_lib.inv(self._t), self.ltype)
 
     def compose(self, other: "LieTensor") -> "LieTensor":
         self._check_ltype(other, "compose")
-        return self.new(self.ltype._fn_lib.compose(self._t, other._t))
+        return self.from_tensor(
+            self.ltype._fn_lib.compose(self._t, other._t), self.ltype
+        )
 
     def transform_from(self, point: torch.Tensor) -> torch.Tensor:
         return self.ltype._fn_lib.transform_from(self._t, point)
 
     def left_act(self, matrix: torch.Tensor) -> torch.Tensor:
         return self.ltype._fn_lib.left_act(self._t, matrix)
 
@@ -262,27 +299,29 @@
         input0: torch.Tensor,
         fn: UnaryOperatorOpFnType,
         out_is_group: bool = True,
     ) -> _JFnReturnType:
         jacs: List[torch.Tensor] = []
         op_res: TensorType = fn(input0, jacobians=jacs)
         if out_is_group:
-            op_res = self.new(op_res)
+            op_res = self.from_tensor(op_res, self.ltype)
         return jacs, op_res
 
     def jlog(self) -> _JFnReturnType:
         return self._unary_jop_base(self._t, self.ltype._fn_lib.log, out_is_group=False)
 
     def jinv(self) -> _JFnReturnType:
         return self._unary_jop_base(self._t, self.ltype._fn_lib.inv)
 
     def jcompose(self, other: "LieTensor") -> _JFnReturnType:
         self._check_ltype(other, "jcompose")
         jacs: List[torch.Tensor] = []
-        op_res = self.new(self.ltype._fn_lib.compose(self._t, other._t, jacobians=jacs))
+        op_res = self.from_tensor(
+            self.ltype._fn_lib.compose(self._t, other._t, jacobians=jacs), self.ltype
+        )
         return jacs, op_res
 
     def jtransform_from(self, point: torch.Tensor) -> _JFnReturnType:
         jacs: List[torch.Tensor] = []
         op_res = self.ltype._fn_lib.transform_from(self._t, point, jacobians=jacs)
         return jacs, op_res
 
@@ -384,36 +423,46 @@
 # ----------------------------
 # Tensor creation functions
 # ----------------------------
 def as_lietensor(
     data: Any,
     ltype: Optional[_ltype] = None,
     dtype: torch.dtype = torch.float,
-    device: Union[torch.device, str] = None,
+    device: DeviceType = None,
 ) -> _LieTensorBase:
     if isinstance(data, LieTensor):
-        return data
+        if data.dtype == dtype and data.device == torch.device(device or "cpu"):
+            return data
+        return type_cast(LieTensor, data.to(device=device, dtype=dtype))
     if ltype is None:
         raise ValueError("ltype must be provided.")
     return type_cast(
-        LieTensor, LieTensor(data, ltype=ltype).to(device=device, dtype=dtype)
+        LieTensor,
+        LieTensor.from_tensor(data, ltype=ltype).to(device=device, dtype=dtype),
     )
 
 
-# With this new version of the code I like @fantaosha's proposal of using the
-# name cast() because it implies type conversion rather than a wrapper being created.
-cast = as_lietensor
+def cast(
+    data: Any,
+    ltype: Optional[_ltype] = None,
+    dtype: torch.dtype = torch.float,
+    device: DeviceType = None,
+) -> _LieTensorBase:
+    return as_lietensor(data, ltype=ltype, dtype=dtype, device=device)
+
 
-from_tensor = LieTensor.from_tensor
+from_tensor: Callable[[torch.Tensor, _ltype], LieTensor] = LieTensor.from_tensor
 
 
 class _FromTensor(torch.autograd.Function):
     @staticmethod
     def forward(ctx: Any, tensor: torch.Tensor, ltype: _ltype) -> LieTensor:  # type: ignore
-        return LieTensor(tensor, ltype, requires_grad=tensor.requires_grad)
+        return LieTensor(
+            tensor, ltype, requires_grad=tensor.requires_grad, _shared_memory=True
+        )
 
     @staticmethod
     def backward(ctx: Any, grad_output: torch.Tensor) -> Tuple[torch.Tensor, None]:  # type: ignore
         return grad_output, None
 
 
 def _build_random_fn(op_name: str, ltype: _ltype) -> _RandFnType:
@@ -440,23 +489,64 @@
                 generator=generator,
                 dtype=dtype,
                 device=device,
                 requires_grad=requires_grad,
             ),
             ltype,
             requires_grad=requires_grad,
+            _shared_memory=True,
         )
 
     return fn
 
 
+def _build_identity_fn(ltype: _ltype) -> _IdentityFnType:
+    def fn(
+        *size: Any,
+        dtype: Optional[torch.dtype] = None,
+        device: DeviceType = None,
+        requires_grad: bool = False,
+    ) -> LieTensor:
+        good = all([isinstance(a, int) for a in size])
+        if not good:
+            arg_types = " ".join(type(a).__name__ for a in size)
+            raise TypeError(
+                f"identity() received invalid combination of arguments - "
+                f"got ({arg_types}), but expected (tuple of ints)."
+            )
+        return LieTensor(
+            ltype._fn_lib.identity(
+                *size,
+                dtype=dtype,
+                device=device,
+                requires_grad=requires_grad,
+            ),
+            ltype,
+            requires_grad=requires_grad,
+            _shared_memory=True,
+        )
+
+    return fn
+
+
+def _build_call_impl(ltype: _ltype) -> Callable[[torch.Tensor], LieTensor]:
+    def fn(tensor: torch.Tensor) -> LieTensor:
+        return LieTensor(tensor, ltype)
+
+    return fn
+
+
 SE3.rand = _build_random_fn("rand", SE3)
 SE3.randn = _build_random_fn("randn", SE3)
+SE3.identity = _build_identity_fn(SE3)
+SE3._call_impl = _build_call_impl(SE3)
 SO3.rand = _build_random_fn("rand", SO3)
 SO3.randn = _build_random_fn("randn", SO3)
+SO3.identity = _build_identity_fn(SO3)
+SO3._call_impl = _build_call_impl(SO3)
 SE3._create_lie_tensor = SO3._create_lie_tensor = LieTensor
 
 
 def log(group: LieTensor) -> torch.Tensor:
     return group.log()
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus/labs/lie/types.py` & `theseus-ai-nightly-2023.4.21/theseus/labs/lie/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,46 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from enum import Enum
 from typing import Any, Callable, List, Optional, Protocol, Tuple, Union, TYPE_CHECKING
 
 import torch
-from theseus.labs.lie.functional import se3 as _se3_impl, so3 as _so3_impl
+from theseus.labs.lie.functional import SE3 as _se3_impl, SO3 as _so3_impl
 from theseus.labs.lie.functional.constants import DeviceType
 from theseus.labs.lie.functional.lie_group import LieGroupFns
 
 if TYPE_CHECKING:
     from .lie_tensor import LieTensor, _LieTensorBase
 
 
-# Similar to the one in functional, except it returns a LieTensor
-# and receives a ltype
+# The next two are similar to the ones in functional, except they return a LieTensor.
 class _RandFnType(Protocol):
     def __call__(
         self,
         *size: Any,
         generator: Optional[torch.Generator] = None,
         dtype: Optional[torch.dtype] = None,
         device: DeviceType = None,
         requires_grad: bool = False,
     ) -> "LieTensor":
         pass
 
 
+class _IdentityFnType(Protocol):
+    def __call__(
+        self,
+        *size: int,
+        dtype: Optional[torch.dtype] = None,
+        device: DeviceType = None,
+        requires_grad: bool = False,
+    ) -> "LieTensor":
+        pass
+
+
 Device = Union[torch.device, str, None]
 TensorType = Union[torch.Tensor, "_LieTensorBase"]
 _JFnReturnType = Tuple[List[torch.Tensor], TensorType]
 
 
 class _ltype(Enum):
     SE3 = 0
@@ -57,14 +67,19 @@
 class ltype:
     def __init__(self, lt: _ltype):
         self._lt = lt
         self._fn_lib = _get_fn_lib(lt)
 
     rand: _RandFnType
     randn: _RandFnType
+    identity: _IdentityFnType
+    _call_impl: Callable[[torch.Tensor], "LieTensor"]
+
+    def __call__(self, tensor: torch.Tensor) -> "LieTensor":
+        return self._call_impl(tensor)
 
     _create_lie_tensor: Callable[[torch.Tensor, "ltype"], "LieTensor"]
 
     def exp(self, tangent_vector: torch.Tensor) -> "LieTensor":
         return self._create_lie_tensor(
             _eval_op(self._fn_lib, "exp", tangent_vector), self
         )
@@ -82,10 +97,13 @@
 
     def lift(self, matrix: torch.Tensor) -> torch.Tensor:
         return _eval_op(self._fn_lib, "lift", matrix)
 
     def project(self, matrix: torch.Tensor) -> torch.Tensor:
         return _eval_op(self._fn_lib, "project", matrix)
 
+    def __str__(self) -> str:
+        return self._lt.name
+
 
 SE3 = ltype(_ltype.SE3)
 SO3 = ltype(_ltype.SO3)
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/baspacho_sparse_autograd.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/baspacho_sparse_autograd.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/cholmod_sparse_autograd.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/cholmod_sparse_autograd.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/common.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/common.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/autograd/lu_cuda_sparse_autograd.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/dense_linearization.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/dense_linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/baspacho_sparse_solver.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/baspacho_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/cholmod_sparse_solver.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/cholmod_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/dense_solver.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/dense_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_optimizer.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/linear_optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/linear_solver.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/linear_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/lu_cuda_sparse_solver.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/lu_cuda_sparse_solver.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear/utils.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linear_system.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linear_system.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/linearization.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/manifold_gaussian.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/manifold_gaussian.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dcem.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/dcem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
+
 from typing import Optional, Union, List, Dict
 
 import numpy as np
 import torch
 from torch.distributions import Normal
 
 from theseus.third_party.lml import LML
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/dogleg.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/dogleg.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/gauss_newton.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/gauss_newton.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/levenberg_marquardt.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_least_squares.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/nonlinear_least_squares.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/nonlinear_optimizer.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/nonlinear_optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/nonlinear/trust_region.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/nonlinear/trust_region.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/optimizer.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/sparse_linearization.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/sparse_linearization.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/optimizer/variable_ordering.py` & `theseus-ai-nightly-2023.4.21/theseus/optimizer/variable_ordering.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/theseus_layer.py` & `theseus-ai-nightly-2023.4.21/theseus/theseus_layer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/third_party/easyaug.py` & `theseus-ai-nightly-2023.4.21/theseus/third_party/easyaug.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/third_party/lml.py` & `theseus-ai-nightly-2023.4.21/theseus/third_party/lml.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/third_party/utils.py` & `theseus-ai-nightly-2023.4.21/theseus/third_party/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/__init__.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/data.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/bundle_adjustment/data.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/bundle_adjustment/util.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/bundle_adjustment/util.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/misc.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/models.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/motion_planning/motion_planner.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/motion_planning/motion_planner.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/pose_graph/dataset.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/pose_graph/dataset.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/misc.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/misc.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/models.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/models.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/pose_estimator.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/examples/tactile_pose_estimation/trainer.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/examples/tactile_pose_estimation/trainer.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/sparse_matrix_utils.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/sparse_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus/utils/utils.py` & `theseus-ai-nightly-2023.4.21/theseus/utils/utils.py`

 * *Files identical despite different names*

### Comparing `theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/PKG-INFO` & `theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theseus-ai-nightly
-Version: 2023.4.12
+Version: 2023.4.21
 Summary: A library for differentiable nonlinear optimization.
 Home-page: https://github.com/facebookresearch/theseus
 Author: Meta Research
 Keywords: differentiable optimization,nonlinear least squares,factor graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.12 Summary: A
+Metadata-Version: 2.1 Name: theseus-ai-nightly Version: 2023.4.21 Summary: A
 library for differentiable nonlinear optimization. Home-page: https://
 github.com/facebookresearch/theseus Author: Meta Research Keywords:
 differentiable optimization,nonlinear least squares,factor graphs Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `theseus-ai-nightly-2023.4.12/theseus_ai_nightly.egg-info/SOURCES.txt` & `theseus-ai-nightly-2023.4.21/theseus_ai_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

