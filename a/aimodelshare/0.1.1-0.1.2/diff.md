# Comparing `tmp/aimodelshare-0.1.1.tar.gz` & `tmp/aimodelshare-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimodelshare-0.1.1.tar", last modified: Tue Apr  4 21:01:12 2023, max compression
+gzip compressed data, was "aimodelshare-0.1.2.tar", last modified: Fri Apr 21 19:57:35 2023, max compression
```

## Comparing `aimodelshare-0.1.1.tar` & `aimodelshare-0.1.2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.721462 aimodelshare-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2501 2023-04-04 21:01:12.721462 aimodelshare-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1940 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.699462 aimodelshare-0.1.1/aimodelshare/
--rw-r--r--   0 root         (0) root         (0)     2014 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/README.md
--rw-r--r--   0 root         (0) root         (0)      539 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68709 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/aimsonnx.py
--rw-r--r--   0 root         (0) root         (0)    34889 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/api.py
--rw-r--r--   0 root         (0) root         (0)    15188 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/aws.py
--rw-r--r--   0 root         (0) root         (0)     6784 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/aws_client.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/base_image.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/bucketpolicy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.701462 aimodelshare-0.1.1/aimodelshare/color_mappings/
--rw-r--r--   0 root         (0) root         (0)     2728 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/color_mappings/color_mapping_keras.csv
--rw-r--r--   0 root         (0) root         (0)     1960 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/color_mappings/color_mapping_pytorch.csv
--rw-r--r--   0 root         (0) root         (0)     8758 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/containerisation.py
--rw-r--r--   0 root         (0) root         (0)    29609 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/containerization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.702462 aimodelshare-0.1.1/aimodelshare/containerization_templates/
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/containerization_templates/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/containerization_templates/Dockerfile_PySpark.txt
--rw-r--r--   0 root         (0) root         (0)      532 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/containerization_templates/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/containerization_templates/lambda_function.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.702462 aimodelshare-0.1.1/aimodelshare/custom_approach/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/custom_approach/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/custom_approach/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/custom_eval_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.703462 aimodelshare-0.1.1/aimodelshare/data_sharing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.704462 aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)     3855 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)    22799 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/download_data.py
--rw-r--r--   0 root         (0) root         (0)    13964 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/share_data.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/data_sharing/utils.py
--rw-r--r--   0 root         (0) root         (0)    11045 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/deploy_custom_lambda.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.704462 aimodelshare-0.1.1/aimodelshare/documentation/
--rw-r--r--   0 root         (0) root         (0)      638 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.705462 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/
--rw-r--r--   0 root         (0) root         (0)      797 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/_version.py
--rw-r--r--   0 root         (0) root         (0)     3099 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     6192 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     1529 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.691462 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.706462 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css.map
--rw-r--r--   0 root         (0) root         (0)    43005 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)   133076 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map
--rw-r--r--   0 root         (0) root         (0)    35271 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css
--rw-r--r--   0 root         (0) root         (0)   161215 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.707462 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/
--rw-r--r--   0 root         (0) root         (0)     8468 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot
--rw-r--r--   0 root         (0) root         (0)     5922 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg
--rw-r--r--   0 root         (0) root         (0)     8300 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf
--rw-r--r--   0 root         (0) root         (0)     5168 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff
--rw-r--r--   0 root         (0) root         (0)     4344 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.707462 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     1948 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js
--rwxr-xr-x   0 root         (0) root         (0)      146 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)      804 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/make.bat
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.709462 aimodelshare-0.1.1/aimodelshare/documentation/source/
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/about.rst
--rw-r--r--   0 root         (0) root         (0)     5598 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/advanced_features.rst
--rw-r--r--   0 root         (0) root         (0)     8528 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/competition.rst
--rw-r--r--   0 root         (0) root         (0)     2028 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/create_credentials.rst
--rw-r--r--   0 root         (0) root         (0)     8854 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/example_notebooks.rst
--rw-r--r--   0 root         (0) root         (0)     4727 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/functions.rst
--rw-r--r--   0 root         (0) root         (0)    14863 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/gettingstarted.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.710462 aimodelshare-0.1.1/aimodelshare/documentation/source/images/
--rw-r--r--   0 root         (0) root         (0)    15684 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds1.png
--rw-r--r--   0 root         (0) root         (0)    80398 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds2.png
--rw-r--r--   0 root         (0) root         (0)   201488 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds3.png
--rw-r--r--   0 root         (0) root         (0)   208089 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds4.png
--rw-r--r--   0 root         (0) root         (0)   123164 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds5.png
--rw-r--r--   0 root         (0) root         (0)    45191 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds_file_example.png
--rw-r--r--   0 root         (0) root         (0)    95857 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/images/predict_tab.png
--rw-r--r--   0 root         (0) root         (0)     2452 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/index.rst
--rw-r--r--   0 root         (0) root         (0)     6712 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/documentation/source/modelplayground.rst
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    59901 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/generatemodelapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.711462 aimodelshare-0.1.1/aimodelshare/iam/
--rw-r--r--   0 root         (0) root         (0)     3855 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/iam/codebuild_policy.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/iam/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/iam/lambda_policy.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/iam/lambda_trust_relationship.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.713462 aimodelshare-0.1.1/aimodelshare/json_templates/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/api_json.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.713462 aimodelshare-0.1.1/aimodelshare/json_templates/auth/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/auth/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/auth/role.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.713462 aimodelshare-0.1.1/aimodelshare/json_templates/eval/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/eval/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/eval/role.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.713462 aimodelshare-0.1.1/aimodelshare/json_templates/function/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/function/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/function/role.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/integration_response.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/lambda_policy_1.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/lambda_policy_2.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/lambda_role_1.txt
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/json_templates/lambda_role_2.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/leaderboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.716462 aimodelshare-0.1.1/aimodelshare/main/
--rw-r--r--   0 root         (0) root         (0)     4146 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/1.txt
--rw-r--r--   0 root         (0) root         (0)     3616 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/1B.txt
--rw-r--r--   0 root         (0) root         (0)     4609 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/2.txt
--rw-r--r--   0 root         (0) root         (0)     4110 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/3.txt
--rw-r--r--   0 root         (0) root         (0)     4260 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/4.txt
--rw-r--r--   0 root         (0) root         (0)     3522 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/5.txt
--rw-r--r--   0 root         (0) root         (0)     3518 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/6.txt
--rw-r--r--   0 root         (0) root         (0)     4377 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/7.txt
--rw-r--r--   0 root         (0) root         (0)     4513 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/8.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10942 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/authorization.txt
--rw-r--r--   0 root         (0) root         (0)     3081 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/eval_classification.txt
--rw-r--r--   0 root         (0) root         (0)    59775 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/eval_lambda.txt
--rw-r--r--   0 root         (0) root         (0)     3111 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/eval_regression.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/lambda_function.txt
--rw-r--r--   0 root         (0) root         (0)     4941 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/main/nst.txt
--rw-r--r--   0 root         (0) root         (0)    49899 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/model.py
--rw-r--r--   0 root         (0) root         (0)     4311 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/modeluser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.717462 aimodelshare-0.1.1/aimodelshare/placeholders/
--rw-r--r--   0 root         (0) root         (0)     3464 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/placeholders/model.onnx
--rw-r--r--   0 root         (0) root         (0)     2930 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/placeholders/preprocessor.zip
--rw-r--r--   0 root         (0) root         (0)    89026 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/playground.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/postprocessormodules.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/preprocessormodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.719462 aimodelshare-0.1.1/aimodelshare/pyspark/
--rw-r--r--   0 root         (0) root         (0)     6529 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/1.txt
--rw-r--r--   0 root         (0) root         (0)     6078 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/1B.txt
--rw-r--r--   0 root         (0) root         (0)     7055 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/2.txt
--rw-r--r--   0 root         (0) root         (0)     6596 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/3.txt
--rw-r--r--   0 root         (0) root         (0)     6377 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/4.txt
--rw-r--r--   0 root         (0) root         (0)     5988 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/5.txt
--rw-r--r--   0 root         (0) root         (0)     5980 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/6.txt
--rw-r--r--   0 root         (0) root         (0)     6819 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/7.txt
--rw-r--r--   0 root         (0) root         (0)     6906 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/8.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10589 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/authorization.txt
--rw-r--r--   0 root         (0) root         (0)     3081 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/eval_classification.txt
--rw-r--r--   0 root         (0) root         (0)    51474 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/eval_lambda.txt
--rw-r--r--   0 root         (0) root         (0)     3111 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/eval_regression.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/lambda_function.txt
--rw-r--r--   0 root         (0) root         (0)     7110 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/pyspark/nst.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.719462 aimodelshare-0.1.1/aimodelshare/python/
--rw-r--r--   0 root         (0) root         (0)     1949 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/python/my_preprocessor.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/readme.md
--rw-r--r--   0 root         (0) root         (0)     5793 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/reproducibility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.720462 aimodelshare-0.1.1/aimodelshare/sam/
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/Dockerfile_PySpark.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      625 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)     3855 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/codebuild_policies.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)     5181 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/codepipeline_policies.txt
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/codepipeline_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/spark-class.txt
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/sam/template.txt
--rw-r--r--   0 root         (0) root         (0)     3109 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/tools.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/aimodelshare/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.700462 aimodelshare-0.1.1/aimodelshare.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2501 2023-04-04 21:01:12.000000 aimodelshare-0.1.1/aimodelshare.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6377 2023-04-04 21:01:12.000000 aimodelshare-0.1.1/aimodelshare.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 21:01:12.000000 aimodelshare-0.1.1/aimodelshare.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      417 2023-04-04 21:01:12.000000 aimodelshare-0.1.1/aimodelshare.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-04 21:01:12.000000 aimodelshare-0.1.1/aimodelshare.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 21:01:12.721462 aimodelshare-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1334 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 21:01:12.721462 aimodelshare-0.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/tests/test_aimsonnx.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-04-04 21:01:04.000000 aimodelshare-0.1.1/tests/test_playground.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.159217 aimodelshare-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-04-21 19:57:35.159217 aimodelshare-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.136215 aimodelshare-0.1.2/aimodelshare/
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/README.md
+-rw-r--r--   0 root         (0) root         (0)      539 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68708 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/aimsonnx.py
+-rw-r--r--   0 root         (0) root         (0)    34889 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/api.py
+-rw-r--r--   0 root         (0) root         (0)    15188 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6784 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/aws_client.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/base_image.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/bucketpolicy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.137215 aimodelshare-0.1.2/aimodelshare/color_mappings/
+-rw-r--r--   0 root         (0) root         (0)     2728 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/color_mappings/color_mapping_keras.csv
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/color_mappings/color_mapping_pytorch.csv
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/containerisation.py
+-rw-r--r--   0 root         (0) root         (0)    29609 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/containerization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.137215 aimodelshare-0.1.2/aimodelshare/containerization_templates/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/containerization_templates/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/containerization_templates/Dockerfile_PySpark.txt
+-rw-r--r--   0 root         (0) root         (0)      532 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/containerization_templates/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/containerization_templates/lambda_function.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.138215 aimodelshare-0.1.2/aimodelshare/custom_approach/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/custom_approach/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/custom_approach/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/custom_eval_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.138215 aimodelshare-0.1.2/aimodelshare/data_sharing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.139216 aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)    22799 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/download_data.py
+-rw-r--r--   0 root         (0) root         (0)    13964 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/share_data.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/data_sharing/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11045 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/deploy_custom_lambda.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.139216 aimodelshare-0.1.2/aimodelshare/documentation/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.140216 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/layout.html
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/search.html
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.129215 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.142216 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css.map
+-rw-r--r--   0 root         (0) root         (0)    43005 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)   133076 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map
+-rw-r--r--   0 root         (0) root         (0)    35271 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css
+-rw-r--r--   0 root         (0) root         (0)   161215 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.143216 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg
+-rw-r--r--   0 root         (0) root         (0)     8300 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf
+-rw-r--r--   0 root         (0) root         (0)     5168 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.143216 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/js/
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js
+-rwxr-xr-x   0 root         (0) root         (0)      146 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/theme.conf
+-rw-r--r--   0 root         (0) root         (0)      804 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/make.bat
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.145216 aimodelshare-0.1.2/aimodelshare/documentation/source/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/about.rst
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/advanced_features.rst
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/competition.rst
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/create_credentials.rst
+-rw-r--r--   0 root         (0) root         (0)     8854 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/example_notebooks.rst
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/functions.rst
+-rw-r--r--   0 root         (0) root         (0)    14863 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/gettingstarted.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.148216 aimodelshare-0.1.2/aimodelshare/documentation/source/images/
+-rw-r--r--   0 root         (0) root         (0)    15684 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds1.png
+-rw-r--r--   0 root         (0) root         (0)    80398 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds2.png
+-rw-r--r--   0 root         (0) root         (0)   201488 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds3.png
+-rw-r--r--   0 root         (0) root         (0)   208089 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds4.png
+-rw-r--r--   0 root         (0) root         (0)   123164 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds5.png
+-rw-r--r--   0 root         (0) root         (0)    45191 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds_file_example.png
+-rw-r--r--   0 root         (0) root         (0)    95857 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/images/predict_tab.png
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/documentation/source/modelplayground.rst
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    59901 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/generatemodelapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.149217 aimodelshare-0.1.2/aimodelshare/iam/
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/iam/codebuild_policy.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/iam/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/iam/lambda_policy.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/iam/lambda_trust_relationship.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.150216 aimodelshare-0.1.2/aimodelshare/json_templates/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/api_json.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.151217 aimodelshare-0.1.2/aimodelshare/json_templates/auth/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/auth/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/auth/role.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.151217 aimodelshare-0.1.2/aimodelshare/json_templates/eval/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/eval/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/eval/role.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.151217 aimodelshare-0.1.2/aimodelshare/json_templates/function/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/function/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/function/role.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/integration_response.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/lambda_policy_1.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/lambda_policy_2.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/lambda_role_1.txt
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/json_templates/lambda_role_2.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/leaderboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.154217 aimodelshare-0.1.2/aimodelshare/main/
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/1.txt
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/1B.txt
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/2.txt
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/3.txt
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/4.txt
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/5.txt
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/6.txt
+-rw-r--r--   0 root         (0) root         (0)     4377 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/7.txt
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/8.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10942 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/authorization.txt
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/eval_classification.txt
+-rw-r--r--   0 root         (0) root         (0)    59775 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/eval_lambda.txt
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/eval_regression.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/lambda_function.txt
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/main/nst.txt
+-rw-r--r--   0 root         (0) root         (0)    49899 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/model.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/modeluser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.154217 aimodelshare-0.1.2/aimodelshare/placeholders/
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/placeholders/model.onnx
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/placeholders/preprocessor.zip
+-rw-r--r--   0 root         (0) root         (0)    88269 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/playground.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/postprocessormodules.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/preprocessormodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.157217 aimodelshare-0.1.2/aimodelshare/pyspark/
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/1.txt
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/1B.txt
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/2.txt
+-rw-r--r--   0 root         (0) root         (0)     6596 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/3.txt
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/4.txt
+-rw-r--r--   0 root         (0) root         (0)     5988 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/5.txt
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/6.txt
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/7.txt
+-rw-r--r--   0 root         (0) root         (0)     6906 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/8.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10589 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/authorization.txt
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/eval_classification.txt
+-rw-r--r--   0 root         (0) root         (0)    51474 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/eval_lambda.txt
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/eval_regression.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/lambda_function.txt
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/pyspark/nst.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.157217 aimodelshare-0.1.2/aimodelshare/python/
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/python/my_preprocessor.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/readme.md
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/reproducibility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.158217 aimodelshare-0.1.2/aimodelshare/sam/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/Dockerfile_PySpark.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/codebuild_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/codepipeline_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/codepipeline_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/spark-class.txt
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/sam/template.txt
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/tools.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/aimodelshare/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.136215 aimodelshare-0.1.2/aimodelshare.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-04-21 19:57:34.000000 aimodelshare-0.1.2/aimodelshare.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-04-21 19:57:34.000000 aimodelshare-0.1.2/aimodelshare.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:57:34.000000 aimodelshare-0.1.2/aimodelshare.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-21 19:57:34.000000 aimodelshare-0.1.2/aimodelshare.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-21 19:57:34.000000 aimodelshare-0.1.2/aimodelshare.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 19:57:35.159217 aimodelshare-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:57:35.159217 aimodelshare-0.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/tests/test_aimsonnx.py
+-rw-r--r--   0 root         (0) root         (0)    12210 2023-04-21 19:57:22.000000 aimodelshare-0.1.2/tests/test_playground.py
```

### Comparing `aimodelshare-0.1.1/LICENSE` & `aimodelshare-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/PKG-INFO` & `aimodelshare-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimodelshare
-Version: 0.1.1
+Version: 0.1.2
 Summary: Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org
 Home-page: https://www.modelshare.org
 Author: Michael Parrott
 Author-email: mikedparrott@modelshare.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimodelshare-0.1.1/README.md` & `aimodelshare-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/README.md` & `aimodelshare-0.1.2/aimodelshare/README.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/__init__.py` & `aimodelshare-0.1.2/aimodelshare/__init__.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/aimsonnx.py` & `aimodelshare-0.1.2/aimodelshare/aimsonnx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1569,15 +1569,14 @@
 
         for k in models_list: 
             models_modules_dict[k] = 'sklearn.'+i
     
     return models_modules_dict
 
 
-
 def model_from_string(model_type):
     models_modules_dict = _get_sklearn_modules()
     module = models_modules_dict[model_type]
     model_class = getattr(importlib.import_module(module), model_type)
     return model_class
 
 def _get_pyspark_modules():
```

### Comparing `aimodelshare-0.1.1/aimodelshare/api.py` & `aimodelshare-0.1.2/aimodelshare/api.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/aws.py` & `aimodelshare-0.1.2/aimodelshare/aws.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/aws_client.py` & `aimodelshare-0.1.2/aimodelshare/aws_client.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/base_image.py` & `aimodelshare-0.1.2/aimodelshare/base_image.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/bucketpolicy.py` & `aimodelshare-0.1.2/aimodelshare/bucketpolicy.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/color_mappings/color_mapping_keras.csv` & `aimodelshare-0.1.2/aimodelshare/color_mappings/color_mapping_keras.csv`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/color_mappings/color_mapping_pytorch.csv` & `aimodelshare-0.1.2/aimodelshare/color_mappings/color_mapping_pytorch.csv`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/containerisation.py` & `aimodelshare-0.1.2/aimodelshare/containerisation.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/containerization.py` & `aimodelshare-0.1.2/aimodelshare/containerization.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/containerization_templates/Dockerfile_PySpark.txt` & `aimodelshare-0.1.2/aimodelshare/containerization_templates/Dockerfile_PySpark.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/containerization_templates/buildspec.txt` & `aimodelshare-0.1.2/aimodelshare/containerization_templates/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/containerization_templates/lambda_function.txt` & `aimodelshare-0.1.2/aimodelshare/containerization_templates/lambda_function.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/custom_eval_metrics.py` & `aimodelshare-0.1.2/aimodelshare/custom_eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt` & `aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt` & `aimodelshare-0.1.2/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/data_sharing/download_data.py` & `aimodelshare-0.1.2/aimodelshare/data_sharing/download_data.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/data_sharing/share_data.py` & `aimodelshare-0.1.2/aimodelshare/data_sharing/share_data.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/deploy_custom_lambda.py` & `aimodelshare-0.1.2/aimodelshare/deploy_custom_lambda.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/Makefile` & `aimodelshare-0.1.2/aimodelshare/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/__init__.py` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/layout.html` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/search.html` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/searchbox.html` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js` & `aimodelshare-0.1.2/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/make.bat` & `aimodelshare-0.1.2/aimodelshare/documentation/make.bat`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/about.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/about.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/advanced_features.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/advanced_features.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/competition.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/competition.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/conf.py` & `aimodelshare-0.1.2/aimodelshare/documentation/source/conf.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/create_credentials.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/create_credentials.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/example_notebooks.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/example_notebooks.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/functions.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/functions.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/gettingstarted.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds1.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds1.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds2.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds2.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds3.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds3.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds4.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds4.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds5.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds5.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/creds_file_example.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/creds_file_example.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/images/predict_tab.png` & `aimodelshare-0.1.2/aimodelshare/documentation/source/images/predict_tab.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/index.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/index.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/documentation/source/modelplayground.rst` & `aimodelshare-0.1.2/aimodelshare/documentation/source/modelplayground.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/generatemodelapi.py` & `aimodelshare-0.1.2/aimodelshare/generatemodelapi.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/iam/codebuild_policy.txt` & `aimodelshare-0.1.2/aimodelshare/iam/codebuild_policy.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/json_templates/api_json.txt` & `aimodelshare-0.1.2/aimodelshare/json_templates/api_json.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/leaderboard.py` & `aimodelshare-0.1.2/aimodelshare/leaderboard.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/1.txt` & `aimodelshare-0.1.2/aimodelshare/main/1.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/1B.txt` & `aimodelshare-0.1.2/aimodelshare/main/1B.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/2.txt` & `aimodelshare-0.1.2/aimodelshare/main/2.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/3.txt` & `aimodelshare-0.1.2/aimodelshare/main/3.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/4.txt` & `aimodelshare-0.1.2/aimodelshare/main/4.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/5.txt` & `aimodelshare-0.1.2/aimodelshare/main/5.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/6.txt` & `aimodelshare-0.1.2/aimodelshare/main/6.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/7.txt` & `aimodelshare-0.1.2/aimodelshare/main/7.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/8.txt` & `aimodelshare-0.1.2/aimodelshare/main/8.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/authorization.txt` & `aimodelshare-0.1.2/aimodelshare/main/authorization.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/eval_classification.txt` & `aimodelshare-0.1.2/aimodelshare/main/eval_classification.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/eval_lambda.txt` & `aimodelshare-0.1.2/aimodelshare/main/eval_lambda.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/eval_regression.txt` & `aimodelshare-0.1.2/aimodelshare/main/eval_regression.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/main/nst.txt` & `aimodelshare-0.1.2/aimodelshare/main/nst.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/model.py` & `aimodelshare-0.1.2/aimodelshare/model.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/modeluser.py` & `aimodelshare-0.1.2/aimodelshare/modeluser.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/placeholders/model.onnx` & `aimodelshare-0.1.2/aimodelshare/placeholders/model.onnx`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/placeholders/preprocessor.zip` & `aimodelshare-0.1.2/aimodelshare/placeholders/preprocessor.zip`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/playground.py` & `aimodelshare-0.1.2/aimodelshare/playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# import packages 
+# import packages
 import os
 import contextlib
 import boto3
 from aimodelshare.api import get_api_json
 import tempfile
 
 try:
@@ -23,26 +23,26 @@
 
 
 class ModelPlayground:
     """
     Parameters:
     ----------
     `model_type` : ``string``
-          values - [ 'text' , 'image' , 'tabular' , 'video', 'audio','timeseries' ] 
-          type of model data     
+          values - [ 'text' , 'image' , 'tabular' , 'video', 'audio','timeseries' ]
+          type of model data
     `classification`:    ``bool, default=True``
         True [DEFAULT] if model is of Classification type with categorical target variables
         False if model is of Regression type with continuous target variables
     `private` :   ``bool, default = False``
         True if model and its corresponding data is not public
-        False [DEFAULT] if model and its corresponding data is public 
+        False [DEFAULT] if model and its corresponding data is public
     `email_list`: ``list of string values``
                 values - list including all emails of users who have access the private playground.
                 list should contain same emails that were used by users to sign up for modelshare.ai account.
-                [OPTIONAL] set by the playground owner for private playgrounds.  Can also be updated by editing deployed 
+                [OPTIONAL] set by the playground owner for private playgrounds.  Can also be updated by editing deployed
                 playground page at www.modelshare.ai.
     """
 
     def __init__(self, input_type=None, task_type=None, private=None, playground_url=None, email_list=None):
         # confirm correct args are provided
         if playground_url == None and any([input_type == None, task_type == None, private == None]):
             raise ValueError(
@@ -86,52 +86,52 @@
                  onnx_timeout=60, pyspark_support=False, model_input=None, input_dict=None, playground_id=False):
 
         """
         Launches a live model playground to the www.modelshare.ai website. The playground can optionally include a live prediction REST API for deploying ML models using model parameters and user credentials, provided by the user.
         Inputs : 7
         Output : model launched to an API
                 detailed API info printed out
-        Parameters: 
+        Parameters:
         ----------
         `model_filepath` :  ``string`` ends with '.onnx'
-              value - Absolute path to model file 
+              value - Absolute path to model file
               .onnx is the only accepted model file extension
               "example_model.onnx" filename for file in directory.
               "/User/xyz/model/example_model.onnx" absolute path to model file from local directory
               if no value is set the playground will be launched with only a placeholder prediction API.
         `preprocessor_filepath`:  ``string``
-            value - absolute path to preprocessor file 
-            "./preprocessor.zip" 
+            value - absolute path to preprocessor file
+            "./preprocessor.zip"
             searches for an exported zip preprocessor file in the current directory
             file is generated using export_preprocessor function from the AI Modelshare library
             if no value is set the playground will be launched with only a placeholder prediction API.
         `y_train` : training labels for classification models.
             expects pandas dataframe of one hot encoded y train data
-            if no value is set ... #TODO 
-        `example_data`: ``Example of X data that will be shown on the online Playground page. 
+            if no value is set ... #TODO
+        `example_data`: ``Example of X data that will be shown on the online Playground page.
             if no example data is submitted, certain functionalities may be limited, including the deployment of live prediction APIs.
             Example data can be updated at a later stage, using the update_example_data() method.``
         `custom_libraries`: ``string``
             "TRUE" if user wants to load custom Python libraries to their prediction runtime
             "FALSE" if user wishes to use AI Model Share base libraries including latest versions of most common ML libs.
         `reproducibility_env_filepath`: ``TODO``
         `memory`: ``TODO``
         `timeout`: ``TODO``
         `onnx_timeout`: ``int``
             Time in seconds after which ONNX conversion should be interrupted.
             Set to False if you want to force ONNX conversion.
         `pyspark_support`: ``TODO``
         `model_input`: ``array_like``
-            Required only when framework="pytorch" 
+            Required only when framework="pytorch"
             One example of X training data in correct format.
-         
+
         Returns:
         --------
         print_api_info : prints statements with generated model playground page and live prediction API details
-                        also prints steps to update the model submissions by the user/team 
+                        also prints steps to update the model submissions by the user/team
         """
 
         # test whether playground is already active
         if self.playground_url:
             print(self.playground_url)
 
             def ask_user():
@@ -142,15 +142,15 @@
                 return response != "yes"
 
             r = ask_user()
 
             if r:
                 return
 
-        # convert model to onnx 
+        # convert model to onnx
         if onnx_timeout == False:
             force_onnx = True
         else:
             force_onnx = False
         model_filepath = model_to_onnx_timed(model_filepath, timeout=onnx_timeout,
                                              force_onnx=force_onnx, model_input=model_input)
 
@@ -248,53 +248,53 @@
                model_input=None, input_dict=None):
 
         """
         Launches a live prediction REST API for deploying ML models using model parameters and user credentials, provided by the user
         Inputs : 7
         Output : model launched to an API
                 detailed API info printed out
-        Parameters: 
+        Parameters:
         ----------
         `model_filepath` :  ``string`` ends with '.onnx'
-              value - Absolute path to model file 
+              value - Absolute path to model file
               [REQUIRED] to be set by the user
               .onnx is the only accepted model file extension
               "example_model.onnx" filename for file in directory.
               "/User/xyz/model/example_model.onnx" absolute path to model file from local directory
         `preprocessor_filepath`:  ``string``
-            value - absolute path to preprocessor file 
+            value - absolute path to preprocessor file
             [REQUIRED] to be set by the user
-            "./preprocessor.zip" 
+            "./preprocessor.zip"
             searches for an exported zip preprocessor file in the current directory
-            file is generated using export_preprocessor function from the AI Modelshare library  
+            file is generated using export_preprocessor function from the AI Modelshare library
         `y_train` : training labels for classification models.
               [REQUIRED] for classification type models
               expects pandas dataframe of one hot encoded y train data
-        `example_data`: ``Example of X data that will be shown on the online Playground page. 
+        `example_data`: ``Example of X data that will be shown on the online Playground page.
             if no example data is submitted, certain functionalities may be limited, including the deployment of live prediction APIs.
             Example data can be updated at a later stage, using the update_example_data() method.``
         `custom_libraries`:   ``string``
             "TRUE" if user wants to load custom Python libraries to their prediction runtime
             "FALSE" if user wishes to use AI Model Share base libraries including latest versions of most common ML libs.
         `image`: ``TODO``
         `reproducibility_env_filepath`: ``TODO``
         `memory`: ``TODO``
         `timeout`: ``TODO``
         `onnx_timeout`: ``int``
             Time in seconds after which ONNX conversion should be interrupted.
             Set to False if you want to force ONNX conversion.
         `pyspark_support`: ``TODO``
         `model_input`: ``array_like``
-            Required only when framework="pytorch" 
+            Required only when framework="pytorch"
             One example of X training data in correct format.
         `input_dict`:   ``dictionary``
              Use to bypass text input boxes Example: {"model_name": "My Model Playground",
                       "model_description": "My Model Description",
                       "tags": "model, classification, awesome"}
-         
+
         Returns:
         --------
         print_api_info : prints statements with generated live prediction API details
                         also prints steps to update the model submissions by the user/team
         """
 
         # check whether playground url exists
@@ -378,15 +378,15 @@
                                     pyspark_support=pyspark_support,
                                     input_dict=input_dict,
                                     print_output=False):
 
                 def upload_playground_zipfile(model_filepath=None, preprocessor_filepath=None, y_train=None,
                                               example_data=None):
                     """
-                  minimally requires model_filepath, preprocessor_filepath 
+                  minimally requires model_filepath, preprocessor_filepath
                   """
                     import json
                     import os
                     import requests
                     import pandas as pd
                     wkingdir = os.getcwd()
                     if os.path.dirname(model_filepath) == '':
@@ -624,36 +624,36 @@
                public=True, public_private_split=0.5, model_input=None, timeout=None, example_data=None,
                custom_libraries="FALSE", image="", reproducibility_env_filepath=None, memory=None,
                pyspark_support=False,
                user_input=False):
 
         """
         Submits model/preprocessor to machine learning experiment leaderboard and model architecture database using live prediction API url generated by AI Modelshare library
-        The submitted model gets evaluated and compared with all existing models and a leaderboard can be generated 
-        
+        The submitted model gets evaluated and compared with all existing models and a leaderboard can be generated
+
         Parameters:
         -----------
         `eval_data` :  ``list`` of y values used to generate metrics from predicted values from predictions submitted via the submit_model() method
             [REQUIRED] to generate eval metrics in experiment leaderboard
         `y_train` :  ``list`` of y values for training data used to extract the set of class labels
             [REQUIRED] for image classification models
         `eval_metric_filepath`: [OPTIONAL] file path of zip file with custon evaluation functions
-        `data_directory` : folder storing training data and test data (excluding Y test data)                   
+        `data_directory` : folder storing training data and test data (excluding Y test data)
         `email_list`: [OPTIONAL] list of comma separated emails for users who are allowed to submit models to experiment leaderboard.  Emails should be strings in a list.
-        `public`: [REQUIRED] True/false. Defaults to False.  If True, experiment is public and ANY AIMODELSHARE USER CAN SUBMIT MODELS.  USE WITH CAUTION b/c one model and 
+        `public`: [REQUIRED] True/false. Defaults to False.  If True, experiment is public and ANY AIMODELSHARE USER CAN SUBMIT MODELS.  USE WITH CAUTION b/c one model and
             one preprocessor file will be be saved to your AWS S3 folder for each model submission.
         `public_private_split`: [REQUIRED] Float between 0 and 1. Defaults to 0. Porportion of test data that is allocated to private hold-out set.
         `model_input`: ``array_like``
-            Required only when framework="pytorch" 
+            Required only when framework="pytorch"
             One example of X training data in correct format.
         `timeout`: ``TODO``
         `onnx_timeout`: ``int``
             Time in seconds after which ONNX conversion should be interrupted.
             Set to False if you want to force ONNX conversion.
-        `example_data`: ``Example of X data that will be shown on the online Playground page. 
+        `example_data`: ``Example of X data that will be shown on the online Playground page.
             if no example data is submitted, certain functionalities may be limited, including the deployment of live prediction APIs.
             Example data can be updated at a later stage, using the update_example_data() method.``
 
         Returns:
         -------
         response:   Model version if the model is submitted sucessfully
                     error  if there is any error while submitting models
@@ -705,15 +705,15 @@
             self.activate(None, None, example_data=example_data,
                           onnx_timeout=None, y_train=y_train, custom_libraries=custom_libraries,
                           image=image, reproducibility_env_filepath=reproducibility_env_filepath,
                           memory=memory, pyspark_support=pyspark_support, timeout=timeout, input_dict=input_dict,
                           playground_id=playground_id)
             print()
 
-        # if playground is active, ask whether user wants to overwrite 
+        # if playground is active, ask whether user wants to overwrite
         else:
 
             print(
                 "The Model Playground is already active. Do you want to overwrite existing competitions and experiments?")
             response = ''
             while response not in {"yes", "no"}:
                 response = input("Please enter yes or no: ").lower()
@@ -801,31 +801,31 @@
 
     def create_competition(self, data_directory, y_test, eval_metric_filepath=None, email_list=None, public=True,
                            public_private_split=0.5, input_dict=None):
         """
         Creates a model competition for a deployed prediction REST API
         Inputs : 4
         Output : Create ML model competition and allow authorized users to submit models to resulting leaderboard/competition
-        
+
         Parameters:
         -----------
         `y_test` :  ``list`` of y values for test data used to generate metrics from predicted values from X test data submitted via the submit_model() function
             [REQUIRED] to generate eval metrics in competition leaderboard
-                                
+
         `data_directory` : folder storing training data and test data (excluding Y test data)
         `eval_metric_filepath`: [OPTIONAL] file path of zip file with custon evaluation functions
         `email_list`: [OPTIONAL] list of comma separated emails for users who are allowed to submit models to competition.  Emails should be strings in a list.
-        `public`: [REQUIRED] True/false. Defaults to False.  If True, competition is public and ANY AIMODELSHARE USER CAN SUBMIT MODELS.  USE WITH CAUTION b/c one model and 
+        `public`: [REQUIRED] True/false. Defaults to False.  If True, competition is public and ANY AIMODELSHARE USER CAN SUBMIT MODELS.  USE WITH CAUTION b/c one model and
             one preprocessor file will be be saved to your AWS S3 folder for each model submission.
         `public_private_split`: [REQUIRED] Float between 0 and 1. Defaults to 0.5. Porportion of test data that is allocated to private hold-out set.
-        
+
         Returns:
         -----------
         finalmessage : Information such as how to submit models to competition
-        
+
         """
 
         if email_list is None:
             email_list = []
 
         # catch email list error
         if public == False and email_list == []:
@@ -858,15 +858,15 @@
                               "data_description": aishare_datadescription, "data_license": aishare_datalicense}
             else:
                 pass
 
             # model competition files
             def upload_comp_exp_zipfile(data_directory, y_test=None, eval_metric_filepath=None, email_list=[]):
                 """
-                minimally requires model_filepath, preprocessor_filepath 
+                minimally requires model_filepath, preprocessor_filepath
                 """
                 zipfilelist = [data_directory]
 
                 import json
                 import os
                 import requests
                 import pandas as pd
@@ -1002,32 +1002,32 @@
 
     def create_experiment(self, data_directory, y_test, eval_metric_filepath=None, email_list=[], public=False,
                           public_private_split=0, input_dict=None):
         """
         Creates an experiment for a deployed prediction REST API
         Inputs : 4
         Output : Create ML model experiment and allows authorized users to submit models to resulting experiment tracking leaderboard
-        
+
         Parameters:
         -----------
         `y_test` :  ``list`` of y values for test data used to generate metrics from predicted values from X test data submitted via the submit_model() function
             [REQUIRED] to generate eval metrics in experiment leaderboard
-                                
+
         `data_directory` : folder storing training data and test data (excluding Y test data)
         `eval_metric_filepath`: [OPTIONAL] file path of zip file with custon evaluation functions
         `email_list`: [OPTIONAL] list of comma separated emails for users who are allowed to submit models to experiment leaderboard.  Emails should be strings in a list.
-        `public`: [REQUIRED] True/false. Defaults to False.  If True, experiment is public and ANY AIMODELSHARE USER CAN SUBMIT MODELS.  USE WITH CAUTION b/c one model and 
+        `public`: [REQUIRED] True/false. Defaults to False.  If True, experiment is public and ANY AIMODELSHARE USER CAN SUBMIT MODELS.  USE WITH CAUTION b/c one model and
             one preprocessor file will be be saved to your AWS S3 folder for each model submission.
         `public_private_split`: [REQUIRED] Float between 0 and 1. Defaults to 0. Porportion of test data that is allocated to private hold-out set.
-        
-        
+
+
         Returns:
         -----------
         finalmessage : Information such as how to submit models to experiment
-        
+
         """
 
         # catch email list error
         if public == False and email_list == []:
             raise ValueError("Please submit valid email list for private experiment.")
         import os
         if os.environ.get("cloud_location") is not None:
@@ -1057,15 +1057,15 @@
                               "data_description": aishare_datadescription, "data_license": aishare_datalicense}
             else:
                 pass
 
             # model competition files
             def upload_comp_exp_zipfile(data_directory, y_test=None, eval_metric_filepath=None, email_list=[]):
                 """
-                minimally requires model_filepath, preprocessor_filepath 
+                minimally requires model_filepath, preprocessor_filepath
                 """
                 zipfilelist = [data_directory]
 
                 import json
                 import os
                 import requests
                 import pandas as pd
@@ -1197,32 +1197,23 @@
 
     def submit_model(self, model, preprocessor, prediction_submission, submission_type="experiment",
                      sample_data=None, reproducibility_env_filepath=None, custom_metadata=None, input_dict=None,
                      onnx_timeout=60, model_input=None):
         """
         Submits model/preprocessor to machine learning competition using live prediction API url generated by AI Modelshare library
         The submitted model gets evaluated and compared with all existing models and a leaderboard can be generated
-        
+
         Parameters:
         -----------
-        `model_filepath`:  ``string`` ends with '.onnx'
-            value - Absolute path to model file [REQUIRED] to be set by the user
-            .onnx is the only accepted model file extension
-            "example_model.onnx" filename for file in directory.
-            "/User/xyz/model/example_model.onnx" absolute path to model file from local directory
+        `model`:  model object (sklearn, keras, pytorch, onnx) or onnx model file path
         `prediction_submission`:   one hot encoded y_pred
             value - predictions for test data
             [REQUIRED] for evaluation metrics of the submitted model
-        `preprocessor_filepath`:   ``string``, default=None
-            value - absolute path to preprocessor file 
-            [REQUIRED] to be set by the user
-            "./preprocessor.zip" 
-            searches for an exported zip preprocessor file in the current directory
-            file is generated from preprocessor module using export_preprocessor function from the AI Modelshare library 
- 
+        `preprocessor`: preprocessor function object
+
         Returns:
         --------
         response:   Model version if the model is submitted sucessfully
         """
 
         if not self.playground_url:
             raise Exception(
@@ -1244,31 +1235,31 @@
             input_dict["tags"] = input("Insert search tags to help users find your model (optional): ")
             input_dict["description"] = input("Provide any useful notes about your model (optional): ")
 
         if submission_type == "competition" or submission_type == "all":
             with HiddenPrints():
                 competition = Competition(self.playground_url)
 
-                version_comp, model_page = competition.submit_model(model_filepath=model,
+                version_comp, model_page = competition.submit_model(model=model,
                                                                     prediction_submission=prediction_submission,
-                                                                    preprocessor_filepath=preprocessor,
+                                                                    preprocessor=preprocessor,
                                                                     reproducibility_env_filepath=reproducibility_env_filepath,
                                                                     custom_metadata=custom_metadata,
                                                                     input_dict=input_dict,
                                                                     print_output=False)
 
             print(f"Your model has been submitted to competition as model version {version_comp}.")
 
         if submission_type == "experiment" or submission_type == "all":
             with HiddenPrints():
                 experiment = Experiment(self.playground_url)
 
-                version_exp, model_page = experiment.submit_model(model_filepath=model,
+                version_exp, model_page = experiment.submit_model(model=model,
                                                                   prediction_submission=prediction_submission,
-                                                                  preprocessor_filepath=preprocessor,
+                                                                  preprocessor=preprocessor,
                                                                   reproducibility_env_filepath=reproducibility_env_filepath,
                                                                   custom_metadata=custom_metadata,
                                                                   input_dict=input_dict,
                                                                   print_output=False)
 
             print(f"Your model has been submitted to experiment as model version {version_exp}.")
 
@@ -1335,24 +1326,24 @@
         from aimodelshare.aimsonnx import instantiate_model
         model = instantiate_model(apiurl=self.playground_url, trained=trained, version=version, reproduce=reproduce,
                                   submission_type=submission_type)
         return model
 
     def replicate_model(self, version=None, submission_type="experiment"):
         """
-        Instantiate an untrained model with reproducibility environment setup. 
-        
-        Parameters: 
+        Instantiate an untrained model with reproducibility environment setup.
+
+        Parameters:
         -----------
         `version`: ``int``
             Model version number from competition or experiment leaderboard
-          
+
         Returns:
         --------
-        model:  model chosen from leaderboard     
+        model:  model chosen from leaderboard
         """
 
         model = self.instantiate_model(version=version, trained=False, reproduce=True, submission_type=submission_type)
 
         return model
 
     def delete_deployment(self, playground_url=None, confirmation=True):
@@ -1379,19 +1370,19 @@
 
     def update_access_list(self, email_list=[], update_type="Replace_list"):
         """
         Updates list of authenticated participants who can submit new models to a competition.
         Parameters:
         -----------
         `apiurl`: string
-                URL of deployed prediction API 
-          
+                URL of deployed prediction API
+
         `email_list`: [REQUIRED] list of comma separated emails for users who are allowed to submit models to competition.  Emails should be strings in a list.
-        `update_type`:[REQUIRED] options, ``string``: 'Add', 'Remove', 'Replace_list','Get. Add appends user emails to original list, Remove deletes users from list, 
-                  'Replace_list' overwrites the original list with the new list provided, and Get returns the current list.    
+        `update_type`:[REQUIRED] options, ``string``: 'Add', 'Remove', 'Replace_list','Get. Add appends user emails to original list, Remove deletes users from list,
+                  'Replace_list' overwrites the original list with the new list provided, and Get returns the current list.
         Returns:
         --------
         response:   "Success" upon successful request
         """
         from aimodelshare.generatemodelapi import update_access_list as update_list
         update = update_list(apiurl=self.playground_url, email_list=email_list, update_type=update_type)
         return update
@@ -1522,17 +1513,17 @@
         response, error = run_function_on_lambda(
             self.playground_url, **{"delete": "FALSE", "versionupdateget": "TRUE"}
         )
         if error is not None:
             raise error
 
         _, api_bucket, model_id = json.loads(response.content.decode("utf-8"))
-        # }}} 
+        # }}}
 
-        # upload eval_data data: 
+        # upload eval_data data:
         eval_data_path = os.path.join(temp_dir, "ytest.pkl")
         import pickle
         # ytest data to load to s3
 
         if eval_data is not None:
             if type(eval_data) is not list:
                 eval_data = eval_data.tolist()
@@ -1549,27 +1540,27 @@
         print(f"\nVisit your Model Playground Page for more.")
         if self.model_page:
             print(self.model_page)
 
     def get_leaderboard(self, verbose=3, columns=None, submission_type="experiment"):
         """
         Get current competition leaderboard to rank all submitted models.
-        Use in conjuction with stylize_leaderboard to visualize data. 
-        
+        Use in conjuction with stylize_leaderboard to visualize data.
+
         Parameters:
         -----------
         `verbose` : optional, ``int``
-            controls the verbosity: the higher, the more detail 
+            controls the verbosity: the higher, the more detail
         `columns` : optional, ``list of strings``
             list of specific column names to include in the leaderboard, all else will be excluded
             performance metrics will always be displayed
-        
+
         Returns:
         --------
-        dictionary of leaderboard data 
+        dictionary of leaderboard data
         """
         from aimodelshare.leaderboard import get_leaderboard
         data = get_leaderboard(verbose=verbose,
                                columns=columns,
                                apiurl=self.playground_url,
                                submission_type=submission_type)
         return data
@@ -1589,22 +1580,22 @@
         return stylized_leaderboard
 
     def compare_models(self, version_list="None", by_model_type=None, best_model=None, verbose=1,
                        naming_convention=None, submission_type="experiment"):
         """
         Compare the structure of two or more models submitted to a competition leaderboard.
         Use in conjunction with stylize_compare to visualize data.
-        
+
         Parameters:
         -----------
         `version_list` = ``list of int``
-            list of model version numbers to compare (previously submitted to competition leaderboard) 
+            list of model version numbers to compare (previously submitted to competition leaderboard)
         `verbose` = ``int``
-            controls the verbosity: the higher, the more detail 
-        
+            controls the verbosity: the higher, the more detail
+
         Returns:
         --------
         data : dictionary of model comparison information
         """
         from aimodelshare.aimsonnx import compare_models as compare
         data = compare(apiurl=self.playground_url,
                        version_list=version_list,
@@ -1617,33 +1608,33 @@
 
     def stylize_compare(self, compare_dict, naming_convention="keras"):
         """
         Stylizes data received from compare_models to highlight similarities & differences.
         Parameters:
         -----------
         `compare_dict` = dictionary of model data from compare_models
- 
+
         Returns:
         --------
-        formatted table of model comparisons 
+        formatted table of model comparisons
         """
         from aimodelshare.aimsonnx import stylize_model_comparison
         stylized_compare = stylize_model_comparison(comp_dict_out=compare_dict, naming_convention=naming_convention)
         return (stylized_compare)
 
     def instantiate_model(self, version=None, trained=False, reproduce=False, submission_type="experiment"):
         """
         Import a model previously submitted to the competition leaderboard to use in your session
         Parameters:
         -----------
         `version`: ``int``
             Model version number from competition leaderboard
         `trained`: ``bool, default=False``
             if True, a trained model is instantiated, if False, the untrained model is instantiated
-       
+
         Returns:
         --------
         model: model chosen from leaderboard
         """
         from aimodelshare.aimsonnx import instantiate_model
         model = instantiate_model(apiurl=self.playground_url, trained=trained, version=version,
                                   reproduce=reproduce, submission_type=submission_type)
@@ -1651,15 +1642,15 @@
 
     def inspect_eval_data(self, submission_type="experiment"):
         """
         Examines structure of evaluation data to hep users understand how to submit models to the competition leaderboad.
         Parameters:
         ------------
         None
- 
+
         Returns:
         --------
         dictionary of a competition's y-test metadata
         """
         from aimodelshare.aimsonnx import inspect_y_test
         data = inspect_y_test(apiurl=self.playground_url, submission_type=submission_type)
         return data
@@ -1677,48 +1668,58 @@
 
     def __init__(self, playground_url):
         self.playground_url = playground_url
 
     def __str__(self):
         return f"Competition class instance for playground: {self.playground_url}"
 
-    def submit_model(self, model_filepath, preprocessor_filepath, prediction_submission,
+    def submit_model(self, model, preprocessor, prediction_submission,
                      sample_data=None, reproducibility_env_filepath=None, custom_metadata=None, input_dict=None,
-                     print_output=True):
+                     print_output=True, onnx_timeout=60, model_input=None):
         """
         Submits model/preprocessor to machine learning competition using live prediction API url generated by AI Modelshare library
         The submitted model gets evaluated and compared with all existing models and a leaderboard can be generated
-        
+
         Parameters:
         -----------
         `model_filepath`:  ``string`` ends with '.onnx'
             value - Absolute path to model file [REQUIRED] to be set by the user
             .onnx is the only accepted model file extension
             "example_model.onnx" filename for file in directory.
             "/User/xyz/model/example_model.onnx" absolute path to model file from local directory
         `prediction_submission`:   one hot encoded y_pred
             value - predictions for test data
             [REQUIRED] for evaluation metrics of the submitted model
         `preprocessor_filepath`:   ``string``, default=None
-            value - absolute path to preprocessor file 
+            value - absolute path to preprocessor file
             [REQUIRED] to be set by the user
-            "./preprocessor.zip" 
+            "./preprocessor.zip"
             searches for an exported zip preprocessor file in the current directory
-            file is generated from preprocessor module using export_preprocessor function from the AI Modelshare library 
- 
+            file is generated from preprocessor module using export_preprocessor function from the AI Modelshare library
+
         Returns:
         --------
         response:   Model version if the model is submitted sucessfully
         """
 
+        # convert model to onnx
+        if onnx_timeout == False:
+            force_onnx = True
+        else:
+            force_onnx = False
+
+        with HiddenPrints():
+            model = model_to_onnx_timed(model, timeout=onnx_timeout,
+                                        force_onnx=force_onnx, model_input=model_input)
+
         from aimodelshare.model import submit_model
-        submission = submit_model(model_filepath=model_filepath,
+        submission = submit_model(model_filepath=model,
                                   apiurl=self.playground_url,
                                   prediction_submission=prediction_submission,
-                                  preprocessor=preprocessor_filepath,
+                                  preprocessor=preprocessor,
                                   reproducibility_env_filepath=reproducibility_env_filepath,
                                   custom_metadata=custom_metadata,
                                   submission_type=self.submission_type,
                                   input_dict=input_dict,
                                   print_output=print_output)
 
         return submission
@@ -1728,66 +1729,66 @@
         Import a model previously submitted to the competition leaderboard to use in your session
         Parameters:
         -----------
         `version`: ``int``
             Model version number from competition leaderboard
         `trained`: ``bool, default=False``
             if True, a trained model is instantiated, if False, the untrained model is instantiated
-       
+
         Returns:
         --------
         model: model chosen from leaderboard
         """
         from aimodelshare.aimsonnx import instantiate_model
         model = instantiate_model(apiurl=self.playground_url, trained=trained, version=version,
                                   reproduce=reproduce, submission_type=self.submission_type)
         return model
 
     def replicate_model(self, version=None):
         """
-        Instantiate an untrained model previously submitted to the competition leaderboard with its reproducibility environment setup. 
-        
-        Parameters: 
+        Instantiate an untrained model previously submitted to the competition leaderboard with its reproducibility environment setup.
+
+        Parameters:
         -----------
         `version`: ``int``
             Model version number from competition or experiment leaderboard
-          
+
         Returns:
         --------
-        model:  model chosen from leaderboard     
+        model:  model chosen from leaderboard
         """
 
         model = self.instantiate_model(version=version, trained=False, reproduce=True)
         return model
 
     def set_model_reproducibility_env(self, version=None):
         """
         Set the reproducibility environment prior to instantiating an untrained model previously submitted to the competition leaderboard.
-        
-        Parameters: 
+
+        Parameters:
         -----------
         `version`: ``int``
             Model version number from competition or experiment leaderboard
-          
+
         Returns:
         --------
-        Sets environment according to reproducibility.json from model if present.  
+        Sets environment according to reproducibility.json from model if present.
         """
         from aimodelshare.reproducibility import import_reproducibility_env_from_competition_model
         import_reproducibility_env_from_competition_model(apiurl=self.playground_url, version=version,
                                                           submission_type=self.submission_type)
 
     def inspect_model(self, version=None, naming_convention=None):
         """
         Examine structure of model submitted to a competition leaderboard
         Parameters:
         ----------
         `version` : ``int``
             Model version number from competition leaderboard
-      
+
         Returns:
         --------
         inspect_pd : dictionary of model summary & metadata
         """
         from aimodelshare.aimsonnx import inspect_model
 
         inspect_pd = inspect_model(apiurl=self.playground_url, version=version,
@@ -1795,23 +1796,23 @@
 
         return inspect_pd
 
     def compare_models(self, version_list="None", by_model_type=None, best_model=None, verbose=1,
                        naming_convention=None):
         """
         Compare the structure of two or more models submitted to a competition leaderboard.
-        Use in conjuction with stylize_compare to visualize data. 
-        
+        Use in conjuction with stylize_compare to visualize data.
+
         Parameters:
         -----------
         `version_list` = ``list of int``
-            list of model version numbers to compare (previously submitted to competition leaderboard) 
+            list of model version numbers to compare (previously submitted to competition leaderboard)
         `verbose` = ``int``
-            controls the verbosity: the higher, the more detail 
-        
+            controls the verbosity: the higher, the more detail
+
         Returns:
         --------
         data : dictionary of model comparison information
         """
         from aimodelshare.aimsonnx import compare_models as compare
         data = compare(apiurl=self.playground_url,
                        version_list=version_list,
@@ -1824,54 +1825,54 @@
 
     def stylize_compare(self, compare_dict, naming_convention="keras"):
         """
         Stylizes data received from compare_models to highlight similarities & differences.
         Parameters:
         -----------
         `compare_dict` = dictionary of model data from compare_models
- 
+
         Returns:
         --------
-        formatted table of model comparisons 
+        formatted table of model comparisons
         """
         from aimodelshare.aimsonnx import stylize_model_comparison
         stylized_compare = stylize_model_comparison(comp_dict_out=compare_dict, naming_convention=naming_convention)
         return (stylized_compare)
 
     def inspect_y_test(self):
         """
         Examines structure of y-test data to hep users understand how to submit models to the competition leaderboad.
         Parameters:
         ------------
         None
- 
+
         Returns:
         --------
         dictionary of a competition's y-test metadata
         """
         from aimodelshare.aimsonnx import inspect_y_test
         data = inspect_y_test(apiurl=self.playground_url, submission_type=self.submission_type)
         return data
 
     def get_leaderboard(self, verbose=3, columns=None):
         """
         Get current competition leaderboard to rank all submitted models.
-        Use in conjuction with stylize_leaderboard to visualize data. 
-        
+        Use in conjuction with stylize_leaderboard to visualize data.
+
         Parameters:
         -----------
         `verbose` : optional, ``int``
-            controls the verbosity: the higher, the more detail 
+            controls the verbosity: the higher, the more detail
         `columns` : optional, ``list of strings``
             list of specific column names to include in the leaderboard, all else will be excluded
             performance metrics will always be displayed
-        
+
         Returns:
         --------
-        dictionary of leaderboard data 
+        dictionary of leaderboard data
         """
         from aimodelshare.leaderboard import get_leaderboard
         data = get_leaderboard(verbose=verbose,
                                columns=columns,
                                apiurl=self.playground_url,
                                submission_type=self.submission_type)
         return data
@@ -1892,19 +1893,19 @@
 
     def update_access_list(self, email_list=[], update_type="Replace_list"):
         """
         Updates list of authenticated participants who can submit new models to a competition.
         Parameters:
         -----------
         `apiurl`: string
-                URL of deployed prediction API 
-          
+                URL of deployed prediction API
+
         `email_list`: [REQUIRED] list of comma separated emails for users who are allowed to submit models to competition.  Emails should be strings in a list.
-        `update_type`:[REQUIRED] options, ``string``: 'Add', 'Remove', 'Replace_list','Get. Add appends user emails to original list, Remove deletes users from list, 
-                  'Replace_list' overwrites the original list with the new list provided, and Get returns the current list.    
+        `update_type`:[REQUIRED] options, ``string``: 'Add', 'Remove', 'Replace_list','Get. Add appends user emails to original list, Remove deletes users from list,
+                  'Replace_list' overwrites the original list with the new list provided, and Get returns the current list.
         Returns:
         --------
         response:   "Success" upon successful request
         """
         from aimodelshare.generatemodelapi import update_access_list as update_list
         update = update_list(apiurl=self.playground_url,
                              email_list=email_list, update_type=update_type,
```

### Comparing `aimodelshare-0.1.1/aimodelshare/postprocessormodules.py` & `aimodelshare-0.1.2/aimodelshare/postprocessormodules.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/preprocessormodules.py` & `aimodelshare-0.1.2/aimodelshare/preprocessormodules.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/1.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/1.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/1B.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/1B.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/2.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/2.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/3.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/3.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/4.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/4.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/5.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/5.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/6.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/6.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/7.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/7.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/8.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/8.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/authorization.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/authorization.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/eval_classification.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/eval_classification.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/eval_lambda.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/eval_lambda.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/eval_regression.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/eval_regression.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/pyspark/nst.txt` & `aimodelshare-0.1.2/aimodelshare/pyspark/nst.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/python/my_preprocessor.py` & `aimodelshare-0.1.2/aimodelshare/python/my_preprocessor.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/readme.md` & `aimodelshare-0.1.2/aimodelshare/readme.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/reproducibility.py` & `aimodelshare-0.1.2/aimodelshare/reproducibility.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/sam/Dockerfile_PySpark.txt` & `aimodelshare-0.1.2/aimodelshare/sam/Dockerfile_PySpark.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/sam/buildspec.txt` & `aimodelshare-0.1.2/aimodelshare/sam/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/sam/codebuild_policies.txt` & `aimodelshare-0.1.2/aimodelshare/sam/codebuild_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/sam/codepipeline_policies.txt` & `aimodelshare-0.1.2/aimodelshare/sam/codepipeline_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/sam/template.txt` & `aimodelshare-0.1.2/aimodelshare/sam/template.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/tools.py` & `aimodelshare-0.1.2/aimodelshare/tools.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare/utils.py` & `aimodelshare-0.1.2/aimodelshare/utils.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/aimodelshare.egg-info/PKG-INFO` & `aimodelshare-0.1.2/aimodelshare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimodelshare
-Version: 0.1.1
+Version: 0.1.2
 Summary: Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org
 Home-page: https://www.modelshare.org
 Author: Michael Parrott
 Author-email: mikedparrott@modelshare.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimodelshare-0.1.1/aimodelshare.egg-info/SOURCES.txt` & `aimodelshare-0.1.2/aimodelshare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.1/setup.py` & `aimodelshare-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='aimodelshare', #TODO:update
-    version='0.1.1',        #TODO:update
+    version='0.1.2',        #TODO:update
     author="Michael Parrott",
     author_email="mikedparrott@modelshare.org",
     description="Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.modelshare.org",
     packages=setuptools.find_packages(),
```

### Comparing `aimodelshare-0.1.1/tests/test_playground.py` & `aimodelshare-0.1.2/tests/test_playground.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,80 @@
 from aimodelshare.playground import ModelPlayground, Experiment, Competition
-from aimodelshare.aws import set_credentials
+from aimodelshare.aws import set_credentials, get_aws_token
 import aimodelshare as ai
 from aimodelshare.data_sharing.utils import redo_with_write
 
+from unittest.mock import patch
+
 from sklearn.compose import ColumnTransformer
 from sklearn.pipeline import Pipeline
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import StandardScaler, OneHotEncoder
 from sklearn.linear_model import LogisticRegression
 
 import pandas as pd
 import shutil
+import os
 
 
 
 
-def test_set_credentials():
+# def test_set_credentials():
 
-	set_credentials(credential_file="../../credentials.txt", type="deploy_model")
+#	set_credentials(credential_file="../../credentials.txt", type="deploy_model")
 
 
 # def test_quickstart_sklearn():
 
 # 	X_train, X_test, y_train, y_test, example_data, y_test_labels = ai.import_quickstart_data("titanic")
 
 # 	assert isinstance(X_train, pd.DataFrame)
 # 	assert isinstance(X_test, pd.DataFrame)
 # 	assert isinstance(y_train, pd.Series)
 # 	assert isinstance(y_test, pd.Series)
 # 	assert isinstance(example_data, pd.DataFrame)
 # 	assert isinstance(y_test_labels, list)
 
 
-def test_playground_sklearn(): 
+def test_configure_credentials():
+
+	# mock user input
+	inputs = [os.environ.get('USERNAME'),
+			  os.environ.get('PASSWORD'),
+			  os.environ.get('AWS_ACCESS_KEY_ID'),
+			  os.environ.get('AWS_SECRET_ACCESS_KEY'),
+			  os.environ.get('AWS_REGION')]
+
+	with patch("getpass.getpass", side_effect=inputs):
+		from aimodelshare.aws import configure_credentials
+		configure_credentials()
+
+	# clean up credentials file
+	os.remove("credentials.txt")
+
+
+def test_playground_sklearn():
+
+	# mock user input
+	inputs = [os.environ.get('USERNAME'),
+			  os.environ.get('PASSWORD'),
+			  os.environ.get('AWS_ACCESS_KEY_ID'),
+			  os.environ.get('AWS_SECRET_ACCESS_KEY'),
+			  os.environ.get('AWS_REGION')]
+
+	with patch("getpass.getpass", side_effect=inputs):
+		from aimodelshare.aws import configure_credentials
+		configure_credentials()
 
 	# set credentials
-	set_credentials(credential_file="../../credentials.txt", type="deploy_model")
+	set_credentials(credential_file="credentials.txt", type="deploy_model")
+	#os.environ["AWS_TOKEN"]=get_aws_token()
+
+	# clean up credentials file
+	os.remove("credentials.txt")
 
 	# Get materials for tutorial
 	X_train, X_test, y_train, y_test, example_data, y_test_labels = ai.import_quickstart_data("titanic")
 
 	# We create the preprocessing pipelines for both numeric and categorical data.
 	numeric_features = ['age', 'fare']
 	numeric_transformer = Pipeline(steps=[
@@ -65,15 +100,15 @@
 	# Write function to transform data with preprocessor 
 	# In this case we use sklearn's Column transformer in our preprocessor function
 	def preprocessor(data):
 	    preprocessed_data=preprocess.transform(data)
 	    return preprocessed_data
 
 	# check shape of X data after preprocessing it using our new function
-	preprocessor(X_train).shape
+	assert preprocessor(X_train).shape == (1047, 10)
 
 	# build model 1
 	model = LogisticRegression(C=10, penalty='l1', solver = 'liblinear')
 	model.fit(preprocessor(X_train), y_train)
 	model.score(preprocessor(X_train), y_train)
 
 	# generate predictions
@@ -103,47 +138,81 @@
 	# Submit Model 2 to Experiment
 	myplayground.submit_model(model= model_2,
 	                          preprocessor=preprocessor,
 	                          prediction_submission=prediction_labels,
 	                          input_dict={"description": "", "tags": ""},
 	                          submission_type="all")
 
+	#submit model through competition
+	mycompetition = ai.playground.Competition(myplayground.playground_url)
+	mycompetition.submit_model(model=model_2,
+							   preprocessor=preprocessor,
+							   prediction_submission=prediction_labels,
+							   input_dict={"description": "", "tags": ""}
+							   )
+
+	#submit model through experiment
+	myexperiment = ai.playground.Experiment(myplayground.playground_url)
+	myexperiment.submit_model(model=model_2,
+							   preprocessor=preprocessor,
+							   prediction_submission=prediction_labels,
+							  input_dict={"description": "", "tags": ""}
+							  )
+
 	# Check Competition Leaderboard
 	data = myplayground.get_leaderboard()
 	myplayground.stylize_leaderboard(data)
+	assert isinstance(data, pd.DataFrame)
 
 	# Compare two or more models
-	data=myplayground.compare_models([1,2], verbose=1)
+	data = myplayground.compare_models([1,2], verbose=1)
 	myplayground.stylize_compare(data)
+	assert isinstance(data, (pd.DataFrame, dict))
 
 	# Check structure of evaluation data
-	myplayground.inspect_eval_data()
+	data = myplayground.inspect_eval_data()
+	assert isinstance(data, dict)
 
 	# deploy model
 	myplayground.deploy_model(model_version=1, example_data=example_data, y_train=y_train)
 
-	# myplayground.update_example_data(example_data)
+	# update example data
+	myplayground.update_example_data(example_data)
 
-	# # swap out runtime model
-	# myplayground.update_runtime_model(model_version=1)
+	# swap out runtime model
+	myplayground.update_runtime_model(model_version=1)
 
 	# delete
 	myplayground.delete_deployment(confirmation=False)
 
 	# local cleanup 
 	shutil.rmtree("titanic_competition_data", onerror=redo_with_write)
 	shutil.rmtree("titanic_quickstart", onerror=redo_with_write)
 
 
 
-def test_playground_keras(): 
+def test_playground_keras():
 
-	# Set credentials 
-	from aimodelshare.aws import set_credentials
-	set_credentials(credential_file="../../credentials.txt", type="deploy_model")
+	# mock user input
+	inputs = [os.environ.get('USERNAME'),
+			  os.environ.get('PASSWORD'),
+			  os.environ.get('AWS_ACCESS_KEY_ID'),
+			  os.environ.get('AWS_SECRET_ACCESS_KEY'),
+			  os.environ.get('AWS_REGION')]
+
+	with patch("getpass.getpass", side_effect=inputs):
+		from aimodelshare.aws import configure_credentials
+		configure_credentials()
+
+	# set credentials
+	set_credentials(credential_file="credentials.txt", type="deploy_model")
+	# os.environ["AWS_TOKEN"]=get_aws_token()
+
+	# clean up credentials file
+	os.remove("credentials.txt")
 
 	# # Download flower image data and and pretrained Keras models
 	from aimodelshare.data_sharing.download_data import import_quickstart_data
 	keras_model, y_train_labels = import_quickstart_data("flowers")
 	keras_model_2, y_test_labels = import_quickstart_data("flowers", "competition")
 
 	# Here is a pre-designed preprocessor, but you could also build your own to prepare the data differently
@@ -200,15 +269,15 @@
 	# Extract correct prediction labels 
 	prediction_labels = [y_train.columns[i] for i in prediction_column_index]
 
 	# Instantiate Model Playground object
 	from aimodelshare.playground import ModelPlayground
 	myplayground=ModelPlayground(input_type="image", task_type="classification", private=False)
 	# Create Model Playground Page on modelshare.ai website
-	myplayground.create(eval_data = y_test_labels)
+	myplayground.create(eval_data=y_test_labels)
 
 	# Submit Model to Experiment Leaderboard
 	myplayground.submit_model(model=keras_model,
 	                          preprocessor=preprocessor,
 	                          prediction_submission=prediction_labels,
 	                          input_dict={"description": "", "tags": ""},
 	                          submission_type="all")
@@ -224,34 +293,53 @@
 	# Generate predicted y values (Model 2)
 	prediction_column_index=keras_model_2.predict(X_test).argmax(axis=1)
 
 	# extract correct prediction labels (Model 2)
 	prediction_labels = [y_train.columns[i] for i in prediction_column_index]
 
 	# Submit Model 2 to Experiment Leaderboard
-	myplayground.submit_model(model = keras_model_2,
+	myplayground.submit_model(model=keras_model_2,
 	                            preprocessor=preprocessor,
 	                            prediction_submission=prediction_labels,
 	                            input_dict={"description": "", "tags": ""},
 	                            submission_type="all")
 
+	#submit model through competition
+	mycompetition = ai.playground.Competition(myplayground.playground_url)
+	mycompetition.submit_model(model=keras_model_2,
+							   preprocessor=preprocessor,
+							   prediction_submission=prediction_labels,
+							   input_dict={"description": "", "tags": ""}
+							   )
+
+	#submit model through experiment
+	myexperiment = ai.playground.Experiment(myplayground.playground_url)
+	myexperiment.submit_model(model=keras_model_2,
+							   preprocessor=preprocessor,
+							   prediction_submission=prediction_labels,
+							  input_dict={"description": "", "tags": ""}
+							  )
+
 	# Check experiment leaderboard
 	data = myplayground.get_leaderboard()
 	myplayground.stylize_leaderboard(data)
+	assert isinstance(data, pd.DataFrame)
 
 	# Compare two or more models
-	data=myplayground.compare_models([1,2], verbose=1)
+	data = myplayground.compare_models([1,2], verbose=1)
 	myplayground.stylize_compare(data)
+	assert isinstance(data, (pd.DataFrame, dict))
 
 	# Check structure of evaluation data
-	myplayground.inspect_eval_data()
+	data = myplayground.inspect_eval_data()
+	assert isinstance(data, dict)
 
 	# Update runtime model
 	myplayground.update_runtime_model(model_version=2)
 
 	# delete
 	myplayground.delete_deployment(confirmation=False)
 
 	# local cleanup 
 	shutil.rmtree("flower_competition_data", onerror=redo_with_write)
 	shutil.rmtree("quickstart_materials", onerror=redo_with_write)
-	shutil.rmtree("quickstart_flowers_competition", onerror=redo_with_write)
+	shutil.rmtree("quickstart_flowers_competition", onerror=redo_with_write)
```

