# Comparing `tmp/truss-0.4.3.tar.gz` & `tmp/truss-0.4.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.3.tar", max compression
+gzip compressed data, was "truss-0.4.4.dev3.tar", max compression
```

## Comparing `truss-0.4.3.tar` & `truss-0.4.4.dev3.tar`

### file list

```diff
@@ -1,156 +1,164 @@
--rw-r--r--   0        0        0     5483 2023-04-13 16:45:41.461156 truss-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-04-13 16:45:41.461156 truss-0.4.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-04-13 16:45:41.461156 truss-0.4.3/LICENSE
--rw-r--r--   0        0        0     5958 2023-04-13 16:45:41.461156 truss-0.4.3/README.md
--rw-r--r--   0        0        0     3316 2023-04-13 16:45:41.461156 truss-0.4.3/ROADMAP.md
--rw-r--r--   0        0        0      465 2023-04-13 16:45:41.461156 truss-0.4.3/context_builder.Dockerfile
--rw-r--r--   0        0        0     2205 2023-04-13 16:45:41.553157 truss-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-13 16:45:41.553157 truss-0.4.3/truss/__init__.py
--rw-r--r--   0        0        0    13286 2023-04-13 16:45:41.553157 truss-0.4.3/truss/build.py
--rw-r--r--   0        0        0    10452 2023-04-13 16:45:41.553157 truss-0.4.3/truss/cli.py
--rw-r--r--   0        0        0     2700 2023-04-13 16:45:41.553157 truss-0.4.3/truss/constants.py
--rw-r--r--   0        0        0     1233 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5791 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4507 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-04-13 16:45:41.553157 truss-0.4.3/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-04-13 16:45:41.553157 truss-0.4.3/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-04-13 16:45:41.553157 truss-0.4.3/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-04-13 16:45:41.553157 truss-0.4.3/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-04-13 16:45:41.553157 truss-0.4.3/truss/errors.py
--rw-r--r--   0        0        0      824 2023-04-13 16:45:41.553157 truss-0.4.3/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-04-13 16:45:41.553157 truss-0.4.3/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2709 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-04-13 16:45:41.553157 truss-0.4.3/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-04-13 16:45:41.553157 truss-0.4.3/truss/notebook.py
--rw-r--r--   0        0        0    10874 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2388 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-04-13 16:45:41.553157 truss-0.4.3/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-04-13 16:45:41.553157 truss-0.4.3/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-04-13 16:45:41.553157 truss-0.4.3/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      979 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0     1196 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      875 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     3318 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     4943 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      162 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0      855 2023-04-13 16:45:41.553157 truss-0.4.3/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1666 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-13 16:45:41.557157 truss-0.4.3/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0     1006 2023-04-13 16:45:41.557157 truss-0.4.3/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/__init__.py
--rw-r--r--   0        0        0    19167 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/conftest.py
--rw-r--r--   0        0        0      783 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    10483 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     1910 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_build.py
--rw-r--r--   0        0        0     2359 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    31557 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      433 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-04-13 16:45:41.557157 truss-0.4.3/truss/tests/test_validation.py
--rw-r--r--   0        0        0     9289 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_config.py
--rw-r--r--   0        0        0     2841 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_gatherer.py
--rw-r--r--   0        0        0    39722 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_handle.py
--rw-r--r--   0        0        0     5195 2023-04-13 16:45:41.557157 truss-0.4.3/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-04-13 16:45:41.557157 truss-0.4.3/truss/types.py
--rw-r--r--   0        0        0     2350 2023-04-13 16:45:41.557157 truss-0.4.3/truss/utils.py
--rw-r--r--   0        0        0     2317 2023-04-13 16:45:41.557157 truss-0.4.3/truss/validation.py
--rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/LICENSE
+-rw-r--r--   0        0        0     5958 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/README.md
+-rw-r--r--   0        0        0     3316 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/ROADMAP.md
+-rw-r--r--   0        0        0      465 2023-04-21 04:27:43.131092 truss-0.4.4.dev3/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2209 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/cli.py
+-rw-r--r--   0        0        0     2742 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/constants.py
+-rw-r--r--   0        0        0     1237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5130 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4511 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1976 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     1686 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6565 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/notebook.py
+-rw-r--r--   0        0        0    10874 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2388 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1409 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1849 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       82 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      979 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0     2616 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/docs/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0     1173 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0     1196 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1708 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1892 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/external_data_resolver.py
+-rw-r--r--   0        0        0     1352 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     3318 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     5511 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      416 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      733 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     5384 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      162 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     1054 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1666 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1898 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0      216 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0      669 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0     1006 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/__init__.py
+-rw-r--r--   0        0        0    19997 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/conftest.py
+-rw-r--r--   0        0        0      783 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    10483 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6937 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2157 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/server/common/test_external_resolver.py
+-rw-r--r--   0        0        0     1910 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_build.py
+-rw-r--r--   0        0        0     2359 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     2605 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    31937 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    12070 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_config.py
+-rw-r--r--   0        0        0     2845 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    40806 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_handle.py
+-rw-r--r--   0        0        0     5331 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/types.py
+-rw-r--r--   0        0        0      227 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/jinja.py
+-rw-r--r--   0        0        0     2018 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/path.py
+-rw-r--r--   0        0        0     2317 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/validation.py
+-rw-r--r--   0        0        0     7302 1970-01-01 00:00:00.000000 truss-0.4.4.dev3/PKG-INFO
```

### Comparing `truss-0.4.3/CODE_OF_CONDUCT.md` & `truss-0.4.4.dev3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/CONTRIBUTING.md` & `truss-0.4.4.dev3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/LICENSE` & `truss-0.4.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/README.md` & `truss-0.4.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/ROADMAP.md` & `truss-0.4.4.dev3/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/pyproject.toml` & `truss-0.4.4.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.3"
+version = "0.4.4dev3"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.3/truss/build.py` & `truss-0.4.4.dev3/truss/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,16 @@
 from truss.errors import FrameworkNotSupportedError
 from truss.model_frameworks import MODEL_FRAMEWORKS_BY_TYPE, model_framework_from_model
 from truss.model_inference import infer_python_version, map_to_supported_python_version
 from truss.notebook import is_notebook_or_ipython
 from truss.truss_config import DEFAULT_EXAMPLES_FILENAME, TrussConfig
 from truss.truss_handle import TrussHandle
 from truss.types import ModelFrameworkType
-from truss.utils import (
-    build_truss_target_directory,
-    copy_file_path,
-    copy_tree_path,
-    get_gpu_memory,
-)
+from truss.util.gpu import get_gpu_memory
+from truss.util.path import build_truss_target_directory, copy_file_path, copy_tree_path
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 if is_notebook_or_ipython():
     logger.setLevel(logging.INFO)
     logger.addHandler(logging.StreamHandler(sys.stdout))
```

### Comparing `truss-0.4.3/truss/cli.py` & `truss-0.4.4.dev3/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/constants.py` & `truss-0.4.4.dev3/truss/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,7 +86,9 @@
 }
 
 MLFLOW_REQ_MODULE_NAMES: Set[str] = {"mlflow"}
 
 INFERENCE_SERVER_PORT = 8080
 
 TRAINING_VARIABLES_FILENAME = "variables.yaml"
+
+HTTP_PUBLIC_BLOB_BACKEND = "http_public"
```

### Comparing `truss-0.4.3/truss/contexts/image_builder/image_builder.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/image_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Optional
 
 from truss.docker import Docker
-from truss.utils import given_or_temporary_dir
+from truss.util.path import given_or_temporary_dir
 
 
 class ImageBuilder(ABC):
     def build_image(
         self,
         build_dir: Optional[Path] = None,
         tag: Optional[str] = None,
```

### Comparing `truss-0.4.3/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from pathlib import Path
 from typing import Optional
 
-import click
-from jinja2 import Environment, FileSystemLoader
 from truss.constants import (
     CONTROL_SERVER_CODE_DIR,
     MODEL_DOCKERFILE_NAME,
-    MODEL_README_NAME,
     REQUIREMENTS_TXT_FILENAME,
     SERVER_CODE_DIR,
     SERVER_DOCKERFILE_TEMPLATE_NAME,
     SERVER_REQUIREMENTS_TXT_FILENAME,
     SHARED_SERVING_AND_TRAINING_CODE_DIR,
     SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME,
     SYSTEM_PACKAGES_TXT_FILENAME,
@@ -22,17 +19,21 @@
     file_is_not_empty,
     to_dotted_python_version,
     truss_base_image_name,
     truss_base_image_tag,
 )
 from truss.contexts.truss_context import TrussContext
 from truss.patch.hash import directory_content_hash
-from truss.readme_generator import generate_readme
 from truss.truss_spec import TrussSpec
-from truss.utils import build_truss_target_directory, copy_file_path, copy_tree_path
+from truss.util.jinja import read_template_from_fs
+from truss.util.path import (
+    build_truss_target_directory,
+    copy_tree_or_file,
+    copy_tree_path,
+)
 
 BUILD_SERVER_DIR_NAME = "server"
 BUILD_CONTROL_SERVER_DIR_NAME = "control"
 
 
 class ServingImageBuilderContext(TrussContext):
     @staticmethod
@@ -51,101 +52,82 @@
 
     def prepare_image_build_dir(self, build_dir: Optional[Path] = None):
         """Prepare a directory for building the docker image from.
 
         Returns:
             docker command to build the docker image.
         """
+        truss_dir = self._truss_dir
+        spec = self._spec
+        model_framework_name = spec.model_framework_name
         if build_dir is None:
-            build_dir = build_truss_target_directory(self._spec.model_framework_name)
-            # todo: Add a logging statement here, suggesting how to clean up the directory.
+            # TODO(pankaj) We probably don't need model framework specific directory.
+            build_dir = build_truss_target_directory(model_framework_name)
 
-        copy_tree_path(self._spec.truss_dir, build_dir)
-        copy_tree_path(
-            SERVER_CODE_DIR,
-            build_dir / BUILD_SERVER_DIR_NAME,
-        )
-        copy_tree_path(
+        def copy_into_build_dir(from_path: Path, path_in_build_dir: str):
+            copy_tree_or_file(from_path, build_dir / path_in_build_dir)  # type: ignore[operator]
+
+        # Copy over truss
+        copy_tree_path(truss_dir, build_dir)
+
+        # Copy inference server code
+        copy_into_build_dir(SERVER_CODE_DIR, BUILD_SERVER_DIR_NAME)
+        copy_into_build_dir(
             SHARED_SERVING_AND_TRAINING_CODE_DIR,
-            build_dir
-            / BUILD_SERVER_DIR_NAME
-            / SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME,
+            BUILD_SERVER_DIR_NAME + "/" + SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME,
         )
+
+        # Copy control server code
         if self._spec.config.live_reload:
-            copy_tree_path(
-                CONTROL_SERVER_CODE_DIR,
-                build_dir / BUILD_CONTROL_SERVER_DIR_NAME,
-            )
+            copy_into_build_dir(CONTROL_SERVER_CODE_DIR, BUILD_CONTROL_SERVER_DIR_NAME)
+
+        # Copy model framework specific requirements file
         server_reqs_filepath = (
-            TEMPLATES_DIR / self._spec.model_framework_name / REQUIREMENTS_TXT_FILENAME
-        )
-        should_install_server_requirements = (
-            server_reqs_filepath.exists() and file_is_not_empty(server_reqs_filepath)
+            TEMPLATES_DIR / model_framework_name / REQUIREMENTS_TXT_FILENAME
         )
+        should_install_server_requirements = file_is_not_empty(server_reqs_filepath)
         if should_install_server_requirements:
-            copy_file_path(
-                TEMPLATES_DIR
-                / self._spec.model_framework_name
-                / REQUIREMENTS_TXT_FILENAME,
-                build_dir / SERVER_REQUIREMENTS_TXT_FILENAME,
-            )
-
-        with (build_dir / REQUIREMENTS_TXT_FILENAME).open("w") as req_file:
-            req_file.write(self._spec.requirements_txt)
-
-        with (build_dir / SYSTEM_PACKAGES_TXT_FILENAME).open("w") as req_file:
-            req_file.write(self._spec.system_packages_txt)
-
-        data_dir_exists = (build_dir / self._spec.config.data_dir).exists()
-        bundled_packages_dir_exists = (
-            build_dir / self._spec.config.bundled_packages_dir
-        ).exists()
-
-        template_loader = FileSystemLoader(str(TEMPLATES_DIR))
-        template_env = Environment(loader=template_loader)
-        dockerfile_template = template_env.get_template(SERVER_DOCKERFILE_TEMPLATE_NAME)
-        config = self._spec.config
+            copy_into_build_dir(server_reqs_filepath, SERVER_REQUIREMENTS_TXT_FILENAME)
+
+        (build_dir / REQUIREMENTS_TXT_FILENAME).write_text(spec.requirements_txt)
+        (build_dir / SYSTEM_PACKAGES_TXT_FILENAME).write_text(spec.system_packages_txt)
+
+        self._render_dockerfile(build_dir, should_install_server_requirements)
 
+    def _render_dockerfile(
+        self,
+        build_dir: Path,
+        should_install_server_requirements: bool,
+    ):
+        config = self._spec.config
+        data_dir = build_dir / config.data_dir
+        bundled_packages_dir = build_dir / config.bundled_packages_dir
+        dockerfile_template = read_template_from_fs(
+            TEMPLATES_DIR, SERVER_DOCKERFILE_TEMPLATE_NAME
+        )
         base_image_name = truss_base_image_name(job_type="server")
+        python_version = to_dotted_python_version(config.python_version)
         tag = truss_base_image_tag(
-            python_version=to_dotted_python_version(config.python_version),
+            python_version=python_version,
             use_gpu=config.resources.use_gpu,
             live_reload=config.live_reload,
             version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
         )
         base_image_name_and_tag = f"{base_image_name}:{tag}"
         should_install_system_requirements = file_is_not_empty(
             build_dir / SYSTEM_PACKAGES_TXT_FILENAME
         )
-        should_install_requirements = file_is_not_empty(
+        should_install_python_requirements = file_is_not_empty(
             build_dir / REQUIREMENTS_TXT_FILENAME
         )
         dockerfile_contents = dockerfile_template.render(
             should_install_server_requirements=should_install_server_requirements,
             base_image_name_and_tag=base_image_name_and_tag,
             should_install_system_requirements=should_install_system_requirements,
-            should_install_requirements=should_install_requirements,
+            should_install_requirements=should_install_python_requirements,
             config=config,
-            data_dir_exists=data_dir_exists,
-            bundled_packages_dir_exists=bundled_packages_dir_exists,
+            data_dir_exists=data_dir.exists(),
+            bundled_packages_dir_exists=bundled_packages_dir.exists(),
             truss_hash=directory_content_hash(self._truss_dir),
         )
         docker_file_path = build_dir / MODEL_DOCKERFILE_NAME
-        with docker_file_path.open("w") as docker_file:
-            docker_file.write(dockerfile_contents)
-
-        readme_file_path = build_dir / MODEL_README_NAME
-        try:
-            readme_contents = generate_readme(self._spec)
-            with readme_file_path.open("w") as readme_file:
-                readme_file.write(readme_contents)
-        except Exception as e:
-            click.echo(
-                click.style(
-                    f"""WARNING: Auto-readme generation has failed.
-                    This is probably due to a malformed config.yaml or
-                    malformed examples.yaml. Error is:
-                    {e}
-                    """,
-                    fg="yellow",
-                )
-            )
+        docker_file_path.write_text(dockerfile_contents)
```

### Comparing `truss-0.4.3/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/training_image_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     file_is_not_empty,
     to_dotted_python_version,
     truss_base_image_name,
     truss_base_image_tag,
 )
 from truss.contexts.truss_context import TrussContext
 from truss.truss_spec import TrussSpec
-from truss.utils import build_truss_target_directory, copy_file_path, copy_tree_path
+from truss.util.path import build_truss_target_directory, copy_file_path, copy_tree_path
 
 BUILD_TRAINING_DIR_NAME = "training"
 
 
 class TrainingImageBuilderContext(TrussContext):
     @staticmethod
     def run(truss_dir: Path):
```

### Comparing `truss-0.4.3/truss/contexts/image_builder/util.py` & `truss-0.4.4.dev3/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/contexts/local_loader/train_local.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/contexts/local_loader/utils.py` & `truss-0.4.4.dev3/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/docker.py` & `truss-0.4.4.dev3/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/environment_inference/requirements_inference.py` & `truss-0.4.4.dev3/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/errors.py` & `truss-0.4.4.dev3/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/local/local_config.py` & `truss-0.4.4.dev3/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/local/local_config_handler.py` & `truss-0.4.4.dev3/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_framework.py` & `truss-0.4.4.dev3/truss/model_framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import yaml
 from truss.constants import CONFIG_FILE, TEMPLATES_DIR
 from truss.environment_inference.requirements_inference import infer_deps
 from truss.model_inference import infer_python_version, map_to_supported_python_version
 from truss.truss_config import DEFAULT_EXAMPLES_FILENAME, TrussConfig
 from truss.types import ModelFrameworkType
-from truss.utils import copy_file_path, copy_tree_path
+from truss.util.path import copy_file_path, copy_tree_path
 
 
 class ModelFramework(ABC):
     @abstractmethod
     def typ(self) -> ModelFrameworkType:
         pass
```

### Comparing `truss-0.4.3/truss/model_frameworks/__init__.py` & `truss-0.4.4.dev3/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.4.dev3/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/keras.py` & `truss-0.4.4.dev3/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/lightgbm.py` & `truss-0.4.4.dev3/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/mlflow.py` & `truss-0.4.4.dev3/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/pytorch.py` & `truss-0.4.4.dev3/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/sklearn.py` & `truss-0.4.4.dev3/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_frameworks/xgboost.py` & `truss-0.4.4.dev3/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/model_inference.py` & `truss-0.4.4.dev3/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/patch/calc_patch.py` & `truss-0.4.4.dev3/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/patch/dir_signature.py` & `truss-0.4.4.dev3/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/patch/hash.py` & `truss-0.4.4.dev3/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/patch/types.py` & `truss-0.4.4.dev3/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/readme_generator.py` & `truss-0.4.4.dev3/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/README.md.jinja` & `truss-0.4.4.dev3/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/base.Dockerfile.jinja` & `truss-0.4.4.dev3/truss/templates/base.Dockerfile.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 {% block install_requirements %}
     {%- if should_install_requirements %}
 COPY ./requirements.txt requirements.txt
 RUN pip install -r requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
     {%- endif %}
 {% endblock %}
 
+{% block b10cp %}
+{% endblock %}
+
 
 ENV APP_HOME /app
 WORKDIR $APP_HOME
 
 
 {% block app_copy %}
 {% endblock %}
```

### Comparing `truss-0.4.3/truss/templates/control/control/application.py` & `truss-0.4.4.dev3/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/endpoints.py` & `truss-0.4.4.dev3/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/helpers/errors.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/helpers/types.py` & `truss-0.4.4.dev3/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/control/control/server.py` & `truss-0.4.4.dev3/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/custom/model/model.py` & `truss-0.4.4.dev3/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/docs/README.md` & `truss-0.4.4.dev3/truss/templates/docs/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/keras/model/model.py` & `truss-0.4.4.dev3/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/lightgbm/model/model.py` & `truss-0.4.4.dev3/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/mlflow/model/model.py` & `truss-0.4.4.dev3/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/pipeline/model/model.py` & `truss-0.4.4.dev3/truss/templates/pipeline/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/pytorch/model/model.py` & `truss-0.4.4.dev3/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/server/common/logging.py` & `truss-0.4.4.dev3/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/server/common/serialization.py` & `truss-0.4.4.dev3/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/server/common/truss_server.py` & `truss-0.4.4.dev3/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/server/inference_server.py` & `truss-0.4.4.dev3/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/server/model_wrapper.py` & `truss-0.4.4.dev3/truss/templates/server/model_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import importlib
 import inspect
 import logging
 import sys
+import time
 import traceback
 from enum import Enum
 from pathlib import Path
 from threading import Lock, Thread
 from typing import Dict, Optional, Union
 
 import kserve
 from cloudevents.http import CloudEvent
+from common.external_data_resolver import download_external_data  # noqa: E402
 from kserve.grpc.grpc_predict_v2_pb2 import ModelInferRequest, ModelInferResponse
 from shared.secrets_resolver import SecretsResolver
 
 MODEL_BASENAME = "model"
 
 
 class ModelWrapper(kserve.Model):
@@ -45,19 +47,21 @@
             return False
 
         self._status = ModelWrapper.Status.LOADING
 
         self.logger.info("Executing model.load()...")
 
         try:
+            start_time = time.perf_counter()
             self.try_load()
             self.ready = True
             self._status = ModelWrapper.Status.READY
-
-            self.logger.info("Completed model.load() execution")
+            self.logger.info(
+                f"Completed model.load() execution in {_elapsed_ms(start_time)} ms"
+            )
 
             return self.ready
         except Exception:
             self.logger.exception("Exception while loading model")
             self._status = ModelWrapper.Status.FAILED
         finally:
             self._load_lock.release()
@@ -77,14 +81,18 @@
         return (
             not self._load_lock.locked()
             and not self._status == ModelWrapper.Status.FAILED
             and not self.ready
         )
 
     def try_load(self):
+        data_dir = Path("data")
+        data_dir.mkdir(exist_ok=True)
+        download_external_data(data_dir, self._config)
+
         if "bundled_packages_dir" in self._config:
             bundled_packages_path = Path("/packages")
             if bundled_packages_path.exists():
                 sys.path.append(str(bundled_packages_path))
         model_module_name = str(
             Path(self._config["model_class_filename"]).with_suffix("")
         )
@@ -93,15 +101,15 @@
         )
         model_class = getattr(module, self._config["model_class_name"])
         model_class_signature = inspect.signature(model_class)
         model_init_params = {}
         if _signature_accepts_keyword_arg(model_class_signature, "config"):
             model_init_params["config"] = self._config
         if _signature_accepts_keyword_arg(model_class_signature, "data_dir"):
-            model_init_params["data_dir"] = Path("data")
+            model_init_params["data_dir"] = data_dir
         if _signature_accepts_keyword_arg(model_class_signature, "secrets"):
             model_init_params["secrets"] = SecretsResolver.get_secrets(self._config)
         self._model = model_class(**model_init_params)
 
         if hasattr(self._model, "load"):
             self._model.load()
 
@@ -145,7 +153,11 @@
 
 
 def _signature_accepts_kwargs(signature: inspect.Signature) -> bool:
     for param in signature.parameters.values():
         if param.kind == inspect.Parameter.VAR_KEYWORD:
             return True
     return False
+
+
+def _elapsed_ms(since_micro_seconds: float) -> int:
+    return int((time.perf_counter() - since_micro_seconds) * 1000)
```

### Comparing `truss-0.4.3/truss/templates/shared/secrets_resolver.py` & `truss-0.4.4.dev3/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/sklearn/model/model.py` & `truss-0.4.4.dev3/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/training/job.py` & `truss-0.4.4.dev3/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/templates/xgboost/model/model.py` & `truss-0.4.4.dev3/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/auto-mpg.data` & `truss-0.4.4.dev3/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/happy.ipynb` & `truss-0.4.4.dev3/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.4.dev3/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.4.dev3/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/readme_int_example.md` & `truss-0.4.4.dev3/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/readme_no_example.md` & `truss-0.4.4.dev3/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/readme_str_example.md` & `truss-0.4.4.dev3/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/test_truss/config.yaml` & `truss-0.4.4.dev3/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/test_data/test_truss/model/model.py` & `truss-0.4.4.dev3/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/conftest.py` & `truss-0.4.4.dev3/truss/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -268,33 +268,35 @@
     def train(self):
         with (self.output_dir / 'variables.json').open('w') as fp:
             fp.write(json.dumps(self.variables))
 
 """
 
 
+EXTERNAL_DATA_ACCESS = """
+class Model:
+    def __init__(self, data_dir):
+        self._data_dir = data_dir
+        pass
+
+    def predict(self, model_input):
+        with (self._data_dir / 'test.txt').open() as file:
+            return file.read()
+"""
+
+
 @pytest.fixture
 def pytorch_model(tmp_path):
-    return _pytorch_model_from_content(
-        tmp_path,
-        PYTORCH_MODEL_FILE_CONTENTS,
-        model_module_name="my_model",
-        model_class_name="MyModel",
-        model_filename="my_model.py",
-    )
+    return _pytorch_model_from_content(tmp_path, PYTORCH_MODEL_FILE_CONTENTS)
 
 
 @pytest.fixture
 def pytorch_model_with_numpy_import(tmp_path):
     return _pytorch_model_from_content(
-        tmp_path,
-        PYTORCH_MODEL_FILE_WITH_NUMPY_IMPORT_CONTENTS,
-        model_module_name="my_model",
-        model_class_name="MyModel",
-        model_filename="my_model.py",
+        tmp_path, PYTORCH_MODEL_FILE_WITH_NUMPY_IMPORT_CONTENTS
     )
 
 
 @pytest.fixture
 def pytorch_model_init_args():
     return {"arg1": 1, "arg2": 2, "kwarg1": 3, "kwarg2": 4}
 
@@ -343,14 +345,45 @@
         "control_truss",
         CUSTOM_MODEL_CODE,
         handle_ops=lambda handle: handle.live_reload(),
     )
 
 
 @pytest.fixture
+def custom_model_external_data_access_tuple_fixture(tmp_path: Path):
+    content = "test"
+    filename = "test.txt"
+    (tmp_path / filename).write_text(content)
+    port = 9089
+    proc = subprocess.Popen(
+        ["python", "-m", "http.server", str(port), "--bind", "0.0.0.0"],
+        cwd=tmp_path,
+    )
+    try:
+        url = f"http://host.docker.internal:{port}/{filename}"
+        # Add arbitrary get params to get that they don't cause issues, the
+        # server above ignores them.
+        # url_with_get_params = f"{url}?foo=bar&baz=bla"
+        url_with_get_params = f"{url}?foo=bar&baz=bla"
+        yield (
+            _custom_model_from_code(
+                tmp_path,
+                "external_data_access",
+                EXTERNAL_DATA_ACCESS,
+                handle_ops=lambda handle: handle.add_external_data_item(
+                    url=url_with_get_params, local_data_path="test.txt"
+                ),
+            ),
+            content,
+        )
+    finally:
+        proc.kill()
+
+
+@pytest.fixture
 def custom_model_with_external_package(tmp_path: Path):
     ext_pkg_path = tmp_path / "ext_pkg"
     ext_pkg_path.mkdir()
     (ext_pkg_path / "subdir").mkdir()
     (ext_pkg_path / "subdir" / "sub_module.py").touch()
     (ext_pkg_path / "top_module.py").touch()
     ext_pkg_path2 = tmp_path / "ext_pkg2"
@@ -552,16 +585,17 @@
     return tokenizer
 
 
 @pytest.fixture
 def custom_model_truss_dir_with_pre_and_post_no_example(tmp_path):
     dir_path = tmp_path / "custom_truss_with_pre_post_no_example"
     handle = init(str(dir_path))
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS)
+    handle.spec.model_class_filepath.write_text(
+        CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS
+    )
     yield dir_path
 
 
 @pytest.fixture
 def huggingface_truss_handle_small_model(
     tmp_path: Path,
     huggingface_transformer_t5_small_pipeline,
@@ -572,48 +606,48 @@
     return dir_path
 
 
 @pytest.fixture
 def custom_model_truss_dir_with_pre_and_post(tmp_path):
     dir_path = tmp_path / "custom_truss_with_pre_post"
     handle = init(str(dir_path))
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS)
+    handle.spec.model_class_filepath.write_text(
+        CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS
+    )
     handle.update_examples([Example("example1", {"inputs": [[0]]})])
     yield dir_path
 
 
 @pytest.fixture
 def variables_to_artifacts_training_truss(tmp_path):
     dir_path = tmp_path / "training_truss"
     handle = init(str(dir_path), trainable=True)
-    with handle.spec.train_class_filepath.open("w") as file:
-        file.write(VARIABLES_TO_ARTIFACTS_TRAIN_CLASS_CODE)
+    handle.spec.train_class_filepath.write_text(VARIABLES_TO_ARTIFACTS_TRAIN_CLASS_CODE)
     yield dir_path
 
 
 @pytest.fixture
 def custom_model_truss_dir_with_bundled_packages(tmp_path):
     truss_dir_path: Path = tmp_path / "custom_model_truss_dir_with_bundled_packages"
     handle = init(str(truss_dir_path))
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_USING_BUNDLED_PACKAGE)
+    handle.spec.model_class_filepath.write_text(CUSTOM_MODEL_CODE_USING_BUNDLED_PACKAGE)
     packages_path = truss_dir_path / DEFAULT_BUNDLED_PACKAGES_DIR / "test_package"
     packages_path.mkdir(parents=True)
     with (packages_path / "test.py").open("w") as file:
         file.write("""X = 1""")
     yield truss_dir_path
 
 
 @pytest.fixture
 def custom_model_truss_dir_with_pre_and_post_str_example(tmp_path):
     dir_path = tmp_path / "custom_truss_with_pre_post_str_example"
     handle = init(str(dir_path))
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS)
+    handle.spec.model_class_filepath.write_text(
+        CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS
+    )
     handle.update_examples(
         [
             Example(
                 "example1",
                 {
                     "inputs": [
                         {
@@ -627,37 +661,36 @@
     yield dir_path
 
 
 @pytest.fixture
 def custom_model_truss_dir_with_pre_and_post_description(tmp_path):
     dir_path = tmp_path / "custom_truss_with_pre_post"
     handle = init(str(dir_path))
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS)
+    handle.spec.model_class_filepath.write_text(
+        CUSTOM_MODEL_CODE_WITH_PRE_AND_POST_PROCESS
+    )
     handle.update_description("This model adds 3 to all inputs")
     yield dir_path
 
 
 @pytest.fixture
 def custom_model_truss_dir_for_gpu(tmp_path):
     dir_path = tmp_path / "custom_truss"
     handle = init(str(dir_path))
     handle.enable_gpu()
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_FOR_GPU_TESTING)
+    handle.spec.model_class_filepath.write_text(CUSTOM_MODEL_CODE_FOR_GPU_TESTING)
     yield dir_path
 
 
 @pytest.fixture
 def custom_model_truss_dir_for_secrets(tmp_path):
     dir_path = tmp_path / "custom_truss"
     handle = init(str(dir_path))
     handle.add_secret("secret_name", "default_secret_value")
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(CUSTOM_MODEL_CODE_FOR_SECRETS_TESTING)
+    handle.spec.model_class_filepath.write_text(CUSTOM_MODEL_CODE_FOR_SECRETS_TESTING)
     yield dir_path
 
 
 @pytest.fixture
 def truss_container_fs(tmp_path):
     ROOT = str(Path(__file__).parent.parent.parent.resolve())
     subprocess.run(["truss", "run-image", "truss/test_data/test_truss"], cwd=ROOT)
@@ -714,17 +747,17 @@
     yield port
     proc.terminate()
 
 
 def _pytorch_model_from_content(
     path: Path,
     content: str,
-    model_module_name: str,
-    model_class_name: str,
-    model_filename: str,
+    model_module_name: str = "my_model",
+    model_class_name: str = "MyModel",
+    model_filename: str = "my_model.py",
 ):
     f = path / model_filename
     f.write_text(content)
 
     sys.path.append(str(path))
     model_class = getattr(importlib.import_module(model_module_name), model_class_name)
     return model_class(), f
@@ -736,10 +769,9 @@
     model_code: str,
     handle_ops: callable = None,
 ) -> Path:
     dir_path = where_dir / truss_name
     handle = init(str(dir_path))
     if handle_ops is not None:
         handle_ops(handle)
-    with handle.spec.model_class_filepath.open("w") as file:
-        file.write(model_code)
+    handle.spec.model_class_filepath.write_text(model_code)
     return dir_path
```

### Comparing `truss-0.4.3/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.4.dev3/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/local/test_local_config_handler.py` & `truss-0.4.4.dev3/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.4.dev3/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/patch/test_calc_patch.py` & `truss-0.4.4.dev3/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/patch/test_hash.py` & `truss-0.4.4.dev3/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/samples.py` & `truss-0.4.4.dev3/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/templates/control/control/test_server.py` & `truss-0.4.4.dev3/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.4.dev3/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.4.dev3/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_backward.py` & `truss-0.4.4.dev3/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_build.py` & `truss-0.4.4.dev3/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_config.py` & `truss-0.4.4.dev3/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_context_builder_image.py` & `truss-0.4.4.dev3/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_docker.py` & `truss-0.4.4.dev3/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_model_inference.py` & `truss-0.4.4.dev3/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_notebooks.py` & `truss-0.4.4.dev3/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.4.dev3/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_truss_gatherer.py` & `truss-0.4.4.dev3/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/tests/test_truss_handle.py` & `truss-0.4.4.dev3/truss/tests/test_truss_handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -848,14 +848,24 @@
         TrussHandle, "_try_patch", new=return_container_dne
     ), pytest.raises(ContainerNotFoundError):
         truss_handle = TrussHandle(truss_dir=custom_model_truss_dir)
         truss_handle.docker_predict([1], local_port=3000)
     kill_all_with_retries()
 
 
+@pytest.mark.integration
+def test_external_data(custom_model_external_data_access_tuple_fixture):
+    truss_dir, expected_content = custom_model_external_data_access_tuple_fixture
+    th = TrussHandle(truss_dir)
+    tag = "test-external-data-access-tag:0.0.1"
+    with ensure_kill_all():
+        result = th.docker_predict([], tag=tag)
+        assert result == expected_content
+
+
 def _container_exists(container) -> bool:
     for row in Docker.client().ps():
         if row.id.startswith(container.id):
             return True
     return False
```

### Comparing `truss-0.4.3/truss/tests/test_validation.py` & `truss-0.4.4.dev3/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/truss_gatherer.py` & `truss-0.4.4.dev3/truss/truss_gatherer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import yaml
 from truss.local.local_config_handler import LocalConfigHandler
 from truss.patch.hash import str_hash_str
 from truss.truss_handle import TrussHandle
-from truss.utils import copy_file_path, copy_tree_path, remove_tree_path
+from truss.util.path import copy_file_path, copy_tree_path, remove_tree_path
 
 
 def gather(truss_path: Path) -> Path:
     handle = TrussHandle(truss_path)
     shadow_truss_dir_name = _calc_shadow_truss_dirname(truss_path)
     shadow_truss_metdata_file_path = (
         LocalConfigHandler.shadow_trusses_dir_path()
```

### Comparing `truss-0.4.3/truss/truss_handle.py` & `truss-0.4.4.dev3/truss/truss_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 from truss.patch.signature import calc_truss_signature
 from truss.patch.types import TrussSignature
 from truss.readme_generator import generate_readme
 from truss.templates.server.common.serialization import (
     truss_msgpack_deserialize,
     truss_msgpack_serialize,
 )
-from truss.truss_config import TrussConfig
+from truss.truss_config import ExternalData, ExternalDataItem, TrussConfig
 from truss.truss_spec import TrussSpec
 from truss.types import Example, PatchDetails
-from truss.utils import copy_file_path, copy_tree_path, get_max_modified_time_of_dir
+from truss.util.path import copy_file_path, copy_tree_path, get_max_modified_time_of_dir
 from truss.validation import validate_secret_name
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 if is_notebook_or_ipython():
     logger.setLevel(logging.INFO)
     logger.addHandler(logging.StreamHandler(sys.stdout))
@@ -457,14 +457,50 @@
                         **conf.train.variables,
                         var_name: default_var_value,
                     },
                 ),
             )
         )
 
+    def add_external_data_item(
+        self,
+        url: str,
+        local_data_path: str,
+        backend: Optional[str] = None,
+        name: Optional[str] = None,
+    ):
+        # todo: write tests for this
+        item = ExternalDataItem(url=url, local_data_path=local_data_path)
+        if backend is not None:
+            item = replace(item, backend=backend)
+        if name is not None:
+            item = replace(item, name=name)
+
+        current_external_data: ExternalData = (
+            self._spec.config.external_data or ExternalData([])
+        )
+        new_external_data = replace(
+            current_external_data,
+            items=current_external_data.items + [item],
+        )
+        self._update_config(
+            lambda conf: replace(
+                conf,
+                external_data=new_external_data,
+            )
+        )
+
+    def remove_all_external_data(self):
+        self._update_config(
+            lambda conf: replace(
+                conf,
+                external_data=None,
+            )
+        )
+
     def update_requirements(self, requirements: List[str]):
         """Update requirements in truss model's config.
 
         Replaces requirements in truss model's config with the provided list.
         """
         self._update_config(lambda conf: replace(conf, requirements=requirements))
```

### Comparing `truss-0.4.3/truss/truss_spec.py` & `truss-0.4.4.dev3/truss/truss_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import yaml
 from truss.constants import CONFIG_FILE
 from truss.errors import ValidationError
-from truss.truss_config import TrussConfig
+from truss.truss_config import ExternalData, TrussConfig
 from truss.types import Example, ModelFrameworkType
 
 
 class TrussSpec:
     """
     Helper class for easy access to information in a Truss.
     """
@@ -27,14 +27,18 @@
         return self._truss_dir / CONFIG_FILE
 
     @property
     def data_dir(self) -> Path:
         return self._truss_dir / self._config.data_dir
 
     @property
+    def external_data(self) -> Optional[ExternalData]:
+        return self._config.external_data
+
+    @property
     def model_module_dir(self) -> Path:
         return self._truss_dir / self._config.model_module_dir
 
     @property
     def training_module_dir(self) -> Path:
         return self._truss_dir / self._config.train.training_module_dir
```

### Comparing `truss-0.4.3/truss/types.py` & `truss-0.4.4.dev3/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/truss/utils.py` & `truss-0.4.4.dev3/truss/util/path.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import os
 import random
 import string
-import subprocess as sp
 import tempfile
 from contextlib import contextmanager
 from distutils.dir_util import copy_tree, remove_tree
 from distutils.file_util import copy_file
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 
 def copy_tree_path(src: Path, dest: Path) -> List[str]:
     return copy_tree(str(src), str(dest))
 
 
 def copy_file_path(src: Path, dest: Path) -> Tuple[str, str]:
     return copy_file(str(src), str(dest))
 
 
+def copy_tree_or_file(src: Path, dest: Path) -> Union[List[str], Tuple[str, str]]:
+    if src.is_file():
+        return copy_file_path(src, dest)
+
+    return copy_tree_path(src, dest)
+
+
 def remove_tree_path(target: Path) -> None:
     return remove_tree(str(target))
 
 
 def get_max_modified_time_of_dir(path: Path) -> float:
     max_modified_time = os.path.getmtime(path)
     for root, dirs, files in os.walk(path):
@@ -50,20 +56,7 @@
     """Builds a directory under ~/.truss/models for the purpose of creating a Truss at."""
     rand_suffix = "".join(random.choices(string.ascii_uppercase + string.digits, k=6))
     target_directory_path = Path(
         Path.home(), ".truss", "models", f"{stub}-{rand_suffix}"
     )
     target_directory_path.mkdir(parents=True)
     return target_directory_path
-
-
-def get_gpu_memory() -> Optional[int]:
-    # https://stackoverflow.com/questions/59567226/how-to-programmatically-determine-available-gpu-memory-with-tensorflow
-    try:
-        command = "nvidia-smi --query-gpu=memory.used --format=csv"
-        memory_free_info = (
-            sp.check_output(command.split()).decode("ascii").split("\n")[1]
-        )
-        memory_free_values = int(memory_free_info.split()[0])
-        return memory_free_values
-    except FileNotFoundError:
-        return None
```

### Comparing `truss-0.4.3/truss/validation.py` & `truss-0.4.4.dev3/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.3/PKG-INFO` & `truss-0.4.4.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.3
+Version: 0.4.4.dev3
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.11
```

