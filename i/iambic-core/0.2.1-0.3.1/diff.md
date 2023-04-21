# Comparing `tmp/iambic_core-0.2.1.tar.gz` & `tmp/iambic_core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.2.1.tar", max compression
+gzip compressed data, was "iambic_core-0.3.1.tar", max compression
```

## Comparing `iambic_core-0.2.1.tar` & `iambic_core-0.3.1.tar`

### file list

```diff
@@ -1,156 +1,158 @@
--rw-r--r--   0        0        0    11356 2023-04-17 21:53:10.610612 iambic_core-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     9929 2023-04-17 21:53:10.610612 iambic_core-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/templates.py
--rw-r--r--   0        0        0     1773 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/utils.py
--rw-r--r--   0        0        0    67805 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/context.py
--rw-r--r--   0        0        0      610 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/logger.py
--rw-r--r--   0        0        0    24817 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/noq_json.py
--rw-r--r--   0        0        0     4991 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/parser.py
--rw-r--r--   0        0        0    42395 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/template_generation.py
--rw-r--r--   0        0        0    24381 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/lambda/app.py
--rw-r--r--   0        0        0    13644 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/main.py
--rw-r--r--   0        0        0      628 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/__init__.py
--rw-r--r--   0        0        0     2763 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1670 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     1715 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     1888 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    12863 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    31927 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10619 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17564 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15802 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17425 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10795 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16726 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21185 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    23407 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    15144 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20504 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22515 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4307 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    29870 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20177 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    34945 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    26764 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    12458 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8455 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      788 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     1690 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      195 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5066 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9468 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    19759 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2687 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9307 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13806 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      878 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      137 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12600 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     1922 2023-04-17 21:53:10.646612 iambic_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    12252 1970-01-01 00:00:00.000000 iambic_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-21 20:14:05.441705 iambic_core-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0    10252 2023-04-21 20:14:05.441705 iambic_core-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/templates.py
+-rw-r--r--   0        0        0     1955 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    68924 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    24862 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5244 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    46094 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    26626 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13644 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2763 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1671 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     1715 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     1842 2023-04-21 20:14:05.469704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     1888 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    13572 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    33240 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17683 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15824 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17544 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10649 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21304 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24395 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20623 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22579 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4534 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31350 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35369 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    28215 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     2973 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10183 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8455 2023-04-21 20:14:05.473704 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5066 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9282 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2687 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9405 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13563 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      137 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-04-21 20:14:05.477705 iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     1922 2023-04-21 20:14:05.481705 iambic_core-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12575 1970-01-01 00:00:00.000000 iambic_core-0.3.1/PKG-INFO
```

### Comparing `iambic_core-0.2.1/LICENSE.md` & `iambic_core-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/README.md` & `iambic_core-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 
 Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
 result in the creation of three roles: "dev_cloudwatch",
 "staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
-identifier: '{{account_name}}_cloudwatch'
+identifier: '{{var.account_name}}_cloudwatch'
 included_accounts:
     - dev
     - staging
     - prod
 properties:
   description:
-    - description: Cloudwatch role for {{account_name}}
+    - description: Cloudwatch role for {{var.account_name}}
   assume_role_policy_document:
     statement:
       - action:
           - sts:AssumeRole
           - sts:TagSession
         effect: Allow
         principal:
@@ -76,34 +76,34 @@
             - logs:TestMetricFilter
             - logs:FilterLogEvents
             - logs:StartQuery
             - logs:StopQuery
         resource: "*"
   managed_policies:
     - policy_arn: arn:aws:iam::aws:policy/AdministratorAccess
-  role_name: '{{account_name}}_cloudwatch'
+  role_name: '{{var.account_name}}_cloudwatch'
   tags:
     - key: owner
       value: devops
 ```
 
 ### AWS Dynamic Permissions
 
 Create a BackendDeveloperRole with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
-identifier: '{{account_name}}_backend_developer'
+identifier: '{{var.account_name}}_backend_developer'
 included_accounts:
   - '*'
 excluded_accounts:
   - compliance
 properties:
   description:
-    - description: Backend developer role for {{account_name}}
+    - description: Backend developer role for {{var.account_name}}
   assume_role_policy_document:
     statement:
       - action:
           - sts:AssumeRole
           - sts:TagSession
         effect: Allow
         principal:
@@ -131,15 +131,15 @@
           action:
               - s3:PutObject
           resource:
               - "*"
           condition:
                 StringNotEquals:
                     s3:ResourceTag/sensitive: 'true'
-  role_name: '{{account_name}}_backend_developer'
+  role_name: '{{var.account_name}}_backend_developer'
   tags:
     - key: owner
       value: devops
 ```
 
 ### Okta Application Assignments
 
@@ -222,14 +222,18 @@
   description: A test group to use with IAMbic
   members:
     - name: user@example.com
       data_type: user
       expires_at: tomorrow
 ```
 
+## Preview standalone IAMbic templates repository
+
+Preview a standalone [IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) on how IAMbic tracks multi-cloud IAM assets in GitHub. The repository is made public for you to study. No need to make your repository public.
+
 ## IAMbic - Beta Software
 
 IAMbic is currently in beta, and is not yet recommended for use in production environments. We are actively working to improve the stability and performance of the software, and welcome feedback from the community.
 
 If you choose to use IAMbic in its current state, please be aware that you may encounter bugs, performance issues, or other unexpected behavior. We strongly recommend testing IAMbic thoroughly in a non-production environment before using it in production.
 
 Please report any issues or feedback to our GitHub issue tracker. Thank you for your support and contributions to the project!
```

### Comparing `iambic_core-0.2.1/iambic/config/dynamic_config.py` & `iambic_core-0.3.1/iambic/config/dynamic_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from pathlib import Path
 from typing import List, Optional, Union
 from uuid import uuid4
 
 import ujson as json
 from pydantic import BaseModel, Field
 from pydantic import create_model as create_pydantic_model
-from iambic.core.exceptions import MultipleSecretsNotAcceptedException
 
 import iambic.plugins.v0_1_0.github
 from iambic.core.context import ctx
+from iambic.core.exceptions import MultipleSecretsNotAcceptedException
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate, ExecutionMessage, TemplateChangeDetails
 from iambic.core.utils import sort_dict, yaml
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION, aws, azure_ad, google_workspace, okta
 
 CURRENT_IAMBIC_VERSION = "1"
```

### Comparing `iambic_core-0.2.1/iambic/config/utils.py` & `iambic_core-0.3.1/iambic/config/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,13 +35,17 @@
     if config.core:
         minimum_ulimit = config.core.minimum_ulimit
     if soft_limit < minimum_ulimit:
         try:
             resource.setrlimit(resource.RLIMIT_NOFILE, (minimum_ulimit, hard_limit))
         except PermissionError:
             log.warning(
-                "Cannot increase resource limit: the process does not have permission."
+                "Cannot increase resource limit: the process does not have permission.",
+                current_ulimit=soft_limit,
+                desired_ulimit=minimum_ulimit,
             )
         except Exception:
             log.warning(
-                "Unable to increase resource limit: please manually update the soft limit."
+                "Unable to increase resource limit: please manually update the soft limit.",
+                current_ulimit=soft_limit,
+                desired_ulimit=minimum_ulimit,
             )
```

### Comparing `iambic_core-0.2.1/iambic/config/wizard.py` & `iambic_core-0.3.1/iambic/config/wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,15 @@
         self.caller_identity = {}
         self.profile_name = ""
 
         asyncio.run(self.set_config_details())
 
         if self.config.aws:
             self.hub_account_id = self.config.aws.hub_role_arn.split(":")[4]
+            self.spoke_role_is_read_only = self.config.aws.spoke_role_is_read_only
         else:
             self.hub_account_id = None
 
         try:
             default_caller_identity = self.boto3_session.client(
                 "sts"
             ).get_caller_identity()
@@ -763,14 +764,23 @@
                 "The templates that will be used can be found here:\n"
                 "  https://github.com/noqdev/iambic/tree/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates"
             ).unsafe_ask():
                 log.info(
                     "Unable to add the AWS Account without creating the required roles."
                 )
                 return
+
+            self.config.aws.spoke_role_is_read_only = bool(
+                questionary.confirm(
+                    "Do you want to restrict IambicSpokeRole to read-only IAM and IdentityCenter service?\n"
+                    "This will limit IAMbic capability to import",
+                    default=False,
+                ).unsafe_ask()
+            )
+
         else:
             if requires_sync:
                 if not questionary.confirm(
                     "Adding this account will require a sync to be ran.\n"
                     "This is to apply any matching templates to the account if the resource does not already exist.\n"
                     "Then, the account resources will be imported into Iambic.\n"
                     "Proceed?"
@@ -799,14 +809,15 @@
                 "  https://github.com/noqdev/iambic/blob/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml"
             ).unsafe_ask():
                 log.info(
                     "Unable to add the AWS account without creating the required role."
                 )
                 return
 
+        read_only = self.config.aws.spoke_role_is_read_only
         session, profile_name = self.get_boto3_session_for_account(account_id)
         if not session:
             return
 
         if is_hub_account and not profile_name:
             profile_name = self.profile_name
         elif not is_hub_account:
@@ -818,37 +829,39 @@
         if is_hub_account:
             created_successfully = asyncio.run(
                 create_iambic_role_stacks(
                     cf_client=cf_client,
                     hub_account_id=account_id,
                     assume_as_arn=self.assume_as_arn,
                     role_arn=role_arn,
+                    read_only=read_only,
                 )
             )
             if not created_successfully:
                 log.error("Failed to create the required IAMbic roles. Exiting.")
                 sys.exit(0)
         else:
             created_successfully = asyncio.run(
                 create_spoke_role_stack(
                     cf_client=cf_client,
                     hub_account_id=account_id,
                     role_arn=role_arn,
+                    read_only=read_only,
                 )
             )
             if not created_successfully:
                 log.error(
                     "Failed to create the required IAMbic role. Account not added."
                 )
                 return
 
         account = AWSAccount(
             account_id=account_id,
             account_name=account_name,
-            spoke_role_arn=get_spoke_role_arn(account_id),
+            spoke_role_arn=get_spoke_role_arn(account_id, read_only=read_only),
             iambic_managed=IambicManaged.READ_AND_WRITE,
             aws_profile=profile_name,
         )
         if is_hub_account:
             account.hub_role_arn = get_hub_role_arn(account_id)
         # account.partition = set_aws_account_partition(account.partition)
 
@@ -1009,33 +1022,44 @@
             "Create required Hub and Spoke roles via CloudFormation?\n"
             "The templates that will be used can be found here:\n"
             "  https://github.com/noqdev/iambic/tree/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates"
         ).unsafe_ask():
             log.info("Unable to add the AWS Org without creating the required roles.")
             return
 
+        read_only = bool(
+            questionary.confirm(
+                "Do you want to restrict IambicSpokeRole to read-only IAM and IdentityCenter service?\n"
+                "This will limit IAMbic capability to import",
+                default=False,
+            ).unsafe_ask()
+        )
+        self.config.aws.spoke_role_is_read_only = read_only
+
         created_successfully = asyncio.run(
             create_iambic_role_stacks(
                 cf_client=session.client("cloudformation"),
                 hub_account_id=account_id,
                 assume_as_arn=self.assume_as_arn,
                 role_arn=self.cf_role_arn,
                 org_client=session.client("organizations"),
+                read_only=read_only,
             )
         )
         if not created_successfully:
             log.error("Failed to create the required IAMbic roles. Exiting.")
             sys.exit(0)
 
         aws_org = AWSOrganization(
             org_id=org_id,
             org_account_id=account_id,
             default_rule=BaseAWSOrgRule(),
             hub_role_arn=get_hub_role_arn(account_id),
             aws_profile=profile_name,
+            spoke_role_is_read_only=read_only,
         )
         aws_org.default_rule.iambic_managed = IambicManaged.READ_AND_WRITE
 
         self.config.aws.organizations.append(aws_org)
 
         log.debug("Attempting to get a session on the AWS org", org_id=org_id)
         try:
@@ -1127,15 +1151,17 @@
             SecretString=yaml.dump({"secrets": self.config.secrets}),
         )
 
         self.config.extends = [
             ExtendsConfig(
                 key=ExtendsConfigKey.AWS_SECRETS_MANAGER,
                 value=response["ARN"],
-                assume_role_arn=get_spoke_role_arn(self.hub_account_id),
+                assume_role_arn=get_spoke_role_arn(
+                    self.hub_account_id, read_only=self.spoke_role_is_read_only
+                ),
             )
         ]
         self.config.write()
 
     def update_secret(self):
         if not self.config.secrets:
             self.config.secrets = {}
```

### Comparing `iambic_core-0.2.1/iambic/core/aio_utils/__init__.py` & `iambic_core-0.3.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/core/exceptions.py` & `iambic_core-0.3.1/iambic/core/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,10 +15,9 @@
 
 
 class RateLimitException(BaseException):
     """Rate Limit Exception"""
 
 
 class MultipleSecretsNotAcceptedException(BaseException):
-
     def __init__(self):
         super().__init__("extends tag does not accept multiples secrets")
```

### Comparing `iambic_core-0.2.1/iambic/core/git.py` & `iambic_core-0.3.1/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/core/iambic_enum.py` & `iambic_core-0.3.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/core/iambic_plugin.py` & `iambic_core-0.3.1/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/core/logger.py` & `iambic_core-0.3.1/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/core/models.py` & `iambic_core-0.3.1/iambic/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
             variables["owner"] = owner
 
         rtemplate = Environment(loader=BaseLoader()).from_string(json.dumps(response))
         valid_characters_re = r"[\w_+=,.@-]"
         variables = {
             k: sanitize_string(v, valid_characters_re) for k, v in variables.items()
         }
-        data = rtemplate.render(**variables)
+        data = rtemplate.render(var=variables)
         return json.loads(data)
 
     async def remove_expired_resources(self):
         # Look at current model and recurse through submodules to see if it is a subclass of ExpiryModel
         # If it is, then call the remove_expired_resources method
 
         if issubclass(type(self), ExpiryModel):
@@ -359,15 +359,17 @@
         json_encoders = {PrettyOrderedSet: list}
         extra = Extra.forbid
 
     @validator("template_path")
     def validate_template_path(cls, v: Union[str, Path]):
         return str(v)
 
-    def extend_changes(self, changes: list[ProposedChange]):
+    def extend_changes(
+        self, changes: list[Union[AccountChangeDetails, ProposedChange]]
+    ):
         for change in changes:
             if change.exceptions_seen:
                 if isinstance(change, AccountChangeDetails) and change.proposed_changes:
                     # If there was a partial failure then split the successes into their own change
                     proposed_change = change.copy()
                     proposed_change.exceptions_seen = []
                     self.proposed_changes.append(proposed_change)
```

### Comparing `iambic_core-0.2.1/iambic/core/noq_json.py` & `iambic_core-0.3.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/core/parser.py` & `iambic_core-0.3.1/iambic/core/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import json
 import os
+import sys
+import time
 import traceback
 from functools import partial
 from typing import Union
 
 from pydantic import ValidationError
 from ruamel.yaml.scanner import ScannerError
 
@@ -93,14 +95,19 @@
 def load_templates(
     template_paths: list[str], raise_validation_err: bool = True
 ) -> list[BaseTemplate]:
     templates = []
     load_template_fn = partial(load_template, raise_validation_err=raise_validation_err)
     with Pool(max(1, cpu_count() // 2)) as p:
         template_dicts = p.map(load_template_fn, template_paths)
+        if getattr(sys, "gettrace", None):
+            # When in debug mode, subprocesses can exit
+            # before debugger can attach
+            # https://github.com/microsoft/debugpy/issues/712
+            time.sleep(0.5)
 
     for template_dict in template_dicts:
         if not template_dict:
             continue
 
         try:
             template_cls = TEMPLATES.template_map[template_dict["template_type"]]
```

### Comparing `iambic_core-0.2.1/iambic/core/template_generation.py` & `iambic_core-0.3.1/iambic/core/template_generation.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from iambic.core.utils import (
     evaluate_on_provider,
     gather_templates,
     get_provider_value,
     is_regex_match,
     sanitize_string,
 )
-from iambic.plugins.v0_1_0.aws.models import AWSAccount
 
 
 async def get_existing_template_map(
     repo_dir: str, template_type: str, nested: bool = False
 ) -> dict:
     """Used to keep track of existing templates on import
 
@@ -38,289 +37,330 @@
 
     response = defaultdict(dict)
     for template in templates:
         response[template.template_type][template.resource_id] = template
     return response
 
 
-def templatize_resource(aws_account: AWSAccount, resource):
-    # TODO: Move away from AWSAccount to a provider agnostic implementation
+def templatize_resource(
+    provider_child: ProviderChild, resource, valid_characters_re: str = r"[\w_+=,.@-]"
+):
     resource_type = type(resource)
 
     if isinstance(resource, dict) or isinstance(resource, list):
         resource = json.dumps(resource)
     elif resource_type != str:
         resource = str(resource)
-    valid_characters_re = r"[\w_+=,.@-]"
-    resource = resource.replace(aws_account.account_id, "{{account_id}}")
-    resource = resource.replace(
-        sanitize_string(aws_account.account_name, valid_characters_re),
-        "{{account_name}}",
-    )
-    for var in aws_account.variables:
-        resource = resource.replace(var.value, "{{{}}}".format(var.key))
+
+    if variables := getattr(provider_child, "variables", None):
+        for var in variables:
+            if isinstance(var.value, str):
+                var.value = sanitize_string(var.value, valid_characters_re)
+
+            var_key_str = "{{var.{}}}".format(var.key)
+            resource = resource.replace(var.value, "{{{}}}".format(var_key_str))
 
     return (
         json.loads(resource)
         if resource_type == dict or resource_type == list
         else resource_type(resource)
     )
 
 
-def base_group_int_attribute(account_vals: dict) -> dict[int, list[dict[str, str]]]:
-    """Groups an int attribute by a shared name across of aws_accounts
+def base_group_int_attribute(
+    provider_child_vals: dict,
+    provider_child_key_id: str,
+) -> dict[int, list[dict[str, str]]]:
+    """Groups an int attribute by a shared name across provider children.
 
     Just call group_int_or_str_attribute
 
-    :param account_vals: dict(resource_val: int = list[str])
-    :return: dict(attribute_val: int = list[dict(account_id: str)])
+    :param provider_child_vals: dict(resource_val: int = list[str])
+    :param provider_child_key_id: The key used to represent the provider child within the resource. For example, in AWS this would be "account_id".
+    :return: dict(attribute_val: int = list[dict(provider_child_key_id: str)])
     """
     response: dict[int, list[dict]] = defaultdict(list)
 
-    for account_id, resource_val in account_vals.items():
-        response[resource_val].append({"account_id": account_id})
+    for provider_child_id, resource_val in provider_child_vals.items():
+        response[resource_val].append({provider_child_key_id: provider_child_id})
 
     return response
 
 
 async def base_group_str_attribute(
-    aws_account_map: dict[str, AWSAccount], account_resources: list[dict]
+    provider_child_map: dict[str, ProviderChild],
+    provider_child_resources: list[dict],
+    provider_child_key_id: str,
 ) -> dict[str, list]:
-    """Groups a string attribute by a shared name across of aws_accounts
+    """Groups a string attribute by a shared name across provider children
 
     The ability to pass in and maintain arbitrary keys is necessary for
-        parsing resource names related to a boto3 response
+        parsing resource names related to a provider response
 
     Call group_int_or_str_attribute instead unless you need to transform this response.
     An example would be grouping role names for generating the template where you need to keep the file_path ref.
 
-    :param aws_account_map: dict(account_id:str = AWSAccount)
-    :param account_resources: list[dict(account_id:str, resources=list[dict(resource_val: str, **)])]
-    :return: dict(attribute_val: str = list[dict(resource_val: str, account_id: str, **)])
+    :param provider_child_map: {child_key_id: ProviderChild}
+    :param provider_child_resources: list[dict(child_key_id:str, resources=list[dict])]
+    :param provider_child_key_id: The key used to represent the provider child within the resource. For example, in AWS this would be "account_id".
+    :return: dict(attribute_val: str = list[dict(resource_val: str, provider_child_key_id: str, **)])
     """
 
     """
     Create map with different representations of a resource value for each account
     (Note that we now only keep the post-templatized version)
 
     The purpose is to add the 2 ways look-ups are done and maintain o(1) performance.
-    The resource_val to the corresponding list element in account_resources[elem]["resources"]
+    The resource_val to the corresponding list element in provider_child_resources[elem]["resources"]
         Under resource_val_map
     The reverse of resource_val_map which is an int representing the elem with a list of all resource_val reprs
         Under elem_resource_val_map
     """
-    # TODO: Move away from AWSAccount to a provider agnostic implementation
-    for account_resource_elem, account_resource in enumerate(account_resources):
-        account_resources[account_resource_elem]["resource_val_map"] = dict()
-        account_resources[account_resource_elem]["elem_resource_val_map"] = dict()
-        aws_account = aws_account_map[account_resource["account_id"]]
-        for resource_elem, resource in enumerate(account_resource["resources"]):
-            account_resource["resources"][resource_elem][
-                "account_id"
-            ] = account_resource["account_id"]
+    for provider_child_resource_elem, provider_child_resource in enumerate(
+        provider_child_resources
+    ):
+        provider_child_resources[provider_child_resource_elem][
+            "resource_val_map"
+        ] = dict()
+        provider_child_resources[provider_child_resource_elem][
+            "elem_resource_val_map"
+        ] = dict()
+        provider_child = provider_child_map[
+            provider_child_resource[provider_child_key_id]
+        ]
+        for resource_elem, resource in enumerate(provider_child_resource["resources"]):
+            provider_child_resource["resources"][resource_elem][
+                provider_child_key_id
+            ] = provider_child_resource[provider_child_key_id]
             resource_val = resource["resource_val"]
-            templatized_resource_val = templatize_resource(aws_account, resource_val)
+            templatized_resource_val = templatize_resource(provider_child, resource_val)
 
             # note about the decision we only kept the post-templatized version
             # we aggressively templatized the incoming information.
             # a note for future reader: if you attempt to conditional decide
             # to templatize or not, you have to be careful regarding greedy
             # algorithm that does not arrive at the same termination state.
             # Concretely, if a literal can both be repeated across accounts
             # or templatized across accounts, greedy algorithm may reach
             # different states.
 
-            account_resources[account_resource_elem]["resource_val_map"][
+            provider_child_resources[provider_child_resource_elem]["resource_val_map"][
                 templatized_resource_val
             ] = resource_elem
-            account_resources[account_resource_elem]["elem_resource_val_map"][
-                resource_elem
-            ] = [templatized_resource_val]
+            provider_child_resources[provider_child_resource_elem][
+                "elem_resource_val_map"
+            ][resource_elem] = [templatized_resource_val]
 
     grouped_resource_map = defaultdict(
         list
     )  # val:str = list(dict(name: str, path: str, account_id: str))
-    # Iterate everything looking for shared names across aws_accounts
-    for outer_elem in range(len(account_resources)):
-        for resource_val, outer_resource_elem in account_resources[outer_elem][
+    # Iterate everything looking for shared names across provider children
+    for outer_elem in range(len(provider_child_resources)):
+        for resource_val, outer_resource_elem in provider_child_resources[outer_elem][
             "resource_val_map"
         ].items():
             if outer_resource_elem is None:  # It hit on something already
                 continue
-            for inner_elem in range(outer_elem + 1, len(account_resources)):
+            for inner_elem in range(outer_elem + 1, len(provider_child_resources)):
                 if (
-                    inner_resource_elem := account_resources[inner_elem][
+                    inner_resource_elem := provider_child_resources[inner_elem][
                         "resource_val_map"
                     ].get(resource_val)
                 ) is not None:
                     if not grouped_resource_map.get(resource_val):
                         # Null out the outer_resource_elem in all the places
-                        for rn in account_resources[outer_elem][
+                        for rn in provider_child_resources[outer_elem][
                             "elem_resource_val_map"
                         ][outer_resource_elem]:
-                            account_resources[outer_elem]["resource_val_map"][rn] = None
-                        account_resources[outer_elem]["elem_resource_val_map"][
+                            provider_child_resources[outer_elem]["resource_val_map"][
+                                rn
+                            ] = None
+                        provider_child_resources[outer_elem]["elem_resource_val_map"][
                             outer_resource_elem
                         ] = []
 
                         grouped_resource_map[resource_val] = [
-                            account_resources[inner_elem]["resources"][
+                            provider_child_resources[inner_elem]["resources"][
                                 inner_resource_elem
                             ],
-                            account_resources[outer_elem]["resources"][
+                            provider_child_resources[outer_elem]["resources"][
                                 outer_resource_elem
                             ],
                         ]
                     else:
                         grouped_resource_map[resource_val].append(
-                            account_resources[inner_elem]["resources"][
+                            provider_child_resources[inner_elem]["resources"][
                                 inner_resource_elem
                             ]
                         )
 
-                    for rn in account_resources[inner_elem]["elem_resource_val_map"][
-                        inner_resource_elem
-                    ]:
-                        account_resources[inner_elem]["resource_val_map"][rn] = None
-                    account_resources[inner_elem]["elem_resource_val_map"][
+                    for rn in provider_child_resources[inner_elem][
+                        "elem_resource_val_map"
+                    ][inner_resource_elem]:
+                        provider_child_resources[inner_elem]["resource_val_map"][
+                            rn
+                        ] = None
+                    provider_child_resources[inner_elem]["elem_resource_val_map"][
                         inner_resource_elem
                     ] = []
 
     # Set the remaining attributes unique attributes
-    for account_resource in account_resources:
-        for elem, resource_vals in account_resource["elem_resource_val_map"].items():
+    for provider_child_resource in provider_child_resources:
+        for elem, resource_vals in provider_child_resource[
+            "elem_resource_val_map"
+        ].items():
             if not resource_vals:
                 continue
             elif len(resource_vals) == 1:
                 resource_val = resource_vals[0]
             else:
                 # Take priority over raw output
                 resource_val = [rv for rv in resource_vals if "{{" not in rv][0]
 
-            account_resource["resources"][elem]["account_id"] = account_resource[
-                "account_id"
+            provider_child_resource["resources"][elem][
+                provider_child_key_id
+            ] = provider_child_resource[provider_child_key_id]
+            grouped_resource_map[resource_val] = [
+                provider_child_resource["resources"][elem]
             ]
-            grouped_resource_map[resource_val] = [account_resource["resources"][elem]]
 
     return grouped_resource_map
 
 
 async def base_group_dict_attribute(
-    aws_account_map: dict[str, AWSAccount],
-    account_resources: list[dict],
+    provider_child_map: dict[str, ProviderChild],
+    provider_child_resources: list[dict],
+    provider_child_key_id: str,
+    included_children_key: str,
     prefer_templatized=False,  # clarification that this keyword parameter has no impact at the moment
 ) -> list[dict]:
-    """Groups an attribute that is a dict or list of dicts with matching aws_accounts
+    """Groups an attribute that is a dict or list of dicts with matching provider children.
 
     Call group_dict_attribute instead unless you need to transform this response.
     An example would be tags which also contain access_rules.
 
-    :param aws_account_map: dict(account_id:str = AWSAccount)
-    :param account_resources: list[dict(account_id:str, resources=list[dict])]
-    :return: list[dict(included_accounts: str, resource_val=list[dict]|dict)]
+    :param provider_child_map: {child_key_id: ProviderChild}
+    :param provider_child_resources: list[dict(child_key_id:str, resources=list[dict])]
+    :param provider_child_key_id: The key used to represent the provider child within the resource. For example, in AWS this would be "account_id".
+    :param included_children_key: The key on the template used to represent the provider children the resource applies to. For example, in AWS this would be "included_accounts"..    :return: list[dict(included_accounts: str, resource_val=list[dict]|dict)]
     """
     """
-    Create map with different representations of a resource value for each account
+    Create map with different representations of a resource value for each provider child
 
-    Create a resource_hash to the corresponding list element in account_resources[elem]["resources"]
+    Create a resource_hash to the corresponding list element in provider_child_resources[elem]["resources"]
         Under resource_hash_map
     Create a reverse of resource_hash_map which is an int representing the elem with a list of all resource_hash reprs
         Under elem_resource_hash_map
     """
-    # TODO: Move away from AWSAccount to a provider agnostic implementation
     hash_map = dict()
 
-    for account_resource_elem, account_resource in enumerate(account_resources):
-        account_resources[account_resource_elem]["resource_hash_map"] = dict()
-        account_resources[account_resource_elem]["elem_resource_hash_map"] = dict()
-        aws_account = aws_account_map[account_resource["account_id"]]
-        for resource_elem, resource in enumerate(account_resource["resources"]):
-            account_resource["resources"][resource_elem][
-                "account_id"
-            ] = account_resource["account_id"]
+    for provider_child_resource_elem, provider_child_resource in enumerate(
+        provider_child_resources
+    ):
+        provider_child_resources[provider_child_resource_elem][
+            "resource_hash_map"
+        ] = dict()
+        provider_child_resources[provider_child_resource_elem][
+            "elem_resource_hash_map"
+        ] = dict()
+        aws_account = provider_child_map[provider_child_resource[provider_child_key_id]]
+        for resource_elem, resource in enumerate(provider_child_resource["resources"]):
+            provider_child_resource["resources"][resource_elem][
+                provider_child_key_id
+            ] = provider_child_resource[provider_child_key_id]
             # Set raw dict
             resource_hash = xxhash.xxh32(
                 json.dumps(resource["resource_val"])
             ).hexdigest()
             hash_map[resource_hash] = resource["resource_val"]
             # Set dict with attempted interpolation
             templatized_dict = templatize_resource(
                 aws_account, resource["resource_val"]
             )
             templatized_resource_hash = xxhash.xxh32(
                 json.dumps(templatized_dict)
             ).hexdigest()
             hash_map[templatized_resource_hash] = templatized_dict
             # Define resource hash mappings
-            account_resources[account_resource_elem]["resource_hash_map"][
+            provider_child_resources[provider_child_resource_elem]["resource_hash_map"][
                 resource_hash
             ] = resource_elem
-            account_resources[account_resource_elem]["elem_resource_hash_map"][
-                resource_elem
-            ] = [resource_hash]
+            provider_child_resources[provider_child_resource_elem][
+                "elem_resource_hash_map"
+            ][resource_elem] = [resource_hash]
             if templatized_resource_hash != resource_hash:
-                account_resources[account_resource_elem]["resource_hash_map"][
-                    templatized_resource_hash
-                ] = resource_elem
-                account_resources[account_resource_elem]["elem_resource_hash_map"][
-                    resource_elem
-                ].append(templatized_resource_hash)
+                provider_child_resources[provider_child_resource_elem][
+                    "resource_hash_map"
+                ][templatized_resource_hash] = resource_elem
+                provider_child_resources[provider_child_resource_elem][
+                    "elem_resource_hash_map"
+                ][resource_elem].append(templatized_resource_hash)
 
     grouped_resource_map = (
         dict()
-    )  # val:str = list(dict(name: str, path: str, account_id: str))
+    )  # val:str = list(dict(name: str, path: str, provider_child_key_id: str))
     # Iterate everything looking for shared names across aws_accounts
-    for outer_elem in range(len(account_resources)):
-        for resource_hash, outer_resource_elem in account_resources[outer_elem][
+    for outer_elem in range(len(provider_child_resources)):
+        for resource_hash, outer_resource_elem in provider_child_resources[outer_elem][
             "resource_hash_map"
         ].items():
             if outer_resource_elem is None:  # It hit on something already
                 continue
-            for inner_elem in range(outer_elem + 1, len(account_resources)):
+            for inner_elem in range(outer_elem + 1, len(provider_child_resources)):
                 if (
-                    inner_resource_elem := account_resources[inner_elem][
+                    inner_resource_elem := provider_child_resources[inner_elem][
                         "resource_hash_map"
                     ].get(resource_hash)
                 ) is not None:
                     if not grouped_resource_map.get(resource_hash):
                         grouped_resource_map[resource_hash] = {
                             "resource_val": hash_map[resource_hash],
-                            "included_accounts": [
-                                account_resources[inner_elem]["account_id"],
-                                account_resources[outer_elem]["account_id"],
+                            included_children_key: [
+                                provider_child_resources[inner_elem][
+                                    provider_child_key_id
+                                ],
+                                provider_child_resources[outer_elem][
+                                    provider_child_key_id
+                                ],
                             ],
                         }
 
                         # Null out the outer_resource_elem in all the places
-                        for rn in account_resources[outer_elem][
+                        for rn in provider_child_resources[outer_elem][
                             "elem_resource_hash_map"
                         ][outer_resource_elem]:
-                            account_resources[outer_elem]["resource_hash_map"][
+                            provider_child_resources[outer_elem]["resource_hash_map"][
                                 rn
                             ] = None
-                        account_resources[outer_elem]["elem_resource_hash_map"][
+                        provider_child_resources[outer_elem]["elem_resource_hash_map"][
                             outer_resource_elem
                         ] = []
                     else:
-                        grouped_resource_map[resource_hash]["included_accounts"].append(
-                            account_resources[inner_elem]["account_id"]
+                        grouped_resource_map[resource_hash][
+                            included_children_key
+                        ].append(
+                            provider_child_resources[inner_elem][provider_child_key_id]
                         )
 
                     # Null out the inner_resource_elem in all the places
-                    for rn in account_resources[inner_elem]["elem_resource_hash_map"][
-                        inner_resource_elem
-                    ]:
-                        account_resources[inner_elem]["resource_hash_map"][rn] = None
-                    account_resources[inner_elem]["elem_resource_hash_map"][
+                    for rn in provider_child_resources[inner_elem][
+                        "elem_resource_hash_map"
+                    ][inner_resource_elem]:
+                        provider_child_resources[inner_elem]["resource_hash_map"][
+                            rn
+                        ] = None
+                    provider_child_resources[inner_elem]["elem_resource_hash_map"][
                         inner_resource_elem
                     ] = []
 
     # Set the remaining attributes unique attributes
-    for account_resource in account_resources:
-        for elem, resource_hashes in account_resource["elem_resource_hash_map"].items():
+    for provider_child_resource in provider_child_resources:
+        for elem, resource_hashes in provider_child_resource[
+            "elem_resource_hash_map"
+        ].items():
             if not resource_hashes:
                 continue
             elif len(resource_hashes) == 1:
                 resource_hash = resource_hashes[0]
             else:
                 # note about the decision we prefer post-templatized version
                 # we aggressively templatized the incoming information.
@@ -332,145 +372,163 @@
                 # different states.
                 resource_hash = resource_hashes[
                     -1
                 ]  # take the last one because it's the templatized version
 
             grouped_resource_map[resource_hash] = {
                 "resource_val": hash_map[resource_hash],
-                "included_accounts": [account_resource["account_id"]],
+                included_children_key: [provider_child_resource[provider_child_key_id]],
             }
 
     return list(grouped_resource_map.values())
 
 
-async def set_included_accounts_for_grouped_attribute(
-    aws_account_map: dict[str, AWSAccount],
-    number_of_accounts_resource_on: int,
+async def set_included_provider_children_for_grouped_attribute(
+    provider_child_map: dict[str, ProviderChild],
+    number_of_children_resource_on: int,
+    provider_child_key_id: str,
+    included_children_key: str,
     grouped_attribute,
 ) -> Union[list, dict]:
     """Takes a grouped attribute and formats its included aws_accounts to * or a list of account names
 
-    :param aws_account_map: {account_id: aws_account}
-    :param number_of_accounts_resource_on:
+    :param provider_child_map: {child_key_id: ProviderChild}
+    :param number_of_children_resource_on:
+    :param provider_child_key_id: The key used to represent the provider child within the resource. For example, in AWS this would be "account_id".
+    :param included_children_key: The key on the template used to represent the provider children the resource applies to. For example, in AWS this would be "included_accounts"..
     :param grouped_attribute:
     :return:
     """
-    # TODO: Move away from AWSAccount to a provider agnostic implementation
     if isinstance(grouped_attribute, dict):  # via base_group_str_attribute
         for k, resource_vals in grouped_attribute.items():
-            if len(resource_vals) == number_of_accounts_resource_on:
-                included_accounts = ["*"]
+            if len(resource_vals) == number_of_children_resource_on:
+                included_children = ["*"]
             else:
-                included_accounts = [
-                    aws_account_map[rv["account_id"]].account_name
+                included_children = [
+                    provider_child_map[rv[provider_child_key_id]].preferred_identifier
                     for rv in resource_vals
                 ]
-            grouped_attribute[k] = included_accounts
+            grouped_attribute[k] = included_children
 
         return grouped_attribute
 
     elif isinstance(grouped_attribute, list):  # Generated via base_group_dict_attribute
         for elem in range(len(grouped_attribute)):
             if (
-                len(grouped_attribute[elem]["included_accounts"])
-                == number_of_accounts_resource_on
+                len(grouped_attribute[elem][included_children_key])
+                == number_of_children_resource_on
             ):
-                grouped_attribute[elem]["included_accounts"] = ["*"]
+                grouped_attribute[elem][included_children_key] = ["*"]
             else:
-                included_accounts = [
-                    aws_account_map[rv].account_name
-                    for rv in grouped_attribute[elem]["included_accounts"]
+                included_children = [
+                    provider_child_map[rv].preferred_identifier
+                    for rv in grouped_attribute[elem][included_children_key]
                 ]
-                grouped_attribute[elem]["included_accounts"] = included_accounts
+                grouped_attribute[elem][included_children_key] = included_children
 
         return grouped_attribute
 
 
 async def group_int_or_str_attribute(
-    aws_account_map: dict[str, AWSAccount],
-    number_of_accounts_resource_on: int,
-    account_resources: Union[dict, list[dict]],
+    provider_child_map: dict[str, ProviderChild],
+    number_of_children_resource_on: int,
+    provider_child_resources: Union[dict, list[dict]],
+    provider_child_key_id: str,
+    included_children_key: str,
     key: Union[int, str],
 ) -> Union[int, str, list[dict]]:
-    """Groups an attribute by aws_accounts, formats the attribute and normalizes the included aws_accounts.
+    """Groups an attribute by provider child, formats the attribute and normalizes the included provider children.
 
-    :param aws_account_map:
-    :param number_of_accounts_resource_on:
-    :param account_resources: dict(account_id: str = int_val) , list[dict(account_id:str, resources=list[dict])]
+    :param provider_child_map: {child_key_id: ProviderChild}
+    :param number_of_children_resource_on:
+    :param provider_child_resources: list[dict(child_key_id:str, resources=list[dict])]
+    :param provider_child_key_id: The key used to represent the provider child within the resource. For example, in AWS this would be "account_id".
+    :param included_children_key: The key on the template used to represent the provider children the resource applies to. For example, in AWS this would be "included_accounts"..
     :param key: Used to form the list[dict] response when there are multiple values for the attribute.
     :return:
     """
-    # TODO: Move away from AWSAccount to a provider agnostic implementation
-    if isinstance(account_resources, list):
+    if isinstance(provider_child_resources, list):
         grouped_attribute = await base_group_str_attribute(
-            aws_account_map, account_resources
+            provider_child_map, provider_child_resources, provider_child_key_id
         )
     else:
-        grouped_attribute = base_group_int_attribute(account_resources)
+        grouped_attribute = base_group_int_attribute(
+            provider_child_resources, provider_child_key_id
+        )
 
     if len(grouped_attribute) == 1:
         return list(grouped_attribute.keys())[0]
 
     response = []
-    grouped_attribute = await set_included_accounts_for_grouped_attribute(
-        aws_account_map, number_of_accounts_resource_on, grouped_attribute
+    grouped_attribute = await set_included_provider_children_for_grouped_attribute(
+        provider_child_map,
+        number_of_children_resource_on,
+        provider_child_key_id,
+        included_children_key,
+        grouped_attribute,
     )
 
     for resource_val, included_accounts in grouped_attribute.items():
         if included_accounts[0] == "*":
             response.append({key: resource_val})
         else:
             response.append({key: resource_val, "included_accounts": included_accounts})
 
     return response
 
 
 async def group_dict_attribute(
-    aws_account_map: dict[str, AWSAccount],
-    number_of_accounts_resource_on: int,
-    account_resources: list[dict],
+    provider_child_map: dict[str, ProviderChild],
+    number_of_children_resource_on: int,
+    provider_child_resources: list[dict],
+    provider_child_key_id: str,
+    included_children_key: str,
     is_dict_attr: bool = True,
     prefer_templatized: bool = False,
 ) -> Union[dict, list[dict]]:
     """Groups an attribute by aws_accounts, formats the attribute and normalizes the included aws_accounts.
 
-    :param aws_account_map: {account_id: aws_account}
-    :param number_of_accounts_resource_on:
-    :param account_resources: list[dict(account_id:str, resources=list[dict])]
-    :param is_dict_attr: If false and only one hit, still return as a list. Useful for things like inline_policies.
+    :param provider_child_map: {child_key_id: ProviderChild}
+    :param number_of_children_resource_on:
+    :param provider_child_resources: list[dict(child_key_id:str, resources=list[dict])]
+    :param provider_child_key_id: The key used to represent the provider child within the resource. For example, in AWS this would be "account_id".
+    :param included_children_key: The key on the template used to represent the provider children the resource applies to. For example, in AWS this would be "included_accounts"..
+    :param is_dict_attr: If false and only one hit, still return as a list. Useful for things like inline_policies with a list of dicts.
     :return:
     """
-
-    # TODO: Move away from AWSAccount to a provider agnostic implementation
     response = []
-    grouped_attributes = await set_included_accounts_for_grouped_attribute(
-        aws_account_map,
-        number_of_accounts_resource_on,
+    grouped_attributes = await set_included_provider_children_for_grouped_attribute(
+        provider_child_map,
+        number_of_children_resource_on,
+        provider_child_key_id,
+        included_children_key,
         (
             await base_group_dict_attribute(
-                aws_account_map,
-                account_resources,
+                provider_child_map,
+                provider_child_resources,
+                provider_child_key_id,
+                included_children_key,
                 prefer_templatized=prefer_templatized,
             )
         ),
     )
 
     if len(grouped_attributes) == 1 and is_dict_attr:
         attr_val = grouped_attributes[0]["resource_val"]
-        included_accounts = grouped_attributes[0]["included_accounts"]
-        if included_accounts != ["*"]:
-            attr_val["included_accounts"] = included_accounts
+        included_children = grouped_attributes[0][included_children_key]
+        if included_children != ["*"]:
+            attr_val[included_children_key] = included_children
 
         return attr_val
 
     for grouped_attr in grouped_attributes:
         attr_val = grouped_attr["resource_val"]
-        included_accounts = grouped_attr["included_accounts"]
-        if included_accounts != ["*"]:
-            attr_val["included_accounts"] = included_accounts
+        included_children = grouped_attr[included_children_key]
+        if included_children != ["*"]:
+            attr_val[included_children_key] = included_children
 
         response.append(attr_val)
 
     return response
 
 
 def create_or_update_template(
@@ -961,16 +1019,23 @@
                 setattr(
                     merged_model,
                     key,
                     merge_model_list(
                         new_value, [existing_value], all_provider_children
                     ),
                 )
+            elif new_value is None:
+                # cloud is represented by None, local is a BaseModel.
+                # this will only work if the local BaseModel does not carry
+                # any local metadata that needs to survive outside of cloud.
+                setattr(merged_model, key, new_value)
             else:
-                raise NotImplementedError
+                raise TypeError(
+                    f"Type of {type(new_value)} is not supported. Please file a github issue"
+                )
         elif key not in iambic_fields:
             setattr(merged_model, key, new_value)
     return merged_model
 
 
 def delete_orphaned_templates(
     existing_templates: list[BaseTemplate], resource_ids: set[str]
```

### Comparing `iambic_core-0.2.1/iambic/core/utils.py` & `iambic_core-0.3.1/iambic/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import contextlib
 import os
 import pathlib
 import re
 import sys
 import tempfile
 import typing
-from datetime import date, datetime
+from datetime import date, datetime, timezone
 from io import StringIO
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Coroutine, Optional, Union
 from urllib.parse import unquote_plus
 
 import aiofiles
 from asgiref.sync import sync_to_async
@@ -661,7 +661,66 @@
             if isinstance(v, list):
                 new_obj[k] = any(exceptions_in_proposed_changes(x) for x in v)
             elif isinstance(v, dict):
                 new_obj[k] = exceptions_in_proposed_changes(v)
         return any(list(new_obj.values())) if new_obj else False
     elif isinstance(obj, list):
         return any(exceptions_in_proposed_changes(x) for x in obj)
+
+
+async def remove_expired_resources(
+    resource,
+    template_resource_type: str,
+    template_resource_id: str,
+    delete_resource_if_expired: bool = True,
+):
+    from iambic.core.models import BaseModel
+
+    if not isinstance(resource, BaseModel):
+        return resource
+
+    log_params = {}
+    if hasattr(resource, "resource_type"):
+        log_params["resource_type"] = resource.resource_type
+    if hasattr(resource, "resource_id"):
+        log_params["resource_id"] = resource.resource_id
+    if template_resource_type != log_params.get(
+        "resource_type"
+    ) or template_resource_id != log_params.get("resource_id"):
+        log_params["parent_resource_type"] = template_resource_type
+        log_params["parent_resource_id"] = template_resource_id
+
+    if isinstance(resource, BaseModel) and hasattr(resource, "expires_at"):
+        if resource.expires_at:
+            cur_time = datetime.now(tz=timezone.utc)
+            if resource.expires_at < cur_time:
+                log.info("Expired resource found, marking for deletion", **log_params)
+                resource.deleted = True
+                return resource
+
+    for field_name in resource.__fields__.keys():
+        field_val = getattr(resource, field_name)
+        if isinstance(field_val, list):
+            new_value = await asyncio.gather(
+                *[
+                    remove_expired_resources(
+                        elem, template_resource_type, template_resource_id
+                    )
+                    for elem in field_val
+                ]
+            )
+            setattr(resource, field_name, new_value)
+            if delete_resource_if_expired:
+                for elem in new_value:
+                    if getattr(elem, "deleted", None) is True:
+                        new_value.remove(elem)
+                        setattr(resource, field_name, new_value)
+        else:
+            new_value = await remove_expired_resources(
+                field_val, template_resource_type, template_resource_id
+            )
+            if getattr(new_value, "deleted", None) is True:
+                setattr(resource, field_name, None)
+            else:
+                setattr(resource, field_name, new_value)
+
+    return resource
```

### Comparing `iambic_core-0.2.1/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.3.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.3.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.3.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/github/templates/iambic-import.yml` & `iambic_core-0.3.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/github/utils.py` & `iambic_core-0.3.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/lambda/app.py` & `iambic_core-0.3.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/main.py` & `iambic_core-0.3.1/iambic/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/output/__init__.py` & `iambic_core-0.3.1/iambic/output/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pathlib
 
 from jinja2 import Environment, FileSystemLoader
 
 from iambic.output.filters import (
     rich_format,
     rich_text,
```

### Comparing `iambic_core-0.2.1/iambic/output/filters.py` & `iambic_core-0.3.1/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/output/models.py` & `iambic_core-0.3.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.3.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.3.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.3.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/output/text.py` & `iambic_core-0.3.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/README.md` & `iambic_core-0.3.1/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
           PolicyDocument:
             Version: '2012-10-17'
             Statement:
               - Effect: Allow
                 Action:
                   - sts:assumerole
                 Resource:
-                  - !Sub 'arn:aws:iam::*:role/${SpokeRoleName}'
+                  - !Sub 'arn:aws:iam::*:role/${SpokeRoleName}*'
         - PolicyName: list_spoke_account_info
           PolicyDocument:
             Version: '2012-10-17'
             Statement:
               - Effect: Allow
                 Action:
                   - organizations:ListAccounts
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 
 def get_iambic_hub_role_template_body() -> str:
     template = f"{TEMPLATE_DIR}/IambicHubRole.yml"
     with open(template, "r") as f:
         return f.read()
 
 
-def get_iambic_spoke_role_template_body() -> str:
-    template = f"{TEMPLATE_DIR}/IambicSpokeRole.yml"
+def get_iambic_spoke_role_template_body(read_only=False) -> str:
+    postfix = "ReadOnly" if read_only else ""
+    template = f"{TEMPLATE_DIR}/IambicSpokeRole{postfix}.yml"
     with open(template, "r") as f:
         return f.read()
 
 
 async def create_stack(
     client, stack_name: str, template_body: str, parameters: list[dict], **kwargs
 ) -> bool:
@@ -283,24 +284,27 @@
             cf_client, org_client, account_id
         )
 
     return successfully_created
 
 
 async def create_spoke_role_stack_set(
-    cf_client, org_client, hub_account_id: str
+    cf_client,
+    org_client,
+    hub_account_id: str,
+    read_only=False,
 ) -> bool:
     org_roots = await legacy_paginated_search(
         org_client.list_roots, response_key="Roots"
     )
 
     return await create_stack_set(
         cf_client,
         stack_set_name="IambicSpokeRole",
-        template_body=get_iambic_spoke_role_template_body(),
+        template_body=get_iambic_spoke_role_template_body(read_only=read_only),
         parameters=[
             {
                 "ParameterKey": "HubRoleArn",
                 "ParameterValue": get_hub_role_arn(hub_account_id),
             },
             {"ParameterKey": "SpokeRoleName", "ParameterValue": IAMBIC_SPOKE_ROLE_NAME},
         ],
@@ -315,45 +319,59 @@
             "FailureToleranceCount": 10,
         },
         Capabilities=["CAPABILITY_NAMED_IAM"],
     )
 
 
 async def create_spoke_role_stack(
-    cf_client, hub_account_id: str, role_arn: str = None
+    cf_client,
+    hub_account_id: str,
+    role_arn: str = None,
+    read_only=False,
 ) -> bool:
     additional_kwargs = {"RoleARN": role_arn} if role_arn else {}
-
+    spoke_role_postfix = "ReadOnly" if read_only else ""
     return await create_stack(
         cf_client,
-        stack_name="IambicSpokeRole",
-        template_body=get_iambic_spoke_role_template_body(),
+        stack_name=f"IambicSpokeRole{spoke_role_postfix}",
+        template_body=get_iambic_spoke_role_template_body(read_only=read_only),
         parameters=[
             {
                 "ParameterKey": "HubRoleArn",
                 "ParameterValue": get_hub_role_arn(hub_account_id),
             },
-            {"ParameterKey": "SpokeRoleName", "ParameterValue": IAMBIC_SPOKE_ROLE_NAME},
+            {
+                "ParameterKey": "SpokeRoleName",
+                "ParameterValue": f"{IAMBIC_SPOKE_ROLE_NAME}{spoke_role_postfix}",
+            },
         ],
         Capabilities=["CAPABILITY_NAMED_IAM"],
         **additional_kwargs,
     )
 
 
 async def create_hub_role_stack(
-    cf_client, hub_account_id: str, assume_as_arn: str, role_arn: str = None
+    cf_client,
+    hub_account_id: str,
+    assume_as_arn: str,
+    role_arn: str = None,
+    spoke_role_read_only=False,
 ) -> bool:
     additional_kwargs = {"RoleARN": role_arn} if role_arn else {}
+    spoke_role_postfix = "ReadOnly" if spoke_role_read_only else ""
     stack_created = await create_stack(
         cf_client,
         stack_name="IambicHubRole",
         template_body=get_iambic_hub_role_template_body(),
         parameters=[
             {"ParameterKey": "HubRoleName", "ParameterValue": IAMBIC_HUB_ROLE_NAME},
-            {"ParameterKey": "SpokeRoleName", "ParameterValue": IAMBIC_SPOKE_ROLE_NAME},
+            {
+                "ParameterKey": "SpokeRoleName",
+                "ParameterValue": f"{IAMBIC_SPOKE_ROLE_NAME}{spoke_role_postfix}",
+            },
             {"ParameterKey": "AssumeAsArn", "ParameterValue": assume_as_arn},
         ],
         Capabilities=["CAPABILITY_NAMED_IAM"],
         **additional_kwargs,
     )
     if stack_created:
         return await create_spoke_role_stack(cf_client, hub_account_id, role_arn)
@@ -363,20 +381,28 @@
 
 async def create_iambic_role_stacks(
     cf_client,
     hub_account_id: str,
     assume_as_arn: str,
     role_arn: str = None,
     org_client=None,
+    read_only=False,
 ) -> bool:
     hub_role_created = await create_hub_role_stack(
-        cf_client, hub_account_id, assume_as_arn, role_arn
+        cf_client,
+        hub_account_id,
+        assume_as_arn,
+        role_arn,
+        spoke_role_read_only=read_only,
     )
+    spoke_role_postfix = "ReadOnly" if read_only else ""
     if hub_role_created and org_client:
         log.info(
             "Creating stack instances. "
-            "You can check the progress here: https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacksets/IambicSpokeRole/stacks"
+            f"You can check the progress here: https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacksets/IambicSpokeRole{spoke_role_postfix}/stacks"
             "WARNING: Don't Exit"
         )
-        return await create_spoke_role_stack_set(cf_client, org_client, hub_account_id)
+        return await create_spoke_role_stack_set(
+            cf_client, org_client, hub_account_id, read_only=read_only
+        )
 
     return hub_role_created
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,38 +9,45 @@
 
 import boto3
 
 from iambic.config.dynamic_config import ExtendsConfig, ExtendsConfigKey
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
-from iambic.core.models import BaseTemplate, ExecutionMessage, TemplateChangeDetails
+from iambic.core.models import (
+    BaseTemplate,
+    ExecutionMessage,
+    TemplateChangeDetails,
+    Variable,
+)
 from iambic.core.parser import load_templates
 from iambic.core.template_generation import get_existing_template_map
 from iambic.core.utils import async_batch_processor, gather_templates, yaml
 from iambic.plugins.v0_1_0.aws.event_bridge.models import (
     GroupMessageDetails,
     ManagedPolicyMessageDetails,
     PermissionSetMessageDetails,
     RoleMessageDetails,
     UserMessageDetails,
 )
+from iambic.plugins.v0_1_0.aws.iam.group.models import AWS_IAM_GROUP_TEMPLATE_TYPE
 from iambic.plugins.v0_1_0.aws.iam.group.template_generation import (
     collect_aws_groups,
     generate_aws_group_templates,
 )
 from iambic.plugins.v0_1_0.aws.iam.policy.models import AWS_MANAGED_POLICY_TEMPLATE_TYPE
 from iambic.plugins.v0_1_0.aws.iam.policy.template_generation import (
     collect_aws_managed_policies,
     generate_aws_managed_policy_templates,
 )
 from iambic.plugins.v0_1_0.aws.iam.role.template_generation import (
     collect_aws_roles,
     generate_aws_role_templates,
 )
+from iambic.plugins.v0_1_0.aws.iam.user.models import AWS_IAM_USER_TEMPLATE_TYPE
 from iambic.plugins.v0_1_0.aws.iam.user.template_generation import (
     collect_aws_users,
     generate_aws_user_templates,
 )
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
     AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE,
 )
@@ -100,14 +107,23 @@
             hub_session_info = hub_account.hub_session_info
             if not hub_session_info:
                 raise Exception("Unable to assume into the hub_role_arn")
             for account in config.accounts:
                 if account.account_id != hub_account.account_id:
                     account.hub_session_info = hub_session_info
 
+    # Set up the dynamic account variables
+    for idx, account in enumerate(config.accounts):
+        config.accounts[idx].variables.extend(
+            [
+                Variable(key="account_id", value=account.account_id),
+                Variable(key="account_name", value=account.account_name),
+            ]
+        )
+
     # Preload the iam client to improve performance
     await asyncio.gather(
         *[account.get_boto3_client("iam") for account in config.accounts],
         return_exceptions=True,
     )
 
     return config
@@ -148,32 +164,49 @@
     :param config: The config object.
     :param templates: The list of templates to apply.
     :param remote_worker: The remote worker to use for applying templates.
     """
     await generate_permission_set_map(config.accounts, templates)
 
     template_changes: list[TemplateChangeDetails] = []
+    excluded_from_batch = [AWS_MANAGED_POLICY_TEMPLATE_TYPE]
 
     if managed_policy_tasks := [
         template.apply(config)
         for template in templates
         if template.template_type == AWS_MANAGED_POLICY_TEMPLATE_TYPE
     ]:
+        # There are other template changes that could rely on the managed policy so create these first
         template_changes.extend(await async_batch_processor(managed_policy_tasks, 40))
         if len(template_changes) > len(managed_policy_tasks):
-            # There are other template changes that could rely on the managed policy
             # Give a few seconds to allow the managed policies to be created in AWS
             await asyncio.sleep(10)
 
+    if any(
+        template.template_type == AWS_IAM_GROUP_TEMPLATE_TYPE for template in templates
+    ) and any(
+        template.template_type == AWS_IAM_USER_TEMPLATE_TYPE for template in templates
+    ):
+        # There are user templates that may rely on the group so groups must be created first
+        excluded_from_batch.append(AWS_IAM_GROUP_TEMPLATE_TYPE)
+        group_tasks = [
+            template.apply(config)
+            for template in templates
+            if template.template_type == AWS_IAM_GROUP_TEMPLATE_TYPE
+        ]
+        template_changes.extend(await async_batch_processor(group_tasks, 30))
+        # Give a few seconds to allow the group to be created in AWS
+        await asyncio.sleep(10)
+
     template_changes.extend(
         await async_batch_processor(
             [
                 template.apply(config)
                 for template in templates
-                if template.template_type != AWS_MANAGED_POLICY_TEMPLATE_TYPE
+                if template.template_type not in excluded_from_batch
             ],
             30,
         )
     )
     return template_changes
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 from itertools import chain
 from typing import Callable, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
-from iambic.core.iambic_enum import Command, IambicManaged
+from iambic.core.iambic_enum import Command
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ProposedChange,
     ProposedChangeType,
 )
@@ -80,30 +80,21 @@
 class AwsIamGroupTemplate(AWSTemplate, AccessModel):
     template_type = AWS_IAM_GROUP_TEMPLATE_TYPE
     owner: Optional[str] = Field(None, description="Owner of the group")
     properties: GroupProperties = Field(
         description="Properties of the group",
     )
 
-    def _is_iambic_import_only(self, aws_account: AWSAccount):
-        return (
-            "aws-service-group" in self.properties.path
-            or aws_account.iambic_managed == IambicManaged.IMPORT_ONLY
-            or self.iambic_managed == IambicManaged.IMPORT_ONLY
-        )
+    def _is_iambic_import_only(self):
+        return "aws-service-group" in self.properties.path
 
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         client = await aws_account.get_boto3_client("iam")
-
-        # Marking for deletion. This shouldn't be done on the fly.
-        # self = await remove_expired_resources(
-        #     self, self.resource_type, self.resource_id
-        # )
         account_group = self.apply_resource_dict(aws_account)
 
         group_name = account_group["GroupName"]
         account_change_details = AccountChangeDetails(
             account=str(aws_account),
             resource_id=group_name,
             resource_type=self.resource_type,
@@ -112,15 +103,17 @@
             exceptions_seen=[],
         )
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=group_name,
             account=str(aws_account),
         )
-        iambic_import_only = self._is_iambic_import_only(aws_account)
+        if self._is_iambic_import_only():
+            return account_change_details
+
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         current_group = await get_group(
             group_name, client, include_policies=bool(not deleted)
         )
         if current_group:
             account_change_details.current_value = {
                 **current_group
@@ -134,99 +127,115 @@
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         if isinstance(deleted, list):
             deleted = deleted[0].deleted
 
         if deleted:
             if current_group:
                 account_change_details.new_value = None
-                account_change_details.proposed_changes.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.DELETE,
                         resource_id=group_name,
                         resource_type=self.resource_type,
                     )
-                )
+                ]
                 log_str = "Active resource found with deleted=false."
-                if ctx.execute and not iambic_import_only:
+                if ctx.execute:
                     log_str = f"{log_str} Deleting resource..."
                 log.debug(log_str, **log_params)
 
                 if ctx.execute:
-                    await delete_iam_group(group_name, client, log_params)
+                    apply_awaitable = delete_iam_group(group_name, client, log_params)
+                    proposed_changes = await plugin_apply_wrapper(
+                        apply_awaitable, proposed_changes
+                    )
+
+                account_change_details.extend_changes(proposed_changes)
 
             return account_change_details
 
         group_exists = bool(current_group)
         inline_policies = account_group.pop("InlinePolicies", [])
         managed_policies = account_group.pop("ManagedPolicies", [])
         existing_inline_policies = current_group.pop("InlinePolicies", [])
         existing_managed_policies = current_group.pop("ManagedPolicies", [])
         tasks = []
-        try:
-            if group_exists:
-                tasks.extend([])
-
-                supported_update_keys = ["Path", "GroupName"]
-                update_resource_log_params = {**log_params}
-                update_group_params = {}
-                for k in supported_update_keys:
-                    if account_group.get(k) is not None and account_group.get(
-                        k
-                    ) != current_group.get(k):
-                        update_resource_log_params[k] = dict(
-                            old_value=current_group.get(k),
-                            new_value=account_group.get(k),
-                        )
-                        update_group_params[f"New{k}"] = account_group.get(k)
-
-                if update_group_params:
-                    log_str = "Out of date resource found."
-                    proposed_changes = [
-                        ProposedChange(
-                            change_type=ProposedChangeType.UPDATE,
-                            resource_id=group_name,
-                            resource_type=self.resource_type,
-                        )
-                    ]
-                    if ctx.execute:
-                        log.debug(
-                            f"{log_str} Updating resource...",
-                            **update_resource_log_params,
-                        )
-                        apply_awaitable = boto_crud_call(
-                            client.update_group,
-                            RoleName=group_name,
-                            **update_group_params,
-                        )
-                        tasks.append(
-                            plugin_apply_wrapper(apply_awaitable, proposed_changes)
-                        )
-                    else:
-                        log.debug(log_str, **update_resource_log_params)
-                        account_change_details.proposed_changes.extend(proposed_changes)
-            else:
-                account_change_details.proposed_changes.append(
+
+        if group_exists:
+            tasks.extend([])
+
+            supported_update_keys = ["Path", "GroupName"]
+            update_resource_log_params = {**log_params}
+            update_group_params = {}
+            for k in supported_update_keys:
+                if account_group.get(k) is not None and account_group.get(
+                    k
+                ) != current_group.get(k):
+                    update_resource_log_params[k] = dict(
+                        old_value=current_group.get(k),
+                        new_value=account_group.get(k),
+                    )
+                    update_group_params[f"New{k}"] = account_group.get(k)
+
+            if update_group_params:
+                log_str = "Out of date resource found."
+                proposed_changes = [
                     ProposedChange(
-                        change_type=ProposedChangeType.CREATE,
+                        change_type=ProposedChangeType.UPDATE,
                         resource_id=group_name,
                         resource_type=self.resource_type,
                     )
+                ]
+                if ctx.execute:
+                    log.debug(
+                        f"{log_str} Updating resource...",
+                        **update_resource_log_params,
+                    )
+                    apply_awaitable = boto_crud_call(
+                        client.update_group,
+                        RoleName=group_name,
+                        **update_group_params,
+                    )
+                    tasks.append(
+                        plugin_apply_wrapper(apply_awaitable, proposed_changes)
+                    )
+                else:
+                    log.debug(log_str, **update_resource_log_params)
+                    account_change_details.extend_changes(proposed_changes)
+        else:
+            proposed_changes = [
+                ProposedChange(
+                    change_type=ProposedChangeType.CREATE,
+                    resource_id=group_name,
+                    resource_type=self.resource_type,
                 )
-                log_str = "New resource found in code."
-                if not ctx.execute:
-                    log.debug(log_str, **log_params)
-                    # Exit now because apply functions won't work if resource doesn't exist
-                    return account_change_details
-
-                log_str = f"{log_str} Creating resource..."
+            ]
+            log_str = "New resource found in code."
+            if not ctx.execute:
+                # Exit now because apply functions won't work if resource doesn't exist
                 log.debug(log_str, **log_params)
-                await boto_crud_call(client.create_group, **account_group)
-        except Exception as e:
-            log.error("Unable to generate tasks for resource", error=e, **log_params)
-            return account_change_details
+                account_change_details.extend_changes(proposed_changes)
+                return account_change_details
+
+            log.debug(f"{log_str} Creating resource...", **log_params)
+            apply_awaitable = boto_crud_call(client.create_group, **account_group)
+            account_change_details.extend_changes(
+                await plugin_apply_wrapper(apply_awaitable, proposed_changes)
+            )
+
+            if account_change_details.exceptions_seen:
+                log.error(
+                    "Unable to create resource on account",
+                    exceptions_seen=[
+                        cd.exceptions_seen
+                        for cd in account_change_details.exceptions_seen
+                    ],
+                    **log_params,
+                )
+                return account_change_details
 
         tasks.extend(
             [
                 apply_group_managed_policies(
                     group_name,
                     client,
                     managed_policies,
@@ -238,28 +247,22 @@
                     client,
                     inline_policies,
                     existing_inline_policies,
                     log_params,
                 ),
             ]
         )
-        try:
-            changes_made = await asyncio.gather(*tasks, return_exceptions=True)
-            if any(changes_made):
-                account_change_details.extend_changes(
-                    list(chain.from_iterable(changes_made))
-                )
 
-        except Exception as e:
-            log.exception("Unable to apply changes to resource", error=e, **log_params)
-            return account_change_details
+        changes_made = await asyncio.gather(*tasks)
+        if any(changes_made):
+            account_change_details.extend_changes(
+                list(chain.from_iterable(changes_made))
+            )
 
         if ctx.execute and not account_change_details.exceptions_seen:
-            # if self.deleted:
-            #     self.delete()
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
         elif account_change_details.exceptions_seen:
             log.error(
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 import aiofiles
 
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
-    base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    group_dict_attribute,
-    group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import GroupMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.group.models import (
     AWS_IAM_GROUP_TEMPLATE_TYPE,
     AwsIamGroupTemplate,
     GroupProperties,
@@ -27,14 +24,19 @@
 from iambic.plugins.v0_1_0.aws.iam.group.utils import (
     get_group_across_accounts,
     get_group_inline_policies,
     get_group_managed_policies,
     list_groups,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
+from iambic.plugins.v0_1_0.aws.template_generation import (
+    base_group_str_attribute,
+    group_dict_attribute,
+    group_int_or_str_attribute,
+)
 from iambic.plugins.v0_1_0.aws.utils import (
     calculate_import_preference,
     get_aws_account_map,
 )
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
@@ -62,15 +64,17 @@
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
 
     file_name = (
-        group_name.replace("{{", "")
+        group_name.replace(" ", "")
+        .replace("{{var.", "")
+        .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
     return str(os.path.join(group_dir, separator, f"{file_name}.yaml"))
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from itertools import chain
 from typing import Callable, List, Optional, Union
 
 from jinja2 import BaseLoader, Environment
 from pydantic import Field, constr, validator
 
 from iambic.core.context import ctx
-from iambic.core.iambic_enum import Command, IambicManaged
+from iambic.core.iambic_enum import Command
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ExpiryModel,
     ProposedChange,
     ProposedChangeType,
 )
-from iambic.core.utils import sanitize_string
+from iambic.core.utils import plugin_apply_wrapper, sanitize_string
 from iambic.plugins.v0_1_0.aws.iam.models import Path
 from iambic.plugins.v0_1_0.aws.iam.policy.utils import (
     apply_managed_policy_tags,
     apply_update_managed_policy,
     delete_managed_policy,
     get_managed_policy,
 )
@@ -302,21 +302,14 @@
 
 class AwsIamManagedPolicyTemplate(AWSTemplate, AccessModel):
     template_type = AWS_MANAGED_POLICY_TEMPLATE_TYPE
     properties: ManagedPolicyProperties = Field(
         description="The properties of the managed policy",
     )
 
-    def _is_iambic_import_only(self, aws_account: AWSAccount):
-        return (
-            aws_account.iambic_managed == IambicManaged.IMPORT_ONLY
-            or self.iambic_managed == IambicManaged.IMPORT_ONLY
-            or ctx.eval_only
-        )
-
     def get_arn_for_account(self, aws_account: AWSAccount) -> str:
         path = self.get_attribute_val_for_account(aws_account, "properties.path", False)
         policy_name = self.properties.policy_name
         return f"arn:{aws_account.partition.value}:iam::{aws_account.account_id}:policy{path}{policy_name}"
 
     def _apply_resource_dict(self, aws_account: AWSAccount = None) -> dict:
         resource_dict = super()._apply_resource_dict(aws_account)
@@ -336,15 +329,14 @@
             exceptions_seen=[],
         )
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=policy_name,
             account=str(aws_account),
         )
-        is_iambic_import_only = self._is_iambic_import_only(aws_account)
         policy_arn = account_policy.pop("Arn")
         current_policy = await get_managed_policy(client, policy_arn)
         if current_policy:
             account_change_details.current_value = {**current_policy}
 
             if ctx.command == Command.CONFIG_DISCOVERY:
                 # Don't overwrite a resource during config discovery
@@ -354,80 +346,88 @@
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         if isinstance(deleted, list):
             deleted = deleted[0].deleted
 
         if deleted:
             if current_policy:
                 account_change_details.new_value = None
-                account_change_details.proposed_changes.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.DELETE,
                         resource_id=policy_name,
                         resource_type=self.resource_type,
                     )
-                )
+                ]
                 log_str = "Active resource found with deleted=false."
-                if not is_iambic_import_only:
+                if ctx.execute:
                     log_str = f"{log_str} Deleting resource..."
                 log.debug(log_str, **log_params)
 
-                if not is_iambic_import_only:
-                    await delete_managed_policy(client, policy_arn, log_params)
+                if ctx.execute:
+                    apply_awaitable = delete_managed_policy(
+                        client, policy_arn, log_params
+                    )
+                    proposed_changes = await plugin_apply_wrapper(
+                        apply_awaitable, proposed_changes
+                    )
+
+                account_change_details.extend_changes(proposed_changes)
 
             return account_change_details
 
         if current_policy:
             tasks = [
                 apply_update_managed_policy(
                     client,
                     policy_arn,
                     json.loads(account_policy["PolicyDocument"]),
                     current_policy["PolicyDocument"],
-                    is_iambic_import_only,
                     log_params,
                 ),
                 apply_managed_policy_tags(
                     client,
                     policy_arn,
                     account_policy.get("Tags", []),
                     current_policy.get("Tags", []),
-                    is_iambic_import_only,
                     log_params,
                 ),
             ]
 
-            changes_made: list[list[ProposedChange]] = await asyncio.gather(
-                *tasks, return_exceptions=True
-            )
+            changes_made: list[list[ProposedChange]] = await asyncio.gather(*tasks)
             if any(changes_made):
                 account_change_details.extend_changes(
                     list(chain.from_iterable(changes_made))
                 )
 
         else:
-            account_change_details.proposed_changes.append(
+            proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.CREATE,
                     resource_id=policy_name,
                     resource_type=self.resource_type,
                 )
-            )
+            ]
             log_str = "New resource found in code."
-            if not is_iambic_import_only:
-                log_str = f"{log_str} Creating resource..."
-                if isinstance(account_policy["PolicyDocument"], dict):
-                    account_policy["PolicyDocument"] = json.dumps(
-                        account_policy["PolicyDocument"]
-                    )
-                await boto_crud_call(client.create_policy, **account_policy)
-            log.debug(log_str, **log_params)
+            if not ctx.execute:
+                # Exit now because apply functions won't work if resource doesn't exist
+                log.debug(log_str, **log_params)
+                account_change_details.extend_changes(proposed_changes)
+                return account_change_details
+
+            log.debug(f"{log_str} Creating resource...", **log_params)
+            if isinstance(account_policy["PolicyDocument"], dict):
+                account_policy["PolicyDocument"] = json.dumps(
+                    account_policy["PolicyDocument"]
+                )
+            apply_awaitable = boto_crud_call(client.create_policy, **account_policy)
+            account_change_details.extend_changes(
+                await plugin_apply_wrapper(apply_awaitable, proposed_changes)
+            )
 
         if ctx.execute and not account_change_details.exceptions_seen:
-            # if self.deleted:
-            #     self.delete()
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
         elif account_change_details.exceptions_seen:
             log.error(
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 
 import aiofiles
 
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
-    base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    group_dict_attribute,
-    group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import ManagedPolicyMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.policy.models import (
     AWS_MANAGED_POLICY_TEMPLATE_TYPE,
     AwsIamManagedPolicyTemplate,
     ManagedPolicyProperties,
 )
 from iambic.plugins.v0_1_0.aws.iam.policy.utils import (
     get_managed_policy_across_accounts,
     list_managed_policies,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
+from iambic.plugins.v0_1_0.aws.template_generation import (
+    base_group_str_attribute,
+    group_dict_attribute,
+    group_int_or_str_attribute,
+)
 from iambic.plugins.v0_1_0.aws.utils import (
     calculate_import_preference,
     get_aws_account_map,
 )
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
@@ -60,15 +62,17 @@
     if len(included_accounts) > 1:
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
     file_name = (
-        policy_name.replace("{{", "")
+        policy_name.replace(" ", "")
+        .replace("{{var.", "")
+        .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
     return str(os.path.join(managed_policy_dir, separator, f"{file_name}.yaml"))
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
 
 
 async def apply_update_managed_policy(
     iam_client,
     policy_arn: str,
     template_policy_document: dict,
     existing_policy_document: dict,
-    iambic_import_only: bool,
     log_params: dict,
 ) -> list[ProposedChange]:
     response = []
     if isinstance(existing_policy_document, str):
         existing_policy_document = json.loads(existing_policy_document)
     policy_drift = await aio_wrapper(
         DeepDiff,
@@ -186,25 +185,24 @@
                 resource_id=policy_arn,
                 current_value=existing_policy_document,
                 new_value=template_policy_document,
             )
         ]
         response.extend(proposed_changes)
 
-        if not iambic_import_only:
-            if ctx.execute:
-                apply_awaitable = new_policy_version(
-                    iam_client,
-                    policy_arn,
-                    template_policy_document,
-                    policy_drift,
-                    log_str,
-                    log_params,
-                )
-                return await plugin_apply_wrapper(apply_awaitable, proposed_changes)
+        if ctx.execute:
+            apply_awaitable = new_policy_version(
+                iam_client,
+                policy_arn,
+                template_policy_document,
+                policy_drift,
+                log_str,
+                log_params,
+            )
+            return await plugin_apply_wrapper(apply_awaitable, proposed_changes)
 
         log.debug(log_str, **log_params)
     return response
 
 
 async def new_policy_version(
     iam_client, policy_arn, template_policy_document, policy_drift, log_str, log_params
@@ -228,15 +226,14 @@
 
 
 async def apply_managed_policy_tags(
     iam_client,
     policy_arn: str,
     template_tags: list[dict],
     existing_tags: list[dict],
-    iambic_import_only: bool,
     log_params: dict,
 ) -> list[ProposedChange]:
     existing_tag_map = {tag["Key"]: tag.get("Value") for tag in existing_tags}
     template_tag_map = {tag["Key"]: tag.get("Value") for tag in template_tags}
     tags_to_apply = [
         tag
         for tag in template_tags
@@ -256,15 +253,15 @@
                 resource_type="aws:policy_document",
                 resource_id=policy_arn,
                 change_summary={"TagKeys": tags_to_remove},
             )
         ]
         response.extend(proposed_changes)
 
-        if not iambic_import_only:
+        if ctx.execute:
             log_str = f"{log_str} Removing tags..."
             apply_awaitable = boto_crud_call(
                 iam_client.untag_policy,
                 PolicyArn=policy_arn,
                 TagKeys=tags_to_remove,
             )
             tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import json
 from itertools import chain
 from typing import Callable, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
-from iambic.core.iambic_enum import Command, IambicManaged
+from iambic.core.iambic_enum import Command
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ExpiryModel,
     ProposedChange,
     ProposedChangeType,
 )
+from iambic.core.utils import plugin_apply_wrapper
 from iambic.plugins.v0_1_0.aws.iam.models import (
     MaxSessionDuration,
     Path,
     PermissionBoundary,
 )
 from iambic.plugins.v0_1_0.aws.iam.policy.models import (
     AssumeRolePolicyDocument,
@@ -205,20 +206,16 @@
         if isinstance(response.get("MaxSessionDuration"), list):
             response["MaxSessionDuration"] = response["MaxSessionDuration"][0][
                 "MaxSessionDuration"
             ]
 
         return response
 
-    def _is_iambic_import_only(self, aws_account: AWSAccount):
-        return (
-            "aws-service-role" in self.properties.path
-            or aws_account.iambic_managed == IambicManaged.IMPORT_ONLY
-            or self.iambic_managed == IambicManaged.IMPORT_ONLY
-        )
+    def _is_iambic_import_only(self):
+        return "aws-service-role" in self.properties.path
 
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         client = await aws_account.get_boto3_client("iam")
         account_role = self.apply_resource_dict(aws_account)
         role_name = account_role["RoleName"]
@@ -226,21 +223,23 @@
             account=str(aws_account),
             resource_id=role_name,
             resource_type=self.resource_type,
             new_value=dict(**account_role),
             proposed_changes=[],
             exceptions_seen=[],
         )
+        if self._is_iambic_import_only():
+            # Don't apply changes to aws-service-roles
+            return account_change_details
+
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=role_name,
             account=str(aws_account),
         )
-        iambic_import_only = self._is_iambic_import_only(aws_account)
-
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         current_role = await get_role(
             role_name, client, include_policies=bool(not deleted)
         )
         if current_role:
             account_change_details.current_value = {**current_role}  # Create a new dict
 
@@ -252,146 +251,149 @@
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         if isinstance(deleted, list):
             deleted = deleted[0].deleted
 
         if deleted:
             if current_role:
                 account_change_details.new_value = None
-                account_change_details.proposed_changes.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.DELETE,
                         resource_id=role_name,
                         resource_type=self.resource_type,
                     )
-                )
+                ]
                 log_str = "Active resource found with deleted=false."
-                if ctx.execute and not iambic_import_only:
+                if ctx.execute:
                     log_str = f"{log_str} Deleting resource..."
                 log.debug(log_str, **log_params)
 
                 if ctx.execute:
-                    await delete_iam_role(role_name, client, log_params)
+                    apply_awaitable = delete_iam_role(role_name, client, log_params)
+                    proposed_changes = await plugin_apply_wrapper(
+                        apply_awaitable, proposed_changes
+                    )
+
+                account_change_details.extend_changes(proposed_changes)
 
             return account_change_details
 
         role_exists = bool(current_role)
         inline_policies = account_role.pop("InlinePolicies", [])
         managed_policies = account_role.pop("ManagedPolicies", [])
         existing_inline_policies = current_role.pop("InlinePolicies", [])
         existing_managed_policies = current_role.pop("ManagedPolicies", [])
         tasks = []
-        try:
-            if role_exists:
-                tasks.extend(
-                    [
-                        apply_role_tags(
-                            role_name,
-                            client,
-                            account_role["Tags"],
-                            current_role.get("Tags", []),
-                            log_params,
-                        ),
-                        update_assume_role_policy(
-                            role_name,
-                            client,
-                            account_role.pop("AssumeRolePolicyDocument", {}),
-                            current_role["AssumeRolePolicyDocument"],
-                            log_params,
-                        ),
-                        apply_role_permission_boundary(
-                            role_name,
-                            client,
-                            account_role.get("PermissionsBoundary", {}),
-                            current_role.get("PermissionsBoundary", {}),
-                            log_params,
-                        ),
-                    ]
-                )
+        if role_exists:
+            tasks.extend(
+                [
+                    apply_role_tags(
+                        role_name,
+                        client,
+                        account_role["Tags"],
+                        current_role.get("Tags", []),
+                        log_params,
+                    ),
+                    update_assume_role_policy(
+                        role_name,
+                        client,
+                        account_role.pop("AssumeRolePolicyDocument", {}),
+                        current_role["AssumeRolePolicyDocument"],
+                        log_params,
+                    ),
+                    apply_role_permission_boundary(
+                        role_name,
+                        client,
+                        account_role.get("PermissionsBoundary", {}),
+                        current_role.get("PermissionsBoundary", {}),
+                        log_params,
+                    ),
+                ]
+            )
 
-                supported_update_keys = ["Description", "MaxSessionDuration"]
-                update_resource_log_params = {**log_params}
-                update_role_params = {}
-                for k in supported_update_keys:
-                    if account_role.get(k) is not None and account_role.get(
-                        k
-                    ) != current_role.get(k):
-                        update_resource_log_params[k] = dict(
-                            old_value=current_role.get(k), new_value=account_role.get(k)
-                        )
-                        update_role_params[k] = current_role.get(k)
+            supported_update_keys = ["Description", "MaxSessionDuration"]
+            update_resource_log_params = {**log_params}
+            update_role_params = {}
+            for k in supported_update_keys:
+                if account_role.get(k) is not None and account_role.get(
+                    k
+                ) != current_role.get(k):
+                    update_resource_log_params[k] = dict(
+                        old_value=current_role.get(k), new_value=account_role.get(k)
+                    )
+                    update_role_params[k] = current_role.get(k)
 
-                if update_role_params:
-                    log_str = "Out of date resource found."
-                    if ctx.execute:
-                        log.debug(
-                            f"{log_str} Updating resource...",
-                            **update_resource_log_params,
-                        )
+            if update_role_params:
+                log_str = "Out of date resource found."
+                if ctx.execute:
+                    log.debug(
+                        f"{log_str} Updating resource...",
+                        **update_resource_log_params,
+                    )
 
-                        async def update_role():
-                            exceptions = []
-                            try:
-                                await boto_crud_call(
-                                    client.update_role,
-                                    RoleName=role_name,
-                                    **{
-                                        k: account_role.get(k)
-                                        for k in supported_update_keys
-                                    },
-                                )
-                            except Exception as e:
-                                exceptions.append(str(e))
-                            return [
-                                ProposedChange(
-                                    change_type=ProposedChangeType.UPDATE,
-                                    resource_id=role_name,
-                                    resource_type=self.resource_type,
-                                    exceptions_seen=exceptions,
-                                )
-                            ]
-
-                        tasks.append(update_role())
-                    else:
-                        log.debug(log_str, **update_resource_log_params)
-                        account_change_details.proposed_changes.append(
+                    async def update_role():
+                        exceptions = []
+                        try:
+                            await boto_crud_call(
+                                client.update_role,
+                                RoleName=role_name,
+                                **{
+                                    k: account_role.get(k)
+                                    for k in supported_update_keys
+                                },
+                            )
+                        except Exception as e:
+                            exceptions.append(str(e))
+                        return [
                             ProposedChange(
                                 change_type=ProposedChangeType.UPDATE,
                                 resource_id=role_name,
                                 resource_type=self.resource_type,
+                                exceptions_seen=exceptions,
                             )
+                        ]
+
+                    tasks.append(update_role())
+                else:
+                    log.debug(log_str, **update_resource_log_params)
+                    account_change_details.proposed_changes.append(
+                        ProposedChange(
+                            change_type=ProposedChangeType.UPDATE,
+                            resource_id=role_name,
+                            resource_type=self.resource_type,
                         )
-            else:
-                account_change_details.proposed_changes.append(
-                    ProposedChange(
-                        change_type=ProposedChangeType.CREATE,
-                        resource_id=role_name,
-                        resource_type=self.resource_type,
                     )
+        else:
+            proposed_changes = [
+                ProposedChange(
+                    change_type=ProposedChangeType.CREATE,
+                    resource_id=role_name,
+                    resource_type=self.resource_type,
                 )
-                log_str = "New resource found in code."
-                if not ctx.execute:
-                    log.debug(log_str, **log_params)
-                    # Exit now because apply functions won't work if resource doesn't exist
-                    return account_change_details
-
-                log_str = f"{log_str} Creating resource..."
+            ]
+            log_str = "New resource found in code."
+            if not ctx.execute:
+                # Exit now because apply functions won't work if resource doesn't exist
                 log.debug(log_str, **log_params)
-                account_role["AssumeRolePolicyDocument"] = json.dumps(
-                    account_role["AssumeRolePolicyDocument"]
-                )
-                if account_role.get("PermissionsBoundary"):
-                    account_role["PermissionsBoundary"] = account_role[
-                        "PermissionsBoundary"
-                    ]["PolicyArn"]
-
-                await boto_crud_call(client.create_role, **account_role)
-        except Exception as e:
-            log.error("Unable to generate tasks for resource", error=e, **log_params)
-            # return account_change_details
-            raise
+                account_change_details.extend_changes(proposed_changes)
+                return account_change_details
+
+            log.debug(f"{log_str} Creating resource...", **log_params)
+            account_role["AssumeRolePolicyDocument"] = json.dumps(
+                account_role["AssumeRolePolicyDocument"]
+            )
+            if account_role.get("PermissionsBoundary"):
+                account_role["PermissionsBoundary"] = account_role[
+                    "PermissionsBoundary"
+                ]["PolicyArn"]
+
+            apply_awaitable = boto_crud_call(client.create_role, **account_role)
+            account_change_details.extend_changes(
+                await plugin_apply_wrapper(apply_awaitable, proposed_changes)
+            )
 
         tasks.extend(
             [
                 apply_role_managed_policies(
                     role_name,
                     client,
                     managed_policies,
@@ -403,26 +405,20 @@
                     client,
                     inline_policies,
                     existing_inline_policies,
                     log_params,
                 ),
             ]
         )
-        try:
-            changes_made: list[list[ProposedChange]] = await asyncio.gather(
-                *tasks, return_exceptions=True
-            )
-            if any(changes_made):
-                account_change_details.extend_changes(
-                    list(chain.from_iterable(changes_made))
-                )
 
-        except Exception as e:
-            log.exception("Unable to apply changes to resource", error=e, **log_params)
-            return account_change_details
+        changes_made = await asyncio.gather(*tasks)
+        if any(changes_made):
+            account_change_details.extend_changes(
+                list(chain.from_iterable(changes_made))
+            )
 
         if ctx.execute and not account_change_details.exceptions_seen:
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 import aiofiles
 
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
-    base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    group_dict_attribute,
-    group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import RoleMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.policy.models import AssumeRolePolicyDocument
 from iambic.plugins.v0_1_0.aws.iam.role.models import (
     AWS_IAM_ROLE_TEMPLATE_TYPE,
     AwsIamRoleTemplate,
@@ -29,14 +26,19 @@
     get_role_across_accounts,
     get_role_inline_policies,
     get_role_managed_policies,
     list_role_tags,
     list_roles,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
+from iambic.plugins.v0_1_0.aws.template_generation import (
+    base_group_str_attribute,
+    group_dict_attribute,
+    group_int_or_str_attribute,
+)
 from iambic.plugins.v0_1_0.aws.utils import (
     calculate_import_preference,
     get_aws_account_map,
 )
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
@@ -64,15 +66,17 @@
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
 
     file_name = (
-        role_name.replace("{{", "")
+        role_name.replace(" ", "")
+        .replace("{{var.", "")
+        .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
     return str(os.path.join(role_dir, separator, f"{file_name}.yaml"))
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                         resource_type="aws:iam:role",
                         resource_id=role_name,
                         new_value=tag,
                     )
                 )
         log.debug(log_str, tags=tags_to_apply, **log_params)
 
-    if tasks and ctx.execute:
+    if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(
             *tasks, return_exceptions=True
         )
         for r in results:
             response.extend(r)
 
     return response
@@ -336,68 +336,89 @@
     new_managed_policies = [
         policy_arn
         for policy_arn in template_policies
         if policy_arn not in existing_managed_policies
     ]
     if new_managed_policies:
         log_str = "New managed policies discovered."
-        for policy_arn in new_managed_policies:
-            response.append(
-                ProposedChange(
-                    change_type=ProposedChangeType.ATTACH,
-                    resource_type="aws:policy_document",
-                    resource_id=policy_arn,
-                    attribute="managed_policies",
-                )
-            )
         if ctx.execute:
             log_str = f"{log_str} Attaching managed policies..."
-            tasks = [
-                boto_crud_call(
+            for policy_arn in new_managed_policies:
+                proposed_changes = [
+                    ProposedChange(
+                        change_type=ProposedChangeType.ATTACH,
+                        resource_type="aws:policy_document",
+                        resource_id=policy_arn,
+                        attribute="managed_policies",
+                    )
+                ]
+                apply_awaitable = boto_crud_call(
                     iam_client.attach_role_policy,
                     RoleName=role_name,
                     PolicyArn=policy_arn,
                 )
-                for policy_arn in new_managed_policies
-            ]
+                tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
+        else:
+            response.extend(
+                [
+                    ProposedChange(
+                        change_type=ProposedChangeType.ATTACH,
+                        resource_type="aws:policy_document",
+                        resource_id=policy_arn,
+                        attribute="managed_policies",
+                    )
+                    for policy_arn in new_managed_policies
+                ]
+            )
+
         log.debug(log_str, managed_policies=new_managed_policies, **log_params)
 
     # Delete existing managed policies not in template
     existing_managed_policies = [
         policy_arn
         for policy_arn in existing_managed_policies
         if policy_arn not in template_policies
     ]
     if existing_managed_policies:
         log_str = "Stale managed policies discovered."
-        for policy_arn in existing_managed_policies:
-            response.append(
-                ProposedChange(
-                    change_type=ProposedChangeType.DETACH,
-                    resource_type="aws:policy_document",
-                    resource_id=policy_arn,
-                    attribute="managed_policies",
-                )
-            )
+
         if ctx.execute:
             log_str = f"{log_str} Detaching managed policies..."
-            tasks.extend(
+            for policy_arn in existing_managed_policies:
+                proposed_changes = [
+                    ProposedChange(
+                        change_type=ProposedChangeType.DETACH,
+                        resource_type="aws:policy_document",
+                        resource_id=policy_arn,
+                        attribute="managed_policies",
+                    )
+                ]
+                apply_awaitable = boto_crud_call(
+                    iam_client.detach_role_policy,
+                    RoleName=role_name,
+                    PolicyArn=policy_arn,
+                )
+                tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
+        else:
+            response.extend(
                 [
-                    boto_crud_call(
-                        iam_client.detach_role_policy,
-                        RoleName=role_name,
-                        PolicyArn=policy_arn,
+                    ProposedChange(
+                        change_type=ProposedChangeType.DETACH,
+                        resource_type="aws:policy_document",
+                        resource_id=policy_arn,
+                        attribute="managed_policies",
                     )
                     for policy_arn in existing_managed_policies
                 ]
             )
         log.debug(log_str, managed_policies=existing_managed_policies, **log_params)
 
     if tasks:
-        await asyncio.gather(*tasks)
+        results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
+        return list(chain.from_iterable(results))
 
     return response
 
 
 async def apply_role_permission_boundary(
     role_name,
     iam_client,
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import asyncio
 from itertools import chain
 from typing import Any, Callable, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
-from iambic.core.iambic_enum import Command, IambicManaged
+from iambic.core.iambic_enum import Command
 from iambic.core.logger import log
 from iambic.core.models import (
     AccountChangeDetails,
     BaseModel,
     ExpiryModel,
     ProposedChange,
     ProposedChangeType,
 )
-from iambic.core.utils import plugin_apply_wrapper
+from iambic.core.utils import plugin_apply_wrapper, remove_expired_resources
 from iambic.plugins.v0_1_0.aws.iam.models import Path, PermissionBoundary
 from iambic.plugins.v0_1_0.aws.iam.policy.models import ManagedPolicyRef, PolicyDocument
 from iambic.plugins.v0_1_0.aws.iam.user.utils import (
     apply_user_groups,
     apply_user_inline_policies,
     apply_user_managed_policies,
     apply_user_permission_boundary,
@@ -42,15 +42,15 @@
     # pass validation.
     arn: Optional[str] = Field("", description="ARN of the group", exclude=True)
     create_date: Optional[str] = Field(
         "", description="Date the group was created", exclude=True
     )
     group_id: Optional[str] = Field("", description="ID of the group", exclude=True)
     path: Optional[str] = Field("", description="Path of the group", exclude=True)
-    extra: Any = Field(None, description=("Extra attributes to store"), exclude=True)
+    extra: Any = Field(None, description="Extra attributes to store", exclude=True)
 
     @property
     def resource_type(self):
         return "aws:iam:group"
 
     @property
     def resource_id(self):
@@ -149,24 +149,21 @@
             response["PermissionsBoundary"] = permissions_boundary
 
         if isinstance(response.get("Description"), list):
             response["Description"] = response["Description"][0]["Description"]
 
         return response
 
-    def _is_iambic_import_only(self, aws_account: AWSAccount):
-        return (
-            aws_account.iambic_managed == IambicManaged.IMPORT_ONLY
-            or self.iambic_managed == IambicManaged.IMPORT_ONLY
-        )
-
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         client = await aws_account.get_boto3_client("iam")
+        self = await remove_expired_resources(
+            self, self.resource_type, self.resource_id
+        )
         account_user = self.apply_resource_dict(aws_account)
 
         user_name = account_user["UserName"]
         account_change_details = AccountChangeDetails(
             account=str(aws_account),
             resource_id=user_name,
             resource_type=self.resource_type,
@@ -175,170 +172,163 @@
             exceptions_seen=[],
         )
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=user_name,
             account=str(aws_account),
         )
-        iambic_import_only = self._is_iambic_import_only(aws_account)
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
-        try:
-            current_user = await get_user(
-                user_name, client, include_policies=bool(not deleted)
-            )
-        except Exception as err:
-            log.error("Failed to retrieve user", **log_params, error=err)
-            return account_change_details
-
+        current_user = await get_user(
+            user_name, client, include_policies=bool(not deleted)
+        )
         if current_user:
             account_change_details.current_value = {**current_user}  # Create a new dict
 
             if ctx.command == Command.CONFIG_DISCOVERY:
                 # Don't overwrite a resource during config discovery
                 account_change_details.new_value = {}
                 return account_change_details
 
+        deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         if isinstance(deleted, list):
             deleted = deleted[0].deleted
 
         if deleted:
             if current_user:
                 account_change_details.new_value = None
                 log_str = "Active resource found with deleted=false."
-                if ctx.execute and not iambic_import_only:
+                if ctx.execute:
                     log_str = f"{log_str} Deleting resource..."
                 log.debug(log_str, **log_params)
+
                 proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.DELETE,
                         resource_id=user_name,
                         resource_type=self.resource_type,
                     )
                 ]
-
                 if ctx.execute:
+                    apply_awaitable = delete_iam_user(user_name, client, log_params)
                     proposed_changes = await plugin_apply_wrapper(
-                        delete_iam_user(user_name, client, log_params), proposed_changes
+                        apply_awaitable, proposed_changes
                     )
 
                 account_change_details.extend_changes(proposed_changes)
 
             return account_change_details
 
         user_exists = bool(current_user)
         inline_policies = account_user.pop("InlinePolicies", [])
         managed_policies = account_user.pop("ManagedPolicies", [])
         groups = account_user.pop("Groups", [])
         existing_inline_policies = current_user.pop("InlinePolicies", [])
         existing_managed_policies = current_user.pop("ManagedPolicies", [])
         existing_groups = current_user.pop("Groups", [])
         tasks = []
-        try:
-            if user_exists:
-                tasks.extend(
-                    [
-                        apply_user_tags(
-                            user_name,
-                            client,
-                            account_user["Tags"],
-                            current_user.get("Tags", []),
-                            log_params,
-                        ),
-                        apply_user_permission_boundary(
-                            user_name,
-                            client,
-                            account_user.get("PermissionsBoundary", {}),
-                            current_user.get("PermissionsBoundary", {}),
-                            log_params,
-                        ),
-                    ]
-                )
 
-                supported_update_keys = ["Path", "UserName"]
-                update_resource_log_params = {**log_params}
-                update_user_params = {}
-                for k in supported_update_keys:
-                    if account_user.get(k) is not None and account_user.get(
-                        k
-                    ) != current_user.get(k):
-                        update_resource_log_params[k] = dict(
-                            old_value=current_user.get(k), new_value=account_user.get(k)
-                        )
-                        update_user_params[f"New{k}"] = account_user.get(k)
-                if update_user_params:
-                    log_str = "Out of date resource found."
-                    if ctx.execute:
-                        log.debug(
-                            f"{log_str} Updating resource...",
-                            **update_resource_log_params,
-                        )
+        if user_exists:
+            tasks.extend(
+                [
+                    apply_user_tags(
+                        user_name,
+                        client,
+                        account_user["Tags"],
+                        current_user.get("Tags", []),
+                        log_params,
+                    ),
+                    apply_user_permission_boundary(
+                        user_name,
+                        client,
+                        account_user.get("PermissionsBoundary", {}),
+                        current_user.get("PermissionsBoundary", {}),
+                        log_params,
+                    ),
+                ]
+            )
+
+            supported_update_keys = ["Path", "UserName"]
+            update_resource_log_params = {**log_params}
+            update_user_params = {}
+            for k in supported_update_keys:
+                if account_user.get(k) is not None and account_user.get(
+                    k
+                ) != current_user.get(k):
+                    update_resource_log_params[k] = dict(
+                        old_value=current_user.get(k), new_value=account_user.get(k)
+                    )
+                    update_user_params[f"New{k}"] = account_user.get(k)
+            if update_user_params:
+                log_str = "Out of date resource found."
+                if ctx.execute:
+                    log.info(
+                        f"{log_str} Updating resource...",
+                        **update_resource_log_params,
+                    )
 
-                        async def update_user():
-                            exceptions = []
-                            try:
-                                await boto_crud_call(
-                                    client.update_user,
-                                    UserName=user_name,
-                                    **{
-                                        k: update_user_params.get(k)
-                                        for k in update_user_params
-                                    },
-                                )
-                            except Exception as e:
-                                exceptions.append(str(e))
-                            return [
-                                ProposedChange(
-                                    change_type=ProposedChangeType.UPDATE,
-                                    resource_id=user_name,
-                                    resource_type=self.resource_type,
-                                    exceptions_seen=exceptions,
-                                )
-                            ]
-
-                        tasks.append(update_user())
-                    else:
-                        log.debug(log_str, **update_resource_log_params)
-                        account_change_details.proposed_changes.append(
+                    async def update_user():
+                        exceptions = []
+                        try:
+                            await boto_crud_call(
+                                client.update_user,
+                                UserName=user_name,
+                                **{
+                                    k: update_user_params.get(k)
+                                    for k in update_user_params
+                                },
+                            )
+                        except Exception as e:
+                            exceptions.append(str(e))
+                        return [
                             ProposedChange(
                                 change_type=ProposedChangeType.UPDATE,
                                 resource_id=user_name,
                                 resource_type=self.resource_type,
+                                exceptions_seen=exceptions,
                             )
+                        ]
+
+                    tasks.append(update_user())
+                else:
+                    log.info(log_str, **update_resource_log_params)
+                    account_change_details.proposed_changes.append(
+                        ProposedChange(
+                            change_type=ProposedChangeType.UPDATE,
+                            resource_id=user_name,
+                            resource_type=self.resource_type,
                         )
-            else:
-                proposed_changes = [
-                    ProposedChange(
-                        change_type=ProposedChangeType.CREATE,
-                        resource_id=user_name,
-                        resource_type=self.resource_type,
                     )
-                ]
-                log_str = "New resource found in code."
-                if not ctx.execute:
-                    account_change_details.proposed_changes.extend(proposed_changes)
-                    log.debug(log_str, **log_params)
-                    # Exit now because apply functions won't work if resource doesn't exist
-                    return account_change_details
-
-                log_str = f"{log_str} Creating resource..."
+        else:
+            proposed_changes = [
+                ProposedChange(
+                    change_type=ProposedChangeType.CREATE,
+                    resource_id=user_name,
+                    resource_type=self.resource_type,
+                )
+            ]
+            log_str = "New resource found in code."
+            if not ctx.execute:
+                # Exit now because apply functions won't work if resource doesn't exist
                 log.debug(log_str, **log_params)
-                if account_user.get("PermissionsBoundary"):
-                    account_user["PermissionsBoundary"] = account_user[
-                        "PermissionsBoundary"
-                    ]["PolicyArn"]
-
-                account_change_details.proposed_changes.extend(
-                    await plugin_apply_wrapper(
-                        boto_crud_call(client.create_user, **account_user),
-                        proposed_changes,
-                    )
+                account_change_details.extend_changes(proposed_changes)
+                return account_change_details
+
+            log_str = f"{log_str} Creating resource..."
+            log.info(log_str, **log_params)
+            if account_user.get("PermissionsBoundary"):
+                account_user["PermissionsBoundary"] = account_user[
+                    "PermissionsBoundary"
+                ]["PolicyArn"]
+
+            account_change_details.extend_changes(
+                await plugin_apply_wrapper(
+                    boto_crud_call(client.create_user, **account_user),
+                    proposed_changes,
                 )
-        except Exception as e:
-            log.error("Unable to generate tasks for resource", error=e, **log_params)
-            return account_change_details
+            )
 
         tasks.extend(
             [
                 apply_user_managed_policies(
                     user_name,
                     client,
                     managed_policies,
@@ -357,26 +347,20 @@
                     client,
                     groups,
                     existing_groups,
                     log_params,
                 ),
             ]
         )
-        try:
-            changes_made: list[list[ProposedChange]] = await asyncio.gather(
-                *tasks, return_exceptions=True
-            )
-            if any(changes_made):
-                account_change_details.extend_changes(
-                    list(chain.from_iterable(changes_made))
-                )
 
-        except Exception as e:
-            log.exception("Unable to apply changes to resource", error=e, **log_params)
-            return account_change_details
+        changes_made = await asyncio.gather(*tasks)
+        if any(changes_made):
+            account_change_details.extend_changes(
+                list(chain.from_iterable(changes_made))
+            )
 
         if ctx.execute and not account_change_details.exceptions_seen:
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 import aiofiles
 
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
-    base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    group_dict_attribute,
-    group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import UserMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.user.models import (
     AWS_IAM_USER_TEMPLATE_TYPE,
     AwsIamUserTemplate,
     UserProperties,
@@ -29,14 +26,19 @@
     get_user_groups,
     get_user_inline_policies,
     get_user_managed_policies,
     list_user_tags,
     list_users,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
+from iambic.plugins.v0_1_0.aws.template_generation import (
+    base_group_str_attribute,
+    group_dict_attribute,
+    group_int_or_str_attribute,
+)
 from iambic.plugins.v0_1_0.aws.utils import (
     calculate_import_preference,
     get_aws_account_map,
 )
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
@@ -64,15 +66,17 @@
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
 
     file_name = (
-        user_name.replace("{{", "")
+        user_name.replace(" ", "")
+        .replace("{{var.", "")
+        .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
     return str(os.path.join(user_dir, separator, f"{file_name}.yaml"))
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
         proposed_changes = [
             ProposedChange(
                 change_type=ProposedChangeType.ATTACH,
                 resource_type="aws:iam:user",
                 resource_id=user_name,
                 attribute="tags",
                 new_value=tag,
+                current_value=existing_tag_map.get(tag["Key"]),
             )
             for tag in tags_to_apply
         ]
         response.extend(proposed_changes)
         if ctx.execute:
             log_str = f"{log_str} Adding tags..."
             apply_awaitable = boto_crud_call(
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         3,
         description=(
             "Iambic will set included_accounts = * on imported resources "
             "that exist on all accounts if the minimum number of accounts is met."
         ),
     )
     sqs_cloudtrail_changes_queues: Optional[list[str]] = []
+    spoke_role_is_read_only: bool = Field(
+        False,
+        description=(
+            "aws iambic spoke role is configured as read_only. "
+            "If true, it will restrict IAMbic capability in AWS"
+        ),
+    )
 
     @validator("organizations", allow_reuse=True)
     def validate_organizations(cls, organizations):
         if len(organizations) > 1:
             raise ValueError("Only one AWS Organization is supported at this time.")
         return organizations
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from itertools import chain
 from typing import TYPE_CHECKING, Callable, List, Optional, Union
 
 from pydantic import Field, validator
 
 from iambic.core.context import ctx
-from iambic.core.iambic_enum import Command, IambicManaged
+from iambic.core.iambic_enum import Command
 from iambic.core.logger import log
 from iambic.core.models import (
     AccessModelMixin,
     AccountChangeDetails,
     BaseModel,
     ProposedChange,
     ProposedChangeType,
@@ -396,20 +396,14 @@
                             ),
                             "account_name": f"{a_account_id} ({aws_account.identity_center_details.org_account_map[a_account_id]})",
                         }
                     )
 
         return response
 
-    def _is_read_only(self, aws_account: AWSAccount):
-        return bool(
-            aws_account.iambic_managed == IambicManaged.IMPORT_ONLY
-            or self.iambic_managed == IambicManaged.IMPORT_ONLY
-        )
-
     async def _apply_to_account(  # noqa: C901
         self, aws_account: AWSAccount
     ) -> AccountChangeDetails:
         """Apply the permission set to the given AWS account
 
         :param aws_account:
         :return:
@@ -441,15 +435,14 @@
         )
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=name,
             account=str(aws_account),
             org_id=aws_account.org_id,
         )
-        read_only = self._is_read_only(aws_account)
 
         current_account_assignments = {}
         current_permission_set = (
             aws_account.identity_center_details.permission_set_map.get(name, {})
         )
         if current_permission_set:
             exclude_keys = ["CreatedDate", "PermissionSetArn"]
@@ -487,113 +480,119 @@
         deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
         if isinstance(deleted, list):
             deleted = deleted[0].deleted
 
         if deleted:
             if current_permission_set:
                 account_change_details.new_value = None
-                account_change_details.proposed_changes.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.DELETE,
                         resource_id=name,
                         resource_type=self.resource_type,
                     )
-                )
+                ]
                 log_str = "Active resource found with deleted=false."
-                if ctx.execute and not read_only:
+                if ctx.execute:
                     log_str = f"{log_str} Deleting resource..."
                 log.debug(log_str, **log_params)
 
                 if ctx.execute:
-                    await delete_permission_set(
+                    apply_awaitable = delete_permission_set(
                         identity_center_client,
                         instance_arn,
                         permission_set_arn,
                         current_permission_set,
                         current_account_assignments,
                         log_params,
                     )
+                    proposed_changes = await plugin_apply_wrapper(
+                        apply_awaitable, proposed_changes
+                    )
+
+                account_change_details.extend_changes(proposed_changes)
 
             return account_change_details
 
         permission_set_exists = bool(current_permission_set)
         tasks = []
-        try:
-            if permission_set_exists:
-                tasks.append(
-                    apply_permission_set_tags(
-                        identity_center_client,
-                        instance_arn,
-                        permission_set_arn,
-                        template_permission_set.get("Tags", []),
-                        current_permission_set.get("Tags", []),
-                        log_params,
-                    )
+
+        if permission_set_exists:
+            tasks.append(
+                apply_permission_set_tags(
+                    identity_center_client,
+                    instance_arn,
+                    permission_set_arn,
+                    template_permission_set.get("Tags", []),
+                    current_permission_set.get("Tags", []),
+                    log_params,
                 )
+            )
 
-                supported_update_keys = ["Description", "SessionDuration", "RelayState"]
-                update_resource_log_params = {**log_params}
-                update_resource_params = {}
-                for k in supported_update_keys:
-                    if template_permission_set.get(
-                        k
-                    ) is not None and template_permission_set.get(
-                        k
-                    ) != current_permission_set.get(
-                        k
-                    ):
-                        update_resource_log_params[k] = dict(
-                            old_value=current_permission_set.get(k),
-                            new_value=template_permission_set.get(k),
-                        )
-                        update_resource_params[k] = template_permission_set.get(k)
+            supported_update_keys = ["Description", "SessionDuration", "RelayState"]
+            update_resource_log_params = {**log_params}
+            update_resource_params = {}
+            for k in supported_update_keys:
+                if template_permission_set.get(
+                    k
+                ) is not None and template_permission_set.get(
+                    k
+                ) != current_permission_set.get(
+                    k
+                ):
+                    update_resource_log_params[k] = dict(
+                        old_value=current_permission_set.get(k),
+                        new_value=template_permission_set.get(k),
+                    )
+                    update_resource_params[k] = template_permission_set.get(k)
 
-                if update_resource_params:
-                    log_str = "Out of date resource found."
-                    proposed_changes = [
-                        ProposedChange(
-                            change_type=ProposedChangeType.UPDATE,
-                            resource_id=name,
-                            resource_type=self.resource_type,
-                        )
-                    ]
-                    if ctx.execute:
-                        log.info(
-                            f"{log_str} Updating resource...",
-                            **update_resource_log_params,
-                        )
-                        apply_awaitable = boto_crud_call(
-                            identity_center_client.update_permission_set,
-                            InstanceArn=instance_arn,
-                            PermissionSetArn=permission_set_arn,
-                            **update_resource_params,
-                        )
-                        tasks.append(
-                            plugin_apply_wrapper(apply_awaitable, proposed_changes)
-                        )
-                    else:
-                        log.info(log_str, **update_resource_log_params)
-                        account_change_details.proposed_changes.extend(proposed_changes)
-            else:
-                account_change_details.proposed_changes.append(
+            if update_resource_params:
+                log_str = "Out of date resource found."
+                proposed_changes = [
                     ProposedChange(
-                        change_type=ProposedChangeType.CREATE,
+                        change_type=ProposedChangeType.UPDATE,
                         resource_id=name,
                         resource_type=self.resource_type,
                     )
+                ]
+                if ctx.execute:
+                    log.info(
+                        f"{log_str} Updating resource...",
+                        **update_resource_log_params,
+                    )
+                    apply_awaitable = boto_crud_call(
+                        identity_center_client.update_permission_set,
+                        InstanceArn=instance_arn,
+                        PermissionSetArn=permission_set_arn,
+                        **update_resource_params,
+                    )
+                    tasks.append(
+                        plugin_apply_wrapper(apply_awaitable, proposed_changes)
+                    )
+                else:
+                    log.info(log_str, **update_resource_log_params)
+                    account_change_details.proposed_changes.extend(proposed_changes)
+        else:
+            proposed_changes = [
+                ProposedChange(
+                    change_type=ProposedChangeType.CREATE,
+                    resource_id=name,
+                    resource_type=self.resource_type,
                 )
-                log_str = "New resource found in code."
-                if not ctx.execute:
-                    log.info(log_str, **log_params)
-                    # Exit now because apply functions won't work if resource doesn't exist
-                    return account_change_details
+            ]
+            log_str = "New resource found in code."
+            if not ctx.execute:
+                # Exit now because apply functions won't work if resource doesn't exist
+                log.debug(log_str, **log_params)
+                account_change_details.extend_changes(proposed_changes)
+                return account_change_details
 
-                log_str = f"{log_str} Creating resource..."
-                log.info(log_str, **log_params)
+            log.debug(f"{log_str} Creating resource...", **log_params)
 
+            try:
                 permission_set = await boto_crud_call(
                     identity_center_client.create_permission_set,
                     Name=name,
                     InstanceArn=instance_arn,
                     **{
                         param: template_permission_set.get(param)
                         for param in [
@@ -601,19 +600,32 @@
                             "RelayState",
                             "SessionDuration",
                             "Tags",
                         ]
                         if template_permission_set.get(param)
                     },
                 )
-                permission_set_arn = permission_set["PermissionSet"]["PermissionSetArn"]
+            except Exception as e:
+                for change in proposed_changes:
+                    change.exceptions_seen.append(str(e))
+
+            account_change_details.extend_changes(proposed_changes)
+
+            if account_change_details.exceptions_seen:
+                log.error(
+                    "Unable to create resource on account",
+                    exceptions_seen=[
+                        cd.exceptions_seen
+                        for cd in account_change_details.exceptions_seen
+                    ],
+                    **log_params,
+                )
+                return account_change_details
 
-        except Exception as e:
-            log.error("Unable to generate tasks for resource", error=e, **log_params)
-            return account_change_details
+            permission_set_arn = permission_set["PermissionSet"]["PermissionSetArn"]
 
         tasks.extend(
             [
                 apply_permission_set_aws_managed_policies(
                     identity_center_client,
                     instance_arn,
                     permission_set_arn,
@@ -649,63 +661,69 @@
                     permission_set_arn,
                     template_permission_set.get("PermissionsBoundary", {}),
                     current_permission_set.get("PermissionsBoundary", {}),
                     log_params,
                 ),
             ]
         )
-        try:
-            changes_made: list[list[ProposedChange]] = await asyncio.gather(*tasks)
 
-            # apply_account_assignments is a dedicated call due to the request limit on CreateAccountAssignment
-            #   per https://docs.aws.amazon.com/singlesignon/latest/userguide/limits.html
-            changes_made.append(
-                await apply_account_assignments(
-                    identity_center_client,
-                    instance_arn,
-                    permission_set_arn,
-                    template_account_assignments,
-                    current_account_assignments,
-                    log_params,
-                )
+        changes_made = await asyncio.gather(*tasks)
+        if any(changes_made):
+            account_change_details.extend_changes(
+                list(chain.from_iterable(changes_made))
             )
-            if any(changes_made):
-                account_change_details.extend_changes(
-                    list(chain.from_iterable(changes_made))
-                )
-        except Exception as e:
-            log.error("Unable to apply changes to resource", error=e, **log_params)
-            return account_change_details
+
+        # apply_account_assignments is a dedicated call due to the request limit on CreateAccountAssignment
+        #   per https://docs.aws.amazon.com/singlesignon/latest/userguide/limits.html
+        account_assignment_changes = await apply_account_assignments(
+            identity_center_client,
+            instance_arn,
+            permission_set_arn,
+            template_account_assignments,
+            current_account_assignments,
+            log_params,
+        )
+        if account_assignment_changes:
+            account_change_details.extend_changes(account_assignment_changes)
 
         if ctx.execute and not account_change_details.exceptions_seen:
             if any(changes_made) and not self.deleted:
-                res = await boto_crud_call(
-                    identity_center_client.provision_permission_set,
-                    InstanceArn=instance_arn,
-                    PermissionSetArn=permission_set_arn,
-                    TargetType="ALL_PROVISIONED_ACCOUNTS",
-                )
-
-                request_id = res["PermissionSetProvisioningStatus"]["RequestId"]
-
-                for _ in range(20):
-                    provision_status = await boto_crud_call(
-                        identity_center_client.describe_permission_set_provisioning_status,
+                try:
+                    res = await boto_crud_call(
+                        identity_center_client.provision_permission_set,
                         InstanceArn=instance_arn,
-                        ProvisionPermissionSetRequestId=request_id,
+                        PermissionSetArn=permission_set_arn,
+                        TargetType="ALL_PROVISIONED_ACCOUNTS",
                     )
 
-                    if (
-                        provision_status["PermissionSetProvisioningStatus"]["Status"]
-                        != "IN_PROGRESS"
-                    ):
-                        break
+                    request_id = res["PermissionSetProvisioningStatus"]["RequestId"]
 
-                    await asyncio.sleep(1)
-                    continue
+                    for _ in range(20):
+                        provision_status = await boto_crud_call(
+                            identity_center_client.describe_permission_set_provisioning_status,
+                            InstanceArn=instance_arn,
+                            ProvisionPermissionSetRequestId=request_id,
+                        )
+
+                        if (
+                            provision_status["PermissionSetProvisioningStatus"][
+                                "Status"
+                            ]
+                            != "IN_PROGRESS"
+                        ):
+                            break
+
+                        await asyncio.sleep(1)
+                        continue
+                except Exception as err:
+                    log.warning(
+                        "Unable to resolve status when provisioning permission set.",
+                        error=str(err),
+                        **log_params,
+                    )
             log.debug(
                 "Successfully finished execution on account for resource",
                 changes_made=bool(account_change_details.proposed_changes),
                 **log_params,
             )
         elif account_change_details.exceptions_seen:
             log.error(
@@ -720,15 +738,17 @@
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
 
         return account_change_details
 
-    async def apply(self, config: AWSConfig) -> TemplateChangeDetails:
+    async def apply(
+        self, config: AWSConfig  # noqa: C901
+    ) -> TemplateChangeDetails:
         tasks = []
         template_changes = TemplateChangeDetails(
             resource_id=self.resource_id,
             resource_type=self.resource_type,
             template_path=self.file_path,
             exceptions_seen=[],
         )
@@ -738,37 +758,64 @@
         relevant_accounts = []
 
         for account in config.accounts:
             if not account.identity_center_details:
                 continue
 
             if evaluate_on_provider(self, account):
-                relevant_accounts.append(str(account))
+                relevant_accounts.append(account)
                 tasks.append(self._apply_to_account(account))
 
         if not relevant_accounts:
             if ctx.execute:
                 if self.deleted:
                     log_str = "Successfully removed resource."
                     self.delete()
                 else:
                     log_str = "No changes detected for resource."
-                log.info(log_str, accounts=relevant_accounts, **log_params)
+                log.info(log_str, **log_params)
 
             return template_changes
 
         if ctx.execute:
             log_str = "Applying changes to resource."
         else:
             log_str = "Detecting changes for resource."
 
-        log.info(log_str, accounts=relevant_accounts, **log_params)
+        relevant_accounts_str = [str(account) for account in relevant_accounts]
+        log.info(log_str, accounts=relevant_accounts_str, **log_params)
+
+        account_changes = await asyncio.gather(*tasks, return_exceptions=True)
+        proposed_changes: list[AccountChangeDetails] = []
+        exceptions_seen = set()
+
+        for account_change in account_changes:
+            if isinstance(account_change, AccountChangeDetails):
+                proposed_changes.append(account_change)
+            else:
+                exceptions_seen.add(str(account_change))
+
+        if exceptions_seen:
+            exceptions_seen = list(exceptions_seen)
+            proposed_change_accounts = set(
+                change.account for change in proposed_changes
+            )
+            for aws_account in relevant_accounts:
+                if str(aws_account) in proposed_change_accounts:
+                    continue
+                proposed_changes.append(
+                    AccountChangeDetails(
+                        account=str(aws_account),
+                        resource_id=self.resource_id,
+                        resource_type=self.resource_type,
+                        exceptions_seen=exceptions_seen,
+                    )
+                )
 
-        account_changes = await asyncio.gather(*tasks)
-        template_changes.extend_changes(account_changes)
+        template_changes.extend_changes(proposed_changes)
 
         if template_changes.exceptions_seen:
             if self.deleted:
                 cmd_verb = "removing"
             elif ctx.execute:
                 cmd_verb = "applying"
             else:
@@ -781,15 +828,15 @@
             else:
                 log_str = "Successfully applied resource changes."
         elif account_changes:
             log_str = "Successfully detected required resource changes."
         else:
             log_str = "No changes detected for resource."
 
-        log.info(log_str, accounts=relevant_accounts, **log_params)
+        log.info(log_str, accounts=relevant_accounts_str, **log_params)
         return template_changes
 
     @property
     def included_children(self):
         return []
 
     def set_included_children(self, value):
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,33 +8,35 @@
 
 import aiofiles
 
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
-    base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    group_dict_attribute,
-    group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import PermissionSetMessageDetails
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
     AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE,
     AwsIdentityCenterPermissionSetTemplate,
     PermissionSetProperties,
 )
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.utils import (
     enrich_permission_set_details,
     get_permission_set_details,
     get_permission_set_users_and_groups,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
+from iambic.plugins.v0_1_0.aws.template_generation import (
+    base_group_str_attribute,
+    group_dict_attribute,
+    group_int_or_str_attribute,
+)
 from iambic.plugins.v0_1_0.aws.utils import (
     calculate_import_preference,
     get_aws_account_map,
 )
 
 # TODO: Update all grouping functions to support org grouping once multiple orgs with IdentityCenter is functional
 # TODO: Update partial import to support permission set only being deleted on a single org
@@ -52,15 +54,17 @@
 
 
 def get_templated_permission_set_file_path(
     permission_set_dir: str,
     permission_set_name: str,
 ):
     file_name = (
-        permission_set_name.replace("{{", "")
+        permission_set_name.replace(" ", "")
+        .replace("{{var.", "")
+        .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
     return str(os.path.join(permission_set_dir, f"{file_name}.yaml"))
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,39 +629,43 @@
                     new_value=template_inline_policy,
                 )
             )
 
         if ctx.execute:
             boto_action = "Creating" if not existing_inline_policy else "Updating"
             log_str = f"{log_str} {boto_action} InlinePolicyDocument..."
-            await boto_crud_call(
+            apply_awaitable = boto_crud_call(
                 identity_center_client.put_inline_policy_to_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
                 InlinePolicy=json.dumps(template_inline_policy),
             )
+            response = await plugin_apply_wrapper(apply_awaitable, response)
+
         log.debug(log_str, **log_params)
     elif not template_inline_policy and existing_inline_policy:
         log_str = "Stale InlinePolicyDocument."
         response.append(
             ProposedChange(
                 change_type=ProposedChangeType.DELETE,
                 attribute="inline_policy",
                 resource_type="aws:identity_center:permission_set",
                 resource_id=permission_set_arn,
                 current_value=existing_inline_policy,
             )
         )
         if ctx.execute:
             log_str = f"{log_str} Removing InlinePolicyDocument..."
-            await boto_crud_call(
+            apply_awaitable = boto_crud_call(
                 identity_center_client.delete_inline_policy_from_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
             )
+            response = await plugin_apply_wrapper(apply_awaitable, response)
+
         log.debug(log_str, **log_params)
 
     return response
 
 
 async def apply_permission_set_permission_boundary(
     identity_center_client,
@@ -709,20 +713,22 @@
                     new_value=template_permission_boundary,
                 )
             )
 
         if ctx.execute:
             boto_action = "Creating" if not existing_permission_boundary else "Updating"
             log_str = f"{log_str} {boto_action} PermissionsBoundary..."
-            await boto_crud_call(
+            apply_awaitable = boto_crud_call(
                 identity_center_client.put_permissions_boundary_to_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
                 PermissionsBoundary=template_permission_boundary,
             )
+            response = await plugin_apply_wrapper(apply_awaitable, response)
+
         log.debug(log_str, **log_params)
     elif existing_permission_boundary and not template_permission_boundary:
         log_str = "Removing PermissionsBoundary discovered."
         response.append(
             ProposedChange(
                 change_type=ProposedChangeType.DELETE,
                 resource_type="aws:identity_center:permission_set",
@@ -730,19 +736,21 @@
                 attribute="permissions_boundary",
                 current_value=existing_permission_boundary,
             )
         )
 
         if ctx.execute:
             log_str = f"{log_str} Deleting PermissionsBoundary..."
-            await boto_crud_call(
+            apply_awaitable = boto_crud_call(
                 identity_center_client.delete_permissions_boundary_from_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
             )
+            response = await plugin_apply_wrapper(apply_awaitable, response)
+
         log.debug(log_str, **log_params)
 
     return response
 
 
 async def apply_permission_set_tags(
     identity_center_client,
@@ -792,14 +800,15 @@
         proposed_changes = [
             ProposedChange(
                 change_type=ProposedChangeType.ATTACH,
                 resource_type="aws:identity_center:permission_set",
                 resource_id=permission_set_arn,
                 attribute="tags",
                 new_value=tag,
+                current_value=existing_tag_map.get(tag["Key"]),
             )
             for tag in tags_to_apply
         ]
         response.extend(proposed_changes)
 
         if ctx.execute:
             log_str = f"{log_str} Adding tags..."
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,26 +41,29 @@
 )
 
 yaml = YAML()
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 
-ARN_RE = r"(^arn:([^:]*):([^:]*):([^:]*):(|\*|[\d]{12}|cloudfront|aws|{{account_id}}):(.+)$)|^\*$"
+ARN_RE = r"(^arn:([^:]*):([^:]*):([^:]*):(|\*|[\d]{12}|cloudfront|aws|{{var.account_id}}):(.+)$)|^\*$"
 
 IAMBIC_HUB_ROLE_NAME = "IambicHubRole"
 IAMBIC_SPOKE_ROLE_NAME = "IambicSpokeRole"
 
 
 def get_hub_role_arn(account_id: str) -> str:
     return f"arn:aws:iam::{account_id}:role/{IAMBIC_HUB_ROLE_NAME}"
 
 
-def get_spoke_role_arn(account_id: str) -> str:
-    return f"arn:aws:iam::{account_id}:role/{IAMBIC_SPOKE_ROLE_NAME}"
+def get_spoke_role_arn(account_id: str, read_only=False) -> str:
+    spoke_role_postfix = "ReadOnly" if read_only else ""
+    return (
+        f"arn:aws:iam::{account_id}:role/{IAMBIC_SPOKE_ROLE_NAME}{spoke_role_postfix}"
+    )
 
 
 @yaml_object(yaml)
 class Partition(Enum):
     AWS = "aws"
     AWS_GOV = "aws-us-gov"
     AWS_CHINA = "aws-cn"
@@ -577,14 +580,18 @@
     account_rules: Optional[List[AWSOrgAccountRule]] = Field(
         [],
         description="A list of rules used to determine how organization accounts are handled",
     )
     hub_role_arn: str = Field(
         description="The role arn to assume into when making calls to the account",
     )
+    spoke_role_is_read_only: bool = Field(
+        False,
+        description="if true, the spoke role name is IambicSpokeRoleReadOnly",
+    )
 
     async def _create_org_account_instance(
         self, account: dict, session: boto3.Session
     ) -> Optional[AWSAccount]:
         """Create an AWSAccount instance from an AWS Organization account and account dict
 
         Evaluate rules to determine if the account should be added to the config and if it is a read-only account.
@@ -611,15 +618,17 @@
         aws_account = AWSAccount(
             account_id=account_id,
             account_name=account_name,
             org_id=self.org_id,
             variables=account["variables"],
             identity_center_details=identity_center_details,
             iambic_managed=account_rule.iambic_managed,
-            spoke_role_arn=get_spoke_role_arn(account_id),
+            spoke_role_arn=get_spoke_role_arn(
+                account_id, read_only=self.spoke_role_is_read_only
+            ),
             hub_session_info=dict(boto3_session=session),
             default_region=region_name,
             boto3_session_map={},
         )
         try:
             await aws_account.get_boto3_session()
             return aws_account
@@ -722,37 +731,66 @@
         log_params = dict(
             resource_type=self.resource_type, resource_id=self.resource_id
         )
         relevant_accounts = []
 
         for account in config.accounts:
             if evaluate_on_provider(self, account):
-                relevant_accounts.append(str(account))
+                relevant_accounts.append(account)
                 tasks.append(self._apply_to_account(account))
 
         if not relevant_accounts:
             if ctx.execute:
                 if self.deleted:
                     log_str = "Successfully removed resource."
                     self.delete()
                 else:
                     log_str = "No changes detected for resource."
-                log.info(log_str, accounts=relevant_accounts, **log_params)
+                log.info(log_str, **log_params)
 
             return template_changes
 
         if ctx.execute:
             log_str = "Applying changes to resource."
         else:
             log_str = "Detecting changes for resource."
 
-        log.info(log_str, accounts=relevant_accounts, **log_params)
+        relevant_accounts_str = [str(account) for account in relevant_accounts]
+        log.info(log_str, accounts=relevant_accounts_str, **log_params)
+
+        account_changes: list[AccountChangeDetails] = await asyncio.gather(
+            *tasks, return_exceptions=True
+        )
+        proposed_changes: list[AccountChangeDetails] = []
+        exceptions_seen = set()
+
+        for account_change in account_changes:
+            if isinstance(account_change, AccountChangeDetails):
+                proposed_changes.append(account_change)
+            else:
+                exceptions_seen.add(str(account_change))
+
+        if exceptions_seen:
+            exceptions_seen = list(exceptions_seen)
+            proposed_change_accounts = set(
+                change.account for change in proposed_changes
+            )
+            for aws_account in relevant_accounts:
+                if str(aws_account) in proposed_change_accounts:
+                    continue
+                proposed_changes.append(
+                    AccountChangeDetails(
+                        account=str(aws_account),
+                        resource_id=self.resource_id,
+                        resource_type=self.resource_type,
+                        exceptions_seen=exceptions_seen,
+                    )
+                )
 
-        account_changes: list[AccountChangeDetails] = await asyncio.gather(*tasks)
-        template_changes.extend_changes(account_changes)
+        template_changes.extend_changes(proposed_changes)
 
         if template_changes.exceptions_seen:
             if self.deleted:
                 cmd_verb = "removing"
             elif ctx.execute:
                 cmd_verb = "applying"
             else:
@@ -765,15 +803,15 @@
             else:
                 log_str = "Successfully applied resource changes."
         elif account_changes:
             log_str = "Successfully detected required resource changes."
         else:
             log_str = "No changes detected for resource."
 
-        log.info(log_str, accounts=relevant_accounts, **log_params)
+        log.info(log_str, accounts=relevant_accounts_str, **log_params)
         return template_changes
 
     @property
     def resource_id(self):
         return self.properties.resource_id
 
     @property
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import asyncio
 import re
-from datetime import datetime, timezone
 from enum import Enum
 from typing import TYPE_CHECKING, Optional, Union
 
 import boto3
 from botocore.exceptions import ClientError, NoCredentialsError
 
 from iambic.core.iambic_enum import IambicManaged
@@ -209,73 +208,14 @@
     # cn_north_1 = "cn-north-1"
 
 
 def is_valid_account_id(account_id: str):
     return bool(re.match(r"^\d{12}$", account_id))
 
 
-async def remove_expired_resources(
-    resource,
-    template_resource_type: str,
-    template_resource_id: str,
-    delete_resource_if_expired: bool = True,
-):
-    from iambic.core.models import BaseModel
-
-    if not isinstance(resource, BaseModel):
-        return resource
-
-    log_params = {}
-    if hasattr(resource, "resource_type"):
-        log_params["resource_type"] = resource.resource_type
-    if hasattr(resource, "resource_id"):
-        log_params["resource_id"] = resource.resource_id
-    if template_resource_type != log_params.get(
-        "resource_type"
-    ) or template_resource_id != log_params.get("resource_id"):
-        log_params["parent_resource_type"] = template_resource_type
-        log_params["parent_resource_id"] = template_resource_id
-
-    if isinstance(resource, BaseModel) and hasattr(resource, "expires_at"):
-        if resource.expires_at:
-            cur_time = datetime.now(tz=timezone.utc)
-            if resource.expires_at < cur_time:
-                log.info("Expired resource found, marking for deletion", **log_params)
-                resource.deleted = True
-                return resource
-
-    for field_name in resource.__fields__.keys():
-        field_val = getattr(resource, field_name)
-        if isinstance(field_val, list):
-            new_value = await asyncio.gather(
-                *[
-                    remove_expired_resources(
-                        elem, template_resource_type, template_resource_id
-                    )
-                    for elem in field_val
-                ]
-            )
-            setattr(resource, field_name, new_value)
-            if delete_resource_if_expired:
-                for elem in new_value:
-                    if getattr(elem, "deleted", None) is True:
-                        new_value.remove(elem)
-                        setattr(resource, field_name, new_value)
-        else:
-            new_value = await remove_expired_resources(
-                field_val, template_resource_type, template_resource_id
-            )
-            if getattr(new_value, "deleted", None) is True:
-                setattr(resource, field_name, None)
-            else:
-                setattr(resource, field_name, new_value)
-
-    return resource
-
-
 async def set_org_account_variables(client, account: dict) -> dict:
     tags = await legacy_paginated_search(
         client.list_tags_for_resource, "Tags", ResourceId=account["Id"]
     )
     account["variables"] = [
         {"key": tag["Key"], "value": tag.get("Value")} for tag in tags
     ]
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.example.handlers import import_example_resources, load
 from iambic.plugins.v0_1_0.example.local_database.models import (
     ExampleLocalDatabaseTemplate,
 )
-from iambic.plugins.v0_1_0.example.local_file.models import ExampleLocalFileTemplate
+from iambic.plugins.v0_1_0.example.local_file.models import (
+    ExampleLocalFileMultiAccountTemplate,
+    ExampleLocalFileTemplate,
+)
 
 
 class ExampleConfig(BaseModel):
     pass
 
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="example",
     version=PLUGIN_VERSION,
     provider_config=ExampleConfig,
     requires_secret=True,
     async_import_callable=import_example_resources,
     async_load_callable=load,
-    templates=[ExampleLocalFileTemplate, ExampleLocalDatabaseTemplate],
+    templates=[
+        ExampleLocalFileTemplate,
+        ExampleLocalFileMultiAccountTemplate,
+        ExampleLocalDatabaseTemplate,
+    ],
 )
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from pydantic import Field
 
 from iambic.core.models import (
     BaseModel,
     BaseTemplate,
     ExpiryModel,
     ProposedChange,
     ProposedChangeType,
     TemplateChangeDetails,
 )
 
 EXAMPLE_LOCAL_FILE_TEMPLATE_TYPE = "NOQ::Example::LocalFile"
+EXAMPLE_LOCAL_FILE_MULTI_ACCOUNT_TEMPLATE_TYPE = "NOQ::Example::LocalFileMultiAccount"
 
 if TYPE_CHECKING:
     from iambic.plugins.v0_1_0.example.iambic_plugin import ExampleConfig
 
 
 class ExampleLocalFileTemplateProperties(BaseModel):
     name: str = Field(..., description="name of local file")
@@ -44,14 +45,62 @@
 
     @property
     def resource_id(self) -> str:
         return self.name
 
     async def apply(self, config: ExampleConfig) -> TemplateChangeDetails:
         template_changes = TemplateChangeDetails(
+            resource_id=self.resource_id,
+            resource_type=self.template_type,
+            template_path=self.file_path,
+        )
+        if self.delete:
+            template_changes.proposed_changes = [
+                ProposedChange(change_type=ProposedChangeType.DELETE)
+            ]
+        else:
+            template_changes.proposed_changes = []
+        return template_changes
+
+
+class ExampleLocalFileMultiAccountTemplateProperties(BaseTemplate, ExpiryModel):
+    name: str = Field(..., description="name of local file")
+
+    @property
+    def resource_type(self) -> str:
+        return "example:local_file_multi_account:properties"
+
+    @property
+    def resource_id(self) -> str:
+        return self.name
+
+
+class ExampleLocalFileMultiAccountTemplate(BaseTemplate, ExpiryModel):
+    template_type = EXAMPLE_LOCAL_FILE_MULTI_ACCOUNT_TEMPLATE_TYPE
+    properties: ExampleLocalFileTemplateProperties = Field(
+        ..., description="Properties for Example Local File Template"
+    )
+    name: str = Field(..., description="name of local file")
+    included_accounts: Optional[list] = Field(
+        ..., description="list of accounts to include"
+    )
+    excluded_accounts: Optional[list] = Field(
+        ..., description="list of accounts to exclude"
+    )
+
+    @property
+    def resource_type(self) -> str:
+        return "example:local_file_multi_account"
+
+    @property
+    def resource_id(self) -> str:
+        return self.name
+
+    async def apply(self, config: ExampleConfig) -> TemplateChangeDetails:
+        template_changes = TemplateChangeDetails(
             resource_id=self.resource_id,
             resource_type=self.template_type,
             template_path=self.file_path,
         )
         if self.delete:
             template_changes.proposed_changes = [
                 ProposedChange(change_type=ProposedChangeType.DELETE)
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,19 +185,14 @@
                 # Don't overwrite a resource during config discovery
                 change_details.new_value = {}
                 return change_details
 
         app_exists = bool(current_app)
         tasks = []
 
-        # Marking for deletion. This shouldn't be done on the fly.
-        # self = await remove_expired_resources(
-        #     self, self.resource_type, self.resource_id
-        # )
-
         if not app_exists and not self.deleted:
             log.error(
                 "Iambic does not support creating new apps. "
                 "Please create the app in Okta and then import it.",
                 **log_params,
             )
             return change_details
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from typing import TYPE_CHECKING, List, Optional
 
 import okta.models as models
+from okta.models.user_status import UserStatus as OktaUserStatus
+
 from iambic.core.context import ctx
 from iambic.core.logger import log
 from iambic.core.models import ProposedChange, ProposedChangeType
 from iambic.core.utils import GlobalRetryController
 from iambic.plugins.v0_1_0.okta.models import Group, User
 from iambic.plugins.v0_1_0.okta.utils import generate_user_profile, handle_okta_fn
 
@@ -25,18 +27,28 @@
     - okta_organization: An instance of the OktaOrganization class, which provides access to the Okta API.
 
     Returns:
     - A list of `User` instances, representing the users in Okta.
     """
 
     client = await okta_organization.get_okta_client()
+
+    filter_operator = " OR ".join(
+        [
+            f'status eq "{status}"'
+            for status in list(map(lambda s: s.name, list(OktaUserStatus)))
+        ]
+    )
+
     async with GlobalRetryController(
         fn_identifier="okta.list_users"
     ) as retry_controller:
-        fn = functools.partial(client.list_users)
+        fn = functools.partial(
+            client.list_users, query_params=dict(filter=filter_operator)
+        )
         users, resp, err = await retry_controller(handle_okta_fn, fn)
         if err:
             log.error("Error encountered when listing users", error=str(err))
             raise Exception(f"Error listing users: {str(err)}")
 
     while resp.has_next():
         async with GlobalRetryController(
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
-from okta.client import Client as OktaClient
 from pydantic import BaseModel, Extra, Field, SecretStr, validator
 
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.okta.app.models import OktaAppTemplate
 from iambic.plugins.v0_1_0.okta.group.models import OktaGroupTemplate
 from iambic.plugins.v0_1_0.okta.handlers import import_okta_resources, load
 from iambic.plugins.v0_1_0.okta.user.models import OktaUserTemplate
+from okta.client import Client as OktaClient
 
 
 class OktaOrganization(BaseModel):
     idp_name: str
     org_url: str
     api_token: SecretStr
     request_timeout: int = 60
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,16 @@
 
             current_user: User = await create_user(
                 self,
                 okta_organization=okta_organization,
             )
             if current_user:
                 change_details.current_value = current_user
+                self.properties.user_id = current_user.user_id
+                self.write()
         if (
             current_user
             and self.deleted
             and current_user.status == UserStatus.deprovisioned
             and proposed_user.get("status") == "deprovisioned"
             and not self.force_delete
         ):
@@ -250,15 +252,15 @@
                     self,
                     current_user,
                     self.properties.profile,
                     okta_organization,
                     log_params,
                 ),
                 maybe_deprovision_user(
-                    self.deleted,
+                    bool(self.deleted),
                     current_user,
                     okta_organization,
                     log_params,
                 ),
             ]
         )
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from typing import TYPE_CHECKING, Any, List, Optional
 
 import okta.models as models
-
 from iambic.core.context import ctx
 from iambic.core.exceptions import RateLimitException
 from iambic.core.logger import log
 from iambic.core.models import ProposedChange, ProposedChangeType
 from iambic.core.utils import GlobalRetryController
 from iambic.plugins.v0_1_0.okta.exceptions import UserProfileNotUpdatableYet
 from iambic.plugins.v0_1_0.okta.models import User
@@ -251,69 +250,68 @@
     """
     response: list = []
     if not user:
         return response
     current_status: str = user.status.value
     if current_status == new_status:
         return response
-    if new_status == "deprovisioned":
-        # maybe_deprovision_user is called in the main loop
-        # and handles this use case
-        return response
     response.append(
         ProposedChange(
             change_type=ProposedChangeType.UPDATE,
             resource_id=user.user_id,
             resource_type=user.resource_type,
             attribute="status",
             change_summary={
                 "current_status": current_status,
                 "proposed_status": new_status,
             },
             current_value=current_status,
             new_value=new_status,
         )
     )
+
+    # TODO: refactor to use an state machine approach
+    method = "POST"
+    base_endpoint = f"/api/v1/users/{user.user_id}"
+    if current_status == "suspended" and new_status == "active":
+        api_endpoint = f"{base_endpoint}/lifecycle/unsuspend"
+    elif current_status == "active" and new_status == "suspended":
+        api_endpoint = f"{base_endpoint}/lifecycle/suspend"
+    elif new_status == "deprovisioned" and current_status != "deprovisioned":
+        api_endpoint = f"{base_endpoint}/lifecycle/deactivate"
+    elif current_status in ["staged", "deprovisioned"] and new_status in [
+        "active",
+        "provisioned",
+    ]:
+        api_endpoint = f"{base_endpoint}/lifecycle/activate"
+    elif current_status in "provisioned" and new_status == "active":
+        api_endpoint = f"{base_endpoint}/lifecycle/reactivate"
+    elif current_status == "locked_out" and new_status == "active":
+        api_endpoint = f"{base_endpoint}/lifecycle/unlock"
+    elif new_status == "recovery":
+        api_endpoint = f"{base_endpoint}/lifecycle/reset_password"
+    elif new_status == "password_expired":
+        api_endpoint = f"{base_endpoint}/lifecycle/expire_password"
+    elif new_status == "deleted":
+        api_endpoint = f"{base_endpoint}"
+        method = "DELETE"
+    else:
+        log.error(
+            "Error updating user status",
+            user=user.username,
+            current_status=current_status,
+            new_status=new_status,
+            **log_params,
+        )
+        raise Exception(
+            f"Error updating user status. Invalid transition from {current_status} to {new_status}"
+        )
+
     if ctx.execute:
         client = await okta_organization.get_okta_client()
-        method = "POST"
-        base_endpoint = f"/api/v1/users/{user.user_id}"
-        if current_status == "suspended" and new_status == "active":
-            api_endpoint = f"{base_endpoint}/lifecycle/unsuspend"
-        elif current_status == "active" and new_status == "suspended":
-            api_endpoint = f"{base_endpoint}/lifecycle/suspend"
-        elif new_status == "deprovisioned" and current_status != "deprovisioned":
-            api_endpoint = f"{base_endpoint}/lifecycle/deactivate"
-        elif current_status in ["staged", "deprovisioned"] and new_status in [
-            "active",
-            "provisioned",
-        ]:
-            api_endpoint = f"{base_endpoint}/lifecycle/activate"
-        elif current_status in "provisioned" and new_status == "active":
-            api_endpoint = f"{base_endpoint}/lifecycle/reactivate"
-        elif current_status == "locked_out" and new_status == "active":
-            api_endpoint = f"{base_endpoint}/lifecycle/unlock"
-        elif new_status == "recovery":
-            api_endpoint = f"{base_endpoint}/lifecycle/reset_password"
-        elif new_status == "password_expired":
-            api_endpoint = f"{base_endpoint}/lifecycle/expire_password"
-        elif new_status == "deleted":
-            api_endpoint = f"{base_endpoint}"
-            method = "DELETE"
-        else:
-            log.error(
-                "Error updating user status",
-                user=user.username,
-                current_status=current_status,
-                new_status=new_status,
-                **log_params,
-            )
-            raise Exception(
-                f"Error updating user status. Invalid transition from {current_status} to {new_status}"
-            )
         request, error = await client.get_request_executor().create_request(
             method=method, url=api_endpoint, body={}, headers={}, oauth=False
         )
         if error:
             log.error(
                 "Error updating user status",
                 error=error,
```

### Comparing `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.3.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/request_handler/expire_resources.py` & `iambic_core-0.3.1/iambic/request_handler/expire_resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 
 from iambic.core.logger import log
 from iambic.core.parser import load_templates
-from iambic.plugins.v0_1_0.aws.utils import remove_expired_resources
+from iambic.core.utils import remove_expired_resources
 
 
 async def flag_expired_resources(template_paths: list[str]):
     # Warning: The dynamic config must be loaded before this is called.
     #   This is done using iambic.config.dynamic_config.load_config(config_path)
     log.info("Scanning for expired resources")
     templates = await asyncio.gather(
```

### Comparing `iambic_core-0.2.1/iambic/request_handler/git_apply.py` & `iambic_core-0.3.1/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/request_handler/git_plan.py` & `iambic_core-0.3.1/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.3.1/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import random
 from multiprocessing import Pipe, Process, TimeoutError
 from multiprocessing.connection import Connection
 from time import time
 from typing import Any, Dict, Iterable, List, Tuple, Union
 from uuid import UUID, uuid4
```

### Comparing `iambic_core-0.2.1/pyproject.toml` & `iambic_core-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.2.1"
+version = "0.3.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.2.1/PKG-INFO` & `iambic_core-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.2.1
+Version: 0.3.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -98,22 +98,22 @@
 
 Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
 result in the creation of three roles: "dev_cloudwatch",
 "staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
-identifier: '{{account_name}}_cloudwatch'
+identifier: '{{var.account_name}}_cloudwatch'
 included_accounts:
     - dev
     - staging
     - prod
 properties:
   description:
-    - description: Cloudwatch role for {{account_name}}
+    - description: Cloudwatch role for {{var.account_name}}
   assume_role_policy_document:
     statement:
       - action:
           - sts:AssumeRole
           - sts:TagSession
         effect: Allow
         principal:
@@ -132,34 +132,34 @@
             - logs:TestMetricFilter
             - logs:FilterLogEvents
             - logs:StartQuery
             - logs:StopQuery
         resource: "*"
   managed_policies:
     - policy_arn: arn:aws:iam::aws:policy/AdministratorAccess
-  role_name: '{{account_name}}_cloudwatch'
+  role_name: '{{var.account_name}}_cloudwatch'
   tags:
     - key: owner
       value: devops
 ```
 
 ### AWS Dynamic Permissions
 
 Create a BackendDeveloperRole with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
-identifier: '{{account_name}}_backend_developer'
+identifier: '{{var.account_name}}_backend_developer'
 included_accounts:
   - '*'
 excluded_accounts:
   - compliance
 properties:
   description:
-    - description: Backend developer role for {{account_name}}
+    - description: Backend developer role for {{var.account_name}}
   assume_role_policy_document:
     statement:
       - action:
           - sts:AssumeRole
           - sts:TagSession
         effect: Allow
         principal:
@@ -187,15 +187,15 @@
           action:
               - s3:PutObject
           resource:
               - "*"
           condition:
                 StringNotEquals:
                     s3:ResourceTag/sensitive: 'true'
-  role_name: '{{account_name}}_backend_developer'
+  role_name: '{{var.account_name}}_backend_developer'
   tags:
     - key: owner
       value: devops
 ```
 
 ### Okta Application Assignments
 
@@ -278,14 +278,18 @@
   description: A test group to use with IAMbic
   members:
     - name: user@example.com
       data_type: user
       expires_at: tomorrow
 ```
 
+## Preview standalone IAMbic templates repository
+
+Preview a standalone [IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) on how IAMbic tracks multi-cloud IAM assets in GitHub. The repository is made public for you to study. No need to make your repository public.
+
 ## IAMbic - Beta Software
 
 IAMbic is currently in beta, and is not yet recommended for use in production environments. We are actively working to improve the stability and performance of the software, and welcome feedback from the community.
 
 If you choose to use IAMbic in its current state, please be aware that you may encounter bugs, performance issues, or other unexpected behavior. We strongly recommend testing IAMbic thoroughly in a non-production environment before using it in production.
 
 Please report any issues or feedback to our GitHub issue tracker. Thank you for your support and contributions to the project!
```

