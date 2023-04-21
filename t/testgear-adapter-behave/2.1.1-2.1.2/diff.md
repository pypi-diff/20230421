# Comparing `tmp/testgear-adapter-behave-2.1.1.tar.gz` & `tmp/testgear-adapter-behave-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-behave-2.1.1.tar", last modified: Fri Mar 31 06:32:34 2023, max compression
+gzip compressed data, was "testgear-adapter-behave-2.1.2.tar", last modified: Fri Apr 21 14:57:11 2023, max compression
```

## Comparing `testgear-adapter-behave-2.1.1.tar` & `testgear-adapter-behave-2.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:34.244522 testgear-adapter-behave-2.1.1/
--rw-rw-rw-   0        0        0    11825 2023-03-31 06:32:34.244522 testgear-adapter-behave-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8983 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.1/README.md
--rw-rw-rw-   0        0        0       50 2023-03-27 12:00:18.000000 testgear-adapter-behave-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 06:32:34.244522 testgear-adapter-behave-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:34.229815 testgear-adapter-behave-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:34.244522 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/
--rw-rw-rw-   0        0        0        0 2023-01-19 07:55:39.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-03-31 06:12:26.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/formatter.py
--rw-rw-rw-   0        0        0     4067 2023-03-31 06:12:19.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/listener.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:34.244522 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/
--rw-rw-rw-   0        0        0        0 2023-01-19 07:55:39.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/__init__.py
--rw-rw-rw-   0        0        0      131 2023-01-19 07:55:39.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/label.py
--rw-rw-rw-   0        0        0      513 2023-01-19 07:58:26.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/option.py
--rw-rw-rw-   0        0        0      282 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/tags.py
--rw-rw-rw-   0        0        0      393 2023-01-19 07:55:39.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/test_result_step.py
--rw-rw-rw-   0        0        0      269 2023-01-19 07:55:39.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/url_link.py
--rw-rw-rw-   0        0        0     4331 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/scenario_parser.py
--rw-rw-rw-   0        0        0     2314 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/tags_parser.py
--rw-rw-rw-   0        0        0     2695 2023-03-16 11:41:45.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:34.244522 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/
--rw-rw-rw-   0        0        0    11825 2023-03-31 06:32:33.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-03-31 06:32:34.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 06:32:33.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-31 06:32:33.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-03-31 06:32:33.000000 testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/
+-rw-rw-rw-   0        0        0     9537 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8983 2023-03-31 06:28:55.000000 testgear-adapter-behave-2.1.2/README.md
+-rw-rw-rw-   0        0        0       48 2023-04-21 13:48:08.000000 testgear-adapter-behave-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-21 14:02:35.000000 testgear-adapter-behave-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.484461 testgear-adapter-behave-2.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-21 14:01:40.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/formatter.py
+-rw-rw-rw-   0        0        0     4152 2023-04-21 14:01:40.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/listener.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/__init__.py
+-rw-rw-rw-   0        0        0      131 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/label.py
+-rw-rw-rw-   0        0        0      513 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/option.py
+-rw-rw-rw-   0        0        0      282 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/tags.py
+-rw-rw-rw-   0        0        0      393 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/test_result_step.py
+-rw-rw-rw-   0        0        0      269 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/url_link.py
+-rw-rw-rw-   0        0        0     4323 2023-04-21 14:01:40.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/scenario_parser.py
+-rw-rw-rw-   0        0        0     2314 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/tags_parser.py
+-rw-rw-rw-   0        0        0     2695 2023-04-21 13:47:37.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:11.493472 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/
+-rw-rw-rw-   0        0        0     9537 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 14:57:11.000000 testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/top_level.txt
```

### Comparing `testgear-adapter-behave-2.1.1/PKG-INFO` & `testgear-adapter-behave-2.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,298 +1,297 @@
 Metadata-Version: 2.1
 Name: testgear-adapter-behave
-Version: 2.1.1
+Version: 2.1.2
 Summary: Behave adapter for Test Gear
 Home-page: https://github.com/testgear-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@test-gear.io
 License: Apache-2.0
-Description: # Test Gear TMS adapter for Behave
-        
-        ![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-        
-        ## Getting Started
-        
-        ### Installation
-        
-        ```
-        pip install testgear-adapter-behave
-        ```
-        
-        ## Usage
-        
-        ### Configuration
-        
-        #### File
-        
-        1. Create **connection_config.ini** file in the root directory of the project:
-            ```
-            [testgear]
-            URL = <url>
-            privateToken = <token>
-            projectId = <id>
-            configurationId = <id>
-            testRunId = <optional id>
-            testRunName = <optional name>
-            adapterMode = <optional>
-            
-            # This section are optional. It enables debug mode.
-            [debug]
-            tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
-            ```
-        
-        2. Fill parameters with your configuration, where:
-            * `URL` - location of the TMS instance
-        
-            * `privateToken` - API secret key
-                1. go to the https://{DOMAIN}/user-profile profile
-                2. copy the API secret key
-        
-            * `projectId` - ID of project in TMS instance.
-        
-                1. create a project
-                2. open DevTools -> network
-                3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-                4. GET-request project, Preview tab, copy id field
-        
-            * `configurationId` - ID of configuration in TMS instance.
-        
-                1. create a project
-                2. open DevTools -> network
-                3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-                4. GET-request configurations, Preview tab, copy id field
-        
-            * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
-              created automatically.
-        
-            * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
-              not provided, it is created automatically.
-        
-            * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
-        
-                * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
-                  test run.
-                * 1 - in this mode, the adapter sends all results to the test run without filtering.
-                * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-            
-            * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-        
-            * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-        
-        #### ENV
-        
-        You can use environment variables (environment variables take precedence over file variables):
-        
-        * `TMS_URL` - location of the TMS instance.
-        
-        * `TMS_PRIVATE_TOKEN` - API secret key.
-        
-        * `TMS_PROJECT_ID` - ID of a project in TMS instance.
-        
-        * `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
-        
-        * `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
-        
-        * `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
-          it is created automatically.
-        
-        * `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
-          automatically.
-        
-        * `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
-          default file name.
-        
-        * `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-        
-        * `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-        
-        #### Command line
-        
-        You also can CLI variables (CLI variables take precedence over environment variables):
-        
-        * `tmsUrl` - location of the TMS instance.
-        
-        * `tmsPrivateToken` - API secret key.
-        
-        * `tmsProjectId` - ID of a project in TMS instance.
-        
-        * `tmsConfigurationId` - ID of a configuration in TMS instance.
-        
-        * `tmsAdapterMode` - adapter mode. Default value - 0.
-        
-        * `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
-          created automatically.
-        
-        * `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
-          automatically.
-        
-        * `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
-          default file name.
-        
-        * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-        
-        * `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
-        
-        #### Examples
-        
-        Launch with a connection_config.ini file in the root directory of the project:
-        
-        ```
-        $ behave -f testgear_adapter_behave.formatter:AdapterFormatter
-        ```
-        
-        Launch with command-line parameters:
-        
-        ```
-        $ behave -f testgear_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
-        tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
-        tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D tmsCertValidation=<optional boolean>
-        ```
-        
-        If you want to enable debug mode then
-        see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-        
-        ### Tags
-        
-        Use tags to specify information about autotest.
-        
-        Description of tags:
-        
-        - `WorkItemIds` - linking an autotest to a test case.
-        - `DisplayName` - name of the autotest in TMS.
-        - `ExternalId` - ID of the autotest within the project in TMS.
-        - `Title` - title in the autotest card.
-        - `Description` - description in the autotest card.
-        - `Labels` - tags in the autotest card.
-        - `Links` - links in the autotest card.
-        - `NameSpace` - directory in the TMS system (default - file's name of test)
-        - `ClassName` - subdirectory in the TMS system (default - class's name of test)
-        
-        Description of methods:
-        
-        - `testgear.addLinks` - links in the autotest result
-        - `testgear.addAttachments` - uploading files in the autotest result
-        - `testgear.addMessage` - information about autotest in the autotest result
-        - `testgear.step` - usage in the "with" construct to designation a step in the body of the test
-        
-        ### Examples
-        
-        #### Simple Test
-        
-        ```py
-        import testgear
-        from behave import given
-        from behave import then
-        from behave import when
-        
-        
-        @given("I authorize on the portal")
-        def authorization(context):
-            with testgear.step("I set login"):
-                pass
-            with testgear.step("I set password"):
-                pass
-        
-        
-        @when("I create a project")
-        def create_project(context):
-            pass
-        
-        
-        @when("I open the project")
-        def enter_project(context):
-            pass
-        
-        
-        @when("I create a section")
-        def create_section(context):
-            testgear.addLinks(
-                title='component_dump.dmp',
-                type=testgear.LinkType.RELATED,
-                url='https://dumps.example.com/module/some_module_dump',
-                description='Description'
-            )
-        
-        
-        @then("I create a test case")
-        def create_test_case(context):
-            testgear.addAttachments('pictures/picture.jpg')
-        ```
-        
-        ```buildoutcfg
-        Feature: Sample
-        
-          Background:
-            Given I authorize on the portal
-        
-          @ExternalId=failed_with_all_annotations
-          @DisplayName=Failed_test_with_all_annotations
-          @WorkItemIds=123
-          @Title=Title_in_the_autotest_card
-          @Description=Test_with_all_annotations
-          @Labels=Tag1,Tag2
-          @Links={"url":"https://dumps.example.com/module/repository","title":"Repository","description":"Example_of_repository","type":"Repository"}
-          Scenario: Create new project, section and test case
-            When I create a project
-            And I open the project
-            And I create a section
-            Then I create a test case
-        ```
-        
-        #### Parameterized test
-        
-        ```py
-        from behave import when
-        from behave import then
-        
-        
-        @when("Summing {left:d}+{right:d}")
-        def step_impl(context, left, right):
-            context.sum = left + right
-        
-        
-        @then("Result is {result:d}")
-        def step_impl(context, result):
-            assert context.sum == result
-        
-        ```
-        
-        ```buildoutcfg
-        Feature: Rule
-          Tests that use Rule
-        
-          Scenario Outline: Summing
-            When Summing <left>+<right>
-            Then Result is <result>
-        
-            Examples:
-              | left | right | result |
-              | 1    | 1     | 3      |
-              | 9    | 9     | 18     |
-        ```
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free
-          to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull
-          request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through
-          the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting
-          your first idea as well.
-        
-        # License
-        
-        Distributed under the Apache-2.0 License.
-        See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# Test Gear TMS adapter for Behave
+
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+
+```
+pip install testgear-adapter-behave
+```
+
+## Usage
+
+### Configuration
+
+#### File
+
+1. Create **connection_config.ini** file in the root directory of the project:
+    ```
+    [testgear]
+    URL = <url>
+    privateToken = <token>
+    projectId = <id>
+    configurationId = <id>
+    testRunId = <optional id>
+    testRunName = <optional name>
+    adapterMode = <optional>
+    
+    # This section are optional. It enables debug mode.
+    [debug]
+    tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+    ```
+
+2. Fill parameters with your configuration, where:
+    * `URL` - location of the TMS instance
+
+    * `privateToken` - API secret key
+        1. go to the https://{DOMAIN}/user-profile profile
+        2. copy the API secret key
+
+    * `projectId` - ID of project in TMS instance.
+
+        1. create a project
+        2. open DevTools -> network
+        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+        4. GET-request project, Preview tab, copy id field
+
+    * `configurationId` - ID of configuration in TMS instance.
+
+        1. create a project
+        2. open DevTools -> network
+        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+        4. GET-request configurations, Preview tab, copy id field
+
+    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
+      created automatically.
+
+    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
+      not provided, it is created automatically.
+
+    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
+
+        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
+          test run.
+        * 1 - in this mode, the adapter sends all results to the test run without filtering.
+        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
+    
+    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
+
+    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
+
+#### ENV
+
+You can use environment variables (environment variables take precedence over file variables):
+
+* `TMS_URL` - location of the TMS instance.
+
+* `TMS_PRIVATE_TOKEN` - API secret key.
+
+* `TMS_PROJECT_ID` - ID of a project in TMS instance.
+
+* `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
+
+* `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
+
+* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
+  it is created automatically.
+
+* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
+  automatically.
+
+* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
+  default file name.
+
+* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
+
+* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
+
+#### Command line
+
+You also can CLI variables (CLI variables take precedence over environment variables):
+
+* `tmsUrl` - location of the TMS instance.
+
+* `tmsPrivateToken` - API secret key.
+
+* `tmsProjectId` - ID of a project in TMS instance.
+
+* `tmsConfigurationId` - ID of a configuration in TMS instance.
+
+* `tmsAdapterMode` - adapter mode. Default value - 0.
+
+* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
+  created automatically.
+
+* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
+  automatically.
+
+* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
+  default file name.
+
+* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
+
+* `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
+
+#### Examples
+
+Launch with a connection_config.ini file in the root directory of the project:
+
+```
+$ behave -f testgear_adapter_behave.formatter:AdapterFormatter
+```
+
+Launch with command-line parameters:
+
+```
+$ behave -f testgear_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
+tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
+tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D tmsCertValidation=<optional boolean>
+```
+
+If you want to enable debug mode then
+see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Use tags to specify information about autotest.
+
+Description of tags:
+
+- `WorkItemIds` - linking an autotest to a test case.
+- `DisplayName` - name of the autotest in TMS.
+- `ExternalId` - ID of the autotest within the project in TMS.
+- `Title` - title in the autotest card.
+- `Description` - description in the autotest card.
+- `Labels` - tags in the autotest card.
+- `Links` - links in the autotest card.
+- `NameSpace` - directory in the TMS system (default - file's name of test)
+- `ClassName` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+
+- `testgear.addLinks` - links in the autotest result
+- `testgear.addAttachments` - uploading files in the autotest result
+- `testgear.addMessage` - information about autotest in the autotest result
+- `testgear.step` - usage in the "with" construct to designation a step in the body of the test
+
+### Examples
+
+#### Simple Test
+
+```py
+import testgear
+from behave import given
+from behave import then
+from behave import when
+
+
+@given("I authorize on the portal")
+def authorization(context):
+    with testgear.step("I set login"):
+        pass
+    with testgear.step("I set password"):
+        pass
+
+
+@when("I create a project")
+def create_project(context):
+    pass
+
+
+@when("I open the project")
+def enter_project(context):
+    pass
+
+
+@when("I create a section")
+def create_section(context):
+    testgear.addLinks(
+        title='component_dump.dmp',
+        type=testgear.LinkType.RELATED,
+        url='https://dumps.example.com/module/some_module_dump',
+        description='Description'
+    )
+
+
+@then("I create a test case")
+def create_test_case(context):
+    testgear.addAttachments('pictures/picture.jpg')
+```
+
+```buildoutcfg
+Feature: Sample
+
+  Background:
+    Given I authorize on the portal
+
+  @ExternalId=failed_with_all_annotations
+  @DisplayName=Failed_test_with_all_annotations
+  @WorkItemIds=123
+  @Title=Title_in_the_autotest_card
+  @Description=Test_with_all_annotations
+  @Labels=Tag1,Tag2
+  @Links={"url":"https://dumps.example.com/module/repository","title":"Repository","description":"Example_of_repository","type":"Repository"}
+  Scenario: Create new project, section and test case
+    When I create a project
+    And I open the project
+    And I create a section
+    Then I create a test case
+```
+
+#### Parameterized test
+
+```py
+from behave import when
+from behave import then
+
+
+@when("Summing {left:d}+{right:d}")
+def step_impl(context, left, right):
+    context.sum = left + right
+
+
+@then("Result is {result:d}")
+def step_impl(context, result):
+    assert context.sum == result
+
+```
+
+```buildoutcfg
+Feature: Rule
+  Tests that use Rule
+
+  Scenario Outline: Summing
+    When Summing <left>+<right>
+    Then Result is <result>
+
+    Examples:
+      | left | right | result |
+      | 1    | 1     | 3      |
+      | 9    | 9     | 18     |
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free
+  to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull
+  request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through
+  the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting
+  your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License.
+See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-behave-2.1.1/README.md` & `testgear-adapter-behave-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `testgear-adapter-behave-2.1.1/setup.py` & `testgear-adapter-behave-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testgear-adapter-behave',
-    version='2.1.1',
+    version='2.1.2',
     description='Behave adapter for Test Gear',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testgear-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@test-gear.io',
     license='Apache-2.0',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testgear_adapter_behave'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'behave',
-        'testgear-python-commons==2.1.1',
+        'testgear-python-commons==2.1.2',
         'attrs'],
 )
```

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/formatter.py` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/formatter.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/listener.py` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 
     def get_step_parameters(self, match):
         scope = self.get_scope()
 
         executable_step = get_test_result_step_model()
 
         for argument in match.arguments:
-            executable_step['description'] += f'{argument.name} = {argument.original} '
-            executable_step['parameters'][argument.name] = argument.original
+            name = argument.name if argument.name else 'param' + str(match.arguments.index(argument))
+            executable_step['description'] += f'{name} = {argument.original} '
+            executable_step['parameters'][name] = argument.original
 
         self.__executable_test[scope].append(executable_step)
 
     def get_step_result(self, result):
         scope = self.get_scope()
         outcome = parse_status(result.status)
```

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/models/option.py` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/models/option.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/scenario_parser.py` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/scenario_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         'labels': [],
         'workItemsID': [],
         # TODO: Add to python-commons
         # 'started_on': '',
         # 'completed_on': None
     }
 
-    if TagType.EXTERNAL_ID in tags:
+    if TagType.TITLE in tags:
         executable_test['title'] = tags[TagType.TITLE]
 
     if TagType.DESCRIPTION in tags:
         executable_test['description'] = tags[TagType.DESCRIPTION]
 
     if TagType.LINKS in tags:
         executable_test['links'] = tags[TagType.LINKS]
@@ -92,15 +92,15 @@
 def get_scenario_namespace(scenario):
     return scenario.feature.filename
 
 
 def get_scenario_parameters(scenario):
     row = scenario._row
 
-    return {name: value for name, value in zip(row.headings, row.cells)} if row else None
+    return {name: value for name, value in zip(row.headings, row.cells)} if row else {}
 
 
 def get_scenario_status(scenario):
     for step in scenario.all_steps:
         if get_step_status(step) != 'passed':
             return get_step_status(step)
     return OutcomeType.PASSED
```

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/tags_parser.py` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/tags_parser.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave/utils.py` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave/utils.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/PKG-INFO` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,298 +1,297 @@
 Metadata-Version: 2.1
 Name: testgear-adapter-behave
-Version: 2.1.1
+Version: 2.1.2
 Summary: Behave adapter for Test Gear
 Home-page: https://github.com/testgear-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@test-gear.io
 License: Apache-2.0
-Description: # Test Gear TMS adapter for Behave
-        
-        ![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-        
-        ## Getting Started
-        
-        ### Installation
-        
-        ```
-        pip install testgear-adapter-behave
-        ```
-        
-        ## Usage
-        
-        ### Configuration
-        
-        #### File
-        
-        1. Create **connection_config.ini** file in the root directory of the project:
-            ```
-            [testgear]
-            URL = <url>
-            privateToken = <token>
-            projectId = <id>
-            configurationId = <id>
-            testRunId = <optional id>
-            testRunName = <optional name>
-            adapterMode = <optional>
-            
-            # This section are optional. It enables debug mode.
-            [debug]
-            tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
-            ```
-        
-        2. Fill parameters with your configuration, where:
-            * `URL` - location of the TMS instance
-        
-            * `privateToken` - API secret key
-                1. go to the https://{DOMAIN}/user-profile profile
-                2. copy the API secret key
-        
-            * `projectId` - ID of project in TMS instance.
-        
-                1. create a project
-                2. open DevTools -> network
-                3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-                4. GET-request project, Preview tab, copy id field
-        
-            * `configurationId` - ID of configuration in TMS instance.
-        
-                1. create a project
-                2. open DevTools -> network
-                3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-                4. GET-request configurations, Preview tab, copy id field
-        
-            * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
-              created automatically.
-        
-            * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
-              not provided, it is created automatically.
-        
-            * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
-        
-                * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
-                  test run.
-                * 1 - in this mode, the adapter sends all results to the test run without filtering.
-                * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-            
-            * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-        
-            * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-        
-        #### ENV
-        
-        You can use environment variables (environment variables take precedence over file variables):
-        
-        * `TMS_URL` - location of the TMS instance.
-        
-        * `TMS_PRIVATE_TOKEN` - API secret key.
-        
-        * `TMS_PROJECT_ID` - ID of a project in TMS instance.
-        
-        * `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
-        
-        * `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
-        
-        * `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
-          it is created automatically.
-        
-        * `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
-          automatically.
-        
-        * `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
-          default file name.
-        
-        * `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-        
-        * `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-        
-        #### Command line
-        
-        You also can CLI variables (CLI variables take precedence over environment variables):
-        
-        * `tmsUrl` - location of the TMS instance.
-        
-        * `tmsPrivateToken` - API secret key.
-        
-        * `tmsProjectId` - ID of a project in TMS instance.
-        
-        * `tmsConfigurationId` - ID of a configuration in TMS instance.
-        
-        * `tmsAdapterMode` - adapter mode. Default value - 0.
-        
-        * `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
-          created automatically.
-        
-        * `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
-          automatically.
-        
-        * `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
-          default file name.
-        
-        * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-        
-        * `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
-        
-        #### Examples
-        
-        Launch with a connection_config.ini file in the root directory of the project:
-        
-        ```
-        $ behave -f testgear_adapter_behave.formatter:AdapterFormatter
-        ```
-        
-        Launch with command-line parameters:
-        
-        ```
-        $ behave -f testgear_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
-        tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
-        tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D tmsCertValidation=<optional boolean>
-        ```
-        
-        If you want to enable debug mode then
-        see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-        
-        ### Tags
-        
-        Use tags to specify information about autotest.
-        
-        Description of tags:
-        
-        - `WorkItemIds` - linking an autotest to a test case.
-        - `DisplayName` - name of the autotest in TMS.
-        - `ExternalId` - ID of the autotest within the project in TMS.
-        - `Title` - title in the autotest card.
-        - `Description` - description in the autotest card.
-        - `Labels` - tags in the autotest card.
-        - `Links` - links in the autotest card.
-        - `NameSpace` - directory in the TMS system (default - file's name of test)
-        - `ClassName` - subdirectory in the TMS system (default - class's name of test)
-        
-        Description of methods:
-        
-        - `testgear.addLinks` - links in the autotest result
-        - `testgear.addAttachments` - uploading files in the autotest result
-        - `testgear.addMessage` - information about autotest in the autotest result
-        - `testgear.step` - usage in the "with" construct to designation a step in the body of the test
-        
-        ### Examples
-        
-        #### Simple Test
-        
-        ```py
-        import testgear
-        from behave import given
-        from behave import then
-        from behave import when
-        
-        
-        @given("I authorize on the portal")
-        def authorization(context):
-            with testgear.step("I set login"):
-                pass
-            with testgear.step("I set password"):
-                pass
-        
-        
-        @when("I create a project")
-        def create_project(context):
-            pass
-        
-        
-        @when("I open the project")
-        def enter_project(context):
-            pass
-        
-        
-        @when("I create a section")
-        def create_section(context):
-            testgear.addLinks(
-                title='component_dump.dmp',
-                type=testgear.LinkType.RELATED,
-                url='https://dumps.example.com/module/some_module_dump',
-                description='Description'
-            )
-        
-        
-        @then("I create a test case")
-        def create_test_case(context):
-            testgear.addAttachments('pictures/picture.jpg')
-        ```
-        
-        ```buildoutcfg
-        Feature: Sample
-        
-          Background:
-            Given I authorize on the portal
-        
-          @ExternalId=failed_with_all_annotations
-          @DisplayName=Failed_test_with_all_annotations
-          @WorkItemIds=123
-          @Title=Title_in_the_autotest_card
-          @Description=Test_with_all_annotations
-          @Labels=Tag1,Tag2
-          @Links={"url":"https://dumps.example.com/module/repository","title":"Repository","description":"Example_of_repository","type":"Repository"}
-          Scenario: Create new project, section and test case
-            When I create a project
-            And I open the project
-            And I create a section
-            Then I create a test case
-        ```
-        
-        #### Parameterized test
-        
-        ```py
-        from behave import when
-        from behave import then
-        
-        
-        @when("Summing {left:d}+{right:d}")
-        def step_impl(context, left, right):
-            context.sum = left + right
-        
-        
-        @then("Result is {result:d}")
-        def step_impl(context, result):
-            assert context.sum == result
-        
-        ```
-        
-        ```buildoutcfg
-        Feature: Rule
-          Tests that use Rule
-        
-          Scenario Outline: Summing
-            When Summing <left>+<right>
-            Then Result is <result>
-        
-            Examples:
-              | left | right | result |
-              | 1    | 1     | 3      |
-              | 9    | 9     | 18     |
-        ```
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free
-          to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull
-          request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through
-          the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting
-          your first idea as well.
-        
-        # License
-        
-        Distributed under the Apache-2.0 License.
-        See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# Test Gear TMS adapter for Behave
+
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+
+```
+pip install testgear-adapter-behave
+```
+
+## Usage
+
+### Configuration
+
+#### File
+
+1. Create **connection_config.ini** file in the root directory of the project:
+    ```
+    [testgear]
+    URL = <url>
+    privateToken = <token>
+    projectId = <id>
+    configurationId = <id>
+    testRunId = <optional id>
+    testRunName = <optional name>
+    adapterMode = <optional>
+    
+    # This section are optional. It enables debug mode.
+    [debug]
+    tmsProxy = {"http": "http://localhost:8888", "https": "http://localhost:8888"}
+    ```
+
+2. Fill parameters with your configuration, where:
+    * `URL` - location of the TMS instance
+
+    * `privateToken` - API secret key
+        1. go to the https://{DOMAIN}/user-profile profile
+        2. copy the API secret key
+
+    * `projectId` - ID of project in TMS instance.
+
+        1. create a project
+        2. open DevTools -> network
+        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+        4. GET-request project, Preview tab, copy id field
+
+    * `configurationId` - ID of configuration in TMS instance.
+
+        1. create a project
+        2. open DevTools -> network
+        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+        4. GET-request configurations, Preview tab, copy id field
+
+    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is
+      created automatically.
+
+    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is
+      not provided, it is created automatically.
+
+    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:
+
+        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the
+          test run.
+        * 1 - in this mode, the adapter sends all results to the test run without filtering.
+        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
+    
+    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
+
+    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
+
+#### ENV
+
+You can use environment variables (environment variables take precedence over file variables):
+
+* `TMS_URL` - location of the TMS instance.
+
+* `TMS_PRIVATE_TOKEN` - API secret key.
+
+* `TMS_PROJECT_ID` - ID of a project in TMS instance.
+
+* `TMS_CONFIGURATION_ID` - ID of a configuration in TMS instance.
+
+* `TMS_ADAPTER_MODE` - adapter mode. Default value - 0.
+
+* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided,
+  it is created automatically.
+
+* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created
+  automatically.
+
+* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used
+  default file name.
+
+* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
+
+* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
+
+#### Command line
+
+You also can CLI variables (CLI variables take precedence over environment variables):
+
+* `tmsUrl` - location of the TMS instance.
+
+* `tmsPrivateToken` - API secret key.
+
+* `tmsProjectId` - ID of a project in TMS instance.
+
+* `tmsConfigurationId` - ID of a configuration in TMS instance.
+
+* `tmsAdapterMode` - adapter mode. Default value - 0.
+
+* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is
+  created automatically.
+
+* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created
+  automatically.
+
+* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used
+  default file name.
+
+* `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
+
+* `tmsCertValidation` - it enables/disables certificate validation. `tmsCertValidation` is optional.
+
+#### Examples
+
+Launch with a connection_config.ini file in the root directory of the project:
+
+```
+$ behave -f testgear_adapter_behave.formatter:AdapterFormatter
+```
+
+Launch with command-line parameters:
+
+```
+$ behave -f testgear_adapter_behave.formatter:AdapterFormatter -D tmsUrl=<url> -D tmsPrivateToken=<token> -D
+tmsProjectId=<id> -D tmsConfigurationId=<id> -D tmsTestRunId=<optional id> -D tmsAdapterMode=<optional> -D
+tmsTestRunName=<optional name> -D tmsProxy='{"http":"http://localhost:8888","https":"http://localhost:8888"}' -D tmsCertValidation=<optional boolean>
+```
+
+If you want to enable debug mode then
+see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Use tags to specify information about autotest.
+
+Description of tags:
+
+- `WorkItemIds` - linking an autotest to a test case.
+- `DisplayName` - name of the autotest in TMS.
+- `ExternalId` - ID of the autotest within the project in TMS.
+- `Title` - title in the autotest card.
+- `Description` - description in the autotest card.
+- `Labels` - tags in the autotest card.
+- `Links` - links in the autotest card.
+- `NameSpace` - directory in the TMS system (default - file's name of test)
+- `ClassName` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+
+- `testgear.addLinks` - links in the autotest result
+- `testgear.addAttachments` - uploading files in the autotest result
+- `testgear.addMessage` - information about autotest in the autotest result
+- `testgear.step` - usage in the "with" construct to designation a step in the body of the test
+
+### Examples
+
+#### Simple Test
+
+```py
+import testgear
+from behave import given
+from behave import then
+from behave import when
+
+
+@given("I authorize on the portal")
+def authorization(context):
+    with testgear.step("I set login"):
+        pass
+    with testgear.step("I set password"):
+        pass
+
+
+@when("I create a project")
+def create_project(context):
+    pass
+
+
+@when("I open the project")
+def enter_project(context):
+    pass
+
+
+@when("I create a section")
+def create_section(context):
+    testgear.addLinks(
+        title='component_dump.dmp',
+        type=testgear.LinkType.RELATED,
+        url='https://dumps.example.com/module/some_module_dump',
+        description='Description'
+    )
+
+
+@then("I create a test case")
+def create_test_case(context):
+    testgear.addAttachments('pictures/picture.jpg')
+```
+
+```buildoutcfg
+Feature: Sample
+
+  Background:
+    Given I authorize on the portal
+
+  @ExternalId=failed_with_all_annotations
+  @DisplayName=Failed_test_with_all_annotations
+  @WorkItemIds=123
+  @Title=Title_in_the_autotest_card
+  @Description=Test_with_all_annotations
+  @Labels=Tag1,Tag2
+  @Links={"url":"https://dumps.example.com/module/repository","title":"Repository","description":"Example_of_repository","type":"Repository"}
+  Scenario: Create new project, section and test case
+    When I create a project
+    And I open the project
+    And I create a section
+    Then I create a test case
+```
+
+#### Parameterized test
+
+```py
+from behave import when
+from behave import then
+
+
+@when("Summing {left:d}+{right:d}")
+def step_impl(context, left, right):
+    context.sum = left + right
+
+
+@then("Result is {result:d}")
+def step_impl(context, result):
+    assert context.sum == result
+
+```
+
+```buildoutcfg
+Feature: Rule
+  Tests that use Rule
+
+  Scenario Outline: Summing
+    When Summing <left>+<right>
+    Then Result is <result>
+
+    Examples:
+      | left | right | result |
+      | 1    | 1     | 3      |
+      | 9    | 9     | 18     |
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free
+  to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull
+  request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through
+  the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting
+  your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License.
+See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-behave-2.1.1/src/testgear_adapter_behave.egg-info/SOURCES.txt` & `testgear-adapter-behave-2.1.2/src/testgear_adapter_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

