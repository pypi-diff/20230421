# Comparing `tmp/ignf_gpf_api-0.1.7.tar.gz` & `tmp/ignf_gpf_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignf_gpf_api-0.1.7.tar", last modified: Fri Mar 31 12:00:54 2023, max compression
+gzip compressed data, was "ignf_gpf_api-0.1.8.tar", last modified: Fri Apr 21 17:10:34 2023, max compression
```

## Comparing `ignf_gpf_api-0.1.7.tar` & `ignf_gpf_api-0.1.8.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     1400 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.github/workflows/ci-dev.yml
--rw-r--r--   0        0        0     1394 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.github/workflows/ci-prod.yml
--rw-r--r--   0        0        0      844 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0     1881 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.gitignore
--rw-r--r--   0        0        0    23461 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.pylintrc
--rw-r--r--   0        0        0      200 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.pypirc
--rw-r--r--   0        0        0     1981 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/.vscode/settings.json
--rw-r--r--   0        0        0    35149 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/LICENSE
--rw-r--r--   0        0        0      122 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/MANIFEST.in
--rw-r--r--   0        0        0      415 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/README.md
--rwxr-xr-x   0        0        0      510 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/check.sh
--rw-r--r--   0        0        0     1956 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docker/Dockerfile
--rw-r--r--   0        0        0      671 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docker/README.md
--rw-r--r--   0        0        0      244 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docker/config/apache/website.conf
--rw-r--r--   0        0        0      291 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docker/docker-compose.yml
--rw-r--r--   0        0        0       42 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/.gitignore
--rw-r--r--   0        0        0     3083 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/comme-executable.md
--rw-r--r--   0        0        0       34 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/comme-module.md
--rw-r--r--   0        0        0     4133 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/configuration.md
--rw-r--r--   0        0        0    23974 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/configuration_details.md
--rw-r--r--   0        0        0      358 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/custom.css
--rw-r--r--   0        0        0     3577 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/development.md
--rw-r--r--   0        0        0    12108 2023-03-31 12:00:50.404129 ignf_gpf_api-0.1.7/docs/images/index__utilisation_module.excalidraw
--rw-r--r--   0        0        0   241521 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/images/index__utilisation_module.png
--rw-r--r--   0        0        0     1223 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/index.md
--rw-r--r--   0        0        0      115 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/reference/auth.md
--rw-r--r--   0        0        0      234 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/reference/io.md
--rw-r--r--   0        0        0      302 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/reference/store.md
--rw-r--r--   0        0        0       60 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/reference/workflow.md
--rw-r--r--   0        0        0      290 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/reference/workflow/action.md
--rw-r--r--   0        0        0      340 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/reference/workflow/resolver.md
--rw-r--r--   0        0        0     5356 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/tutoriel_1_archive.md
--rw-r--r--   0        0        0     4551 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/tutoriel_2_flux_vecteur.md
--rw-r--r--   0        0        0     4171 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/upload_descriptor.md
--rw-r--r--   0        0        0       12 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/docs/workflow.md
--rw-r--r--   0        0        0      687 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/Errors.py
--rw-r--r--   0        0        0       82 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/__init__.py
--rw-r--r--   0        0        0    15799 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/__main__.py
--rw-r--r--   0        0        0     8997 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_conf/default.ini
--rw-r--r--   0        0        0     2247 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json
--rw-r--r--   0        0        0     3001 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_conf/json_schemas/workflow.json
--rw-r--r--   0        0        0      285 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON.md5
--rwxr-xr-x   0        0        0        5 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2297 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
--rwxr-xr-x   0        0        0      449 2023-03-31 12:00:50.408129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
--rw-r--r--   0        0        0   430828 2023-03-31 12:00:50.412129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
--rw-r--r--   0        0        0      588 2023-03-31 12:00:50.412129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
--rw-r--r--   0        0        0      529 2023-03-31 12:00:50.412129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json
--rw-r--r--   0        0        0       57 2023-03-31 12:00:50.412129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON.md5
--rw-r--r--   0        0        0   991843 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
--rw-r--r--   0        0        0      525 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json
--rw-r--r--   0        0        0     4798 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/workflows/archive-generic.jsonc
--rw-r--r--   0        0        0     8404 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/_data/workflows/wfs-generic.jsonc
--rw-r--r--   0        0        0     5790 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/auth/Authentifier.py
--rw-r--r--   0        0        0      270 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/auth/Errors.py
--rw-r--r--   0        0        0     1493 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/auth/Token.py
--rw-r--r--   0        0        0       46 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/auth/__init__.py
--rw-r--r--   0        0        0     2585 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/helper/FileHelper.py
--rw-r--r--   0        0        0     6947 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/helper/JsonHelper.py
--rw-r--r--   0        0        0      916 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/helper/PrintLogHelper.py
--rw-r--r--   0        0        0       59 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/helper/__init__.py
--rw-r--r--   0        0        0    11135 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/ApiRequester.py
--rw-r--r--   0        0        0      607 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/Color.py
--rw-r--r--   0        0        0     5018 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/Config.py
--rw-r--r--   0        0        0     5310 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/Dataset.py
--rw-r--r--   0        0        0     4037 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/DescriptorFileReader.py
--rw-r--r--   0        0        0     7308 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/Errors.py
--rw-r--r--   0        0        0     2752 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/JsonConverter.py
--rw-r--r--   0        0        0     4379 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/OutputManager.py
--rw-r--r--   0        0        0       47 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/io/__init__.py
--rw-r--r--   0        0        0      793 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/pattern/SingleInstance.py
--rw-r--r--   0        0        0      637 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/pattern/Singleton.py
--rw-r--r--   0        0        0       33 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/pattern/__init__.py
--rw-r--r--   0        0        0        1 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/py.typed
--rw-r--r--   0        0        0      218 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Check.py
--rw-r--r--   0        0        0     1025 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/CheckExecution.py
--rw-r--r--   0        0        0     1947 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Configuration.py
--rw-r--r--   0        0        0     2002 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Endpoint.py
--rw-r--r--   0        0        0      179 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Errors.py
--rw-r--r--   0        0        0      608 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Offering.py
--rw-r--r--   0        0        0      227 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Processing.py
--rw-r--r--   0        0        0     2378 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/ProcessingExecution.py
--rw-r--r--   0        0        0    11618 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/StoreEntity.py
--rw-r--r--   0        0        0      699 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/StoredData.py
--rw-r--r--   0        0        0     7653 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/Upload.py
--rw-r--r--   0        0        0       57 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/__init__.py
--rw-r--r--   0        0        0     2397 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/CommentInterface.py
--rw-r--r--   0        0        0     1047 2023-03-31 12:00:50.416129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/CsfInterface.py
--rw-r--r--   0        0        0      767 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/EventInterface.py
--rw-r--r--   0        0        0      789 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/FullEditInterface.py
--rw-r--r--   0        0        0      831 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/PartialEditInterface.py
--rw-r--r--   0        0        0     2014 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/SharingInterface.py
--rw-r--r--   0        0        0     2255 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/TagInterface.py
--rw-r--r--   0        0        0       88 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/__init__.py
--rw-r--r--   0        0        0      204 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/Errors.py
--rw-r--r--   0        0        0    14121 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/Workflow.py
--rw-r--r--   0        0        0       40 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/__init__.py
--rw-r--r--   0        0        0     4424 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/ActionAbstract.py
--rw-r--r--   0        0        0     5031 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/ConfigurationAction.py
--rw-r--r--   0        0        0     4304 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/OfferingAction.py
--rw-r--r--   0        0        0    15865 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py
--rw-r--r--   0        0        0    11298 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/UploadAction.py
--rw-r--r--   0        0        0       72 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/__init__.py
--rw-r--r--   0        0        0      802 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/AbstractResolver.py
--rw-r--r--   0        0        0     1271 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/DictResolver.py
--rw-r--r--   0        0        0     4333 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/Errors.py
--rw-r--r--   0        0        0     5295 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/FileResolver.py
--rw-r--r--   0        0        0     3469 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/GlobalResolver.py
--rw-r--r--   0        0        0     3489 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py
--rw-r--r--   0        0        0     1462 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/UserResolver.py
--rw-r--r--   0        0        0      110 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/__init__.py
--rw-r--r--   0        0        0     1757 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/mkdocs.yml
--rw-r--r--   0        0        0     1280 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      956 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/ErrorsTestCase.py
--rw-r--r--   0        0        0     1735 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/GpfTestCase.py
--rw-r--r--   0        0        0     3366 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/MainTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      336 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_conf/test_authentifier.ini
--rw-r--r--   0        0        0      308 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_conf/test_overload.ini
--rw-r--r--   0        0        0      313 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_conf/test_requester.ini
--rw-r--r--   0        0        0       40 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_conf/test_upload.ini
--rw-r--r--   0        0        0       69 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_conf/test_value_type.ini
--rw-r--r--   0        0        0      460 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
--rw-r--r--   0        0        0      341 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
--rw-r--r--   0        0        0        5 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2023-03-31 12:00:50.420129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
--rw-r--r--   0        0        0       11 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
--rw-r--r--   0        0        0        5 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2023-03-31 12:00:50.428129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
--rw-r--r--   0        0        0     2659 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_data/workflows/bad-workflow.jsonc
--rw-r--r--   0        0        0       53 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/helper/FileHelper/md5.txt
--rw-r--r--   0        0        0       78 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/helper/JsonHelper/json_not_parsable.json
--rw-r--r--   0        0        0       52 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/helper/JsonHelper/json_not_valid.json
--rw-r--r--   0        0        0      108 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/helper/JsonHelper/json_parsable.json
--rw-r--r--   0        0        0      563 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/helper/JsonHelper/schema.json
--rw-r--r--   0        0        0      485 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/helper/JsonHelper/schema_invalid.json
--rw-r--r--   0        0        0       23 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/workflow/resolver/FileResolver/dict.json
--rw-r--r--   0        0        0       21 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/workflow/resolver/FileResolver/list.json
--rw-r--r--   0        0        0        2 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/workflow/resolver/FileResolver/not-valid.json
--rw-r--r--   0        0        0       31 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/_test/workflow/resolver/FileResolver/text.txt
--rw-r--r--   0        0        0     7383 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/auth/AuthentifierTestCase.py
--rw-r--r--   0        0        0     1183 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/auth/TokenTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/auth/__init__.py
--rw-r--r--   0        0        0     1056 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/helper/FileHelperTestCase.py
--rw-r--r--   0        0        0     9959 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/helper/JsonHelperTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/helper/__init__.py
--rw-r--r--   0        0        0    13575 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/ApiRequesterTestCase.py
--rw-r--r--   0        0        0     3595 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/ConfigTestCase.py
--rw-r--r--   0        0        0     2218 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/DatasetTestCase.py
--rw-r--r--   0        0        0     1716 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/DescriptorFileReaderTestCase.py
--rw-r--r--   0        0        0     1974 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/ErrorsTestCase.py
--rw-r--r--   0        0        0     1198 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/JsonConverterTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/io/__init__.py
--rw-r--r--   0        0        0     1431 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/CheckExecutionTestCase.py
--rw-r--r--   0        0        0     2855 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/ConfigurationTestCase.py
--rw-r--r--   0        0        0     3487 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/EndpointTestCase.py
--rw-r--r--   0        0        0     1144 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/ErrorsTestCase.py
--rw-r--r--   0        0        0     1503 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/EventInterfaceTestCase.py
--rw-r--r--   0        0        0     3865 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/ProcessingExecutionTestCase.py
--rw-r--r--   0        0        0    18439 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/StoreEntityTestCase.py
--rw-r--r--   0        0        0    11477 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/UploadTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/__init__.py
--rw-r--r--   0        0        0     4538 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/CommentInterfaceTestCase.py
--rw-r--r--   0        0        0     2532 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/CsfInterfaceTestCase.py
--rw-r--r--   0        0        0     1699 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/FullEditInterfaceTestCase.py
--rw-r--r--   0        0        0     1745 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/PartialEditInterfaceTestCase.py
--rw-r--r--   0        0        0     3585 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/SharingInterfaceTestCase.py
--rw-r--r--   0        0        0     3600 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/TagInterfaceTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/store/interface/__init__.py
--rw-r--r--   0        0        0    14646 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/WorkflowTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/__init__.py
--rw-r--r--   0        0        0     3100 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/action/ActionAbstractTestCase.py
--rw-r--r--   0        0        0     5384 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/action/ConfigurationActionTestCase.py
--rw-r--r--   0        0        0     7133 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/action/OfferingActionTestCase.py
--rw-r--r--   0        0        0    16012 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/action/ProcessingExecutionActionTestCase.py
--rw-r--r--   0        0        0    19409 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/action/UploadActionTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/action/__init__.py
--rw-r--r--   0        0        0     1116 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/resolver/DictResolverTestCase.py
--rw-r--r--   0        0        0     4492 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/resolver/FileResolverTestCase.py
--rw-r--r--   0        0        0     2492 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/resolver/GlobalResolverTestCase.py
--rw-r--r--   0        0        0     6705 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/resolver/StoreEntityResolverTestCase.py
--rw-r--r--   0        0        0     2225 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/resolver/UserResolverTestCase.py
--rw-r--r--   0        0        0        0 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/tests/workflow/resolver/__init__.py
--rw-r--r--   0        0        0   116760 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/uml/classes.png
--rw-r--r--   0        0        0     9175 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/uml/classes.uxf
--rw-r--r--   0        0        0    43510 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/uml/interfaces.png
--rw-r--r--   0        0        0     7059 2023-03-31 12:00:50.440129 ignf_gpf_api-0.1.7/uml/interfaces.uxf
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 ignf_gpf_api-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1400 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.github/workflows/ci-dev.yml
+-rw-r--r--   0        0        0     1394 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.github/workflows/ci-prod.yml
+-rw-r--r--   0        0        0      844 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0     1881 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.gitignore
+-rw-r--r--   0        0        0    23461 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.pylintrc
+-rw-r--r--   0        0        0      200 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.pypirc
+-rw-r--r--   0        0        0     1981 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.vscode/settings.json
+-rw-r--r--   0        0        0    35149 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/LICENSE
+-rw-r--r--   0        0        0      122 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/MANIFEST.in
+-rw-r--r--   0        0        0      415 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/README.md
+-rwxr-xr-x   0        0        0      510 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/check.sh
+-rw-r--r--   0        0        0     1956 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/Dockerfile
+-rw-r--r--   0        0        0      671 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/README.md
+-rw-r--r--   0        0        0      244 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/config/apache/website.conf
+-rw-r--r--   0        0        0      291 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/docker-compose.yml
+-rw-r--r--   0        0        0       42 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/.gitignore
+-rw-r--r--   0        0        0     3083 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/comme-executable.md
+-rw-r--r--   0        0        0       34 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/comme-module.md
+-rw-r--r--   0        0        0     4133 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/configuration.md
+-rw-r--r--   0        0        0    23974 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/configuration_details.md
+-rw-r--r--   0        0        0      358 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/custom.css
+-rw-r--r--   0        0        0     3577 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/development.md
+-rw-r--r--   0        0        0    12108 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.excalidraw
+-rw-r--r--   0        0        0   241521 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.png
+-rw-r--r--   0        0        0     1223 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/index.md
+-rw-r--r--   0        0        0      115 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/auth.md
+-rw-r--r--   0        0        0      234 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/io.md
+-rw-r--r--   0        0        0      302 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/store.md
+-rw-r--r--   0        0        0       60 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/workflow.md
+-rw-r--r--   0        0        0      290 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/workflow/action.md
+-rw-r--r--   0        0        0      340 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/workflow/resolver.md
+-rw-r--r--   0        0        0     5356 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/tutoriel_1_archive.md
+-rw-r--r--   0        0        0     4551 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/tutoriel_2_flux_vecteur.md
+-rw-r--r--   0        0        0     4171 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/upload_descriptor.md
+-rw-r--r--   0        0        0       12 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/workflow.md
+-rw-r--r--   0        0        0      687 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/Errors.py
+-rw-r--r--   0        0        0       82 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/__init__.py
+-rw-r--r--   0        0        0    15799 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/__main__.py
+-rw-r--r--   0        0        0     8997 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/default.ini
+-rw-r--r--   0        0        0     2247 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json
+-rw-r--r--   0        0        0     3001 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/workflow.json
+-rw-r--r--   0        0        0      285 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON.md5
+-rwxr-xr-x   0        0        0        5 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2297 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
+-rwxr-xr-x   0        0        0      449 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
+-rw-r--r--   0        0        0   430828 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      588 2023-04-21 17:10:28.531663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
+-rw-r--r--   0        0        0      529 2023-04-21 17:10:28.531663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json
+-rw-r--r--   0        0        0       57 2023-04-21 17:10:28.531663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON.md5
+-rw-r--r--   0        0        0   991843 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
+-rw-r--r--   0        0        0      525 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json
+-rw-r--r--   0        0        0     4798 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/archive-generic.jsonc
+-rw-r--r--   0        0        0     8404 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/wfs-generic.jsonc
+-rw-r--r--   0        0        0     5790 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Authentifier.py
+-rw-r--r--   0        0        0      270 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Errors.py
+-rw-r--r--   0        0        0     1493 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Token.py
+-rw-r--r--   0        0        0       46 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/FileHelper.py
+-rw-r--r--   0        0        0     6947 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/JsonHelper.py
+-rw-r--r--   0        0        0      916 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/PrintLogHelper.py
+-rw-r--r--   0        0        0       59 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/__init__.py
+-rw-r--r--   0        0        0    11135 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/ApiRequester.py
+-rw-r--r--   0        0        0      607 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Color.py
+-rw-r--r--   0        0        0     5018 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Config.py
+-rw-r--r--   0        0        0     5310 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Dataset.py
+-rw-r--r--   0        0        0     4037 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/DescriptorFileReader.py
+-rw-r--r--   0        0        0     7308 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Errors.py
+-rw-r--r--   0        0        0     2752 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/JsonConverter.py
+-rw-r--r--   0        0        0     4379 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/OutputManager.py
+-rw-r--r--   0        0        0       47 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/__init__.py
+-rw-r--r--   0        0        0      793 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/SingleInstance.py
+-rw-r--r--   0        0        0      637 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/Singleton.py
+-rw-r--r--   0        0        0       33 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/py.typed
+-rw-r--r--   0        0        0      218 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Check.py
+-rw-r--r--   0        0        0     1025 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/CheckExecution.py
+-rw-r--r--   0        0        0     1947 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Configuration.py
+-rw-r--r--   0        0        0     2002 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Endpoint.py
+-rw-r--r--   0        0        0      179 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Errors.py
+-rw-r--r--   0        0        0      608 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Offering.py
+-rw-r--r--   0        0        0      227 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Processing.py
+-rw-r--r--   0        0        0     2378 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/ProcessingExecution.py
+-rw-r--r--   0        0        0    11618 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoreEntity.py
+-rw-r--r--   0        0        0      699 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoredData.py
+-rw-r--r--   0        0        0     7653 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Upload.py
+-rw-r--r--   0        0        0       57 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/__init__.py
+-rw-r--r--   0        0        0     2397 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CommentInterface.py
+-rw-r--r--   0        0        0     1047 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CsfInterface.py
+-rw-r--r--   0        0        0      768 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/EventInterface.py
+-rw-r--r--   0        0        0      789 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/FullEditInterface.py
+-rw-r--r--   0        0        0      831 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/PartialEditInterface.py
+-rw-r--r--   0        0        0     2014 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/SharingInterface.py
+-rw-r--r--   0        0        0     2255 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/TagInterface.py
+-rw-r--r--   0        0        0       88 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/__init__.py
+-rw-r--r--   0        0        0      204 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/Errors.py
+-rw-r--r--   0        0        0    14121 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/Workflow.py
+-rw-r--r--   0        0        0       40 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/__init__.py
+-rw-r--r--   0        0        0     4424 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ActionAbstract.py
+-rw-r--r--   0        0        0     5031 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ConfigurationAction.py
+-rw-r--r--   0        0        0     4304 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/OfferingAction.py
+-rw-r--r--   0        0        0    15865 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py
+-rw-r--r--   0        0        0    11298 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/UploadAction.py
+-rw-r--r--   0        0        0       72 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/__init__.py
+-rw-r--r--   0        0        0      802 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/AbstractResolver.py
+-rw-r--r--   0        0        0     1271 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/DictResolver.py
+-rw-r--r--   0        0        0     4333 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/Errors.py
+-rw-r--r--   0        0        0     5295 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/FileResolver.py
+-rw-r--r--   0        0        0     3469 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/GlobalResolver.py
+-rw-r--r--   0        0        0     3489 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py
+-rw-r--r--   0        0        0     1462 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/UserResolver.py
+-rw-r--r--   0        0        0      110 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/mkdocs.yml
+-rw-r--r--   0        0        0     1280 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      956 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1735 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/GpfTestCase.py
+-rw-r--r--   0        0        0     3366 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/MainTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      336 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_authentifier.ini
+-rw-r--r--   0        0        0      308 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_overload.ini
+-rw-r--r--   0        0        0      313 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_requester.ini
+-rw-r--r--   0        0        0       40 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_upload.ini
+-rw-r--r--   0        0        0       69 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_value_type.ini
+-rw-r--r--   0        0        0      460 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
+-rw-r--r--   0        0        0      341 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
+-rw-r--r--   0        0        0        5 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
+-rw-r--r--   0        0        0       11 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
+-rw-r--r--   0        0        0        5 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
+-rw-r--r--   0        0        0     2659 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/workflows/bad-workflow.jsonc
+-rw-r--r--   0        0        0       53 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/FileHelper/md5.txt
+-rw-r--r--   0        0        0       78 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/json_not_parsable.json
+-rw-r--r--   0        0        0       52 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/json_not_valid.json
+-rw-r--r--   0        0        0      108 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/json_parsable.json
+-rw-r--r--   0        0        0      563 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/schema.json
+-rw-r--r--   0        0        0      485 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/schema_invalid.json
+-rw-r--r--   0        0        0       23 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/dict.json
+-rw-r--r--   0        0        0       21 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/list.json
+-rw-r--r--   0        0        0        2 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/not-valid.json
+-rw-r--r--   0        0        0       31 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/text.txt
+-rw-r--r--   0        0        0     7383 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/auth/AuthentifierTestCase.py
+-rw-r--r--   0        0        0     1183 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/auth/TokenTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/auth/__init__.py
+-rw-r--r--   0        0        0     1056 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/helper/FileHelperTestCase.py
+-rw-r--r--   0        0        0     9959 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/helper/JsonHelperTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/helper/__init__.py
+-rw-r--r--   0        0        0    13575 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/ApiRequesterTestCase.py
+-rw-r--r--   0        0        0     3595 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/ConfigTestCase.py
+-rw-r--r--   0        0        0     2218 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/DatasetTestCase.py
+-rw-r--r--   0        0        0     1716 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/DescriptorFileReaderTestCase.py
+-rw-r--r--   0        0        0     1974 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1198 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/JsonConverterTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/__init__.py
+-rw-r--r--   0        0        0     1431 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/CheckExecutionTestCase.py
+-rw-r--r--   0        0        0     2855 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/ConfigurationTestCase.py
+-rw-r--r--   0        0        0     3487 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/EndpointTestCase.py
+-rw-r--r--   0        0        0     1144 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1504 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/EventInterfaceTestCase.py
+-rw-r--r--   0        0        0     3865 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/ProcessingExecutionTestCase.py
+-rw-r--r--   0        0        0    18439 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/StoreEntityTestCase.py
+-rw-r--r--   0        0        0    11477 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/UploadTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/__init__.py
+-rw-r--r--   0        0        0     4538 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/CommentInterfaceTestCase.py
+-rw-r--r--   0        0        0     2532 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/CsfInterfaceTestCase.py
+-rw-r--r--   0        0        0     1699 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/FullEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     1745 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/PartialEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     3585 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/SharingInterfaceTestCase.py
+-rw-r--r--   0        0        0     3600 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/TagInterfaceTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/__init__.py
+-rw-r--r--   0        0        0    14646 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/WorkflowTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/__init__.py
+-rw-r--r--   0        0        0     3100 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/ActionAbstractTestCase.py
+-rw-r--r--   0        0        0     5384 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/ConfigurationActionTestCase.py
+-rw-r--r--   0        0        0     7133 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/OfferingActionTestCase.py
+-rw-r--r--   0        0        0    16012 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/ProcessingExecutionActionTestCase.py
+-rw-r--r--   0        0        0    19409 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/UploadActionTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/__init__.py
+-rw-r--r--   0        0        0     1116 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/DictResolverTestCase.py
+-rw-r--r--   0        0        0     4492 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/FileResolverTestCase.py
+-rw-r--r--   0        0        0     2492 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/GlobalResolverTestCase.py
+-rw-r--r--   0        0        0     6705 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/StoreEntityResolverTestCase.py
+-rw-r--r--   0        0        0     2225 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/UserResolverTestCase.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0   116760 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/classes.png
+-rw-r--r--   0        0        0     9175 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/classes.uxf
+-rw-r--r--   0        0        0    43510 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/interfaces.png
+-rw-r--r--   0        0        0     7059 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/interfaces.uxf
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 ignf_gpf_api-0.1.8/PKG-INFO
```

### Comparing `ignf_gpf_api-0.1.7/.github/workflows/ci-dev.yml` & `ignf_gpf_api-0.1.8/.github/workflows/ci-dev.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/.github/workflows/ci-prod.yml` & `ignf_gpf_api-0.1.8/.github/workflows/ci-prod.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/.github/workflows/code-quality.yml` & `ignf_gpf_api-0.1.8/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/.gitignore` & `ignf_gpf_api-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/.pylintrc` & `ignf_gpf_api-0.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/.vscode/settings.json` & `ignf_gpf_api-0.1.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/LICENSE` & `ignf_gpf_api-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docker/Dockerfile` & `ignf_gpf_api-0.1.8/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docker/README.md` & `ignf_gpf_api-0.1.8/docker/README.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/comme-executable.md` & `ignf_gpf_api-0.1.8/docs/comme-executable.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/configuration.md` & `ignf_gpf_api-0.1.8/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/configuration_details.md` & `ignf_gpf_api-0.1.8/docs/configuration_details.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/development.md` & `ignf_gpf_api-0.1.8/docs/development.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/images/index__utilisation_module.excalidraw` & `ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.excalidraw`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/images/index__utilisation_module.png` & `ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.png`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/index.md` & `ignf_gpf_api-0.1.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/tutoriel_1_archive.md` & `ignf_gpf_api-0.1.8/docs/tutoriel_1_archive.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/tutoriel_2_flux_vecteur.md` & `ignf_gpf_api-0.1.8/docs/tutoriel_2_flux_vecteur.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/docs/upload_descriptor.md` & `ignf_gpf_api-0.1.8/docs/upload_descriptor.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/Errors.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/Errors.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/__main__.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/__main__.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_conf/default.ini` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/default.ini`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_conf/json_schemas/workflow.json` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/workflows/archive-generic.jsonc` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/archive-generic.jsonc`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/_data/workflows/wfs-generic.jsonc` & `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/wfs-generic.jsonc`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/auth/Authentifier.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Authentifier.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/auth/Token.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Token.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/helper/FileHelper.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/helper/FileHelper.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/helper/JsonHelper.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/helper/JsonHelper.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/helper/PrintLogHelper.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/helper/PrintLogHelper.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/ApiRequester.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/ApiRequester.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/Color.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Color.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/Config.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Config.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/Dataset.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Dataset.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/DescriptorFileReader.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/DescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/Errors.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Errors.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/JsonConverter.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/JsonConverter.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/io/OutputManager.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/io/OutputManager.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/pattern/SingleInstance.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/SingleInstance.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/pattern/Singleton.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/Singleton.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/CheckExecution.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/CheckExecution.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/Configuration.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Configuration.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/Endpoint.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Endpoint.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/Offering.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Offering.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/ProcessingExecution.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/ProcessingExecution.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/StoreEntity.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoreEntity.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/StoredData.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoredData.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/Upload.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Upload.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/CommentInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CommentInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/CsfInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CsfInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/EventInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/EventInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def api_events(self) -> List[Dict[str, Any]]:
         """Liste les événements.
 
         Returns:
             List[Dict[str, Any]]: liste des événements
         """
         # Génération du nom de la route
-        s_route = f"{self._entity_name}_list_event"
+        s_route = f"{self._entity_name}_list_events"
         # Requête "get" à l'API
         o_response = ApiRequester().route_request(
             s_route,
             route_params={self._entity_name: self.id},
         )
         l_events: List[Dict[str, Any]] = o_response.json()
         return l_events
```

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/FullEditInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/FullEditInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/PartialEditInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/PartialEditInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/SharingInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/SharingInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/store/interface/TagInterface.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/TagInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/Workflow.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/ActionAbstract.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ActionAbstract.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/ConfigurationAction.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/OfferingAction.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/OfferingAction.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/action/UploadAction.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/UploadAction.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/AbstractResolver.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/AbstractResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/DictResolver.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/DictResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/Errors.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/Errors.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/FileResolver.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/FileResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/GlobalResolver.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/GlobalResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/ignf_gpf_api/workflow/resolver/UserResolver.py` & `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/UserResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/mkdocs.yml` & `ignf_gpf_api-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/pyproject.toml` & `ignf_gpf_api-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/ErrorsTestCase.py` & `ignf_gpf_api-0.1.8/tests/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/GpfTestCase.py` & `ignf_gpf_api-0.1.8/tests/GpfTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/MainTestCase.py` & `ignf_gpf_api-0.1.8/tests/MainTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf` & `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp` & `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx` & `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json` & `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf` & `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp` & `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx` & `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json` & `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_data/workflows/bad-workflow.jsonc` & `ignf_gpf_api-0.1.8/tests/_data/workflows/bad-workflow.jsonc`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/_test/helper/JsonHelper/schema.json` & `ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/schema.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/auth/AuthentifierTestCase.py` & `ignf_gpf_api-0.1.8/tests/auth/AuthentifierTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/auth/TokenTestCase.py` & `ignf_gpf_api-0.1.8/tests/auth/TokenTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/helper/FileHelperTestCase.py` & `ignf_gpf_api-0.1.8/tests/helper/FileHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/helper/JsonHelperTestCase.py` & `ignf_gpf_api-0.1.8/tests/helper/JsonHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/io/ApiRequesterTestCase.py` & `ignf_gpf_api-0.1.8/tests/io/ApiRequesterTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/io/ConfigTestCase.py` & `ignf_gpf_api-0.1.8/tests/io/ConfigTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/io/DatasetTestCase.py` & `ignf_gpf_api-0.1.8/tests/io/DatasetTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/io/DescriptorFileReaderTestCase.py` & `ignf_gpf_api-0.1.8/tests/io/DescriptorFileReaderTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/io/ErrorsTestCase.py` & `ignf_gpf_api-0.1.8/tests/io/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/io/JsonConverterTestCase.py` & `ignf_gpf_api-0.1.8/tests/io/JsonConverterTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/CheckExecutionTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/CheckExecutionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/ConfigurationTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/ConfigurationTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/EndpointTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/EndpointTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/ErrorsTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/EventInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/EventInterfaceTestCase.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons param
         with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
             # on appelle la fonction à tester :api_list_events
             o_event_interface = EventInterface({"_id": "id_entité"})
             l_data_recupere = o_event_interface.api_events()
             # on vérifie que route_request est appelé correctement
             o_mock_request.assert_called_once_with(
-                "store_entity_list_event",
+                "store_entity_list_events",
                 route_params={"store_entity": "id_entité"},
             )
             # on vérifie la similitude des données retournées
             self.assertEqual(l_data, l_data_recupere)
```

### Comparing `ignf_gpf_api-0.1.7/tests/store/ProcessingExecutionTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/ProcessingExecutionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/StoreEntityTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/StoreEntityTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/UploadTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/UploadTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/interface/CommentInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/interface/CommentInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/interface/CsfInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/interface/CsfInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/interface/FullEditInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/interface/FullEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/interface/PartialEditInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/interface/PartialEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/interface/SharingInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/interface/SharingInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/store/interface/TagInterfaceTestCase.py` & `ignf_gpf_api-0.1.8/tests/store/interface/TagInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/WorkflowTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/WorkflowTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/action/ActionAbstractTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/action/ActionAbstractTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/action/ConfigurationActionTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/action/ConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/action/OfferingActionTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/action/OfferingActionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/action/ProcessingExecutionActionTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/action/ProcessingExecutionActionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/action/UploadActionTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/action/UploadActionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/resolver/DictResolverTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/resolver/DictResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/resolver/FileResolverTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/resolver/FileResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/resolver/GlobalResolverTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/resolver/GlobalResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/resolver/StoreEntityResolverTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/resolver/StoreEntityResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/tests/workflow/resolver/UserResolverTestCase.py` & `ignf_gpf_api-0.1.8/tests/workflow/resolver/UserResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/uml/classes.png` & `ignf_gpf_api-0.1.8/uml/classes.png`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/uml/classes.uxf` & `ignf_gpf_api-0.1.8/uml/classes.uxf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/uml/interfaces.png` & `ignf_gpf_api-0.1.8/uml/interfaces.png`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/uml/interfaces.uxf` & `ignf_gpf_api-0.1.8/uml/interfaces.uxf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.7/PKG-INFO` & `ignf_gpf_api-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignf_gpf_api
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python API to simplify the use of the GPF HTTPS API.
 Author-email: Valentin Sasyan <valentin.sasyan@ign.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

