# Comparing `tmp/dingo-gw-0.4.3.tar.gz` & `tmp/dingo-gw-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingo-gw-0.4.3.tar", last modified: Wed Apr  5 09:48:40 2023, max compression
+gzip compressed data, was "dingo-gw-0.5.0.tar", last modified: Thu Apr 20 21:59:39 2023, max compression
```

## Comparing `dingo-gw-0.4.3.tar` & `dingo-gw-0.5.0.tar`

### file list

```diff
@@ -1,208 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.334947 dingo-gw-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.306946 dingo-gw-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.310947 dingo-gw-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-05 09:48:40.334947 dingo-gw-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.310947 dingo-gw-0.4.3/compatibility/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/remove_domain_window_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_model_input_dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_saved_model_for_train_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_saved_model_gnpe_context_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_saved_model_new_gnpe.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_saved_model_new_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/compatibility/update_waveform_dataset_svd_refactor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.310947 dingo-gw-0.4.3/dingo/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.310947 dingo-gw-0.4.3/dingo/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.314947 dingo-gw-0.4.3/dingo/core/density/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/density/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/density/nde_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/density/unconditional_density_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.314947 dingo-gw-0.4.3/dingo/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15083 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/models/posterior_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.314947 dingo-gw-0.4.3/dingo/core/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/nn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14095 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/nn/enets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/nn/nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    25545 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.314947 dingo-gw-0.4.3/dingo/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/condor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/gnpeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/torchutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/core/utils/trainutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.314947 dingo-gw-0.4.3/dingo/gw/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/SVD.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.318947 dingo-gw-0.4.3/dingo/gw/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/conversion/spin_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.318947 dingo-gw-0.4.3/dingo/gw/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/data/data_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/data/data_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/data/event_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.318947 dingo-gw-0.4.3/dingo/gw/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/dataset/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/dataset/generate_dataset_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/dataset/waveform_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/download_strain_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/gwutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.318947 dingo-gw-0.4.3/dingo/gw/importance_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/importance_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/importance_sampling/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/importance_sampling/importance_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.318947 dingo-gw-0.4.3/dingo/gw/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/inference/gw_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/inference/inference_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/inference/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/injection.py
--rw-r--r--   0 runner    (1001) docker     (123)    32152 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/ls_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.318947 dingo-gw-0.4.3/dingo/gw/noise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/noise/asd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/noise/asd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/noise/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/noise/generate_dataset_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/noise/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.322947 dingo-gw-0.4.3/dingo/gw/pipe/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/ACKNOWLEDGMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/dag_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/dingo_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.322947 dingo-gw-0.4.3/dingo/gw/pipe/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/nodes/generation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/nodes/importance_sampling_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/nodes/merge_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/nodes/plot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/nodes/sampling_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    43561 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/pipe/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    24220 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/temporary_debug_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.322947 dingo-gw-0.4.3/dingo/gw/training/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/training/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12660 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/training/train_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/training/train_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/training/train_pipeline_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.322947 dingo-gw-0.4.3/dingo/gw/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15299 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/detector_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/general_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/gnpe_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/inference_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/noise_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/transforms/parameter_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.322947 dingo-gw-0.4.3/dingo/gw/waveform_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/waveform_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/waveform_generator/frame_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39208 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/waveform_generator/waveform_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/dingo/gw/waveform_generator/wfg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.326947 dingo-gw-0.4.3/dingo_gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo_gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo_gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo_gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo_gw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo_gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:48:40.000000 dingo-gw-0.4.3/dingo_gw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.326947 dingo-gw-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/code_design.md
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/dingo_pipe.md
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/example_injection.md
--rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/generating_waveforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/gibbs_figure.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/gnpe.md
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/inference.md
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/network_architecture.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/noise_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/result.md
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/sbi.md
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/training.md
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/training_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25293 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/docs/source/waveform_dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/examples/dataset_generation/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/dataset_generation/asd_dataset_settings.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/dataset_generation/dingo_generate_dataset_dag_example.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/dataset_generation/waveform_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/event_settings.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/is_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/examples/pipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/pipe/GW150914.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/examples/training/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/stage_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/train_settings_init_production.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/train_settings_init_toy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/train_settings_no_gnpe_production.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/train_settings_no_gnpe_toy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/train_settings_production.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/examples/training/train_settings_toy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:48:40.334947 dingo-gw-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.310947 dingo-gw-0.4.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/core/test_enets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/core/test_nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/core/test_posterior_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/core/testutils_enets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/tests/gw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.330947 dingo-gw-0.4.3/tests/gw/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/conversion/test_spin_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/conversion/test_time_delay_from_geocenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/test_noise_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/test_prior_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/test_waveform_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.334947 dingo-gw-0.4.3/tests/gw/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/transforms/test_detector_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/transforms/test_general_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/transforms/test_gnpe_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/transforms/test_parameter_transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   263605 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/transforms/waveform_data.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:48:40.334947 dingo-gw-0.4.3/tests/gw/waveform_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/waveform_generator/test_wfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-05 09:48:30.000000 dingo-gw-0.4.3/tests/gw/waveform_generator/test_wfg_m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.461245 dingo-gw-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.389245 dingo-gw-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.397245 dingo-gw-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-20 21:59:39.461245 dingo-gw-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.397245 dingo-gw-0.5.0/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/remove_domain_window_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_model_input_dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_saved_model_for_train_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_saved_model_gnpe_context_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_saved_model_new_gnpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_saved_model_new_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/compatibility/update_waveform_dataset_svd_refactor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.397245 dingo-gw-0.5.0/dingo/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.397245 dingo-gw-0.5.0/dingo/asimov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/asimov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/asimov/asimov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/asimov/dingo.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.401245 dingo-gw-0.5.0/dingo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.401245 dingo-gw-0.5.0/dingo/core/density/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/density/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/density/nde_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/density/unconditional_density_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.405245 dingo-gw-0.5.0/dingo/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16789 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/models/posterior_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.405245 dingo-gw-0.5.0/dingo/core/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/nn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14095 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/nn/enets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/nn/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.409245 dingo-gw-0.5.0/dingo/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/condor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/gnpeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/pt_to_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/torchutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/core/utils/trainutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.417245 dingo-gw-0.5.0/dingo/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/SVD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.417245 dingo-gw-0.5.0/dingo/gw/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/conversion/spin_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.417245 dingo-gw-0.5.0/dingo/gw/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/data/data_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/data/data_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/data/event_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.421245 dingo-gw-0.5.0/dingo/gw/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/dataset/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/dataset/generate_dataset_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/dataset/waveform_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/download_strain_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/gwutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.421245 dingo-gw-0.5.0/dingo/gw/importance_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/importance_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/importance_sampling/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/importance_sampling/importance_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.421245 dingo-gw-0.5.0/dingo/gw/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/inference/gw_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/inference/inference_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/inference/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31426 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/ls_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.425245 dingo-gw-0.5.0/dingo/gw/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/asd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/asd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/generate_dataset_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.425245 dingo-gw-0.5.0/dingo/gw/noise/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/synthetic/asd_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/synthetic/asd_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/synthetic/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/synthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/noise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/temporary_debug_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.429245 dingo-gw-0.5.0/dingo/gw/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/training/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12660 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/training/train_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/training/train_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/training/train_pipeline_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.429245 dingo-gw-0.5.0/dingo/gw/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/detector_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/general_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/gnpe_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/inference_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/noise_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/transforms/parameter_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.429245 dingo-gw-0.5.0/dingo/gw/waveform_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/waveform_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/waveform_generator/frame_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57836 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/waveform_generator/waveform_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/gw/waveform_generator/wfg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.433245 dingo-gw-0.5.0/dingo/pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/ACKNOWLEDGMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/dag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/dingo_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.437245 dingo-gw-0.5.0/dingo/pipe/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/importance_sampling_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/merge_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/pe_summary_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/plot_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/nodes/sampling_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44079 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/dingo/pipe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.437245 dingo-gw-0.5.0/dingo_gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo_gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo_gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo_gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo_gw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo_gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 21:59:39.000000 dingo-gw-0.5.0/dingo_gw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.441245 dingo-gw-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.449245 dingo-gw-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/code_design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/dingo_pipe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/example_gnpe_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/example_injection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/example_npe_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/example_toy_npe_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42481 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/generating_waveforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/gibbs_figure.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/gnpe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/inference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/network_architecture.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/noise_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/result.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/sbi.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/training.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/training_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/docs/source/waveform_dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.449245 dingo-gw-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.449245 dingo-gw-0.5.0/examples/dataset_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/dataset_generation/asd_dataset_settings_synthetic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.449245 dingo-gw-0.5.0/examples/gnpe_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/gnpe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/gnpe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/gnpe_model/asd_dataset_settings_fiducial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/gnpe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/gnpe_model/train_settings_init.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/gnpe_model/waveform_dataset_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.449245 dingo-gw-0.5.0/examples/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/misc/is_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/misc/stage_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.453245 dingo-gw-0.5.0/examples/npe_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/npe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/npe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/npe_model/asd_dataset_settings_fiducial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/npe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/npe_model/waveform_dataset_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.453245 dingo-gw-0.5.0/examples/toy_npe_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/toy_npe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/toy_npe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/toy_npe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/examples/toy_npe_model/waveform_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:59:39.461245 dingo-gw-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.393245 dingo-gw-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.453245 dingo-gw-0.5.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/core/test_enets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/core/test_nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/core/test_posterior_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/core/testutils_enets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.457245 dingo-gw-0.5.0/tests/gw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.457245 dingo-gw-0.5.0/tests/gw/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/conversion/test_spin_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/conversion/test_time_delay_from_geocenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/test_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/test_noise_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/test_prior_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/test_waveform_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.457245 dingo-gw-0.5.0/tests/gw/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/transforms/test_detector_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/transforms/test_general_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/transforms/test_gnpe_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/transforms/test_parameter_transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   263605 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/transforms/waveform_data.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:59:39.461245 dingo-gw-0.5.0/tests/gw/waveform_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/waveform_generator/test_wfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-20 21:59:14.000000 dingo-gw-0.5.0/tests/gw/waveform_generator/test_wfg_m.py
```

### Comparing `dingo-gw-0.4.3/.github/workflows/python-publish.yml` & `dingo-gw-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/.readthedocs.yaml` & `dingo-gw-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/LICENSE` & `dingo-gw-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/PKG-INFO` & `dingo-gw-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingo-gw
-Version: 0.4.3
+Version: 0.5.0
 Summary: Deep inference for gravitational-wave observations
 Author-email: Maximilian Dax <maximilian.dax@tuebingen.mpg.de>, Stephen Green <Stephen.Green2@nottingham.ac.uk>
 License: MIT
 Project-URL: homepage, https://github.com/dingo-gw/dingo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,22 +36,29 @@
 * performing inference on real or simulated data; and
 * verifying and correcting model results using importance sampling.
 
 ## Installation
 
 ### Pip
 
-The easiest way to install Dingo is using pip. Within a suitable virtual environment, run
-the command
+To install using pip, run the following within a suitable virtual environment:
 ```sh
 pip install dingo-gw
 ```
-This will install Dingo as well as all of its requirements, listed in
+This will install Dingo as well as all of its requirements, which are listed in
 [pyproject.toml](https://github.com/dingo-gw/dingo/blob/main/pyproject.toml).
 
+### Conda
+
+Dingo is also available from the [conda-forge](https://conda-forge.org) repository.
+To install using conda, first activate a conda environment, and then run
+```sh
+conda install -c conda-forge dingo-gw
+```
+
 ### Development install
 
 If you would like to make changes to Dingo, or to contribute to its development, you
 should install Dingo from source. To do so, first clone this repository:
 ```sh
 git clone git@github.com:dingo-gw/dingo.git
 ```
```

### Comparing `dingo-gw-0.4.3/README.md` & `dingo-gw-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,29 @@
 * performing inference on real or simulated data; and
 * verifying and correcting model results using importance sampling.
 
 ## Installation
 
 ### Pip
 
-The easiest way to install Dingo is using pip. Within a suitable virtual environment, run
-the command
+To install using pip, run the following within a suitable virtual environment:
 ```sh
 pip install dingo-gw
 ```
-This will install Dingo as well as all of its requirements, listed in
+This will install Dingo as well as all of its requirements, which are listed in
 [pyproject.toml](https://github.com/dingo-gw/dingo/blob/main/pyproject.toml).
 
+### Conda
+
+Dingo is also available from the [conda-forge](https://conda-forge.org) repository.
+To install using conda, first activate a conda environment, and then run
+```sh
+conda install -c conda-forge dingo-gw
+```
+
 ### Development install
 
 If you would like to make changes to Dingo, or to contribute to its development, you
 should install Dingo from source. To do so, first clone this repository:
 ```sh
 git clone git@github.com:dingo-gw/dingo.git
 ```
```

### Comparing `dingo-gw-0.4.3/compatibility/remove_domain_window_factor.py` & `dingo-gw-0.5.0/compatibility/remove_domain_window_factor.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/compatibility/update_model_input_dims.py` & `dingo-gw-0.5.0/compatibility/update_model_input_dims.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/compatibility/update_model_metadata.py` & `dingo-gw-0.5.0/compatibility/update_model_metadata.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/compatibility/update_saved_model_for_train_stages.py` & `dingo-gw-0.5.0/compatibility/update_saved_model_for_train_stages.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/compatibility/update_saved_model_gnpe_context_names.py` & `dingo-gw-0.5.0/compatibility/update_saved_model_gnpe_context_names.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/compatibility/update_saved_model_new_gnpe.py` & `dingo-gw-0.5.0/compatibility/update_saved_model_new_gnpe.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/compatibility/update_saved_model_new_truncation.py` & `dingo-gw-0.5.0/compatibility/update_saved_model_new_truncation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/dataset.py` & `dingo-gw-0.5.0/dingo/core/dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/density/interpolation.py` & `dingo-gw-0.5.0/dingo/core/density/interpolation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/density/nde_settings.py` & `dingo-gw-0.5.0/dingo/core/density/nde_settings.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/density/unconditional_density_estimation.py` & `dingo-gw-0.5.0/dingo/core/density/unconditional_density_estimation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/likelihood.py` & `dingo-gw-0.5.0/dingo/core/likelihood.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/models/posterior_model.py` & `dingo-gw-0.5.0/dingo/core/models/posterior_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 TODO: Docstring
 """
 
 from typing import Callable
 import torch
 import dingo.core.utils as utils
 from torch.utils.data import Dataset
+import os
 import time
+import numpy as np
 from threadpoolctl import threadpool_limits
 import dingo.core.utils.trainutils
 import math
+import h5py
+import json
+from collections import OrderedDict
 
 from dingo.core.nn.nsf import (
     create_nsf_with_rb_projection_embedding_net,
     create_nsf_wrapped,
 )
 from dingo.core.utils.misc import get_version
 
@@ -181,14 +186,55 @@
                 model_dict["optimizer_state_dict"] = self.optimizer.state_dict()
             if self.scheduler is not None:
                 model_dict["scheduler_state_dict"] = self.scheduler.state_dict()
             # TODO
 
         torch.save(model_dict, model_filename)
 
+
+    def _load_model_from_hdf5(
+        self,
+        model_filename: str
+    ):
+        """
+        Helper function to load a trained model that has been
+        saved in HDF5 format using `dingo_pt_to_hdf5`.
+
+        Parameters
+        ----------
+        model_filename: str
+            path to saved model; must have extension '.hdf5'
+
+        Returns
+        -------
+        d: dict
+            A stripped down version of the dict saved by torch.save()
+            Specifically, it does not include 'optimizer_state_dict'
+            to save space at inference time.
+        """
+        d = {}
+        with h5py.File(model_filename, 'r') as fp:
+            model_basename = os.path.basename(model_filename)
+            if fp.attrs['CANONICAL_FILE_BASENAME'] != model_basename:
+                raise ValueError('HDF5 attribute CANONICAL_FILE_BASENAME differs from model name',
+                        model_basename)
+
+            # Load small nested dicts from json
+            for k, v in fp['serialized_dicts'].items():
+                d[k] = json.loads(v[()])
+
+            # Load model weights
+            model_state_dict = OrderedDict()
+            for k, v in fp['model_weights'].items():
+                model_state_dict[k] = torch.from_numpy(np.array(v, dtype=np.float32))
+            d['model_state_dict'] = model_state_dict
+
+        return d
+
+
     def load_model(
         self,
         model_filename: str,
         load_training_info: bool = True,
         device: str = "cuda",
     ):
         """
@@ -198,19 +244,24 @@
         ----------
         model_filename: str
             path to saved model
         load_training_info: bool #TODO: load information for training
             specifies whether information required to proceed with training is
             loaded, e.g. optimizer state dict
         """
-
         # Make sure that when the model is loaded, the torch tensors are put on the
         # device indicated in the saved metadata. External routines run on a cpu
         # machine may have moved the model from 'cuda' to 'cpu'.
-        d = torch.load(model_filename, map_location=device)
+        ext = os.path.splitext(model_filename)[-1]
+        if ext == '.pt':
+            d = torch.load(model_filename, map_location=device)
+        elif ext == '.hdf5':
+            d = self._load_model_from_hdf5(model_filename)
+        else:
+            raise ValueError('Models should be ether in .pt or .hdf5 format.')
 
         self.version = d.get("version")
 
         self.model_kwargs = d["model_kwargs"]
         self.initialize_model()
         self.model.load_state_dict(d["model_state_dict"])
```

### Comparing `dingo-gw-0.4.3/dingo/core/multiprocessing.py` & `dingo-gw-0.5.0/dingo/core/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/nn/enets.py` & `dingo-gw-0.5.0/dingo/core/nn/enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/nn/nsf.py` & `dingo-gw-0.5.0/dingo/core/nn/nsf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/result.py` & `dingo-gw-0.5.0/dingo/core/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -645,14 +645,16 @@
                 f"Target log probabilities\n({n_below} below {y_lower:.2f})\n"
                 f"log(evidence) = {self.log_evidence:.3f} +- {self.log_evidence_std:.3f}"
             )
             plt.scatter(x, y, s=0.5)
             plt.plot([y_upper - 20, y_upper], [y_upper - 20, y_upper], color="black")
             plt.tight_layout()
             plt.savefig(filename)
+        else:
+            print("Results not importance sampled. Cannot produce log_prob plot.")
 
     def plot_weights(self, filename="weights.png"):
         """Make a scatter plot of samples weights vs log proposal."""
         theta = self._cleaned_samples()
         if "weights" in theta and "log_prob" in theta:
             x = theta["log_prob"].to_numpy()
             y = theta["weights"].to_numpy()
@@ -672,14 +674,16 @@
                 f"Importance sampling weights\n({n_below} below {y_lower})\n"
                 f"Effective samples: {self.n_eff:.0f} (Efficiency = "
                 f"{100 * self.sample_efficiency:.2f}%)."
             )
             plt.scatter(x, y, s=0.5)
             plt.tight_layout()
             plt.savefig(filename)
+        else:
+            print("Results not importance sampled. Cannot plot weights.")
 
 
 def check_equal_dict_of_arrays(a, b):
 
     if type(a) != type(b):
         return False
```

### Comparing `dingo-gw-0.4.3/dingo/core/samplers.py` & `dingo-gw-0.5.0/dingo/core/samplers.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/condor_utils.py` & `dingo-gw-0.5.0/dingo/core/utils/condor_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/gnpeutils.py` & `dingo-gw-0.5.0/dingo/core/utils/gnpeutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/logging_utils.py` & `dingo-gw-0.5.0/dingo/core/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/misc.py` & `dingo-gw-0.5.0/dingo/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/plotting.py` & `dingo-gw-0.5.0/dingo/core/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/torchutils.py` & `dingo-gw-0.5.0/dingo/core/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/core/utils/trainutils.py` & `dingo-gw-0.5.0/dingo/core/utils/trainutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/SVD.py` & `dingo-gw-0.5.0/dingo/gw/SVD.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/conversion/spin_conversion.py` & `dingo-gw-0.5.0/dingo/gw/conversion/spin_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,29 +173,33 @@
                 f"{sc_phase}."
             )
 
     phase_old = sc_phase_old
     phase_new = sc_phase_new
     samples_new = {}
     for idx, sample in samples.to_dict(orient="index").items():
-        if sc_phase_old is None:
-            phase_old = sample["phase"]
-        if sc_phase_new is None:
-            phase_new = sample["phase"]
+        try:
+            if sc_phase_old is None:
+                phase_old = sample["phase"]
+            if sc_phase_new is None:
+                phase_new = sample["phase"]
 
-        # transform to cartesian spins (which is the fundamental basis, independent of
-        # the phase) with the old spin conversion phase, and back to PE spins with the
-        # new spin conversion phase
-        sample_cartesian = cartesian_spins({**sample, "phase": phase_old}, f_ref)
-        sample_pe_new = pe_spins({**sample_cartesian, "phase": phase_new}, f_ref)
+            # transform to cartesian spins (which is the fundamental basis, independent of
+            # the phase) with the old spin conversion phase, and back to PE spins with the
+            # new spin conversion phase
+            sample_cartesian = cartesian_spins({**sample, "phase": phase_old}, f_ref)
+            sample_pe_new = pe_spins({**sample_cartesian, "phase": phase_new}, f_ref)
 
-        # The conversions above will set the phase parameter to sc_phase_new, however,
-        # this is only the phase used for spin conversion, *not* the actual phase for
-        # the parameters. Below, we set the phase to its correct (i.e., input) value.
-        if "phase" in sample:
-            sample_pe_new["phase"] = sample["phase"]
-        else:
-            sample_pe_new.pop("phase")
+            # The conversions above will set the phase parameter to sc_phase_new, however,
+            # this is only the phase used for spin conversion, *not* the actual phase for
+            # the parameters. Below, we set the phase to its correct (i.e., input) value.
+            if "phase" in sample:
+                sample_pe_new["phase"] = sample["phase"]
+            else:
+                sample_pe_new.pop("phase")
 
-        samples_new[idx] = sample_pe_new
+            samples_new[idx] = sample_pe_new
+        except RuntimeError:
+            print("Failed to convert spins. Saving sample unchanged.")
+            samples_new[idx] = sample
 
     return pd.DataFrame.from_dict(samples_new, orient="index")
```

### Comparing `dingo-gw-0.4.3/dingo/gw/data/data_download.py` & `dingo-gw-0.5.0/dingo/gw/data/data_download.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/data/data_preparation.py` & `dingo-gw-0.5.0/dingo/gw/data/data_preparation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/dataset/generate_dataset.py` & `dingo-gw-0.5.0/dingo/gw/dataset/generate_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 from torchvision.transforms import Compose
 from bilby.gw.prior import BBHPriorDict
 
 from dingo.gw.dataset.waveform_dataset import WaveformDataset
 from dingo.gw.prior import build_prior_with_defaults
 from dingo.gw.domains import build_domain
 from dingo.gw.transforms import WhitenFixedASD
-from dingo.gw.waveform_generator import WaveformGenerator, generate_waveforms_parallel
+from dingo.gw.waveform_generator import (
+    WaveformGenerator,
+    NewInterfaceWaveformGenerator,
+    generate_waveforms_parallel,
+)
 from dingo.gw.SVD import SVDBasis, ApplySVD
 
 
 def generate_parameters_and_polarizations(
     waveform_generator: WaveformGenerator,
     prior: BBHPriorDict,
     num_samples: int,
@@ -145,18 +149,26 @@
     Returns
     -------
     A WaveformDataset based on the settings.
     """
 
     prior = build_prior_with_defaults(settings["intrinsic_prior"])
     domain = build_domain(settings["domain"])
-    waveform_generator = WaveformGenerator(
-        domain=domain,
-        **settings["waveform_generator"],
-    )
+
+    new_interface_flag = settings["waveform_generator"].get("new_interface", False)
+    if new_interface_flag:
+        waveform_generator = NewInterfaceWaveformGenerator(
+            domain=domain,
+            **settings["waveform_generator"],
+        )
+    else:
+        waveform_generator = WaveformGenerator(
+            domain=domain,
+            **settings["waveform_generator"],
+        )
 
     dataset_dict = {"settings": settings}
 
     if "compression" in settings:
         compression_transforms = []
 
         if "whitening" in settings["compression"]:
```

### Comparing `dingo-gw-0.4.3/dingo/gw/dataset/generate_dataset_dag.py` & `dingo-gw-0.5.0/dingo/gw/dataset/generate_dataset_dag.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/dataset/utils.py` & `dingo-gw-0.5.0/dingo/gw/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/dataset/waveform_dataset.py` & `dingo-gw-0.5.0/dingo/gw/dataset/waveform_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/domains.py` & `dingo-gw-0.5.0/dingo/gw/domains.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/download_strain_data.py` & `dingo-gw-0.5.0/dingo/gw/download_strain_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,48 +6,57 @@
 from dingo.gw.gwutils import (
     get_window,
     get_window_factor,
 )
 
 
 def estimate_single_psd(
-    det, time_start, time_segment, window, f_s=4096, num_segments: int = 128, channel=None
+    time_start,
+    time_segment,
+    window,
+    f_s=4096,
+    num_segments: int = 128,
+    det=None,
+    channel=None,
 ):
     """
     Download strain data and generate a PSD based on these. Use num_segments of length
-    time_segment, starting at GPS time time_start.
+    time_segment, starting at GPS time time_start. If no channel is specified, GWOSC is used
+    to download the data.
 
     Parameters
     ----------
-    det: str
-        detector
     time_start: float
         start GPS time for PSD estimation
     time_segment: float
         time for a single segment for PSD information, in seconds
     window: Union(np.ndarray, dict)
         Window used for PSD generation, needs to be the same as used for Fourier
         transform of event strain data.
         Either provided directly as np.ndarray, or as dict in which case the window is
         generated by window = dingo.gw.gwutils.get_window(**window).
     num_segments: int = 256
         number of segments used for PSD generation
+    det: str
+        If provided, will download data from GWOSC using TimeSeries.fetch_open_data(). Mutually exclusive with 'channel'.
     channel: str
         If provided, will download the data from the channel instead of gwosc using TimeSeries.get()
     Returns
     -------
     psd: np.array
         array of psd
     """
     # download strain data for psd
     time_end = time_start + time_segment * num_segments
+    assert (
+        det is not None and channel is None or det is None and channel is not None
+    ), "det and channel are mutually exclusive!"
+
     if channel:
-        psd_strain = TimeSeries.get(
-            channel, time_start, time_end
-        )
+        psd_strain = TimeSeries.get(channel, time_start, time_end)
         # TODO: We currently assume that sample rate of channel matches that provided in the settings?
     else:
         psd_strain = TimeSeries.fetch_open_data(
             det, time_start, time_end, sample_rate=f_s, cache=False
         )
     psd_strain = psd_strain.to_pycbc()
 
@@ -159,22 +168,22 @@
     for det in detectors:
         print("Detector {:}:".format(det))
 
         data["waveform"][det] = download_strain_data_in_FD(
             det, time_event, time_segment, time_buffer, window
         )
         data["asds"][det] = (
-                estimate_single_psd(
-                det,
+            estimate_single_psd(
                 time_event + time_buffer - time_segment * (num_segments_psd + 1),
                 time_segment,
                 window,
                 num_segments_psd,
+                det=det
             )
-                ** 0.5
+            ** 0.5
         )
 
     # build domain object
     f_s = len(data["waveform"][detectors[0]]) / time_segment
     domain = FrequencyDomain(
         f_min=0,
         f_max=f_s / 2,
```

### Comparing `dingo-gw-0.4.3/dingo/gw/gwutils.py` & `dingo-gw-0.5.0/dingo/gw/gwutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/importance_sampling/diagnostics.py` & `dingo-gw-0.5.0/dingo/gw/importance_sampling/diagnostics.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/importance_sampling/importance_weights.py` & `dingo-gw-0.5.0/dingo/gw/importance_sampling/importance_weights.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/inference/gw_samplers.py` & `dingo-gw-0.5.0/dingo/gw/inference/gw_samplers.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/inference/inference_pipeline.py` & `dingo-gw-0.5.0/dingo/gw/inference/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/inference/visualization.py` & `dingo-gw-0.5.0/dingo/gw/inference/visualization.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/injection.py` & `dingo-gw-0.5.0/dingo/gw/injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from dingo.gw.prior import build_prior_with_defaults, split_off_extrinsic_parameters
 from dingo.gw.transforms import (
     GetDetectorTimes,
     ProjectOntoDetectors,
     WhitenAndScaleStrain,
     ApplyCalibrationUncertainty,
 )
-from dingo.gw.waveform_generator.waveform_generator import WaveformGenerator
+from dingo.gw.waveform_generator.waveform_generator import (
+    WaveformGenerator,
+    NewInterfaceWaveformGenerator,
+)
 
 
 class GWSignal(object):
     """
     Base class for generating gravitational wave signals in interferometers. Generates
     waveform polarizations based on provided parameters, and then projects to detectors.
 
@@ -54,21 +57,29 @@
         self._check_domains(wfg_domain, data_domain)
         self.data_domain = data_domain
 
         # The waveform generator potentially has a larger frequency range than the
         # domain of the trained network / requested injection / etc. This is typically
         # the case for EOB waveforms, which require the larger range to generate
         # robustly. For this reason we have two domains.
-        self.waveform_generator = WaveformGenerator(domain=wfg_domain, **wfg_kwargs)
+
+        new_interface_flag = wfg_kwargs.get("new_interface", False)
+        if new_interface_flag:
+            self.waveform_generator = NewInterfaceWaveformGenerator(
+                domain=wfg_domain, **wfg_kwargs
+            )
+        else:
+            self.waveform_generator = WaveformGenerator(domain=wfg_domain, **wfg_kwargs)
 
         self.t_ref = t_ref
         self.ifo_list = InterferometerList(ifo_list)
 
         # When we set self.whiten, the projection transforms are automatically prepared.
         self._calibration_envelope = None
+        self._calibration_marginalization_kwargs = None
         self.whiten = False
 
         self.asd = None
 
     @staticmethod
     def _check_domains(domain_in, domain_out):
         if domain_in.f_min > domain_out.f_min or domain_in.f_max < domain_out.f_max:
@@ -87,39 +98,46 @@
 
     @whiten.setter
     def whiten(self, value):
         self._whiten = value
         self._initialize_transform()
 
     @property
-    def calibration_envelope(self):
+    def calibration_marginalization_kwargs(self):
         """
-        Either None, str 'generate' or a dict with
-        {"H1": filepath, "L1":filepath, ...} with locations of
-        lookup tables for the calibration uncertainty curves
+        Dictionary with the following keys:
+
+        calibration_envelope
+            Dictionary of the form {"H1": filepath, "L1": filepath, ...} with locations of
+            lookup tables for the calibration uncertainty curves.
+
+        num_calibration_nodes
+            Number of nodes for the calibration model.
+
+        num_calibration_curves
+            Number of calibration curves to use in marginalization.
         """
-        return self._calibration_envelope
+        return self._calibration_marginalization_kwargs
 
-    @calibration_envelope.setter
-    def calibration_envelope(self, value):
-        self._calibration_envelope = value
+    @calibration_marginalization_kwargs.setter
+    def calibration_marginalization_kwargs(self, value):
+        self._calibration_marginalization_kwargs = value
         self._initialize_transform()
 
     def _initialize_transform(self):
         transforms = [
             GetDetectorTimes(self.ifo_list, self.t_ref),
             ProjectOntoDetectors(self.ifo_list, self.data_domain, self.t_ref),
         ]
-        if self.calibration_envelope is not None:
+        if self.calibration_marginalization_kwargs:
             transforms.append(
                 ApplyCalibrationUncertainty(
                     self.ifo_list,
                     self.data_domain,
-                    self.calibration_envelope,
-                    self.num_calibration_curves,
+                    **self.calibration_marginalization_kwargs,
                 )
             )
         if self.whiten:
             transforms.append(WhitenAndScaleStrain(self.data_domain.noise_std))
         self.projection_transforms = Compose(transforms)
 
     def signal(self, theta):
```

### Comparing `dingo-gw-0.4.3/dingo/gw/likelihood.py` & `dingo-gw-0.5.0/dingo/gw/likelihood.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from multiprocessing import Pool
 
 import numpy as np
 import pandas as pd
 from scipy.fft import fft
 from scipy.special import logsumexp
 from bilby.gw.utils import ln_i0
@@ -116,41 +117,16 @@
             if not self.pm_approx_22_mode:
                 n_grid = phase_marginalization_kwargs.get("n_grid", 1_000)
                 # use endpoint = False for grid, since phase = 0/2pi are equivalent
                 self.phase_grid = np.linspace(0, 2 * np.pi, n_grid, endpoint=False)
             else:
                 print("Using phase marginalization with (2,2) mode approximation.")
 
-        # optionally initialize calibration marginalization
-        self.calibration_marginalization = False
-        if calibration_marginalization_kwargs is not None:
-            self.calibration_marginalization = True
-            self.initialize_calibration_marginalization(
-                **calibration_marginalization_kwargs
-            )
-
-    def initialize_calibration_marginalization(
-        self, calibration_envelope, num_calibration_curves=1
-    ):
-        """
-        Initialize calibration marginalization table which will use the files provided to
-        multiply the signal by a calibration envelope.
-
-        Parameters
-        ----------
-        num_calibration_curves : int
-            The number of calibration curves to average over. Will default to 1. Increasing this will
-            decrease the sample efficiency due to the calibration errors.
-
-        calibration_lookup_table : dict
-            Dict with locations of .h5 files of calibration envelopes {"H1":, filepath,...}
-            optionally can be set to 'generate'
-        """
-        self.num_calibration_curves = num_calibration_curves
-        self.calibration_envelope = calibration_envelope
+        # Initialize calibration marginalization using the setter from GWSignal.
+        self.calibration_marginalization_kwargs = calibration_marginalization_kwargs
 
     def initialize_time_marginalization(self, t_lower, t_upper, n_fft=1):
         """
         Initialize time marginalization. Time marginalization can be performed via FFT,
         which is super fast. However, this limits the time resolution to delta_t =
         1/self.data_domain.f_max. In order to allow for a finer time resolution we
         compute the time marginalized likelihood n_fft via FFT on a grid of n_fft
@@ -201,29 +177,29 @@
 
     def log_likelihood(self, theta):
         if (
             sum(
                 [
                     self.time_marginalization,
                     self.phase_marginalization,
-                    self.calibration_marginalization,
+                    bool(self.calibration_marginalization_kwargs),
                 ]
             )
             > 1
         ):
             raise NotImplementedError(
                 "Only one out of time-marginalization, phase-marginalization and calibration-marginalization "
                 "can be used at a time."
             )
 
         if self.time_marginalization:
             return self._log_likelihood_time_marginalized(theta)
         elif self.phase_marginalization:
             return self._log_likelihood_phase_marginalized(theta)
-        elif self.calibration_marginalization:
+        elif self.calibration_marginalization_kwargs:
             return self._log_likelihood_calibration_marginalized(theta)
         else:
             return self._log_likelihood(theta)
 
     def _log_likelihood(self, theta):
         """
         The likelihood is given by
@@ -545,33 +521,37 @@
         -------
         log_likelihood: float
         """
 
         # Step 1: Compute whitened GW strain mu(theta) for parameters theta.
         mu = self.signal(theta)["waveform"]
         d = self.whitened_strains
-        d = {ifo: np.tile(v, (self.num_calibration_curves, 1)) for ifo, v in d.items()}
+
+        # In the calibration-marginalization case, the values of mu for each detector
+        # have an additional leading dimension, which corresponds to the calibration
+        # draws. These are averaged over in computing the likelihood.
+        # TODO: Combine with _log_likelihood() into a single method.
 
         # Step 2: Compute likelihood. log_Zn is precomputed, so we only need to
         # compute the remaining terms rho2opt and kappa2
 
         rho2opt = np.sum(
             [inner_product(mu_ifo.T, mu_ifo.T) for mu_ifo in mu.values()], axis=0
         )
         kappa2 = np.sum(
             [
-                inner_product(d_ifo.T, mu_ifo.T)
+                inner_product(d_ifo[:, None], mu_ifo.T)
                 for d_ifo, mu_ifo in zip(d.values(), mu.values())
             ],
             axis=0,
         )
 
         likelihoods = self.log_Zn + kappa2 - 1 / 2.0 * rho2opt
         # Return the average over calibration envelopes
-        return np.mean(likelihoods)
+        return logsumexp(likelihoods) - np.log(len(likelihoods))
 
     def d_inner_h_complex_multi(
         self, theta: pd.DataFrame, num_processes: int = 1
     ) -> np.ndarray:
         """
         Calculate the complex inner product (d | h(theta)) between the stored data d
         and a simulated waveform with given parameters theta. Works with multiprocessing.
@@ -584,15 +564,14 @@
             Number of parallel processes to use.
 
         Returns
         -------
         complex : Inner product
         """
         with threadpool_limits(limits=1, user_api="blas"):
-
             # Generator object for theta rows. For idx this yields row idx of
             # theta dataframe, converted to dict, ready to be passed to
             # self.log_likelihood.
             theta_generator = (d[1].to_dict() for d in theta.iterrows())
 
             if num_processes > 1:
                 with Pool(processes=num_processes) as pool:
```

### Comparing `dingo-gw-0.4.3/dingo/gw/ls_cli.py` & `dingo-gw-0.5.0/dingo/gw/ls_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 from pathlib import Path
 
 import h5py
 import torch
 import yaml
+import json
+from pprint import pprint
 
 from dingo.core.dataset import DingoDataset
 from dingo.gw.SVD import SVDBasis
 from dingo.core.result import Result
 from dingo.gw.dataset import WaveformDataset
 from dingo.gw.noise.asd_dataset import ASDDataset
 
@@ -118,14 +120,27 @@
                 + "--------\n"
                 + yaml.dump(
                     asd_dataset.settings,
                     default_flow_style=False,
                     sort_keys=False,
                 )
             )
+
+        elif dataset_type == "trained_model":
+            with h5py.File(args.file_name, "r") as f:
+                print("Extracting information about torch model.\n")
+                print(f"Version: {f.attrs['version']}")
+                print(f"Model epoch: {f.attrs['epoch']}")
+                print("Model metadata:")
+
+                for d in ['model_kwargs', 'metadata']:
+                    json_data = json.loads(f['serialized_dicts'][d][()])
+                    print(f"\n{d}:\n" + "-"*(len(d)+1))
+                    pprint(json_data)
+
         else:
             # Legacy (before dataset_type identifier).
             try:
                 svd = SVDBasis(file_name=args.file_name)
                 print(f"SVD dataset of size n={svd.n}.")
                 print("Validation summary:")
                 svd.print_validation_summary()
```

### Comparing `dingo-gw-0.4.3/dingo/gw/noise/asd_dataset.py` & `dingo-gw-0.5.0/dingo/gw/noise/asd_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         domain_update : dict
             If provided, update domain from existing domain using new settings.
         """
         self.precision = precision
         super().__init__(
             file_name=file_name,
             dictionary=dictionary,
-            data_keys=["asds", "gps_times"],
+            data_keys=["asds", "gps_times", "asd_parameterizations"],
         )
 
         if ifos is not None:
             for ifo in list(self.asds.keys()):
                 if ifo not in ifos:
                     self.asds.pop(ifo)
                     self.gps_times.pop(ifo)
```

### Comparing `dingo-gw-0.4.3/dingo/gw/noise/asd_estimation.py` & `dingo-gw-0.5.0/dingo/gw/noise/asd_estimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     data_dir: str,
     settings: dict,
     time_segments: dict,
     verbose=False,
 ):
     """
     Downloads strain data for the specified time segments and estimates PSDs based on these
+
     Parameters
     ----------
     data_dir : str
         Path to the directory where the PSD dataset will be stored
     settings : dict
         Settings that determine the segments
     time_segments : dict
@@ -69,22 +70,24 @@
     }
     w = get_window(window_kwargs)
     asd_filename_list = {det: [] for det in detectors}
     for det in detectors:
         psd_path = psd_data_path(data_dir, run, det)
         os.makedirs(psd_path, exist_ok=True)
         estimation_kwargs = {
-            "det": det,
             "time_segment": T,
             "window": w,
             "f_s": f_s,
             "num_segments": int(time_psd / T),
         }
         if channels:
             estimation_kwargs["channel"] = channels[det]
+        else:
+            estimation_kwargs["det"] = det
+
         for index, (start, end) in enumerate(
             tqdm(time_segments[det], disable=not verbose)
         ):
             filename = join(psd_path, f"asd_{start}.hdf5")
             asd_filename_list[det].append(filename)
             if not os.path.exists(filename):
                 dataset_dict = {
@@ -112,21 +115,21 @@
     parallelized ASD dataset generation.
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--data_dir",
         type=str,
         required=True,
-        help="Path where the PSD data is to be stored. Must contain a 'settings.yaml' file.",
+        help="Path where the PSD data is to be stored.",
     )
     parser.add_argument(
         "--settings_file",
         type=str,
         required=True,
-        help="Path to a settings file in case two different datasets are generated in the sam directory",
+        help="Path to a settings file containing the settings for the dataset generation",
     )
     parser.add_argument(
         "--time_segments_file",
         type=str,
         default=None,
         help="Path to a file containing the time segments for which PSDs should be estimated",
     )
```

### Comparing `dingo-gw-0.4.3/dingo/gw/noise/generate_dataset.py` & `dingo-gw-0.5.0/dingo/gw/noise/generate_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         except:
             pass
 
         dagman.build()
         print(f"DAG submission file written.")
 
     else:
+
         print("Downloading strain data and estimating PSDs...")
         asd_filename_list = download_and_estimate_psds(
             args.data_dir, settings, time_segments, verbose=args.verbose
         )
         asd_dataset_list = {
             det: [ASDDataset(asd_file) for asd_file in asd_file_list]
             for det, asd_file_list in asd_filename_list.items()
```

### Comparing `dingo-gw-0.4.3/dingo/gw/noise/generate_dataset_dag.py` & `dingo-gw-0.5.0/dingo/gw/noise/generate_dataset_dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     return "".join([f"--{k} {v} " for k, v in args_dict.items()])
 
 
 def split_time_segments(time_segments, condor_dir, num_jobs):
     """
     Split up all time segments used for estimating PSDs into num_jobs-many
     segments and save them into a condor directory
+
     Parameters
     ----------
     time_segments : dict
         contains all time segments used for estimating PSDs
     condor_dir : str
         path to a directory where condr-related files are stored
     num_jobs : int
@@ -48,14 +49,15 @@
     return time_segments_path_list
 
 
 def create_dag(data_dir, settings_file, time_segments, out_name):
     """
     Create a Condor DAG to (a) download, estimate,
     individual PSDs and (b) merge them into one dataset
+
     Parameters
     ----------
     data_dir : str
         Path to the directory where the PSD dataset will be stored
     settings_file : str
         Settings : Path to settings file relevant for PSD generation
     time_segments : dict
```

### Comparing `dingo-gw-0.4.3/dingo/gw/noise/utils.py` & `dingo-gw-0.5.0/dingo/gw/noise/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from gwpy.table import EventTable
 from dingo.gw.noise.asd_dataset import ASDDataset
 
 """
 Catalogue against which to check that no event is present in the estimated PSDs
 """
-CATALOGUEs = ["GWTC-1-confident", "GWTC-2.1-confident", "GWTC-3-confident"]
+CATALOGS = ["GWTC-1-confident", "GWTC-2.1-confident", "GWTC-3-confident"]
 
 """
 Contains links for PSD segment lists with quality label BURST_CAT2 from the Gravitational Wave Open Science Center.
 Some events are split up into multiple chunks such that there are multiple URLs for one observing run
 """
 URL_DIRECTORY = {
     "O1_L1": [
@@ -70,15 +70,15 @@
     the path where the data is stored
     """
     return join(data_dir, "tmp", run, detector)
 
 
 def get_event_gps_times():
     event_list = []
-    for catalogue in CATALOGUEs:
+    for catalogue in CATALOGS:
         events = EventTable.fetch_open_data(catalogue)
         event_list += list(events["GPS"])
     return event_list
 
 
 def get_time_segments(settings):
     """
@@ -178,21 +178,21 @@
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--data_dir",
         type=str,
         required=True,
-        help="Path where the PSD data is to be stored. Must contain a 'settings.yaml' file.",
+        help="Path where the PSD data is to be stored.",
     )
     parser.add_argument(
         "--settings_file",
         type=str,
         required=True,
-        help="Path to a settings file in case two different datasets are generated in the same directory",
+        help="Path to a settings file that contains the settings for the ASD dataset generation",
     )
     parser.add_argument(
         "--time_segments_file",
         type=str,
         default=None,
         help="Path to a file containing the time segments for which PSDs should be estimated",
     )
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/dag_creator.py` & `dingo-gw-0.5.0/dingo/pipe/dag_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 #
 
 import copy
 
 from bilby_pipe.job_creation.dag import Dag
 from bilby_pipe.utils import BilbyPipeError, logger
 
-from dingo.gw.pipe.nodes.generation_node import GenerationNode
+from dingo.pipe.nodes.generation_node import GenerationNode
 from .nodes.importance_sampling_node import ImportanceSamplingNode
 from .nodes.merge_node import MergeNode
+from .nodes.pe_summary_node import PESummaryNode
 from .nodes.plot_node import PlotNode
 from .nodes.sampling_node import SamplingNode
 
+logger.name = "dingo_pipe"
+
 
 def get_trigger_time_list(inputs):
     """Returns a list of GPS trigger times for each data segment"""
     # if (inputs.gaussian_noise or inputs.zero_noise) and inputs.trigger_time is None:
     #     trigger_times = [0] * inputs.n_simulation
     # elif (inputs.gaussian_noise or inputs.zero_noise) and isinstance(
     #     inputs.trigger_time, float
@@ -36,15 +39,15 @@
 def get_parallel_list(inputs):
     if inputs.n_parallel == 1:
         return [""]
     else:
         return [f"part{idx}" for idx in range(inputs.n_parallel)]
 
 
-def generate_dag(inputs):
+def generate_dag(inputs, model_args):
     inputs = copy.deepcopy(inputs)
     dag = Dag(inputs)
     trigger_times = get_trigger_time_list(inputs)
 
     #
     # 1. Generate data for inference.
     #
@@ -72,85 +75,94 @@
         sampling_node = SamplingNode(
             inputs,
             generation_node=generation_node,
             dag=dag,
         )
         sampling_node_list.append(sampling_node)
 
-    #
-    # 3. Generate new data for importance sampling **if different settings requested**.
-    #
-    # If injecting into simulated noise, be sure to use consistent noise realization.
+    if inputs.importance_sample:
+        #
+        # 3. Generate new data for importance sampling **if different settings requested**.
+        #
+        # If injecting into simulated noise, be sure to use consistent noise realization.
+
+        if len(inputs.importance_sampling_updates) > 0:
+            # Iterate over all generation nodes and store them in a list
+            importance_sampling_generation_node_list = []
+            for idx, trigger_time in enumerate(trigger_times):
+                kwargs = dict(trigger_time=trigger_time, idx=idx, dag=dag)
+                if idx > 0:
+                    # Make all generation nodes depend on the 0th generation node
+                    # Ensures any cached files (e.g. the distance-marginalization
+                    # lookup table) are only built once.
+                    kwargs["parent"] = generation_node_list[0]
+                generation_node = GenerationNode(inputs, importance_sampling=True, **kwargs)
+                importance_sampling_generation_node_list.append(generation_node)
+        else:
+            importance_sampling_generation_node_list = generation_node_list
 
-    if len(inputs.importance_sampling_updates) > 0:
-        # Iterate over all generation nodes and store them in a list
-        importance_sampling_generation_node_list = []
-        for idx, trigger_time in enumerate(trigger_times):
-            kwargs = dict(trigger_time=trigger_time, idx=idx, dag=dag)
-            if idx > 0:
-                # Make all generation nodes depend on the 0th generation node
-                # Ensures any cached files (e.g. the distance-marginalization
-                # lookup table) are only built once.
-                kwargs["parent"] = generation_node_list[0]
-            generation_node = GenerationNode(inputs, importance_sampling=True, **kwargs)
-            importance_sampling_generation_node_list.append(generation_node)
-    else:
-        importance_sampling_generation_node_list = generation_node_list
+        #
+        # 4. Importance sample
+        #
+        # If the phase is not present and phase marginalization is not being used, also
+        # sample the phase synthetically. This adds between 1x and 50x to the cost of
+        # importance sampling, depending on the waveform model. Indeed, IMRPhenomXPHM
+        # waveform modes are much more expensive to generate than polarizations.
+
+        merged_importance_sampling_node_list = []
+        parallel_list = get_parallel_list(inputs)
+        all_parallel_node_list = []
+        for sampling_node, generation_node in zip(
+            sampling_node_list, importance_sampling_generation_node_list
+        ):
+            parallel_node_list = []
+            for parallel_idx in parallel_list:
+                importance_sampling_node = ImportanceSamplingNode(
+                    inputs,
+                    sampling_node=sampling_node,
+                    generation_node=generation_node,
+                    parallel_idx=parallel_idx,
+                    dag=dag,
+                )
+                parallel_node_list.append(importance_sampling_node)
+                all_parallel_node_list.append(importance_sampling_node)
+
+            if len(parallel_node_list) == 1:
+                merged_importance_sampling_node_list.append(importance_sampling_node)
+            else:
+                # 4.(b) Recombine jobs into single Result.
+                #       (Automatically calculates evidence.)
+                merge_node = MergeNode(
+                    inputs=inputs,
+                    parallel_node_list=parallel_node_list,
+                    dag=dag,
+                )
+                merged_importance_sampling_node_list.append(merge_node)
 
-    #
-    # 4. Importance sample
-    #
-    # If the phase is not present and phase marginalization is not being used, also
-    # sample the phase synthetically. This adds between 1x and 50x to the cost of
-    # importance sampling, depending on the waveform model. Indeed, IMRPhenomXPHM
-    # waveform modes are much more expensive to generate than polarizations.
-
-    merged_importance_sampling_node_list = []
-    parallel_list = get_parallel_list(inputs)
-    all_parallel_node_list = []
-    for sampling_node, generation_node in zip(
-        sampling_node_list, importance_sampling_generation_node_list
-    ):
-        parallel_node_list = []
-        for parallel_idx in parallel_list:
-            importance_sampling_node = ImportanceSamplingNode(
-                inputs,
-                sampling_node=sampling_node,
-                generation_node=generation_node,
-                parallel_idx=parallel_idx,
-                dag=dag,
-            )
-            parallel_node_list.append(importance_sampling_node)
-            all_parallel_node_list.append(importance_sampling_node)
-
-        if len(parallel_node_list) == 1:
-            merged_importance_sampling_node_list.append(importance_sampling_node)
-        else:
-            # 4.(b) Recombine jobs into single Result.
-            #       (Automatically calculates evidence.)
-            merge_node = MergeNode(
-                inputs=inputs,
-                parallel_node_list=parallel_node_list,
-                dag=dag,
-            )
-            merged_importance_sampling_node_list.append(merge_node)
+    else:
+        merged_importance_sampling_node_list = sampling_node_list
 
     #
     # 5. Plotting
     #
 
     plot_nodes_list = []
     for merged_node in merged_importance_sampling_node_list:
         if inputs.plot_node_needed:
             plot_nodes_list.append(PlotNode(inputs, merged_node, dag=dag))
 
     #
     # 6. PESummary
     #
 
+    if inputs.create_summary:
+        # Add the waveform approximant to inputs, so that it can be fed to PESummary.
+        inputs.waveform_approximant = model_args["waveform_approximant"]
+        PESummaryNode(inputs, merged_importance_sampling_node_list, generation_node_list, dag=dag)
+
     dag.build()
     # create_overview(
     #     inputs,
     #     generation_node_list,
     #     all_parallel_node_list,
     #     merged_node_list,
     #     plot_nodes_list,
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/data_generation.py` & `dingo-gw-0.5.0/dingo/pipe/data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import sys
 
 from bilby_pipe.input import Input
 from bilby_pipe.main import parse_args
-from bilby_pipe.utils import log_version_information, logger, convert_string_to_dict
+from bilby_pipe.utils import logger, convert_string_to_dict
 from bilby_pipe.data_generation import DataGenerationInput as BilbyDataGenerationInput
 
 from dingo.gw.data.event_dataset import EventDataset
 from dingo.gw.domains import FrequencyDomain
-from dingo.gw.pipe.parser import create_parser
+from dingo.pipe.parser import create_parser
+
+logger.name = "dingo_pipe"
 
 
 class DataGenerationInput(BilbyDataGenerationInput):
     def __init__(self, args, unknown_args, create_data=True):
         Input.__init__(self, args, unknown_args)
 
         # Generic initialisation
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/default_settings.py` & `dingo-gw-0.5.0/dingo/pipe/default_settings.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/dingo_result.py` & `dingo-gw-0.5.0/dingo/pipe/dingo_result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/importance_sampling.py` & `dingo-gw-0.5.0/dingo/pipe/importance_sampling.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import sys
 
 import yaml
 from bilby_pipe.input import Input
 from bilby_pipe.utils import parse_args, logger, convert_string_to_dict
 
 from dingo.gw.data.event_dataset import EventDataset
-from dingo.gw.inference.inference_pipeline import prepare_log_prob
-from dingo.gw.pipe.default_settings import IMPORTANCE_SAMPLING_SETTINGS
-from dingo.gw.pipe.parser import create_parser
+from dingo.pipe.default_settings import IMPORTANCE_SAMPLING_SETTINGS
+from dingo.pipe.parser import create_parser
 from dingo.gw.result import Result
 
+logger.name = "dingo_pipe"
+
 
 class ImportanceSamplingInput(Input):
     def __init__(self, args, unknown_args):
         super().__init__(args, unknown_args)
 
         # Generic initialisation
         self.meta_data = dict()
@@ -76,18 +77,19 @@
         # self.extra_likelihood_kwargs = args.extra_likelihood_kwargs
         # self.enforce_signal_duration = args.enforce_signal_duration
         #
         # # ROQ
         # self.roq_folder = args.roq_folder
         # self.roq_scale_factor = args.roq_scale_factor
         #
-        # # Calibration
-        # self.calibration_model = args.calibration_model
-        # self.spline_calibration_nodes = args.spline_calibration_nodes
-        # self.spline_calibration_envelope_dict = args.spline_calibration_envelope_dict
+        # Calibration
+        self.calibration_model = args.calibration_model
+        self.spline_calibration_nodes = args.spline_calibration_nodes
+        self.spline_calibration_envelope_dict = args.spline_calibration_envelope_dict
+        self.spline_calibration_curves = args.spline_calibration_curves
 
         # # Marginalization
         # self.distance_marginalization = args.distance_marginalization
         # self.distance_marginalization_lookup_table = None
         # self.phase_marginalization = args.phase_marginalization
         # self.time_marginalization = args.time_marginalization
         # self.jitter_time = args.jitter_time
@@ -105,20 +107,34 @@
             )
 
     def _load_event(self):
         event_dataset = EventDataset(file_name=self.event_data_file)
         self.result.reset_event(event_dataset)
 
     @property
+    def calibration_marginalization_kwargs(self):
+        if self.calibration_model == "CubicSpline":
+            return {
+                "calibration_envelope": self.spline_calibration_envelope_dict,
+                "num_calibration_nodes": self.spline_calibration_nodes,
+                "num_calibration_curves": self.spline_calibration_curves,
+            }
+        elif self.calibration_model == None:
+            return None
+        else:
+            raise ValueError(
+                "The only calibration model which is supported is 'CubicSpline'"
+            )
+
+    @property
     def importance_sampling_settings(self):
         return self._importance_sampling_settings
 
     @importance_sampling_settings.setter
     def importance_sampling_settings(self, settings):
-
         # Set up defaults.
         if "phase" not in self.result.samples.columns:
             self._importance_sampling_settings = IMPORTANCE_SAMPLING_SETTINGS[
                 "PhaseRecoveryDefault"
             ]
         else:
             self._importance_sampling_settings = dict()
@@ -150,31 +166,30 @@
             num_processes=self.request_cpus,
             time_marginalization_kwargs=self.importance_sampling_settings.get(
                 "time_marginalization"
             ),
             phase_marginalization_kwargs=self.importance_sampling_settings.get(
                 "phase_marginalization"
             ),
+            calibration_marginalization_kwargs=self.calibration_marginalization_kwargs,
         )
 
         if self.prior_dict:
             logger.info("Updating prior from network prior. Changes:")
             logger.info(
                 yaml.dump(
                     self.prior_dict,
                     default_flow_style=False,
                     sort_keys=False,
                 )
             )
             self.result.update_prior(self.prior_dict)
 
         self.result.print_summary()
-        self.result.to_file(
-            os.path.join(self.result_directory, self.label + ".hdf5")
-        )
+        self.result.to_file(os.path.join(self.result_directory, self.label + ".hdf5"))
 
     @property
     def priors(self):
         """Read in and compose the prior at run-time"""
         if getattr(self, "_priors", None) is None:
             self._priors = self._get_priors(add_time=False)
         return self._priors
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/main.py` & `dingo-gw-0.5.0/dingo/pipe/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,18 @@
     logger,
     convert_string_to_dict,
 )
 
 from .dag_creator import generate_dag
 from .parser import create_parser
 
-from ..domains import build_domain_from_model_metadata
-from ...core.models import PosteriorModel
+from dingo.gw.domains import build_domain_from_model_metadata
+from dingo.core.models import PosteriorModel
+
+logger.name = "dingo_pipe"
 
 
 def fill_in_arguments_from_model(args):
     # FIXME: It would be better if we did not have to load an entire model just to
     #  gain access to the metadata. Store a copy of metadata separately?
     logger.info(f"Loading dingo model from {args.model} in order to access settings.")
     model = PosteriorModel(args.model, device="cpu", load_training_info=False)
@@ -77,15 +79,15 @@
     else:
         importance_sampling_updates = convert_string_to_dict(
             args.importance_sampling_updates
         )
         importance_sampling_updates = {
             k.replace("-", "_"): v for k, v in importance_sampling_updates.items()
         }
-    return {**changed_args, **importance_sampling_updates}
+    return {**changed_args, **importance_sampling_updates}, model_args
 
 
 class MainInput(BilbyMainInput):
     def __init__(self, args, unknown_args, importance_sampling_updates):
 
         # Settings added for dingo.
 
@@ -119,19 +121,19 @@
         self.desired_sites = args.desired_sites
         # self.analysis_executable = args.analysis_executable
         # self.analysis_executable_parser = args.analysis_executable_parser
         self.result_format = "hdf5"
         self.final_result = args.final_result
         self.final_result_nsamples = args.final_result_nsamples
 
-        # self.webdir = args.webdir
+        self.webdir = args.webdir
         self.email = args.email
         self.notification = args.notification
         self.queue = args.queue
-        # self.existing_dir = args.existing_dir
+        self.existing_dir = args.existing_dir
 
         self.scheduler = args.scheduler
         self.scheduler_args = args.scheduler_args
         self.scheduler_module = args.scheduler_module
         self.scheduler_env = args.scheduler_env
         self.scheduler_analysis_time = args.scheduler_analysis_time
 
@@ -171,14 +173,16 @@
         # self.injection_dict = args.injection_dict
         # self.injection_waveform_arguments = args.injection_waveform_arguments
         # self.injection_waveform_approximant = args.injection_waveform_approximant
         # self.generation_seed = args.generation_seed
         # if self.injection:
         #     self.check_injection()
 
+        self.importance_sample = args.importance_sample
+
         self.request_disk = args.request_disk
         self.request_memory = args.request_memory
         self.request_memory_generation = args.request_memory_generation
         self.request_cpus = args.request_cpus
         self.request_cpus_importance_sampling = args.request_cpus_importance_sampling
         # self.sampler_kwargs = args.sampler_kwargs
         # self.mpi_samplers = ["pymultinest"]
@@ -208,15 +212,15 @@
         #     setattr(self, attr, getattr(args, attr))
         #
         # self.postprocessing_executable = args.postprocessing_executable
         # self.postprocessing_arguments = args.postprocessing_arguments
         # self.single_postprocessing_executable = args.single_postprocessing_executable
         # self.single_postprocessing_arguments = args.single_postprocessing_arguments
         #
-        # self.summarypages_arguments = args.summarypages_arguments
+        self.summarypages_arguments = args.summarypages_arguments
         #
         self.psd_dict = args.psd_dict
 
         # self.check_source_model(args)
 
         self.requirements = []
         self.device = args.device
@@ -308,18 +312,18 @@
     # )
 
 
 def main():
     parser = create_parser(top_level=True)
     args, unknown_args = parse_args(get_command_line_arguments(), parser)
 
-    importance_sampling_updates = fill_in_arguments_from_model(args)
+    importance_sampling_updates, model_args = fill_in_arguments_from_model(args)
     inputs = MainInput(args, unknown_args, importance_sampling_updates)
     write_complete_config_file(parser, args, inputs)
 
     # TODO: Use two sets of inputs! The first must match the network; the second is
     #  used in importance sampling.
 
-    generate_dag(inputs)
+    generate_dag(inputs, model_args)
 
     if len(unknown_args) > 0:
         print(f"Unrecognized arguments {unknown_args}")
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/nodes/generation_node.py` & `dingo-gw-0.5.0/dingo/pipe/nodes/generation_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from bilby_pipe.job_creation.nodes import GenerationNode as BilbyGenerationNode
 
-from dingo.gw.pipe.utils import _strip_unwanted_submission_keys
+from dingo.pipe.utils import _strip_unwanted_submission_keys
 
 
 class GenerationNode(BilbyGenerationNode):
 
     def __init__(self, inputs, importance_sampling=False, **kwargs):
         self.importance_sampling = importance_sampling
         super().__init__(inputs, **kwargs)
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/nodes/importance_sampling_node.py` & `dingo-gw-0.5.0/dingo/pipe/nodes/importance_sampling_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from bilby_pipe.job_creation.nodes import AnalysisNode
 
-from dingo.gw.pipe.utils import _strip_unwanted_submission_keys
+from dingo.pipe.utils import _strip_unwanted_submission_keys
 
 
 class ImportanceSamplingNode(AnalysisNode):
     def __init__(self, inputs, sampling_node, generation_node, parallel_idx, dag):
         super(AnalysisNode, self).__init__(inputs)
         self.dag = dag
         self.sampling_node = sampling_node
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/nodes/merge_node.py` & `dingo-gw-0.5.0/dingo/pipe/nodes/merge_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bilby_pipe.job_creation.nodes import MergeNode as BilbyMergeNode
 
-from dingo.gw.pipe.utils import _strip_unwanted_submission_keys
+from dingo.pipe.utils import _strip_unwanted_submission_keys
 
 
 class MergeNode(BilbyMergeNode):
     def __init__(self, **kwargs):
         super().__init__(**kwargs, detectors=[])
         if self.inputs.simple_submission:
             _strip_unwanted_submission_keys(self.job)
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/nodes/plot_node.py` & `dingo-gw-0.5.0/dingo/pipe/nodes/plot_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bilby_pipe.job_creation.nodes import PlotNode as BilbyPlotNode
 
-from dingo.gw.pipe.utils import _strip_unwanted_submission_keys
+from dingo.pipe.utils import _strip_unwanted_submission_keys
 
 
 class PlotNode(BilbyPlotNode):
     def __init__(self, inputs, merged_node, dag):
         super(BilbyPlotNode, self).__init__(inputs)
         self.dag = dag
         self.job_name = merged_node.job_name.replace("_merge", "") + "_plot"
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/nodes/sampling_node.py` & `dingo-gw-0.5.0/dingo/pipe/nodes/sampling_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 
 from bilby_pipe.job_creation.nodes import AnalysisNode
 
-from dingo.gw.pipe.utils import _strip_unwanted_submission_keys
+from dingo.pipe.utils import _strip_unwanted_submission_keys
 
 
 class SamplingNode(AnalysisNode):
-
     def __init__(self, inputs, generation_node, dag):
         super(AnalysisNode, self).__init__(inputs)
         self.dag = dag
         self.generation_node = generation_node
         self.request_cpus = inputs.request_cpus
         self.device = inputs.device
 
@@ -61,7 +60,11 @@
 
     @property
     def samples_file(self):
         # TODO: Maybe remove -- not needed.
         return os.path.join(
             self.inputs.result_directory, self.label + ".hdf5"
         )
+
+    @property
+    def result_file(self):
+        return self.samples_file
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/parser.py` & `dingo-gw-0.5.0/dingo/pipe/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     get_version_information,
     logger,
     nonefloat,
     noneint,
     nonestr,
 )
 
+logger.name = "dingo_pipe"
+
 
 class StoreBoolean(argparse.Action):
     """argparse class for robust handling of booleans with configargparse
 
     When using configargparse, if the argument is setup with
     action="store_true", but the default is set to True, then there is no way,
     in the config file to switch the parameter off. To resolve this, this class
@@ -58,39 +60,48 @@
     parser.add("-v", "--verbose", action="store_true", help="Verbose output")
     # parser.add(
     #     "--version",
     #     action="version",
     #     version=f"%(prog)s={get_version_information()}\nbilby={bilby.__version__}",
     # )
 
-    # calibration_parser = parser.add_argument_group(
-    #     "Calibration arguments",
-    #     description="Which calibration model and settings to use.",
-    # )
-    # calibration_parser.add(
-    #     "--calibration-model",
-    #     type=nonestr,
-    #     default=None,
-    #     choices=["CubicSpline", None],
-    #     help="Choice of calibration model, if None, no calibration is used",
-    # )
-    #
-    # calibration_parser.add(
-    #     "--spline-calibration-envelope-dict",
-    #     type=nonestr,
-    #     default=None,
-    #     help=("Dictionary pointing to the spline calibration envelope files"),
-    # )
-    #
-    # calibration_parser.add(
-    #     "--spline-calibration-nodes",
-    #     type=int,
-    #     default=10,
-    #     help=("Number of calibration nodes"),
-    # )
+    calibration_parser = parser.add_argument_group(
+        "Calibration arguments",
+        description="Which calibration model and settings to use. Calibration "
+                    "uncertainty is marginalizaed over during importance sampling.",
+    )
+    calibration_parser.add(
+        "--calibration-model",
+        type=nonestr,
+        default=None,
+        choices=["CubicSpline", None],
+        help="Choice of calibration model, if None, no calibration is used",
+    )
+
+    calibration_parser.add(
+        "--spline-calibration-envelope-dict",
+        type=nonestr,
+        default=None,
+        help=("Dictionary pointing to the spline calibration envelope files"),
+    )
+
+    calibration_parser.add(
+        "--spline-calibration-nodes",
+        type=int,
+        default=10,
+        help=("Number of calibration nodes"),
+    )
+
+    calibration_parser.add(
+        "--spline-calibration-curves",
+        type=int,
+        default=1000,
+        help=("Number of calibration curves to use in marginalizing over calibration "
+              "uncertainty"),
+    )
     #
     # calibration_parser.add(
     #     "--spline-calibration-amplitude-uncertainty-dict",
     #     type=nonestr,
     #     default=None,
     #     help=(
     #         "Dictionary of the amplitude uncertainties for the constant "
@@ -1217,14 +1228,22 @@
         help=(
             "Dictionary of density-recovery-settings to pass in, e.g., {num_samples: "
             "400_000, nde_settings: (...)} OR pass pre-defined set of "
             "density-recovery-settings {ProxyRecoveryDefault}"
         ),
     )
     sampler_parser.add(
+        "--importance-sample",
+        action=StoreBoolean,
+        default=True,
+        help=(
+            "Whether to perform importance sampling on result. (Default: True)"
+        ),
+    )
+    sampler_parser.add(
         "--importance-sampling-settings",
         type=str,
         default="Default",
         help=(
             "Dictionary of importance-sampling-settings to pass in, e.g., "
             "{synthetic_phase: {approximation_22_mode: False, (...)}} OR pass"
             "pre-defined set of density-recovery-settings {PhaseRecoveryDefault}"
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/plot.py` & `dingo-gw-0.5.0/dingo/pipe/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pathlib import Path
 
 from bilby_pipe.bilbyargparser import BilbyArgParser
 from bilby_pipe.utils import get_command_line_arguments, logger, parse_args
 
 from dingo.gw.result import Result
 
+logger.name = "dingo_pipe"
+
 
 def create_parser():
     """Generate a parser for the plot script
 
     Returns
     -------
     parser: BilbyArgParser
```

### Comparing `dingo-gw-0.4.3/dingo/gw/pipe/sampling.py` & `dingo-gw-0.5.0/dingo/pipe/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from bilby_pipe.input import Input
 from bilby_pipe.utils import parse_args, logger, convert_string_to_dict
 
 from dingo.core.models import PosteriorModel
 from dingo.gw.data.event_dataset import EventDataset
 from dingo.gw.inference.gw_samplers import GWSampler, GWSamplerGNPE
 from dingo.gw.inference.inference_pipeline import prepare_log_prob
-from dingo.gw.pipe.default_settings import DENSITY_RECOVERY_SETTINGS
-from dingo.gw.pipe.parser import create_parser
+from dingo.pipe.default_settings import DENSITY_RECOVERY_SETTINGS
+from dingo.pipe.parser import create_parser
+
+logger.name = "dingo_pipe"
 
 
 class SamplingInput(Input):
     def __init__(self, args, unknown_args):
         super().__init__(args, unknown_args)
 
         # Generic initialisation
```

### Comparing `dingo-gw-0.4.3/dingo/gw/prior.py` & `dingo-gw-0.5.0/dingo/gw/prior.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/result.py` & `dingo-gw-0.5.0/dingo/gw/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,14 +502,33 @@
             log_prob_array = np.full(len(theta), -np.nan)
             log_prob_array[within_prior] = log_prob
             self.samples["log_prob"] = log_prob_array
             del self.samples["phase"]
 
         print(f"Done. This took {time.time() - t0:.2f} s.")
 
+    def get_samples_bilby_phase(self):
+        """
+        Convert the spin angles phi_jl and theta_jn to account for a difference in
+        phase definition compared to Bilby.
+
+        Returns
+        -------
+        pd.DataFrame
+            Samples
+        """
+        spin_conversion_phase_old = self.base_metadata["dataset_settings"][
+            "waveform_generator"
+        ].get("spin_conversion_phase")
+
+        # Redefine phase parameter to be consistent with Bilby.
+        return change_spin_conversion_phase(
+            self.samples, self.f_ref, spin_conversion_phase_old, None
+        )
+
     @property
     def pesummary_samples(self):
         """Samples in a form suitable for PESummary.
 
         These samples are adjusted to undo certain conventions used internally by
         Dingo:
             * Times are corrected by the reference time t_ref.
@@ -539,17 +558,17 @@
                 samples.loc[:, col] += self.t_ref
 
         spin_conversion_phase_old = self.base_metadata["dataset_settings"][
             "waveform_generator"
         ].get("spin_conversion_phase")
 
         # Redefine phase parameter to be consistent with Bilby. COMMENTED BECAUSE SLOW
-        # samples = change_spin_conversion_phase(
-        #     samples, self.f_ref, spin_conversion_phase_old, None
-        # )
+        samples = change_spin_conversion_phase(
+            samples, self.f_ref, spin_conversion_phase_old, None
+        )
 
         return samples
 
     @property
     def pesummary_prior(self):
         """The prior in a form suitable for PESummary.
```

### Comparing `dingo-gw-0.4.3/dingo/gw/temporary_debug_utils.py` & `dingo-gw-0.5.0/dingo/gw/temporary_debug_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/training/train_builders.py` & `dingo-gw-0.5.0/dingo/gw/training/train_builders.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/training/train_pipeline.py` & `dingo-gw-0.5.0/dingo/gw/training/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/training/train_pipeline_condor.py` & `dingo-gw-0.5.0/dingo/gw/training/train_pipeline_condor.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/training/utils.py` & `dingo-gw-0.5.0/dingo/gw/training/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/transforms/detector_transforms.py` & `dingo-gw-0.5.0/dingo/gw/transforms/detector_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from lal import GreenwichMeanSiderealTime
 from typing import Union
 from bilby.gw.detector import calibration
 from bilby.gw.prior import CalibrationPriorDict
 
 
 CC = 299792458.0
-NUM_CALIBRATION_NODES = 10
 
 
 def time_delay_from_geocenter(
     ifo: Interferometer,
     ra: Union[float, np.ndarray, torch.Tensor],
     dec: Union[float, np.ndarray, torch.Tensor],
     time: float,
@@ -236,85 +235,98 @@
         sample["waveform"] = strains
         sample["extrinsic_parameters"] = extrinsic_parameters
 
         return sample
 
 
 class ApplyCalibrationUncertainty(object):
-    """
-    Based off: 
+    r"""
+    Expand out a waveform using several detector calibration draws. These multiple
+    draws are intended to be used for marginalizing over calibration uncertainty.
 
+    Detector calibration uncertainty is modeled as described in
     https://dcc.ligo.org/LIGO-T1400682/public
 
-    Usually gravitational wave data is in the form 
-    
-    d(f) = h_obs(f) + n(f)                                          (1)
-
-    Where d is the data, h is the waveform and n is the noise. However, since
-    the detector is not perfectly calibrated, there are corrections to the
-    waveform in the form
-    
-    h_obs(f) = h(f) * (1 + \delta A(f)) * exp(i \delta \phi(f))      (2)
-
-    We can parameterize A(f) and \phi(f) with a cubic spline i.e.
-
-    \delta A(f) = spline(f; {f_i, \delta A_i})                       (3)
-    \delta \phi(f) = spline(f; {f_i, \delta \phi_i})                 (4)
-
-    The \A_i and \phi_i are drawn from gaussians centered at 0 with standard
-    deviations determined by the calibration envelope which varies event to
-    event. This method draws multiple splines and multiplies the waveform 
-    by the splines. Later when computing the likelihoods, we can marginalize
-    over these waveforms thereby mitigating the effects of calibration 
-    uncertainties in the detectors.  
-    
-
-    calibration_marginalization_kwargs: dict
-        Calibration marginalization kwargs. If None no calibration marginalization is
-        used. This should contain a dict with
-        {"num_calibration_curves": 100, "calibration_lookup_table": {"H1": filepath, "L1"...}}.
-        Optionally, you can also set "calibration_lookup_table" to None
+    Gravitational wave data $d$ is assumed to be of the form
+
+    $$d(f) = h_{obs}(f) + n(f),$$
+
+    where $h_{obs}$ is the observed waveform and $n$ is the noise. Since the detector
+    is not perfectly calibrated, the observed waveform is not identical to the true
+    waveform $h(f)$. Rather, it is assumed to have corrections of the form
+
+    $$h_{obs}(f) = h(f) * (1 + \delta A(f)) * \exp(i \delta \phi(f)),$$
+
+    where $\delta A(f)$ and $\delta \phi(f)$ are frequency-dependent amplitude and
+    phase errors. Under the calibration model, these are parametrized with cubic
+    splines, defined in terms of calibration parameters $A_i$ and $\phi_i$, defined
+    at log-spaced frequency nodes,
+
+    $$
+    \delta A(f) &= \mathrm{spline}(f; {f_i, \delta A_i}), \\
+    \delta \phi(f) &= \mathrm{spline}(f; {f_i, \delta \phi_i}).
+    $$
+
+    The calibration parameters are not known precisely, rather they are assumed to be
+    normally distributed, with mean 0 and standard deviation  determined by the
+    "calibration envelope", which varies from event to event.
+
+    For each detector waveform, this transform draws a collection of $N$
+    calibration curves $\{(\delta A^n(f), \delta \phi^n(f))\}_{n=1}^N$ according to a
+    calibration envelope, and applies them to generate $N$ observed waveforms $\{h^n_{
+    obs}(f)\}$. This is intended to be used for marginalizing over the calibration
+    uncertainty when evaluating the likelihood for importance sampling.
     """
 
     def __init__(
-        self, ifo_list, data_domain, calibration_envelope, num_calibration_curves
+        self,
+        ifo_list,
+        data_domain,
+        calibration_envelope,
+        num_calibration_curves,
+        num_calibration_nodes,
     ):
-        """
-        Initialize calibration marginalization. This requires the user to give
-        an event specific calibration curve.
-
-        Calibration marginalization takes a median and sigma (of amplitude and
-        phase) for each point in frequency space. Then it creates a spline on
-        the median and sigma. NOTE this is a DIFFERENT spline from the cubic
-        spline that will be generated later. This spline is just needed to
-        create priors on the the node points for the calibration cubic spline.
-        This spline will give you the node points, i.e. f_i (log spaced) and
-        Priors(\delta A_i, \delta \psi_i).
-
-        These node points are the calibration parameters. From these node points
-        and priors you can draw values for \delta A_i and \delta \psi_i which
-        will give you a calibration curve. This is the calibration curve which
-        you then multiply against the waveform.
+        r"""
+        Parameters
+        ---------
+
+        ifo_list : InterferometerList
+            List of Interferometers present in the analysis.
+        data_domain : Domain
+            Domain on which data is defined.
+        calibration_envelope : dict
+            Dictionary of the form ``{"H1": filepath, "L1": filepath}``,
+            where the filepaths are strings pointing to ".txt" files containing
+            calibration envelopes. The calibration envelope depends on the event analyzed,
+            and therefore  remains fixed for all applications of the transform. The
+            calibration envelope is used to define the variances $(\sigma_{\delta A_i},
+            \sigma_{\delta \phi_i})$ of the calibration paramters.
+        num_calibration_curves : int
+            Number of calibration curves $N$ to produce and apply to the
+            waveform. Ultimately, this will translate to the number of samples in the
+            Monte Carlo estimate of the marginalized likelihood integral.
+        num_calibration_nodes : int
+            Number of log-spaced frequency nodes $f_i$ to use in defining the spline.
         """
 
         self.ifo_list = ifo_list
         self.num_calibration_curves = num_calibration_curves
 
         self.data_domain = data_domain
         self.calibration_prior = {}
         if all([s.endswith(".txt") for s in calibration_envelope.values()]):
             # Generating .h5 lookup table from priors in .txt file
             self.calibration_envelope = calibration_envelope
-            for i, ifo in enumerate(self.ifo_list):
+            for ifo in self.ifo_list:
                 # Setting calibration model to cubic spline
                 ifo.calibration_model = calibration.CubicSpline(
                     f"recalib_{ifo.name}_",
                     minimum_frequency=data_domain.f_min,
                     maximum_frequency=data_domain.f_max,
-                    n_points=NUM_CALIBRATION_NODES,
+                    n_points=num_calibration_nodes,
                 )
 
                 # Setting priors
                 # What this will do is take the the calibration envelope and set
                 # a spline on the median and sigma of the amplitude and phase.
                 # Then in log frequency it will setup node points say at
                 # frequency points, $f_i$.  Then for each node point f_i, it
@@ -322,15 +334,15 @@
                 # median and sigma found earlier
                 self.calibration_prior[
                     ifo.name
                 ] = CalibrationPriorDict.from_envelope_file(
                     self.calibration_envelope[ifo.name],
                     self.data_domain.f_min,
                     self.data_domain.f_max,
-                    NUM_CALIBRATION_NODES,
+                    num_calibration_nodes,
                     ifo.name,
                 )
 
         else:
             raise Exception("Calibration envelope must be specified in a .txt file!")
 
     def __call__(self, input_sample):
```

### Comparing `dingo-gw-0.4.3/dingo/gw/transforms/gnpe_transforms.py` & `dingo-gw-0.5.0/dingo/gw/transforms/gnpe_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/transforms/inference_transforms.py` & `dingo-gw-0.5.0/dingo/gw/transforms/inference_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/transforms/noise_transforms.py` & `dingo-gw-0.5.0/dingo/gw/transforms/noise_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/transforms/parameter_transforms.py` & `dingo-gw-0.5.0/dingo/gw/transforms/parameter_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo/gw/waveform_generator/frame_utils.py` & `dingo-gw-0.5.0/dingo/gw/waveform_generator/frame_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_JL0_euler_angles(p, wfg, spin_conversion_phase=None):
     p = p.copy()
     p["f_ref"] = wfg.f_ref
     phase = p["phase"]
 
     if spin_conversion_phase is not None:
         p["phase"] = 0.0
-    p_lal = wfg._convert_parameters_to_lal_frame(p)
+    p_lal = wfg._convert_parameters(p)
     p_lal = list(p_lal)
 
     m1, m2 = p_lal[0:2]
     chi1x, chi1y, chi1z, chi2x, chi2y, chi2z = p_lal[2:8]
     iota = p_lal[9]
 
     m1 = m1 / lal.MSUN_SI
```

### Comparing `dingo-gw-0.4.3/dingo/gw/waveform_generator/waveform_generator.py` & `dingo-gw-0.5.0/dingo/gw/waveform_generator/waveform_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 from functools import partial
 from multiprocessing import Pool
 from math import isclose
 
 import numpy as np
+import astropy.units as u
 from typing import Dict, List, Tuple, Union
 from numbers import Number
 import warnings
 import lal
 import lalsimulation as LS
 import pandas as pd
+
+try:
+    from lalsimulation.gwsignal.core import waveform as gws_wfm
+    from lalsimulation.gwsignal.models import (
+        gwsignal_get_waveform_generator as new_interface_get_waveform_generator,
+    )
+except ImportError:
+    pass
+
 from bilby.gw.conversion import (
     convert_to_lal_binary_black_hole_parameters,
     bilby_to_lalsimulation_spins,
 )
-
 import dingo.gw.waveform_generator.wfg_utils as wfg_utils
 import dingo.gw.waveform_generator.frame_utils as frame_utils
 from dingo.gw.domains import Domain, FrequencyDomain, TimeDomain
 
 
 class WaveformGenerator:
-    """Generate polarizations in the specified domain for a
+    """Generate polarizations using LALSimulation routines in the specified domain for a
     single GW coalescence given a set of waveform parameters.
     """
 
     def __init__(
         self,
         approximant: str,
         domain: Domain,
         f_ref: float,
         f_start: float = None,
         mode_list: List[Tuple] = None,
         transform=None,
         spin_conversion_phase=None,
+        **kwargs,
     ):
         """
         Parameters
         ----------
         approximant : str
             Waveform "approximant" string understood by lalsimulation
             This is defines which waveform model is used.
@@ -68,31 +78,33 @@
             By setting spin_conversion_phase != None, we impose the convention to always
             use phase = spin_conversion_phase when computing the cartesian spins.
         """
         if not isinstance(approximant, str):
             raise ValueError("approximant should be a string, but got", approximant)
         else:
             self.approximant_str = approximant
-            self.approximant = LS.GetApproximantFromString(approximant)
+            self.lal_params = None
+            try:
+                self.approximant = LS.GetApproximantFromString(approximant)
+                if mode_list is not None:
+                    self.lal_params = self.setup_mode_array(mode_list)
+            except:
+                pass
 
         if not issubclass(type(domain), Domain):
             raise ValueError(
                 "domain should be an instance of a subclass of Domain, but got",
                 type(domain),
             )
         else:
             self.domain = domain
 
         self.f_ref = f_ref
         self.f_start = f_start
 
-        self.lal_params = None
-        if mode_list is not None:
-            self.lal_params = self.setup_mode_array(mode_list)
-
         self.transform = transform
         self._spin_conversion_phase = None
         self.spin_conversion_phase = spin_conversion_phase
 
     @property
     def spin_conversion_phase(self):
         return self._spin_conversion_phase
@@ -164,38 +176,35 @@
         elif not isinstance(list(parameters.values())[0], float):
             raise ValueError("parameters dictionary must contain floats", parameters)
 
         # Include reference frequency with the parameters. Copy the dict first for safety.
         parameters = parameters.copy()
         parameters["f_ref"] = self.f_ref
 
-        # Convert to lalsimulation parameters according to the specified domain
-        parameters_lal = self._convert_parameters_to_lal_frame(
-            parameters, self.lal_params
-        )
+        parameters_generator = self._convert_parameters(parameters, self.lal_params)
 
         # Generate GW polarizations
         if isinstance(self.domain, FrequencyDomain):
             wf_generator = self.generate_FD_waveform
         elif isinstance(self.domain, TimeDomain):
             wf_generator = self.generate_TD_waveform
         else:
             raise ValueError(f"Unsupported domain type {type(self.domain)}.")
 
         try:
-            wf_dict = wf_generator(parameters_lal)
+            wf_dict = wf_generator(parameters_generator)
         except Exception as e:
             if not catch_waveform_errors:
                 raise
             else:
                 EDOM = e.args[0] == "Internal function call failed: Input domain error"
                 if EDOM:
                     warnings.warn(
                         f"Evaluating the waveform failed with error: {e}\n"
-                        f"The parameters were {parameters_lal}\n"
+                        f"The parameters were {parameters_generator}\n"
                     )
                     pol_nan = np.ones(len(self.domain)) * np.nan
                     wf_dict = {"h_plus": pol_nan, "h_cross": pol_nan}
                 else:
                     raise
 
         if self.transform is not None:
@@ -222,15 +231,15 @@
             else:
                 raise ValueError(
                     f"Expected an array of length one, but shape = {x.shape}"
                 )
         else:
             return x
 
-    def _convert_parameters_to_lal_frame(
+    def _convert_parameters(
         self,
         parameter_dict: Dict,
         lal_params=None,
         lal_target_function=None,
     ) -> Tuple:
         """Convert to lal source frame parameters
 
@@ -428,15 +437,15 @@
         Returns
         -------
         lal_params:
             A lal parameter dictionary
         """
         lal_params = lal.CreateDict()
         ma = LS.SimInspiralCreateModeArray()
-        for (ell, m) in mode_list:
+        for ell, m in mode_list:
             LS.SimInspiralModeArrayActivateMode(ma, ell, m)
             # LS.SimInspiralModeArrayActivateMode(ma, ell, -m)
         LS.SimInspiralWaveformParamsInsertModeArray(lal_params, ma)
         return lal_params
 
     def generate_FD_waveform(self, parameters_lal: Tuple) -> Dict[str, np.ndarray]:
         """
@@ -656,15 +665,15 @@
             Dictionary with (l,m) as keys and the corresponding FD modes in lal format as
             values.
         iota: float
         """
         # TD approximants that are implemented in J frame. Currently tested for:
         #   101: IMRPhenomXPHM
         if self.approximant in [101]:
-            parameters_lal_fd_modes = self._convert_parameters_to_lal_frame(
+            parameters_lal_fd_modes = self._convert_parameters(
                 {**parameters, "f_ref": self.f_ref},
                 lal_target_function="SimInspiralChooseFDModes",
             )
             iota = parameters_lal_fd_modes[14]
             hlm_fd = LS.SimInspiralChooseFDModes(*parameters_lal_fd_modes)
             # unpack linked list, convert lal objects to arrays
             hlm_fd = wfg_utils.linked_list_modes_to_dict_modes(hlm_fd)
@@ -709,15 +718,15 @@
             Dictionary with (l,m) as keys and the corresponding TD modes in lal format as
             values.
         iota: float
         """
         # TD approximants that are implemented in L0 frame. Currently tested for:
         #   52: SEOBNRv4PHM
         if self.approximant in [52]:
-            parameters_lal_td_modes, iota = self._convert_parameters_to_lal_frame(
+            parameters_lal_td_modes, iota = self._convert_parameters(
                 {**parameters, "f_ref": self.f_ref},
                 lal_target_function="SimInspiralChooseTDModes",
             )
             hlm_td = LS.SimInspiralChooseTDModes(*parameters_lal_td_modes)
             return wfg_utils.linked_list_modes_to_dict_modes(hlm_td), iota
         else:
             raise NotImplementedError(
@@ -760,14 +769,429 @@
         hp, hc = LS.SimInspiralTD(*parameters_lal)
         h_plus = hp.data.data
         h_cross = hc.data.data
         pol_dict = {"h_plus": h_plus, "h_cross": h_cross}
         return pol_dict
 
 
+class NewInterfaceWaveformGenerator(WaveformGenerator):
+    """Generate polarizations using GWSignal routines in the specified domain for a
+    single GW coalescence given a set of waveform parameters.
+    """
+
+    def __init__(self, **kwargs):
+        WaveformGenerator.__init__(self, **kwargs)
+
+        self.mode_list = kwargs.get("mode_list", None)
+
+    def _convert_parameters(
+        self,
+        parameter_dict: Dict,
+        lal_params=None,
+    ):
+        # Transform mass, spin, and distance parameters
+        p, _ = convert_to_lal_binary_black_hole_parameters(parameter_dict)
+        # Transform to lal source frame: iota and Cartesian spin components
+        param_keys_in = (
+            "theta_jn",
+            "phi_jl",
+            "tilt_1",
+            "tilt_2",
+            "phi_12",
+            "a_1",
+            "a_2",
+            "mass_1",
+            "mass_2",
+            "f_ref",
+            "phase",
+        )
+        param_values_in = [p[k] for k in param_keys_in]
+        # if spin_conversion_phase is set, use this as fixed phiRef when computing the
+        # cartesian spins instead of using the phase parameter
+        if self.spin_conversion_phase is not None:
+            param_values_in[-1] = self.spin_conversion_phase
+        iota_and_cart_spins = bilby_to_lalsimulation_spins(*param_values_in)
+        iota, s1x, s1y, s1z, s2x, s2y, s2z = [
+            float(self._convert_to_scalar(x)) for x in iota_and_cart_spins
+        ]
+
+        f_ref = p["f_ref"]
+        delta_f = self.domain.delta_f
+        f_max = self.domain.f_max
+        if self.f_start is not None:
+            f_min = self.f_start
+        else:
+            f_min = self.domain.f_min
+        # parameters needed for TD waveforms
+        delta_t = 0.5 / self.domain.f_max
+
+        params_gwsignal = {
+            "mass1": p["mass_1"] * u.solMass,
+            "mass2": p["mass_2"] * u.solMass,
+            "spin1x": s1x * u.dimensionless_unscaled,
+            "spin1y": s1y * u.dimensionless_unscaled,
+            "spin1z": s1z * u.dimensionless_unscaled,
+            "spin2x": s2x * u.dimensionless_unscaled,
+            "spin2y": s2y * u.dimensionless_unscaled,
+            "spin2z": s2z * u.dimensionless_unscaled,
+            "deltaT": delta_t * u.s,
+            "f22_start": f_min * u.Hz,
+            "f22_ref": f_ref * u.Hz,
+            "f_max": f_max * u.Hz,
+            "deltaF": delta_f * u.Hz,
+            "phi_ref": p["phase"] * u.rad,
+            "distance": p["luminosity_distance"] * u.Mpc,
+            "inclination": iota * u.rad,
+            "ModeArray": self.mode_list,
+            "condition": 1,
+        }
+
+        # SEOBNRv5 specific parameters
+        if "postadiabatic" in p:
+            params_gwsignal["postadiabatic"] = p["postadiabatic"]
+
+            if "postadiabatic_type" in p:
+                params_gwsignal["postadiabatic_type"] = p["postadiabatic_type"]
+
+        if "lmax_nyquist" in p:
+            params_gwsignal["lmax_nyquist"] = p["lmax_nyquist"]
+        else:
+            params_gwsignal["lmax_nyquist"] = 2
+
+        return params_gwsignal
+
+    def generate_FD_waveform(self, parameters_gwsignal: Dict) -> Dict[str, np.ndarray]:
+        """
+        Generate Fourier domain GW polarizations (h_plus, h_cross).
+
+        Parameters
+        ----------
+        parameters_lal:
+            A tuple of parameters for the lalsimulation waveform generator
+
+        Returns
+        -------
+        pol_dict:
+            A dictionary of generated waveform polarizations
+        """
+        # Note: SEOBNRv4PHM does not support the specification of spins at a
+        # reference frequency different from the starting frequency. In addition,
+        # waveform generation will fail if the orbital distance is smaller than ~ 10M.
+        # To avoid this, we can start at a sufficiently low and consistent starting frequency
+        # for the entire dataset. If the number of generation failures is a very small
+        # fraction over the prior distribution then the dataset should be good to use.
+        #
+        # Note: XLALSimInspiralFD() internally calls XLALSimInspiralTD() to generate
+        # a conditioned time-domain waveform. In the past, this function lowered
+        # the starting frequency, but this is thankfully no longer the case
+        # for models such as SEOBNRv4PHM where the reference frequency is equal
+        # to the starting frequency. So, the TD waveform will be generated by
+        # calling XLALSimInspiralChooseTDWaveform().
+        # See https://git.ligo.org/waveforms/reviews/lalsuite/-/commit/195f9127682de19f5fce19cc5828116dd2d23461
+        #
+        # LS.SimInspiralFD takes parameters:
+        #   m1, m2, S1x, S1y, S1z, S2x, S2y, S2z,
+        #   distance, inclination, phiRef,
+        #   longAscNodes, eccentricity, meanPerAno,
+        #   deltaF, f_min, f_max, f_ref,
+        #   lal_params, approximant
+
+        # Sanity check types of arguments
+        # check_floats = all(map(lambda x: isinstance(x, float), parameters_lal[:18]))
+        # check_int = isinstance(parameters_lal[19], int)
+        # parameters_lal[18]  # lal_params could be None or a LALDict
+        # if not (check_floats and check_int):
+        #    raise ValueError(
+        #        "SimInspiralFD received invalid argument(s)", parameters_lal
+        #    )
+
+        # Depending on whether the domain is uniform or non-uniform call the appropriate wf generator
+        generator = new_interface_get_waveform_generator(self.approximant_str)
+        hpc = gws_wfm.GenerateFDWaveform(parameters_gwsignal, generator)
+        hp = hpc.hp
+        hc = hpc.hc
+
+        # Ensure that the waveform agrees with the frequency grid defined in the domain.
+        if not isclose(self.domain.delta_f, hp.df.value, rel_tol=1e-6):
+            raise ValueError(
+                f"Waveform delta_f is inconsistent with domain: {hp.df.value} vs {self.domain.delta_f}!"
+                f"To avoid this, ensure that f_max = {self.domain.f_max} is a power of two"
+                "when you are using a native time-domain waveform model."
+            )
+
+        frequency_array = self.domain()
+        h_plus = np.zeros_like(frequency_array, dtype=complex)
+        h_cross = np.zeros_like(frequency_array, dtype=complex)
+        # Ensure that length of wf agrees with length of domain. Enforce by truncating frequencies beyond f_max
+        if len(hp) > len(frequency_array):
+            warnings.warn(
+                "GWSignal waveform longer than domain's `frequency_array`"
+                f"({len(hp)} vs {len(frequency_array)}). Truncating gwsignal array."
+            )
+            h_plus = hp[: len(h_plus)].value
+            h_cross = hc[: len(h_cross)].value
+        else:
+            h_plus = hp.value
+            h_cross = hc.value
+
+        # Undo the time shift done in SimInspiralFD to the waveform
+        dt = 1 / hp.df.value + hp.epoch.value
+        time_shift = np.exp(-1j * 2 * np.pi * dt * frequency_array)
+        h_plus *= time_shift
+        h_cross *= time_shift
+        pol_dict = {"h_plus": h_plus, "h_cross": h_cross}
+        return pol_dict
+
+    def generate_hplus_hcross_m(
+        self, parameters: Dict[str, float]
+    ) -> Dict[tuple, Dict[str, np.ndarray]]:
+        """
+        Generate GW polarizations (h_plus, h_cross), separated into contributions from
+        the different modes. This method is identical to self.generate_hplus_hcross,
+        except that it generates the individual contributions of the modes to the
+        polarizations and sorts these according to their transformation behavior (see
+        below), instead of returning the overall sum.
+
+        This is useful in order to treat the phase as an extrinsic parameter. Instead of
+        {"h_plus": hp, "h_cross": hc}, this method returns a dict in the form of
+        {m: {"h_plus": hp_m, "h_cross": hc_m} for m in [-l_max,...,0,...,l_max]}. Each
+        key m contains the contribution to the polarization that transforms according
+        to exp(-1j * m * phase) under phase transformations (due to the spherical
+        harmonics).
+
+        Note:
+            - pol_m[m] contains contributions of the m modes *and* and the -m modes.
+              This is because the frequency domain (FD) modes have a positive frequency
+              part which transforms as exp(-1j * m * phase), while the negative
+              frequency part transforms as exp(+1j * m * phase). Typically, one of these
+              dominates [e.g., the (2,2) mode is dominated by the negative frequency
+              part and the (-2,2) mode is dominated by the positive frequency part]
+              such that the sum of (l,|m|) and (l,-|m|) modes transforms approximately as
+              exp(1j * |m| * phase), which is e.g. used for phase marginalization in
+              bilby/lalinference. However, this is not exact. In this method we account
+              for this effect, such that each contribution pol_m[m] transforms
+              *exactly* as exp(-1j * m * phase).
+            - Phase shifts contribute in two ways: Firstly via the spherical harmonics,
+              which we account for with the exp(-1j * m * phase) transformation.
+              Secondly, the phase determines how the PE spins transform to cartesian
+              spins, by rotating (sx,sy) by phase. This is *not* accounted for in this
+              function. Instead, the phase for computing the cartesian spins is fixed
+              to self.spin_conversion_phase (if not None). This effectively changes the
+              PE parameters {phi_jl, phi_12} to parameters {phi_jl_prime, phi_12_prime}.
+              For parameter estimation, a postprocessing operation can be applied to
+              account for this, {phi_jl_prime, phi_12_prime} -> {phi_jl, phi_12}.
+              See also documentation of __init__ method for more information on
+              self.spin_conversion_phase.
+
+        Differences to self.generate_hplus_hcross:
+        - We don't catch errors yet TODO
+        - We don't apply transforms yet TODO
+
+        Parameters
+        ----------
+        parameters: dict
+            Dictionary of parameters for the waveform.
+            For details see see self.generate_hplus_hcross.
+
+        Returns
+        -------
+        pol_m: dict
+            Dictionary with contributions to h_plus and h_cross, sorted by their
+            transformation behaviour under phase shifts:
+            {m: {"h_plus": hp_m, "h_cross": hc_m} for m in [-l_max,...,0,...,l_max]}
+            Each contribution h_m transforms as exp(-1j * m * phase) under phase shifts
+            (for fixed self.spin_conversion_phase, see above).
+        """
+        if not isinstance(parameters, dict):
+            raise ValueError("parameters should be a dictionary, but got", parameters)
+        elif not isinstance(list(parameters.values())[0], float):
+            raise ValueError("parameters dictionary must contain floats", parameters)
+
+        generator = new_interface_get_waveform_generator(self.approximant_str)
+        if isinstance(self.domain, FrequencyDomain):
+            # Generate FD modes in for frequencies [-f_max, ..., 0, ..., f_max].
+            if generator.domain == "freq":
+                # Step 1: generate waveform modes in L0 frame in native domain of
+                # approximant (here: FD)
+                hlm_fd, iota = self.generate_FD_modes_LO(parameters)
+
+                # Step 2: Transform modes to target domain.
+                # Not required here, as approximant domain and target domain are both FD.
+
+            else:
+                # assert LS.SimInspiralImplementedTDApproximants(self.approximant)
+                # Step 1: generate waveform modes in L0 frame in native domain of
+                # approximant (here: TD)
+                hlm_td, iota = self.generate_TD_modes_L0(parameters)
+
+                # Step 2: Transform modes to target domain.
+                # This requires tapering of TD modes, and FFT to transform to FD.
+                wfg_utils.taper_td_modes_in_place(hlm_td)
+                hlm_fd = wfg_utils.td_modes_to_fd_modes(hlm_td, self.domain)
+
+            # Step 3: Separate negative and positive frequency parts of the modes,
+            # and add contributions according to their transformation behavior under
+            # phase shifts.
+            pol_m = wfg_utils.get_polarizations_from_fd_modes_m(
+                hlm_fd, iota, parameters["phase"]
+            )
+
+        else:
+            raise NotImplementedError(
+                f"Target domain of type {type(self.domain)} not yet implemented."
+            )
+
+        return pol_m
+
+    def generate_FD_modes_LO(self, parameters):  # Pending to adapt
+        """
+        Generate FD modes in the L0 frame.
+
+        Parameters
+        ----------
+        parameters: dict
+            Dictionary of parameters for the waveform.
+            For details see see self.generate_hplus_hcross.
+
+        Returns
+        -------
+        hlm_fd: dict
+            Dictionary with (l,m) as keys and the corresponding FD modes in lal format as
+            values.
+        iota: float
+        """
+        # TD approximants that are implemented in J frame. Currently tested for:
+        #   101: IMRPhenomXPHM
+        if self.approximant_str in ["IMRPhenomXPHM"]:
+            parameters_gwsignal = self._convert_parameters(
+                {**parameters, "f_ref": self.f_ref}
+            )
+            iota = parameters_gwsignal["inclination"]
+            generator = new_interface_get_waveform_generator(self.approximant_str)
+            hlm_fd = gws_wfm.GenerateFDModes(parameters_gwsignal, generator)
+            # unpack linked list, convert lal objects to arrays
+
+            hlms_lal = {}
+            for key, value in hlm_fd.items():
+                if type(key) != str:
+                    hlm_lal = lal.CreateCOMPLEX16TimeSeries(
+                        "hplus",
+                        value.epoch.value,
+                        0,
+                        value.dt.value,
+                        lal.DimensionlessUnit,
+                        len(value),
+                    )
+                    hlm_lal.data.data = value.value
+                    hlms_lal[key] = hlm_lal
+
+            hlm_fd = wfg_utils.linked_list_modes_to_dict_modes(hlms_lal)
+            hlm_fd = {k: v.data.data for k, v in hlm_fd.items()}
+            # For the waveform models considered here (e.g., IMRPhenomXPHM), the modes
+            # are returned in the J frame (where the observer is at inclination=theta_JN,
+            # azimuth=0). In this frame, the dependence on the reference phase enters
+            # via the modes themselves. We need to convert to the L0 frame so that the
+            # dependence on phase enters via the spherical harmonics.
+            hlm_fd = frame_utils.convert_J_to_L0_frame(
+                hlm_fd,
+                parameters,
+                self,
+                spin_conversion_phase=self.spin_conversion_phase,
+            )
+            return hlm_fd, iota
+        else:
+            raise NotImplementedError(
+                f"Approximant {LS.GetApproximantFromString(self.approximant)} not "
+                f"implemented. When adding this approximant to this method, make sure "
+                f"the the output dict hlm_td contains the TD modes in the *L0 frame*. "
+                f"In particular, adding an approximant that is implemented in the same "
+                f"domain and frame as one of the approximants should just be a matter of "
+                f"adding the approximant number (here: {self.approximant}) to the "
+                f"corresponding if statement. However, when doing this please make sure "
+                f"to test that this works as intended! Ideally, add some unit tests."
+            )
+
+    def generate_TD_modes_L0(self, parameters):
+        """
+        Generate TD modes in the L0 frame.
+
+        Parameters
+        ----------
+        parameters: dict
+            Dictionary of parameters for the waveform.
+            For details see see self.generate_hplus_hcross.
+
+        Returns
+        -------
+        hlm_td: dict
+            Dictionary with (l,m) as keys and the corresponding TD modes in lal format as
+            values.
+        iota: float
+        """
+        # TD approximants that are implemented in L0 frame. Currently tested for:
+        #   52: SEOBNRv4PHM
+
+        parameters_gwsignal = self._convert_parameters(
+            {**parameters, "f_ref": self.f_ref}
+        )
+
+        generator = new_interface_get_waveform_generator(self.approximant_str)
+        hlm_td = gws_wfm.GenerateTDModes(parameters_gwsignal, generator)
+        hlms_lal = {}
+
+        for key, value in hlm_td.items():
+            if type(key) != str:
+                hlm_lal = lal.CreateCOMPLEX16TimeSeries(
+                    "hplus",
+                    value.epoch.value,
+                    0,
+                    value.dt.value,
+                    lal.DimensionlessUnit,
+                    len(value),
+                )
+                hlm_lal.data.data = value.value
+                hlms_lal[key] = hlm_lal
+
+        return hlms_lal, parameters_gwsignal["inclination"].value
+
+    def generate_TD_waveform(self, parameters_gwsignal: Dict) -> Dict[str, np.ndarray]:
+        """
+        Generate time domain GW polarizations (h_plus, h_cross)
+
+        Parameters
+        ----------
+        parameters_gwsignal:
+            A dict of parameters for the gwsignal waveform generator
+
+        Returns
+        -------
+        pol_dict:
+            A dictionary of generated waveform polarizations
+        """
+        # Note: XLALSimInspiralTD() now calls XLALSimInspiralChooseTDWaveform()
+        # for models such as SEOBNRv4PHM where the reference frequency is equal
+        # to the starting frequency and thus leaves our choice of starting
+        # frequency untouched.
+        #
+        # LS.SimInspiralTD takes parameters:
+        #   m1, m2, S1x, S1y, S1z, S2x, S2y, S2z,
+        #   distance, inclination, phiRef,
+        #   longAscNodes, eccentricity, meanPerAno,
+        #   deltaT, f_min, f_ref
+        #   lal_params, approximant
+
+        generator = new_interface_get_waveform_generator(self.approximant_str)
+        hpc = gws_wfm.GenerateTDWaveform(parameters_gwsignal, generator)
+
+        h_plus = hpc.hp.value
+        h_cross = hpc.hc.value
+        pol_dict = {"h_plus": h_plus, "h_cross": h_cross}
+        return pol_dict
+
+
 def SEOBNRv4PHM_maximum_starting_frequency(
     total_mass: float, fudge: float = 0.99
 ) -> float:
     """
     Given a total mass return the largest possible starting frequency allowed
     for SEOBNRv4PHM and similar effective-one-body models.
 
@@ -790,15 +1214,15 @@
     """
     total_mass_sec = total_mass * lal.MTSUN_SI
     f_max_Hz = fudge * 10.5 ** (-1.5) / (np.pi * total_mass_sec)
     return f_max_Hz
 
 
 def generate_waveforms_task_func(
-    args: Tuple, waveform_generator: WaveformGenerator = None
+    args: Tuple, waveform_generator: WaveformGenerator
 ) -> Dict[str, np.ndarray]:
     """
     Picklable wrapper function for parallel waveform generation.
 
     Parameters
     ----------
     args:
@@ -837,14 +1261,15 @@
     """
     # logger.info('Generating waveform polarizations ...')
 
     task_func = partial(
         generate_waveforms_task_func, waveform_generator=waveform_generator
     )
     task_data = parameter_samples.iterrows()
+
     if pool is not None:
         polarizations_list = pool.map(task_func, task_data)
     else:
         polarizations_list = list(map(task_func, task_data))
     polarizations = {
         pol: np.stack([wf[pol] for wf in polarizations_list])
         for pol in polarizations_list[0].keys()
```

### Comparing `dingo-gw-0.4.3/dingo/gw/waveform_generator/wfg_utils.py` & `dingo-gw-0.5.0/dingo/gw/waveform_generator/wfg_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/dingo_gw.egg-info/PKG-INFO` & `dingo-gw-0.5.0/dingo_gw.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingo-gw
-Version: 0.4.3
+Version: 0.5.0
 Summary: Deep inference for gravitational-wave observations
 Author-email: Maximilian Dax <maximilian.dax@tuebingen.mpg.de>, Stephen Green <Stephen.Green2@nottingham.ac.uk>
 License: MIT
 Project-URL: homepage, https://github.com/dingo-gw/dingo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,22 +36,29 @@
 * performing inference on real or simulated data; and
 * verifying and correcting model results using importance sampling.
 
 ## Installation
 
 ### Pip
 
-The easiest way to install Dingo is using pip. Within a suitable virtual environment, run
-the command
+To install using pip, run the following within a suitable virtual environment:
 ```sh
 pip install dingo-gw
 ```
-This will install Dingo as well as all of its requirements, listed in
+This will install Dingo as well as all of its requirements, which are listed in
 [pyproject.toml](https://github.com/dingo-gw/dingo/blob/main/pyproject.toml).
 
+### Conda
+
+Dingo is also available from the [conda-forge](https://conda-forge.org) repository.
+To install using conda, first activate a conda environment, and then run
+```sh
+conda install -c conda-forge dingo-gw
+```
+
 ### Development install
 
 If you would like to make changes to Dingo, or to contribute to its development, you
 should install Dingo from source. To do so, first clone this repository:
 ```sh
 git clone git@github.com:dingo-gw/dingo.git
 ```
```

### Comparing `dingo-gw-0.4.3/dingo_gw.egg-info/SOURCES.txt` & `dingo-gw-0.5.0/dingo_gw.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 compatibility/update_saved_model_for_train_stages.py
 compatibility/update_saved_model_gnpe_context_names.py
 compatibility/update_saved_model_new_gnpe.py
 compatibility/update_saved_model_new_truncation.py
 compatibility/update_waveform_dataset_svd_refactor.py
 dingo/__init__.py
 dingo/_version.py
+dingo/asimov/__init__.py
+dingo/asimov/asimov.py
+dingo/asimov/dingo.ini
 dingo/core/__init__.py
 dingo/core/dataset.py
 dingo/core/likelihood.py
 dingo/core/multiprocessing.py
 dingo/core/result.py
 dingo/core/samplers.py
 dingo/core/transforms.py
@@ -33,14 +36,15 @@
 dingo/core/nn/nsf.py
 dingo/core/utils/__init__.py
 dingo/core/utils/condor_utils.py
 dingo/core/utils/gnpeutils.py
 dingo/core/utils/logging_utils.py
 dingo/core/utils/misc.py
 dingo/core/utils/plotting.py
+dingo/core/utils/pt_to_hdf5.py
 dingo/core/utils/torchutils.py
 dingo/core/utils/trainutils.py
 dingo/gw/SVD.py
 dingo/gw/__init__.py
 dingo/gw/domains.py
 dingo/gw/download_strain_data.py
 dingo/gw/gwutils.py
@@ -70,32 +74,19 @@
 dingo/gw/inference/visualization.py
 dingo/gw/noise/__init__.py
 dingo/gw/noise/asd_dataset.py
 dingo/gw/noise/asd_estimation.py
 dingo/gw/noise/generate_dataset.py
 dingo/gw/noise/generate_dataset_dag.py
 dingo/gw/noise/utils.py
-dingo/gw/pipe/ACKNOWLEDGMENT.md
-dingo/gw/pipe/__init__.py
-dingo/gw/pipe/dag_creator.py
-dingo/gw/pipe/data_generation.py
-dingo/gw/pipe/default_settings.py
-dingo/gw/pipe/dingo_result.py
-dingo/gw/pipe/importance_sampling.py
-dingo/gw/pipe/main.py
-dingo/gw/pipe/parser.py
-dingo/gw/pipe/plot.py
-dingo/gw/pipe/sampling.py
-dingo/gw/pipe/utils.py
-dingo/gw/pipe/nodes/__init__.py
-dingo/gw/pipe/nodes/generation_node.py
-dingo/gw/pipe/nodes/importance_sampling_node.py
-dingo/gw/pipe/nodes/merge_node.py
-dingo/gw/pipe/nodes/plot_node.py
-dingo/gw/pipe/nodes/sampling_node.py
+dingo/gw/noise/synthetic/__init__.py
+dingo/gw/noise/synthetic/asd_parameterization.py
+dingo/gw/noise/synthetic/asd_sampling.py
+dingo/gw/noise/synthetic/generate_dataset.py
+dingo/gw/noise/synthetic/utils.py
 dingo/gw/training/__init__.py
 dingo/gw/training/train_builders.py
 dingo/gw/training/train_pipeline.py
 dingo/gw/training/train_pipeline_condor.py
 dingo/gw/training/utils.py
 dingo/gw/transforms/__init__.py
 dingo/gw/transforms/detector_transforms.py
@@ -104,27 +95,49 @@
 dingo/gw/transforms/inference_transforms.py
 dingo/gw/transforms/noise_transforms.py
 dingo/gw/transforms/parameter_transforms.py
 dingo/gw/waveform_generator/__init__.py
 dingo/gw/waveform_generator/frame_utils.py
 dingo/gw/waveform_generator/waveform_generator.py
 dingo/gw/waveform_generator/wfg_utils.py
+dingo/pipe/ACKNOWLEDGMENT.md
+dingo/pipe/__init__.py
+dingo/pipe/dag_creator.py
+dingo/pipe/data_generation.py
+dingo/pipe/default_settings.py
+dingo/pipe/dingo_result.py
+dingo/pipe/importance_sampling.py
+dingo/pipe/main.py
+dingo/pipe/parser.py
+dingo/pipe/plot.py
+dingo/pipe/sampling.py
+dingo/pipe/utils.py
+dingo/pipe/nodes/__init__.py
+dingo/pipe/nodes/generation_node.py
+dingo/pipe/nodes/importance_sampling_node.py
+dingo/pipe/nodes/merge_node.py
+dingo/pipe/nodes/pe_summary_node.py
+dingo/pipe/nodes/plot_node.py
+dingo/pipe/nodes/sampling_node.py
 dingo_gw.egg-info/PKG-INFO
 dingo_gw.egg-info/SOURCES.txt
 dingo_gw.egg-info/dependency_links.txt
 dingo_gw.egg-info/entry_points.txt
 dingo_gw.egg-info/requires.txt
 dingo_gw.egg-info/top_level.txt
 docs/Makefile
 docs/README.md
 docs/make.bat
 docs/source/code_design.md
 docs/source/conf.py
 docs/source/dingo_pipe.md
+docs/source/example_gnpe_model.md
 docs/source/example_injection.md
+docs/source/example_npe_model.md
+docs/source/example_toy_npe_model.md
 docs/source/generating_waveforms.ipynb
 docs/source/gibbs_figure.jpg
 docs/source/gnpe.md
 docs/source/index.md
 docs/source/inference.md
 docs/source/installation.md
 docs/source/network_architecture.ipynb
@@ -134,27 +147,32 @@
 docs/source/refs.bib
 docs/source/result.md
 docs/source/sbi.md
 docs/source/training.md
 docs/source/training_transforms.ipynb
 docs/source/waveform_dataset.ipynb
 examples/README.md
-examples/event_settings.yaml
-examples/is_settings.yaml
-examples/dataset_generation/asd_dataset_settings.yaml
-examples/dataset_generation/dingo_generate_dataset_dag_example.sh
-examples/dataset_generation/waveform_dataset_settings.yaml
-examples/pipe/GW150914.ini
-examples/training/stage_settings.yaml
-examples/training/train_settings_init_production.yaml
-examples/training/train_settings_init_toy.yaml
-examples/training/train_settings_no_gnpe_production.yaml
-examples/training/train_settings_no_gnpe_toy.yaml
-examples/training/train_settings_production.yaml
-examples/training/train_settings_toy.yaml
+examples/dataset_generation/asd_dataset_settings_synthetic.yaml
+examples/gnpe_model/GW150914.ini
+examples/gnpe_model/asd_dataset_settings.yaml
+examples/gnpe_model/asd_dataset_settings_fiducial.yaml
+examples/gnpe_model/train_settings.yaml
+examples/gnpe_model/train_settings_init.yaml
+examples/gnpe_model/waveform_dataset_settings.yaml
+examples/misc/is_settings.yaml
+examples/misc/stage_settings.yaml
+examples/npe_model/GW150914.ini
+examples/npe_model/asd_dataset_settings.yaml
+examples/npe_model/asd_dataset_settings_fiducial.yaml
+examples/npe_model/train_settings.yaml
+examples/npe_model/waveform_dataset_settings.yaml
+examples/toy_npe_model/GW150914.ini
+examples/toy_npe_model/asd_dataset_settings.yaml
+examples/toy_npe_model/train_settings.yaml
+examples/toy_npe_model/waveform_dataset_settings.yaml
 tests/core/test_enets.py
 tests/core/test_nsf.py
 tests/core/test_posterior_model.py
 tests/core/testutils_enets.py
 tests/gw/test_domains.py
 tests/gw/test_injection.py
 tests/gw/test_noise_dataset.py
```

### Comparing `dingo-gw-0.4.3/dingo_gw.egg-info/entry_points.txt` & `dingo-gw-0.5.0/dingo_gw.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+[asimov.pipelines]
+dingo = dingo.asimov.asimov:Dingo
+
 [console_scripts]
 dingo_analyze_event = dingo.gw.inference:analyze_event
 dingo_append_training_stage = dingo.gw.training:append_stage
 dingo_build_svd = dingo.gw.dataset.utils:build_svd_cli
 dingo_estimate_psds = dingo.gw.noise.asd_estimation:download_and_estimate_cli
 dingo_generate_asd_dataset = dingo.gw.noise.generate_dataset:generate_dataset
 dingo_generate_dataset = dingo.gw.dataset.generate_dataset:main
 dingo_generate_dataset_dag = dingo.gw.dataset.generate_dataset_dag:main
+dingo_generate_synthetic_asd_dataset = dingo.gw.noise.synthetic_noise.generate_dataset:main
 dingo_ls = dingo.gw.ls_cli:ls
 dingo_merge_asd_datasets = dingo.gw.noise.utils:merge_datasets_cli
 dingo_merge_datasets = dingo.gw.dataset.utils:merge_datasets_cli
-dingo_pipe = dingo.gw.pipe.main:main
-dingo_pipe_generation = dingo.gw.pipe.data_generation:main
-dingo_pipe_importance_sampling = dingo.gw.pipe.importance_sampling:main
-dingo_pipe_plot = dingo.gw.pipe.plot:main
-dingo_pipe_sampling = dingo.gw.pipe.sampling:main
-dingo_result = dingo.gw.pipe.dingo_result:main
+dingo_pipe = dingo.pipe.main:main
+dingo_pipe_generation = dingo.pipe.data_generation:main
+dingo_pipe_importance_sampling = dingo.pipe.importance_sampling:main
+dingo_pipe_plot = dingo.pipe.plot:main
+dingo_pipe_sampling = dingo.pipe.sampling:main
+dingo_pt_to_hdf5 = dingo.core.utils.pt_to_hdf5:main
+dingo_result = dingo.pipe.dingo_result:main
 dingo_train = dingo.gw.training:train_local
 dingo_train_condor = dingo.gw.training.train_pipeline_condor:train_condor
```

### Comparing `dingo-gw-0.4.3/docs/Makefile` & `dingo-gw-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/README.md` & `dingo-gw-0.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/make.bat` & `dingo-gw-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/code_design.md` & `dingo-gw-0.5.0/docs/source/code_design.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/conf.py` & `dingo-gw-0.5.0/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.mathjax',
     'sphinx.ext.napoleon',
     'myst_nb',
     'sphinxcontrib.mermaid',
     'sphinxcontrib.bibtex',
+    'sphinx_math_dollar',
 ]
 
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
     "deflist",
     "dollarmath",
@@ -52,14 +53,28 @@
     "replacements",
     "smartquotes",
     "strikethrough",
     "substitution",
     "tasklist",
 ]
 
+mathjax_config = {
+    'tex2jax': {
+        'inlineMath': [ ["\\(","\\)"] ],
+        'displayMath': [["\\[","\\]"] ],
+    },
+}
+
+mathjax3_config = {
+  "tex": {
+    "inlineMath": [['\\(', '\\)']],
+    "displayMath": [["\\[", "\\]"]],
+  }
+}
+
 myst_heading_anchors = 2
 
 bibtex_bibfiles = ['refs.bib']
 bibtex_default_style = 'unsrt'
 
 # Include the __init__ docstring with the autoclass
 autoclass_content = 'both'
```

### Comparing `dingo-gw-0.4.3/docs/source/dingo_pipe.md` & `dingo-gw-0.5.0/docs/source/dingo_pipe.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 model-init = /data/sgreen/dingo-experiments/XPHM/O1_init/model_stage_1.pt
 model = /data/sgreen/dingo-experiments/XPHM/testing_inference/model.pt
 device = 'cuda'
 num-gnpe-iterations = 30
 num-samples = 50000
 batch-size = 50000
 recover-log-prob = true
+importance-sample = true
 prior-dict = {
 luminosity_distance = bilby.gw.prior.UniformComovingVolume(minimum=100, maximum=2000, name='luminosity_distance'),
 }
 
 ################################################################################
 ## Data generation arguments
 ################################################################################
@@ -46,14 +47,23 @@
 outdir = outdir_GW150914
 channel-dict = {H1:GWOSC, L1:GWOSC}
 psd-length = 128
 sampling-frequency = 2048.0
 importance-sampling-updates = {'duration': 4.0}
 
 ################################################################################
+## Calibration marginalization arguments
+################################################################################
+
+calibration-model = CubicSpline
+spline-calibration-envelope-dict = {H1: GWTC1_GW150914_H_CalEnv.txt, L1: GWTC1_GW150914_L_CalEnv.txt}
+spline-calibration-nodes = 10
+spline-calibration-curves = 1000
+
+################################################################################
 ## Plotting arguments
 ################################################################################
 
 plot-corner = true
 plot-weights = true
 plot-log-probs = true
 ```
@@ -89,18 +99,34 @@
 
 If a `prior-dict` is specified in the `.ini` file, then this will be used for the importance sampling prior. One example where this is useful is for the luminosity distance prior. Indeed, Dingo tends to train better using a uniform prior over luminosity distance, but physically one would prefer a uniform in volume prior. By specifying a `prior-dict` this change can be made in importance sampling.
 
 ```{caution}
 If extending the prior support during importance sampling, be sure that the posterior does not rail up against the prior boundary being extended.
 ```
 
-By default, dingo_pipe assumes that it is necessary to sample the phase synthetically, so it will do so before importance sampling. This can be turned off by passing an empty dictionary to `importance-sampling-settings`.
+By default, dingo_pipe assumes that it is necessary to sample the phase synthetically, so it will do so before importance sampling. This can be turned off by passing an empty dictionary to `importance-sampling-settings`. Note that importance sampling itself can be switched off by setting the `importance-sample` flag to False (it defaults to True). 
 
 Importance sampling (including synthetic phase sampling) is an expensive step, so dingo_pipe allows for parallelization: this step is split over `n-parallel` jobs, each of which uses `request-cpus-importance-sampling` processes. In the backend, this makes use of the Result [split()](dingo.core.result.Result.split) and [merge()](dingo.core.result.Result.merge) methods.
 
+### Calibration marginalization
+
+Settings related to calibration are used to **marginalize** over calibration uncertainty during importance sampling.
+
+calibration-model
+: None or "CubicSpline". If "CubicSpline", perform calibration marginalization using a cubic spline calibration model. If None do not perform calibration marginalization. (Default: None)
+
+spline-calibration-envelope-dict
+: Dictionary pointing to the spline calibration envelope files. This is required if calibration-model is "CubicSpline".
+
+spline-calibration-nodes
+: Number of calibration nodes. (Default: 10)
+
+spline-calibration-curves
+: Number of calibration curves to use for marginalization. (Default: 1000)
+
 ## Plotting
 
 The standard Result [plots](result.md#plotting) are turned on using the `plot-corner`, `plot-weights`, and `plot-log-probs` flags.
 
 ## Additional options
 
 extra-lines
```

### Comparing `dingo-gw-0.4.3/docs/source/example_injection.md` & `dingo-gw-0.5.0/docs/source/example_injection.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/generating_waveforms.ipynb` & `dingo-gw-0.5.0/docs/source/generating_waveforms.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974772135416667%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, 'Waveforms are generated using the `WaveformGenerator` "*

 * *            'class (or its subclass `NewInterfaceWaveformGenerator`, for employing the new LIGO '*

 * *            'waveform interface, needed for some approximants). This depends on a `Domain` as well '*

 * *            'as a waveform approximant and a reference frequency `f_ref`. In the backend, the '*

 * *            '`WaveformGenerator` class calls '*

 * *            '[LALSimulation](https://lscsoft.docs.ligo.org/lalsuite/lal […]*

```diff
@@ -79,33 +79,35 @@
                 "```{eval-rst}\n",
                 ".. autoclass:: dingo.gw.domains.FrequencyDomain\n",
                 "    :members:\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "8e3be82f-5213-402a-8c4b-e2b3c568cbad",
             "metadata": {},
             "source": [
                 "## Waveform generator\n",
                 "\n",
-                "Waveforms are generated using the `WaveformGenerator` class. This depends on a `Domain` as well as a waveform approximant and a reference frequency `f_ref`. In the backend, this calls [LALSimulation](https://lscsoft.docs.ligo.org/lalsuite/lalsimulation/) functions (typically `SimInspiralFD`) via the Python interface. For time domain waveforms, `SimInspiralFD` takes care of FFTing to frequency domain."
+                "Waveforms are generated using the `WaveformGenerator` class (or its subclass `NewInterfaceWaveformGenerator`, for employing the new LIGO waveform interface, needed for some approximants). This depends on a `Domain` as well as a waveform approximant and a reference frequency `f_ref`. In the backend, the `WaveformGenerator` class calls [LALSimulation](https://lscsoft.docs.ligo.org/lalsuite/lalsimulation/) functions (typically `SimInspiralFD`) via the SWIG-Python interface. For time domain waveforms, `SimInspiralFD` takes care of FFTing to frequency domain. The `NewInterfaceWaveformGenerator` class calls the [gwsignal]() module, a Python interface recently implemented in LALSimulation, which is needed for employing some of the latest waveform approximants, as the `SEOBNRv5HM` and `SEOBNRv5PHM`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "c11d621d-a2e8-4cb5-bc1c-88188f53e41c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from dingo.gw.waveform_generator import WaveformGenerator\n",
+                "from dingo.gw.waveform_generator import WaveformGenerator #, NewInterfaceWaveformGenerator\n",
                 "\n",
-                "wfg = WaveformGenerator(approximant='IMRPhenomXPHM', domain=domain, f_ref=20.0)"
+                "wfg = WaveformGenerator(approximant='IMRPhenomXPHM', domain=domain, f_ref=20.0)\n",
+                "# wfg = NewInterfaceWaveformGenerator(approximant='SEOBNRv5PHM', domain=domain, f_ref=20.0)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1e93275f-2176-436c-8729-da183b27efbf",
             "metadata": {},
             "source": [
@@ -218,15 +220,15 @@
             "cell_type": "code",
             "execution_count": 22,
             "id": "2981b324-87cb-434c-ac53-105515b373a1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 432x288 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
```

### Comparing `dingo-gw-0.4.3/docs/source/gibbs_figure.jpg` & `dingo-gw-0.5.0/docs/source/gibbs_figure.jpg`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/gnpe.md` & `dingo-gw-0.5.0/docs/source/gnpe.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/index.md` & `dingo-gw-0.5.0/docs/source/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,17 @@
    overview
    quickstart
 
 .. toctree::
    :caption: Examples
    :maxdepth: 1
    
+   example_toy_npe_model
+   example_npe_model
+   example_gnpe_model
    example_injection
 
 .. toctree::
    :caption: Advanced guide
    :maxdepth: 1
 
    sbi
```

### Comparing `dingo-gw-0.4.3/docs/source/inference.md` & `dingo-gw-0.5.0/docs/source/inference.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/installation.md` & `dingo-gw-0.5.0/docs/source/installation.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # Installation
 
 ## Standard
 
 ### Pip
 
-The easiest way to install Dingo is using pip. Within a suitable virtual environment, run
-the command
+To install using pip, run the following within a suitable virtual environment:
 ```sh
 pip install dingo-gw
 ```
-This will install Dingo as well as all of its requirements, listed in
+This will install Dingo as well as all of its requirements, which are listed in
 [pyproject.toml](https://github.com/dingo-gw/dingo/blob/main/pyproject.toml).
 
+### Conda
+
+Dingo is also available from the [conda-forge](https://conda-forge.org) repository.
+To install using conda, first activate a conda environment, and then run
+```sh
+conda install -c conda-forge dingo-gw
+```
+
 ## Development
 
 If you would like to make changes to Dingo, or to contribute to its development, you
 should install Dingo from source. To do so, first clone this repository:
 ```sh
 git clone git@github.com:dingo-gw/dingo.git
 ```
@@ -64,8 +71,8 @@
 
 #### Cleanup
 
 To remove generated docs, execute
 ```sh
 make clean
 rm source/dingo.* source/modules.rst
-```
+```
```

### Comparing `dingo-gw-0.4.3/docs/source/network_architecture.ipynb` & `dingo-gw-0.5.0/docs/source/network_architecture.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/noise_dataset.ipynb` & `dingo-gw-0.5.0/docs/source/noise_dataset.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972047018348624%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(39, '## Generating an ASDDataset\\n'), (69, '  f_min: "*

 * *            "0\\n'), (70, '  f_max: 2048\\n'), (94, '\\n'), (95, '`f_min`, `f_max` "*

 * *            "(optional)\\n'), (96, ': Lower and upper frequency range of the ASDs. Defaults to 0 "*

 * *            "and `f_s/2`, respectively.\\n'), (108, ': Gap between duration-`T` segments. E.g., if "*

 * *            '`time_psd=1024`, `T=8`, `time_gap=8`, then for each PSD, 64 periodigrams are '*

 * *            'computed, each using data s […]*

```diff
@@ -40,15 +40,15 @@
                 "    :show-inheritance:\n",
                 "```\n",
                 "\n",
                 "As with the noise realizations, a random ASD is chosen from the dataset when preparing each sample during training. This augments the training set compared to fixing the noise ASD for each sample prior to training.\n",
                 "\n",
                 "Similarly to the `WaveformDataset`, the `ASDDataset` is just a container. Dingo includes routines for building such a dataset from observational data.\n",
                 "\n",
-                "## Command-line scripts\n",
+                "## Generating an ASDDataset\n",
                 "\n",
                 "### `dingo_generate_asd_dataset`\n",
                 " The basic approach is as follows:\n",
                 "1. Identify stretches of data within an observing run meeting certain criteria (sufficiently long, without events, and sufficiently high quality, ...) or take-in user-specified stretches.\n",
                 "2. Fetch data corresponding to these stretches using either\n",
                 "    - [GWOSC](https://www.gw-openscience.org)\n",
                 "    - channels, optionally specified in the settings file.\n",
@@ -70,14 +70,16 @@
                 "  --out_name OUT_NAME   Path to resulting ASD dataset\n",
                 "  --verbose\n",
                 "\n",
                 "```\n",
                 "where the settings file is of the form\n",
                 "```yaml\n",
                 "dataset_settings:\n",
+                "  f_min: 0\n",
+                "  f_max: 2048\n",
                 "  f_s: 4096\n",
                 "  time_psd: 1024\n",
                 "  T: 8\n",
                 "  time_gap: 0\n",
                 "  window:\n",
                 "    roll_off: 0.4\n",
                 "    type: tukey\n",
@@ -90,49 +92,117 @@
                 "    - L1\n",
                 "  observing_run: O2\n",
                 "condor:\n",
                 "  env_path: path/to/environment\n",
                 "  num_jobs: 2    # per detector\n",
                 "  num_cpus: 16\n",
                 "  memory_cpus: 16000\n",
-                "  bid: 200\n",
                 "```\n",
                 "\n",
                 "Options correspond to the following:\n",
                 "\n",
+                "`f_min`, `f_max` (optional)\n",
+                ": Lower and upper frequency range of the ASDs. Defaults to 0 and `f_s/2`, respectively.\n",
+                "\n",
                 "Sampling rate `f_s` (Hz)\n",
                 ": This should be at least twice the value of `f_max` expected to be used.\n",
                 "\n",
                 "Data length `time_psd` (s)\n",
                 ": The entire length of data from which to estimate a PSD using Welch's method. Periodigrams are calculated on segments of this, and then averaged using the `median` method.\n",
                 "\n",
                 "Segment length `T` (s)\n",
                 ": The length of each segment on which to take the DFT and calculate a periodigram.\n",
                 "\n",
                 "Gap `time_gap` (s)\n",
-                ": Gap between duration-`T` segments. E.g., if `T_PSD=1024`, `T=8`, `T_gap=8`, then for each PSD, 64 periodigrams are computed, each using data stretches 8 s long, with gaps of 8 s between segments. Segments would then be $[0~\\text{s}, 8~\\text{s}], [16~\\text{s}, 24~\\text{s}], \\ldots$.\n",
+                ": Gap between duration-`T` segments. E.g., if `time_psd=1024`, `T=8`, `time_gap=8`, then for each PSD, 64 periodigrams are computed, each using data stretches 8 s long, with gaps of 8 s between segments. Segments would then be $[0~\\text{s}, 8~\\text{s}], [16~\\text{s}, 24~\\text{s}], \\ldots$.\n",
                 "\n",
                 "Window function\n",
                 ": Parameters of the window function used before taking DFT of data segments.\n",
                 "\n",
                 "`num_psds_max` (optional)\n",
                 ": If set, stop building the dataset after this number of PSDs have been estimated. This setting is useful for building a single-PSD dataset for pretraining a network.\n",
                 "\n",
-                "Channels 'channels (optional)\n",
+                "Channels (optional)\n",
                 ": If set, data will be fetched from these channels, instead of using GWOSC.\n",
                 "\n",
                 "Detectors\n",
                 ": Which detectors (H1, L1, V1, ...) to include in the dataset.\n",
                 "\n",
                 "Observing run\n",
                 ": Which observing run to use when estimating PSDs.\n",
                 "\n",
                 "Condor (optional)\n",
                 ": Settings for [HTCondor](https://htcondor.readthedocs.io/en/latest/index.html) useful for parallelizing the ASD estimation across condor jobs.\n",
                 "\n",
+                "### `dingo_generate_synthetic_asd_dataset`\n",
+                "This method generates a dataset of synthetic ASDs from a dataset of existing ASDs to enhance robustness against ASD distribution shifts. In particular, this allows to generate a dataset of synthetic ASDs that are *scaled* by a fiducial ASD in order to adapt to a new observing run. This is particularly useful for training Dingo networks at the beginning of an observing run, when the number of training ASDs is limited. It also allows to generate smoother synthetic ASDs that more closely resemble those from BayesWave. The implementation follows the steps explained in this [paper](https://inspirehep.net/literature/2182788).\n",
+                "```text\n",
+                "usage: dingo_generate_synthetic_asd_dataset [-h] --asd_dataset ASD_DATASET --settings_file SETTINGS_FILE [--num_processes NUM_PROCESSES] [--out_file OUT_FILE] [--verbose]\n",
+                "\n",
+                "Generate a synthetic noise ASD dataset from an existing dataset of real ASDs.\n",
+                "\n",
+                "optional arguments:\n",
+                "  -h, --help            show this help message and exit\n",
+                "  --asd_dataset ASD_DATASET\n",
+                "                        Path to existing ASD dataset to be parameterized and re-sampled\n",
+                "  --settings_file SETTINGS_FILE\n",
+                "                        YAML file containing database settings\n",
+                "  --num_processes NUM_PROCESSES\n",
+                "                        Number of processes to use in pool for parallel parameterization\n",
+                "  --out_file OUT_FILE   Name of file for storing dataset.\n",
+                "  --verbose\n",
+                "```\n",
+                "with a settings file of the form\n",
+                "```yaml\n",
+                "parameterization_settings:\n",
+                "  num_spline_positions: 30\n",
+                "  num_spectral_segments: 400\n",
+                "  sigma: 0.14\n",
+                "  delta_f: -1\n",
+                "  smoothen: True\n",
+                "sampling_settings:\n",
+                "   bandwidth_spectral: 0.5\n",
+                "   bandwidth_spline: 0.25\n",
+                "   num_samples: 500\n",
+                "   split_frequencies:\n",
+                "     - 30\n",
+                "     - 100\n",
+                "   rescaling_psd_paths:\n",
+                "     H1: /path/to/rescaling_asd_H1.hdf5\n",
+                "     L1: /path/to/rescaling_asd_L1.hdf5\n",
+                "```\n",
+                "Options correspond to the following:\n",
+                "\n",
+                "`num_spline_positions`\n",
+                ": Number of nodes to use for the cubic spline interpolating the broad-band noise PSD.\n",
+                "\n",
+                "`num_spectral_segments`\n",
+                ": Maximum number of spectral lines to model.\n",
+                "\n",
+                "`sigma`\n",
+                ": Standard deviation of the Normal distribution parameterizing $p(\\log S_n|z)$.\n",
+                "\n",
+                "`delta_f`\n",
+                ": If > 0, truncates each spectral line.\n",
+                "\n",
+                "`smoothen`\n",
+                ": Whether to save the smooth ASDs (True) or the noisy ASDs (False). The noisy synthetic ASDs resemble real ASDs estimated with Welch's method more closely, while the smooth ASDs are more similar to ASDs generated with BayesWave. (Default: False) \n",
+                "\n",
+                "`bandwidth_spectral, bandwidth_spline`\n",
+                ": Bandwidths for the KDEs modeling the distribution over spectral lines and broad-band noise, respectively. These determine the width of the resulting distribution.\n",
+                "\n",
+                "`num_samples`\n",
+                ": Number of synthetic ASDs to generate.\n",
+                "\n",
+                "`split_frequencies`\n",
+                ": (Set of) frequencies at dividing the broad-band noise into independent segments, e.g. due to different dominant noise sources (shot noise, seismic noise, etc.).\n",
+                "\n",
+                "`rescaling_psd_paths`\n",
+                ": Paths to ASD datasets for each detector to which the synthetic ASDs should be rescaled, e.g. the PSDs from the target observing run. If the dataset contains multiple ASDs, we use the first one. (Optional; if not provided, no rescaling will be done.)\n",
+                "\n",
                 "(ref:window-factor)=\n",
                 "## Data conditioning\n",
                 "\n",
                 "Importantly, the variance of *white* noise in each frequency bin is not 1, but rather\n",
                 "\n",
                 "$$\n",
                 "\\sigma^2_{\\text{white}} = \\frac{w}{4\\delta f}\n",
```

### Comparing `dingo-gw-0.4.3/docs/source/overview.md` & `dingo-gw-0.5.0/docs/source/overview.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,27 +44,28 @@
 
 ```{table}
 
 | Command | Description |
 |---|---|
 |`dingo_ls`| Inspect a file produced by Dingo and print a summary.|
 |`dingo_append_training_stage`| Modify the training plan of a model checkpoint.|
+|`dingo_pt_to_hdf5`| Convert a trained Dingo model from a PyTorch pickle .pt file to HDF5.|
 ```
 
 ```{hint}
 
 The `dingo_ls` command is very useful for inspecting Dingo files. It will print all settings that went in to producing the file, as well as some derived quantities.
 ```
 
 ### File types
 
-As noted above, most Dingo commands take a YAML file to specify configuration options (except for `dingo_pipe`, which uses an INI file, as is standard for LVK parameter estimation). When run, these commands generate data, which is usually stored in HDF5 files. One exception is when training a neural network. This saves the network weights using the PyTorch `.pt` format.
+As noted above, most Dingo commands take a YAML file to specify configuration options (except for `dingo_pipe`, which uses an INI file, as is standard for LVK parameter estimation). When run, these commands generate data, which is usually stored in HDF5 files. One exception is when training a neural network. This saves the network weights using the PyTorch `.pt` format. However, primarily for LVK use, `dingo_pt_to_hdf5` can convert the weights of a trained model to a HDF5 file.
 
 ```{important}
 
 In all cases, Dingo will save the YAML file settings within the final output file. This is needed for downstream tasks and for maintaining reproducibility.
 ```
 
 
 ## GNPE
 
-A slightly more complicated workflow occurs when using [](gnpe.md). GNPE is an algorithm that combines physical symmetries with Gibbs sampling to significantly improve results. When using GNPE, however, it is necessary to train **two networks**---one main (conditional) network that will be repeatedly sampled during Gibbs sampling and one smaller network used to initialize the Gibbs sampler. At inference time, `dingo_pipe` must be pointed to **both** of these networks. See the section on [GNPE usage](gnpe.md#usage) for further details.
+A slightly more complicated workflow occurs when using [](gnpe.md). GNPE is an algorithm that combines physical symmetries with Gibbs sampling to significantly improve results. When using GNPE, however, it is necessary to train **two networks**---one main (conditional) network that will be repeatedly sampled during Gibbs sampling and one smaller network used to initialize the Gibbs sampler. At inference time, `dingo_pipe` must be pointed to **both** of these networks. See the section on [GNPE usage](gnpe.md#usage) for further details.
```

### Comparing `dingo-gw-0.4.3/docs/source/quickstart.md` & `dingo-gw-0.5.0/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/refs.bib` & `dingo-gw-0.5.0/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/result.md` & `dingo-gw-0.5.0/docs/source/result.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/sbi.md` & `dingo-gw-0.5.0/docs/source/sbi.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/training.md` & `dingo-gw-0.5.0/docs/source/training.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/training_transforms.ipynb` & `dingo-gw-0.5.0/docs/source/training_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/docs/source/waveform_dataset.ipynb` & `dingo-gw-0.5.0/docs/source/waveform_dataset.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984288194444444%*

 * *Differences: {"'cells'": "{13: {'source': {insert: [(27, '  # new_interface: true # Optional setting for "*

 * *            'employing new waveform interface. This is needed for SEOBNRv5 approximants, and '*

 * *            "optional for standard LAL approximants.\\n')]}, 'attachments': OrderedDict()}}"}*

```diff
@@ -452,14 +452,15 @@
             "source": [
                 "```{note}\n",
                 "The sample is represented as a *nested dictionary*. This is a standard format for Dingo.\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "11d4167a-e6a1-44c0-abd0-9184c56d40f5",
             "metadata": {},
             "source": [
                 "## Automated dataset construction\n",
                 "\n",
                 "The simple dataset constructed above is useful for illustrative purposes, but it lacks the several important features:\n",
@@ -483,14 +484,15 @@
                 "  f_max: 1024.0\n",
                 "  delta_f: 0.125\n",
                 "\n",
                 "waveform_generator:\n",
                 "  approximant: IMRPhenomXPHM\n",
                 "  f_ref: 20.0\n",
                 "  # f_start: 15.0  # Optional setting useful for EOB waveforms. Overrides f_min when generating waveforms.\n",
+                "  # new_interface: true # Optional setting for employing new waveform interface. This is needed for SEOBNRv5 approximants, and optional for standard LAL approximants.\n",
                 "\n",
                 "# Dataset only samples over intrinsic parameters. Extrinsic parameters are chosen at train time.\n",
                 "intrinsic_prior:\n",
                 "  mass_1: bilby.core.prior.Constraint(minimum=10.0, maximum=80.0)\n",
                 "  mass_2: bilby.core.prior.Constraint(minimum=10.0, maximum=80.0)\n",
                 "  chirp_mass: bilby.gw.prior.UniformInComponentsChirpMass(minimum=25.0, maximum=100.0)\n",
                 "  mass_ratio: bilby.gw.prior.UniformInComponentsMassRatio(minimum=0.125, maximum=1.0)\n",
```

### Comparing `dingo-gw-0.4.3/examples/README.md` & `dingo-gw-0.5.0/examples/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 
 One can use `dingo_generate_dataset_dag` to set up a condor DAG for generating waveforms on a cluster. This is typically useful for slower waveform models.
 
 ### Noise ASDs
 
 Training also requires a dataset of noise ASDs, which are sampled randomly for each training sample. To generate this dataset based on noise observed during a run, execute
 ```
-dingo_generate_ASD_dataset --data_dir data_dir --settings_file asd_dataset_settings.yaml
+dingo_generate_asd_dataset --data_dir data_dir --settings_file asd_dataset_settings.yaml
 ```
-This will download data from the GWOSC website and create a `/tmp` directory, in which the estimated PSDs are stored. Subsequently, these are collected together into a final `.hdf5` ASD dataset. 
-If no `settings_file` is passed, the script will attempt to use the default one `data_dir/asd_dataset_settings.yaml`. 
+This will download data and create a `/tmp` directory, in which the estimated PSDs are stored. Subsequently, these are collected together into a final `.hdf5` ASD dataset. 
 
 ## Training
 
 With a waveform dataset and ASD dataset(s), one can train a neural network. Configure the `train_settings.yaml` file to point to these datasets, and run
 ```
 dingo_train --settings_file train_settings.yaml --train_dir train_dir
 ```
```

### Comparing `dingo-gw-0.4.3/examples/dataset_generation/asd_dataset_settings.yaml` & `dingo-gw-0.5.0/examples/gnpe_model/asd_dataset_settings.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dataset_settings:
+#  f_min: 0         # defaults to 0
+#  f_max: 2048      # defaults to f_s/2
   f_s: 4096
   time_psd: 1024
   T: 8
   window:
     roll_off: 0.4
     type: tukey
   time_gap: 0          # specifies the time skipped between to consecutive PSD estimates. If set < 0, the time segments overlap
-  num_psds_max: 20   # if set > 0, only a subset of all available PSDs will be used
+  num_psds_max: 0   # if set > 0, only a subset of all available PSDs will be used
 #  channels:
 #    H1: H1:DCS-CALIB_STRAIN_C02
 #    L1: L1:DCS-CALIB_STRAIN_C02
   detectors:
     - H1
+    - L1
   observing_run: O2
 # condor:
-#   env_path: /Users/jonaswildberger/Desktop/dingo-devel/venv
+#   env_path: /path/to/environment
 #   num_jobs: 2 # per detector
 #   num_cpus: 16
 #   memory_cpus: 16000
-#   bid: 200
```

### Comparing `dingo-gw-0.4.3/examples/dataset_generation/waveform_dataset_settings.yaml` & `dingo-gw-0.5.0/examples/gnpe_model/waveform_dataset_settings.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 waveform_generator:
   approximant: IMRPhenomXPHM  # SEOBNRv4PHM
   f_ref: 20.0
   # f_start: 15.0  # Optional setting useful for EOB waveforms. Overrides f_min when generating waveforms.
 
 # Dataset only samples over intrinsic parameters. Extrinsic parameters are chosen at train time.
 intrinsic_prior:
-  mass_1: bilby.core.prior.Constraint(minimum=10.0, maximum=80.0)
-  mass_2: bilby.core.prior.Constraint(minimum=10.0, maximum=80.0)
-  chirp_mass: bilby.gw.prior.UniformInComponentsChirpMass(minimum=25.0, maximum=100.0)
+  mass_1: bilby.core.prior.Constraint(minimum=10.0, maximum=120.0)
+  mass_2: bilby.core.prior.Constraint(minimum=10.0, maximum=120.0)
+  chirp_mass: bilby.gw.prior.UniformInComponentsChirpMass(minimum=15.0, maximum=150.0)
   mass_ratio: bilby.gw.prior.UniformInComponentsMassRatio(minimum=0.125, maximum=1.0)
   phase: default
   a_1: bilby.core.prior.Uniform(minimum=0.0, maximum=0.99)
   a_2: bilby.core.prior.Uniform(minimum=0.0, maximum=0.99)
   tilt_1: default
   tilt_2: default
   phi_12: default
@@ -33,8 +33,8 @@
 # Save a compressed representation of the dataset
 compression:
   svd:
     # Truncate the SVD basis at this size. No truncation if zero.
     size: 200
     num_training_samples: 50000
     num_validation_samples: 10000
-  whitening: aLIGO_ZERO_DET_high_P_asd.txt
+  whitening: aLIGO_ZERO_DET_high_P_asd.txt
```

### Comparing `dingo-gw-0.4.3/examples/is_settings.yaml` & `dingo-gw-0.5.0/examples/misc/is_settings.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -39,10 +39,11 @@
       lr: 0.003
     scheduler:
       type: cosine
       T_max: 20
 
 calibration_marginalization:
   num_calibration_curves: 100
+  num_calibration_nodes: 10
   calibration_envelope:
     H1: <path/to/H1-calibration-envelope>
     L1: <path/to/L1-calibration-envelope>
```

### Comparing `dingo-gw-0.4.3/examples/pipe/GW150914.ini` & `dingo-gw-0.5.0/examples/gnpe_model/GW150914.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ################################################################################
 ##  Job submission arguments
 ################################################################################
 
 local = True
 accounting = dingo
-request-cpus-importance-sampling = 16
-n-parallel = 4
+request-cpus-importance-sampling = 64
 sampling-requirements = [TARGET.CUDAGlobalMemoryMb>40000]
 # extra-lines = [+WantsGPUNode = True]
-simple-submission = false
 
 ################################################################################
 ##  Sampler arguments
 ################################################################################
 
-model-init = /data/sgreen/dingo-experiments/XPHM/O1_init/model_stage_1.pt
-model = /data/sgreen/dingo-experiments/XPHM/testing_inference/model.pt
+model-init = training/init_train_dir/model_latest.pt
+model = training/main_train_dir/model_latest.pt
 device = 'cuda'
 num-gnpe-iterations = 30
 num-samples = 50000
 batch-size = 50000
 recover-log-prob = true
 prior-dict = {
 luminosity_distance = bilby.gw.prior.UniformComovingVolume(minimum=100, maximum=2000, name='luminosity_distance'),
@@ -40,8 +38,8 @@
 
 ################################################################################
 ## Plotting arguments
 ################################################################################
 
 plot-corner = true
 plot-weights = true
-plot-log-probs = true
+plot-log-probs = true
```

### Comparing `dingo-gw-0.4.3/examples/training/train_settings_init_production.yaml` & `dingo-gw-0.5.0/examples/gnpe_model/train_settings_init.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 data:
-  waveform_dataset_path: /path/to/waveform_dataset.hdf5  # Contains intrinsic waveforms
+  waveform_dataset_path: training_data/waveform_dataset.hdf5  # Contains intrinsic waveforms
   train_fraction: 0.95
   window:  # Needed to calculate window factor for simulated data
     type: tukey
     f_s: 4096
     T: 8.0
     roll_off: 0.4
   domain_update:
@@ -53,46 +53,45 @@
       num_validation_samples: 10000
       size: 200
 
 # Training is divided in stages. They each require all settings as indicated below.
 training:
   stage_0:  # Pre-training stage (fixed ASD, typically)
     epochs: 150
-    asd_dataset_path: /path/to/asds_fiducial.hdf5 # This should just contain a single 'fiducial' ASD for each detector.
+    asd_dataset_path: training_data/asd_dataset_fiducial/asds_O1_fiducial.hdf5 # This should just contain a single 'fiducial' ASD for each detector.
     freeze_rb_layer: True
     optimizer:
       type: adam
       lr: 5.0e-5
     scheduler:
       type: cosine
       T_max: 150
     batch_size: 4096
 
   stage_1:  # Fine-tuning stage
     epochs: 75
-    asd_dataset_path: /path/to/asds.hdf5 # This should contain a large collection of ASDs for each detector.
+    asd_dataset_path: training_data/asd_dataset/asds_O1.hdf5 # This should contain a large collection of ASDs for each detector.
     freeze_rb_layer: False
     optimizer:
       type: adam
       lr: 1.0e-5
     scheduler:
       type: cosine
       T_max: 75
     batch_size: 4096
 
 # Local settings for training that have no impact on the final trained network.
 local:
   device: cpu  # Change this to 'cuda' for training on a GPU.
   num_workers: 6  # num_workers >0 does not work on Mac, see https://stackoverflow.com/questions/64772335/pytorch-w-parallelnative-cpp206
-  #  wandb:
-  #    project: dingo
-  #    group: O4
+  use_wandb: True
+  wandb_api_key:  # insert_here for monitoring many runs. Can be obtained from https://wandb.ai/settings
   runtime_limits:
     max_time_per_run: 36000
     max_epochs_per_run: 500
   checkpoint_epochs: 10
   condor:
     bid: 100
     num_cpus: 16
     memory_cpus: 128000
     num_gpus: 1
-    memory_gpus: 8000
+    memory_gpus: 8000
```

### Comparing `dingo-gw-0.4.3/examples/training/train_settings_no_gnpe_production.yaml` & `dingo-gw-0.5.0/examples/gnpe_model/train_settings.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 data:
-  waveform_dataset_path: /path/to/waveform_dataset.hdf5  # Contains intrinsic waveforms
+  waveform_dataset_path: training_data/waveform_dataset.hdf5  # Contains intrinsic waveforms
   train_fraction: 0.95
   window:  # Needed to calculate window factor for simulated data
     type: tukey
     f_s: 4096
     T: 8.0
     roll_off: 0.4
   domain_update:
@@ -16,15 +16,32 @@
   extrinsic_prior:  # Sampled at train time
     dec: default
     ra: default
     geocent_time: bilby.core.prior.Uniform(minimum=-0.10, maximum=0.10)
     psi: default
     luminosity_distance: bilby.core.prior.Uniform(minimum=100.0, maximum=1000.0)
   ref_time: 1126259462.391
-  inference_parameters: default # [chirp_mass, mass_ratio,  luminosity_distance, dec]
+  gnpe_time_shifts:
+    kernel: bilby.core.prior.Uniform(minimum=-0.001, maximum=0.001)
+    exact_equiv: True
+  inference_parameters: 
+    - chirp_mass
+    - mass_ratio
+    - a_1
+    - a_2
+    - tilt_1
+    - tilt_2
+    - phi_12
+    - phi_jl
+    - theta_jn
+    - luminosity_distance
+    - geocent_time
+    - ra
+    - dec
+    - psi
 
 # Model architecture
 model:
   type: nsf+embedding
   # kwargs for neural spline flow
   nsf_kwargs:
     num_flow_steps: 30
@@ -51,47 +68,44 @@
       num_validation_samples: 10000
       size: 200
 
 # Training is divided in stages. They each require all settings as indicated below.
 training:
   stage_0:
     epochs: 300
-    asd_dataset_path: /path/to/asds_fiducial.hdf5 # this should just contain a single fiducial ASD per detector for pretraining
+    asd_dataset_path: training_data/asd_dataset_folder_fiducial/asds_O1_fiducial.hdf5 # this should just contain a single fiducial ASD per detector for pretraining
     freeze_rb_layer: True
     optimizer:
       type: adam
       lr: 5.0e-5
     scheduler:
       type: cosine
       T_max: 300
     batch_size: 4096
 
   stage_1:
     epochs: 150
-    asd_dataset_path: /path/to/asds.hdf5 # this should contain many different ASDS per detector for finetuning
+    asd_dataset_path: training_data/asd_dataset_folder/asds_O1.hdf5 # this should contain many different ASDS per detector for finetuning
     freeze_rb_layer: False
     optimizer:
       type: adam
       lr: 1.0e-5
     scheduler:
       type: cosine
       T_max: 150
     batch_size: 4096
 
 # Local settings for training that have no impact on the final trained network.
 local:
-  device: cpu  # Change this to 'cuda' for training on a GPU.
+  device: cuda # Change this to 'cuda' for training on a GPU.
   num_workers: 32  # num_workers >0 does not work on Mac, see https://stackoverflow.com/questions/64772335/pytorch-w-parallelnative-cpp206
-  #  wandb:
-  #    project: dingo
-  #    group: O4
   runtime_limits:
     max_time_per_run: 36000
     max_epochs_per_run: 500
   checkpoint_epochs: 10
   # Local settings related to condor, remove if not used on cluster
   condor:
     bid: 100
     num_cpus: 16
     memory_cpus: 128000
     num_gpus: 1
-    memory_gpus: 8000
+    memory_gpus: 8000
```

### Comparing `dingo-gw-0.4.3/examples/training/train_settings_no_gnpe_toy.yaml` & `dingo-gw-0.5.0/examples/npe_model/train_settings.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 data:
-  waveform_dataset_path: /path/to/waveform_dataset.hdf5  # Contains intrinsic waveforms
+  waveform_dataset_path: training_data/waveform_dataset.hdf5  # Contains intrinsic waveforms
   train_fraction: 0.95
   window:  # Needed to calculate window factor for simulated data
     type: tukey
     f_s: 4096
     T: 8.0
     roll_off: 0.4
   domain_update:
@@ -16,81 +16,89 @@
   extrinsic_prior:  # Sampled at train time
     dec: default
     ra: default
     geocent_time: bilby.core.prior.Uniform(minimum=-0.10, maximum=0.10)
     psi: default
     luminosity_distance: bilby.core.prior.Uniform(minimum=100.0, maximum=1000.0)
   ref_time: 1126259462.391
-  gnpe_time_shifts:
-    kernel: bilby.core.prior.Uniform(minimum=-0.001, maximum=0.001)
-    exact_equiv: True
-  inference_parameters: default # [chirp_mass, mass_ratio,  luminosity_distance, dec]
+  inference_parameters:
+  - chirp_mass
+  - mass_ratio
+  - chi_1
+  - chi_2
+  - theta_jn
+  - dec
+  - ra
+  - geocent_time
+  - luminosity_distance
+  - psi
 
 # Model architecture
 model:
   type: nsf+embedding
   # kwargs for neural spline flow
   nsf_kwargs:
-    num_flow_steps: 3
+    num_flow_steps: 30
     base_transform_kwargs:
-      hidden_dim: 64 
+      hidden_dim: 1024
       num_transform_blocks: 5
       activation: elu
       dropout_probability: 0.0
       batch_norm: True
       num_bins: 8
       base_transform_type: rq-coupling
   # kwargs for embedding net
   embedding_net_kwargs:
     output_dim: 128
-    hidden_dims: [1024, 512, 256, 128]
+    hidden_dims: [1024, 1024, 1024, 1024, 1024, 1024,
+                  512, 512, 512, 512, 512, 512,
+                  256, 256, 256, 256, 256, 256,
+                  128, 128, 128, 128, 128, 128]
     activation: elu
     dropout: 0.0
     batch_norm: True
     svd:
-      num_training_samples: 20000
-      num_validation_samples: 5000
+      num_training_samples: 50000
+      num_validation_samples: 10000
       size: 200
 
 # Training is divided in stages. They each require all settings as indicated below.
 training:
   stage_0:
     epochs: 300
-    asd_dataset_path: /path/to/asds_fiducial.hdf5 # this should just contain a single fiducial ASD per detector for pretraining
+    asd_dataset_path: training_data/asd_dataset_fiducial/asds_O1_fiducial.hdf5 # this should just contain a single fiducial ASD per detector for pretraining
     freeze_rb_layer: True
     optimizer:
       type: adam
-      lr: 0.0001
+      lr: 5.0e-5
     scheduler:
       type: cosine
       T_max: 300
-    batch_size: 64
+    batch_size: 4096
 
   stage_1:
     epochs: 150
-    asd_dataset_path: /path/to/asds.hdf5 # this should contain many different ASDS per detector for finetuning
+    asd_dataset_path: training_data/asd_dataset/asds_O1.hdf5 # this should contain many different ASDS per detector for finetuning
     freeze_rb_layer: False
     optimizer:
       type: adam
-      lr: 0.00001
+      lr: 1.0e-5
     scheduler:
       type: cosine
       T_max: 150
-    batch_size: 64
+    batch_size: 4096
 
 # Local settings for training that have no impact on the final trained network.
 local:
-  device: cpu  # Change this to 'cuda' for training on a GPU.
-  num_workers: 6  # num_workers >0 does not work on Mac, see https://stackoverflow.com/questions/64772335/pytorch-w-parallelnative-cpp206
-#  wandb:
-#    project: dingo
-#    group: O4
+  device: cuda # Change this to 'cuda' for training on a GPU.
+  num_workers: 32  # num_workers >0 does not work on Mac, see https://stackoverflow.com/questions/64772335/pytorch-w-parallelnative-cpp206
   runtime_limits:
     max_time_per_run: 36000
     max_epochs_per_run: 500
-  checkpoint_epochs: 10
+  checkpoint_epochs: 50
+  # Local settings related to condor, remove if not used on cluster
   condor:
     bid: 100
     num_cpus: 16
     memory_cpus: 128000
     num_gpus: 1
-    memory_gpus: 8000
+    memory_gpus: 8000
```

### Comparing `dingo-gw-0.4.3/examples/training/train_settings_production.yaml` & `dingo-gw-0.5.0/examples/toy_npe_model/train_settings.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,79 @@
 data:
-  waveform_dataset_path: /path/to/waveform_dataset.hdf5  # Contains intrinsic waveforms
+  waveform_dataset_path: training_data/waveform_dataset.hdf5  # Contains intrinsic waveforms
   train_fraction: 0.95
   window:  # Needed to calculate window factor for simulated data
     type: tukey
     f_s: 4096
     T: 8.0
     roll_off: 0.4
-  domain_update:
-    f_min: 20.0
-    f_max: 1024.0
-  svd_size_update: 200  # Optionally, reduce the SVD size when decompressing (for performance)
   detectors:
     - H1
     - L1
   extrinsic_prior:  # Sampled at train time
     dec: default
     ra: default
     geocent_time: bilby.core.prior.Uniform(minimum=-0.10, maximum=0.10)
     psi: default
     luminosity_distance: bilby.core.prior.Uniform(minimum=100.0, maximum=1000.0)
   ref_time: 1126259462.391
-  gnpe_time_shifts:
-    kernel: bilby.core.prior.Uniform(minimum=-0.001, maximum=0.001)
-    exact_equiv: True
-  inference_parameters: default # [chirp_mass, mass_ratio,  luminosity_distance, dec]
+  inference_parameters: 
+  - chirp_mass
+  - mass_ratio
+  - chi_1
+  - chi_2
+  - theta_jn
+  - dec
+  - ra
+  - geocent_time
+  - luminosity_distance
+  - psi
+  - phase
 
 # Model architecture
 model:
   type: nsf+embedding
   # kwargs for neural spline flow
   nsf_kwargs:
-    num_flow_steps: 30
+    num_flow_steps: 5
     base_transform_kwargs:
-      hidden_dim: 1024
+      hidden_dim: 64 
       num_transform_blocks: 5
       activation: elu
       dropout_probability: 0.0
       batch_norm: True
       num_bins: 8
       base_transform_type: rq-coupling
   # kwargs for embedding net
   embedding_net_kwargs:
     output_dim: 128
-    hidden_dims: [1024, 1024, 1024, 1024, 1024, 1024,
-                  512, 512, 512, 512, 512, 512,
-                  256, 256, 256, 256, 256, 256,
-                  128, 128, 128, 128, 128, 128]
+    hidden_dims: [1024, 512, 256, 128]
     activation: elu
     dropout: 0.0
     batch_norm: True
     svd:
-      num_training_samples: 50000
-      num_validation_samples: 10000
-      size: 200
+      num_training_samples: 1000
+      num_validation_samples: 100
+      size: 50
 
-# Training is divided in stages. They each require all settings as indicated below.
+# The first stage (and only) stage of training. 
 training:
   stage_0:
-    epochs: 300
-    asd_dataset_path: /path/to/asds_fiducial.hdf5 # this should just contain a single fiducial ASD per detector for pretraining
+    epochs: 20
+    asd_dataset_path: training_data/asd_dataset/asds_O1.hdf5  # this should just contain a single fiducial ASD per detector for pretraining
     freeze_rb_layer: True
     optimizer:
       type: adam
-      lr: 5.0e-5
+      lr: 0.0001
     scheduler:
       type: cosine
-      T_max: 300
-    batch_size: 4096
-
-  stage_1:
-    epochs: 150
-    asd_dataset_path: /path/to/asds.hdf5 # this should contain many different ASDS per detector for finetuning
-    freeze_rb_layer: False
-    optimizer:
-      type: adam
-      lr: 1.0e-5
-    scheduler:
-      type: cosine
-      T_max: 150
-    batch_size: 4096
+      T_max: 20
+    batch_size: 64
 
 # Local settings for training that have no impact on the final trained network.
 local:
   device: cpu  # Change this to 'cuda' for training on a GPU.
-  num_workers: 32  # num_workers >0 does not work on Mac, see https://stackoverflow.com/questions/64772335/pytorch-w-parallelnative-cpp206
-#  wandb:
-#    project: dingo
-#    group: O4
+  num_workers: 6  # num_workers >0 does not work on Mac, see https://stackoverflow.com/questions/64772335/pytorch-w-parallelnative-cpp206
   runtime_limits:
     max_time_per_run: 36000
-    max_epochs_per_run: 500
-  checkpoint_epochs: 10
-  # Local settings related to condor, remove if not used on cluster
-  condor:
-    bid: 100
-    num_cpus: 16
-    memory_cpus: 128000
-    num_gpus: 1
-    memory_gpus: 8000
+    max_epochs_per_run: 30
+  checkpoint_epochs: 15
```

### Comparing `dingo-gw-0.4.3/pyproject.toml` & `dingo-gw-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "pyopenssl",
     "pyyaml",
     "scikit-learn",
     "scipy",
     "threadpoolctl",
     "torch",
     "torchvision",
+    "tqdm",
 ]
 
 
 [tool.setuptools.packages.find]
 include = ["dingo*"]
 namespaces = false
 
@@ -68,14 +69,15 @@
     "black",
     "linkify-it-py",
     "myst-nb",
     "myst-parser",
     "pylint",
     "pytest",
     "sphinx",
+    "sphinx-math-dollar",
     "sphinx-rtd-theme",
     "sphinxcontrib-mermaid",
     "sphinxcontrib-bibtex",
     "wandb",
 ]
 
 
@@ -83,18 +85,23 @@
 dingo_append_training_stage = "dingo.gw.training:append_stage"
 dingo_analyze_event = "dingo.gw.inference:analyze_event"
 dingo_build_svd = "dingo.gw.dataset.utils:build_svd_cli"
 dingo_estimate_psds = "dingo.gw.noise.asd_estimation:download_and_estimate_cli"
 dingo_generate_asd_dataset = "dingo.gw.noise.generate_dataset:generate_dataset"
 dingo_generate_dataset = "dingo.gw.dataset.generate_dataset:main"
 dingo_generate_dataset_dag = "dingo.gw.dataset.generate_dataset_dag:main"
+dingo_generate_synthetic_asd_dataset = "dingo.gw.noise.synthetic_noise.generate_dataset:main"
 dingo_ls = "dingo.gw.ls_cli:ls"
 dingo_merge_datasets = "dingo.gw.dataset.utils:merge_datasets_cli"
 dingo_merge_asd_datasets = "dingo.gw.noise.utils:merge_datasets_cli"
-dingo_pipe = "dingo.gw.pipe.main:main"
-dingo_pipe_importance_sampling = "dingo.gw.pipe.importance_sampling:main"
-dingo_pipe_generation = "dingo.gw.pipe.data_generation:main"
-dingo_pipe_sampling = "dingo.gw.pipe.sampling:main"
-dingo_pipe_plot = "dingo.gw.pipe.plot:main"
+dingo_pipe = "dingo.pipe.main:main"
+dingo_pipe_importance_sampling = "dingo.pipe.importance_sampling:main"
+dingo_pipe_generation = "dingo.pipe.data_generation:main"
+dingo_pipe_sampling = "dingo.pipe.sampling:main"
+dingo_pipe_plot = "dingo.pipe.plot:main"
+dingo_pt_to_hdf5 = "dingo.core.utils.pt_to_hdf5:main"
+dingo_result = "dingo.pipe.dingo_result:main"
 dingo_train = "dingo.gw.training:train_local"
 dingo_train_condor = "dingo.gw.training.train_pipeline_condor:train_condor"
-dingo_result = "dingo.gw.pipe.dingo_result:main"
+
+[project.entry-points."asimov.pipelines"]
+dingo = "dingo.asimov.asimov:Dingo"
```

### Comparing `dingo-gw-0.4.3/tests/core/test_enets.py` & `dingo-gw-0.5.0/tests/core/test_enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/core/test_nsf.py` & `dingo-gw-0.5.0/tests/core/test_nsf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/core/test_posterior_model.py` & `dingo-gw-0.5.0/tests/core/test_posterior_model.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/core/testutils_enets.py` & `dingo-gw-0.5.0/tests/core/testutils_enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/conversion/test_spin_conversion.py` & `dingo-gw-0.5.0/tests/gw/conversion/test_spin_conversion.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/conversion/test_time_delay_from_geocenter.py` & `dingo-gw-0.5.0/tests/gw/conversion/test_time_delay_from_geocenter.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/test_domains.py` & `dingo-gw-0.5.0/tests/gw/test_domains.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/test_injection.py` & `dingo-gw-0.5.0/tests/gw/test_injection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/test_noise_dataset.py` & `dingo-gw-0.5.0/tests/gw/test_noise_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/test_prior_split.py` & `dingo-gw-0.5.0/tests/gw/test_prior_split.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/test_waveform_dataset.py` & `dingo-gw-0.5.0/tests/gw/test_waveform_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/transforms/test_detector_projection.py` & `dingo-gw-0.5.0/tests/gw/transforms/test_detector_projection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/transforms/test_gnpe_transforms.py` & `dingo-gw-0.5.0/tests/gw/transforms/test_gnpe_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/transforms/test_parameter_transforms.py` & `dingo-gw-0.5.0/tests/gw/transforms/test_parameter_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/transforms/waveform_data.npy` & `dingo-gw-0.5.0/tests/gw/transforms/waveform_data.npy`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/waveform_generator/test_wfg.py` & `dingo-gw-0.5.0/tests/gw/waveform_generator/test_wfg.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.4.3/tests/gw/waveform_generator/test_wfg_m.py` & `dingo-gw-0.5.0/tests/gw/waveform_generator/test_wfg_m.py`

 * *Files identical despite different names*

