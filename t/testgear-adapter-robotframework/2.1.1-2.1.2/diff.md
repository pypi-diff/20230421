# Comparing `tmp/testgear-adapter-robotframework-2.1.1.tar.gz` & `tmp/testgear-adapter-robotframework-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-robotframework-2.1.1.tar", last modified: Fri Mar 31 06:30:37 2023, max compression
+gzip compressed data, was "testgear-adapter-robotframework-2.1.2.tar", last modified: Fri Apr 21 14:55:07 2023, max compression
```

## Comparing `testgear-adapter-robotframework-2.1.1.tar` & `testgear-adapter-robotframework-2.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 06:30:37.240697 testgear-adapter-robotframework-2.1.1/
--rw-rw-rw-   0        0        0    13499 2023-03-31 06:30:37.240697 testgear-adapter-robotframework-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10640 2023-03-31 06:28:55.000000 testgear-adapter-robotframework-2.1.1/README.md
--rw-rw-rw-   0        0        0       21 2023-01-19 07:55:39.000000 testgear-adapter-robotframework-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 06:30:37.240697 testgear-adapter-robotframework-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-03-31 06:28:55.000000 testgear-adapter-robotframework-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:30:37.209123 testgear-adapter-robotframework-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 06:30:37.227013 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/
--rw-rw-rw-   0        0        0     4319 2023-03-27 12:00:18.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/TMSLibrary.py
--rw-rw-rw-   0        0        0        0 2023-03-27 12:00:18.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/__init__.py
--rw-rw-rw-   0        0        0     4210 2023-03-27 12:00:18.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/listeners.py
--rw-rw-rw-   0        0        0     8974 2023-03-27 12:00:18.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/models.py
--rw-rw-rw-   0        0        0      297 2023-03-27 12:00:18.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:30:37.240697 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/
--rw-rw-rw-   0        0        0    13499 2023-03-31 06:30:36.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-03-31 06:30:37.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 06:30:36.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-03-31 06:30:36.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-03-31 06:30:36.000000 testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/
+-rw-rw-rw-   0        0        0    11211 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10640 2023-03-31 06:28:55.000000 testgear-adapter-robotframework-2.1.2/README.md
+-rw-rw-rw-   0        0        0       21 2023-01-19 07:55:39.000000 testgear-adapter-robotframework-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      939 2023-04-21 14:03:38.000000 testgear-adapter-robotframework-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.239820 testgear-adapter-robotframework-2.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/
+-rw-rw-rw-   0        0        0     4343 2023-04-21 13:55:56.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/TMSLibrary.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/__init__.py
+-rw-rw-rw-   0        0        0     4210 2023-04-21 13:55:13.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/listeners.py
+-rw-rw-rw-   0        0        0     8974 2023-04-21 13:55:56.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/models.py
+-rw-rw-rw-   0        0        0      297 2023-04-21 13:47:37.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:55:07.248342 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/
+-rw-rw-rw-   0        0        0    11211 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-04-21 14:55:07.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-21 14:55:06.000000 testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testgear-adapter-robotframework-2.1.1/PKG-INFO` & `testgear-adapter-robotframework-2.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,298 +1,297 @@
 Metadata-Version: 2.1
 Name: testgear-adapter-robotframework
-Version: 2.1.1
+Version: 2.1.2
 Summary: Robot Framework adapter for Test Gear
 Home-page: https://github.com/testgear-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@test-gear.io
 License: Apache-2.0
-Description: # Test Gear TMS adapter for Robot Framework
-        ![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-        
-        ## Getting Started
-        
-        ### Installation
-        ```
-        pip install testgear-adapter-robotframework
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
-            certValidation = <optional boolean>
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
-            * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
-              
-            * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
-            
-            * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
-                
-                * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
-                * 1 - in this mode, the adapter sends all results to the test run without filtering.
-                * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-           
-            * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-            
-            * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-            
-        3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
-        * `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
-          
-        * `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
-          
-        * `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
-        
-        * `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-        
-        * `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-        
-        #### Command line
-        
-        You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
-        * `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
-          
-        * `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
-          
-        * `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
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
-        $ robot -v testgear <test directory>
-        ```
-        
-        Launch with command-line parameters (parameters are case-insensitive):
-        
-        ```
-        $ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
-        ```
-        
-        If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-        
-        ### Tags
-        
-        Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
-        
-        Description of tags:
-        - `testgear.workItemsId` - linking an autotest to a test case
-        - `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
-        - `testgear.externalId` - ID of the autotest within the project in the TMS System
-        - `testgear.title` - title in the autotest card (default - name of test)
-        - `testgear.description` - description in the autotest card (default - documentation of test)
-        - `testgear.links` - links in the autotest card
-        - `testgear.labels` - labels in the autotest card
-        - `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
-        - `testgear.className` - subdirectory in the TMS system (default - class's name of test)
-        
-        Description of methods:
-        - `Add Links` - links in the autotest result
-        - `Add Link` - add one link in the autotest result
-        - `Add Attachments` - uploading files in the autotest result
-        - `Add Attachment` - upload given content with given filename in the autotest result
-        - `Add Message` - information about autotest in the autotest result
-        
-        ### Parallel execution
-        
-        You can also run your test in parallel with [Pabot](https://pabot.org/).
-        
-        ```
-        $ pabot --pabotlib -v testgear <test directory>
-        ```
-        
-        All other settings are the same as for standard execution.
-        
-        ### Examples
-        
-        ```robotframework
-        *** Settings ***
-        Documentation      Main Suite with examples
-        Library            testgear_adapter_robotframework.TMSLibrary
-        
-        *** Variables ***
-        &{SIMPLE_LINK}             url=http://google.com
-        &{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
-        
-        @{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
-        
-        
-        *** Test Cases ***
-        Simple Test
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with link as variable
-            [Tags]   testgear.links:${SIMPLE_LINK}
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with link as dict
-            [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with WorkitemId as string
-            [Tags]   testgear.workitemsID:123
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with WorkitemId as list
-            [Tags]   testgear.workitemsID:${{[123, '456']}}
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with Title or Description or DisplayName with simple formatting
-            [Documentation]  Tags are space sensitive, use only one space between words
-            [Tags]   testgear.displayName:This works     testgear.title:'This also works'
-            ...    testgear.description:"This works too"
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Test With All Params
-            [Documentation]  It's better to use this kind of formatting for different data types in tags
-            [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
-            ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
-            ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
-            [Setup]  Setup
-            Log    Something
-            Log    Another
-            [Teardown]  Teardown
-        
-        Test With Add Link
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Add Links    @{LINKS}
-        #    You can also add one link (default type is Defect)
-            Add Link    http://ya.ru
-            Add Link    http://ya.ru    type=Issue
-            Add Link    ${SIMPLE_LINK}[url]
-            [Teardown]  Teardown
-        
-        Test With Add Attachment
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            ${V}   Get Variables
-            Add Attachment    '${V}'    file.txt
-            Add Attachments    images/banner.png     images/icon.png
-            [Teardown]  Teardown
-        
-        Test With Add Message
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Add Message    Wow, it's my error message!
-            Fail
-            [Teardown]  Teardown
-        ```
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-        
-        # License
-        
-        Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
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
+# Test Gear TMS adapter for Robot Framework
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+```
+pip install testgear-adapter-robotframework
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
+    certValidation = <optional boolean>
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
+    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
+      
+    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
+    
+    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
+        
+        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
+        * 1 - in this mode, the adapter sends all results to the test run without filtering.
+        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
+   
+    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
+    
+    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
+    
+3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
+* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
+  
+* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
+  
+* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
+
+* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
+
+* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
+
+#### Command line
+
+You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
+* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
+  
+* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
+  
+* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
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
+$ robot -v testgear <test directory>
+```
+
+Launch with command-line parameters (parameters are case-insensitive):
+
+```
+$ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
+```
+
+If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
+
+Description of tags:
+- `testgear.workItemsId` - linking an autotest to a test case
+- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
+- `testgear.externalId` - ID of the autotest within the project in the TMS System
+- `testgear.title` - title in the autotest card (default - name of test)
+- `testgear.description` - description in the autotest card (default - documentation of test)
+- `testgear.links` - links in the autotest card
+- `testgear.labels` - labels in the autotest card
+- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
+- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+- `Add Links` - links in the autotest result
+- `Add Link` - add one link in the autotest result
+- `Add Attachments` - uploading files in the autotest result
+- `Add Attachment` - upload given content with given filename in the autotest result
+- `Add Message` - information about autotest in the autotest result
+
+### Parallel execution
+
+You can also run your test in parallel with [Pabot](https://pabot.org/).
+
+```
+$ pabot --pabotlib -v testgear <test directory>
+```
+
+All other settings are the same as for standard execution.
+
+### Examples
+
+```robotframework
+*** Settings ***
+Documentation      Main Suite with examples
+Library            testgear_adapter_robotframework.TMSLibrary
+
+*** Variables ***
+&{SIMPLE_LINK}             url=http://google.com
+&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
+
+@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
+
+
+*** Test Cases ***
+Simple Test
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as variable
+    [Tags]   testgear.links:${SIMPLE_LINK}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as dict
+    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as string
+    [Tags]   testgear.workitemsID:123
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as list
+    [Tags]   testgear.workitemsID:${{[123, '456']}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with Title or Description or DisplayName with simple formatting
+    [Documentation]  Tags are space sensitive, use only one space between words
+    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
+    ...    testgear.description:"This works too"
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Test With All Params
+    [Documentation]  It's better to use this kind of formatting for different data types in tags
+    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
+    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
+    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
+    [Setup]  Setup
+    Log    Something
+    Log    Another
+    [Teardown]  Teardown
+
+Test With Add Link
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Links    @{LINKS}
+#    You can also add one link (default type is Defect)
+    Add Link    http://ya.ru
+    Add Link    http://ya.ru    type=Issue
+    Add Link    ${SIMPLE_LINK}[url]
+    [Teardown]  Teardown
+
+Test With Add Attachment
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    ${V}   Get Variables
+    Add Attachment    '${V}'    file.txt
+    Add Attachments    images/banner.png     images/icon.png
+    [Teardown]  Teardown
+
+Test With Add Message
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Message    Wow, it's my error message!
+    Fail
+    [Teardown]  Teardown
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-robotframework-2.1.1/README.md` & `testgear-adapter-robotframework-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `testgear-adapter-robotframework-2.1.1/setup.py` & `testgear-adapter-robotframework-2.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testgear-adapter-robotframework',
-    version='2.1.1',
+    version='2.1.2',
     description='Robot Framework adapter for Test Gear',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testgear-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@test-gear.io',
     license='Apache-2.0',
@@ -16,9 +16,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testgear_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testgear-python-commons==2.1.1']
+    install_requires=['attrs', 'robotframework', 'testgear-python-commons==2.1.2']
 )
```

### Comparing `testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/TMSLibrary.py` & `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/TMSLibrary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from robot.libraries.BuiltIn import BuiltIn
 
-from testgear_python_commons.services import AdapterManager
+from testgear_python_commons.services import TmsPluginManager
 
 from .listeners import AutotestAdapter, TestRunAdapter
 from .models import Link, Option
 
 
 def enabled(func):
     def wrapped(self, *args, **kwargs):
@@ -40,15 +40,15 @@
         built_in = BuiltIn()
         self.enabled = built_in.get_variable_value("${testgear}", None) is not None
         if self.enabled:
             cli_params = ["tmsUrl", "tmsPrivateToken", "tmsProjectId",
                           "tmsConfigurationId", "tmsTestRunId", "tmsTestRunName",
                           "tmsAdapterMode", "tmsConfigFile", "tmsCertValidation", "tmsAutomaticCreationTestCases"]
             option = Option(**{param: built_in.get_variable_value(f'${{{param}}}', None) for param in cli_params})
-            self.adapter_manager = AdapterManager(option)
+            self.adapter_manager = TmsPluginManager.get_adapter_manager(option)
             pabot_index = built_in.get_variable_value('${PABOTQUEUEINDEX}', None)
             if pabot_index is not None:
                 try:
                     from pabot import PabotLib
                     pabot = PabotLib()
                     if int(pabot_index) == 0:
                         test_run_id = self.adapter_manager.get_test_run_id()
```

### Comparing `testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/listeners.py` & `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/listeners.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework/models.py` & `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework/models.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/PKG-INFO` & `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,298 +1,297 @@
 Metadata-Version: 2.1
 Name: testgear-adapter-robotframework
-Version: 2.1.1
+Version: 2.1.2
 Summary: Robot Framework adapter for Test Gear
 Home-page: https://github.com/testgear-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@test-gear.io
 License: Apache-2.0
-Description: # Test Gear TMS adapter for Robot Framework
-        ![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
-        
-        ## Getting Started
-        
-        ### Installation
-        ```
-        pip install testgear-adapter-robotframework
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
-            certValidation = <optional boolean>
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
-            * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
-              
-            * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
-            
-            * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
-                
-                * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
-                * 1 - in this mode, the adapter sends all results to the test run without filtering.
-                * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
-           
-            * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
-            
-            * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
-            
-        3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
-        * `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
-          
-        * `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
-          
-        * `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
-        
-        * `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
-        
-        * `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
-        
-        #### Command line
-        
-        You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
-        * `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
-          
-        * `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
-          
-        * `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
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
-        $ robot -v testgear <test directory>
-        ```
-        
-        Launch with command-line parameters (parameters are case-insensitive):
-        
-        ```
-        $ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
-        ```
-        
-        If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
-        
-        ### Tags
-        
-        Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
-        
-        Description of tags:
-        - `testgear.workItemsId` - linking an autotest to a test case
-        - `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
-        - `testgear.externalId` - ID of the autotest within the project in the TMS System
-        - `testgear.title` - title in the autotest card (default - name of test)
-        - `testgear.description` - description in the autotest card (default - documentation of test)
-        - `testgear.links` - links in the autotest card
-        - `testgear.labels` - labels in the autotest card
-        - `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
-        - `testgear.className` - subdirectory in the TMS system (default - class's name of test)
-        
-        Description of methods:
-        - `Add Links` - links in the autotest result
-        - `Add Link` - add one link in the autotest result
-        - `Add Attachments` - uploading files in the autotest result
-        - `Add Attachment` - upload given content with given filename in the autotest result
-        - `Add Message` - information about autotest in the autotest result
-        
-        ### Parallel execution
-        
-        You can also run your test in parallel with [Pabot](https://pabot.org/).
-        
-        ```
-        $ pabot --pabotlib -v testgear <test directory>
-        ```
-        
-        All other settings are the same as for standard execution.
-        
-        ### Examples
-        
-        ```robotframework
-        *** Settings ***
-        Documentation      Main Suite with examples
-        Library            testgear_adapter_robotframework.TMSLibrary
-        
-        *** Variables ***
-        &{SIMPLE_LINK}             url=http://google.com
-        &{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
-        
-        @{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
-        
-        
-        *** Test Cases ***
-        Simple Test
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with link as variable
-            [Tags]   testgear.links:${SIMPLE_LINK}
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with link as dict
-            [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with WorkitemId as string
-            [Tags]   testgear.workitemsID:123
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with WorkitemId as list
-            [Tags]   testgear.workitemsID:${{[123, '456']}}
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Simple Test with Title or Description or DisplayName with simple formatting
-            [Documentation]  Tags are space sensitive, use only one space between words
-            [Tags]   testgear.displayName:This works     testgear.title:'This also works'
-            ...    testgear.description:"This works too"
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Log  I'am a step
-            [Teardown]  Teardown
-        
-        Test With All Params
-            [Documentation]  It's better to use this kind of formatting for different data types in tags
-            [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
-            ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
-            ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
-            [Setup]  Setup
-            Log    Something
-            Log    Another
-            [Teardown]  Teardown
-        
-        Test With Add Link
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Add Links    @{LINKS}
-        #    You can also add one link (default type is Defect)
-            Add Link    http://ya.ru
-            Add Link    http://ya.ru    type=Issue
-            Add Link    ${SIMPLE_LINK}[url]
-            [Teardown]  Teardown
-        
-        Test With Add Attachment
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            ${V}   Get Variables
-            Add Attachment    '${V}'    file.txt
-            Add Attachments    images/banner.png     images/icon.png
-            [Teardown]  Teardown
-        
-        Test With Add Message
-            [Setup]  Setup
-            Do Something
-            Do Another Thing
-            Add Message    Wow, it's my error message!
-            Fail
-            [Teardown]  Teardown
-        ```
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-        
-        # License
-        
-        Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
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
+# Test Gear TMS adapter for Robot Framework
+![Test Gear](https://raw.githubusercontent.com/testgear-tms/adapters-python/master/images/banner.png)
+
+## Getting Started
+
+### Installation
+```
+pip install testgear-adapter-robotframework
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
+    certValidation = <optional boolean>
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
+    * `testRunId` - id of the created test run in TMS instance. `testRunId` is optional. If it is not provided, it is created automatically.  
+      
+    * `testRunName` - parameter for specifying the name of test run in TMS instance. `testRunName` is optional. If it is not provided, it is created automatically.   
+    
+    * `adapterMode` - adapter mode. Default value - 0. The adapter supports following modes:  
+        
+        * 0 - in this mode, the adapter filters tests by test run ID and configuration ID, and sends the results to the test run.
+        * 1 - in this mode, the adapter sends all results to the test run without filtering.
+        * 2 - in this mode, the adapter creates a new test run and sends results to the new test run.
+   
+    * `certValidation` - it enables/disables certificate validation. `certValidation` is optional.
+    
+    * `tmsProxy` - it enables debug mode. `tmsProxy` is optional.
+    
+3. Import `TMSLibrary` in your RobotFramework Tests (see `examples` directory)
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
+* `TMS_TEST_RUN_ID` - ID of the created test-run in TMS instance. `TMS_TEST_RUN_ID` is optional. If it is not provided, it is created automatically.
+  
+* `TMS_TEST_RUN_NAME` - name of the new test-run.`TMS_TEST_RUN_NAME` is optional. If it is not provided, it is created automatically.
+  
+* `TMS_CONFIG_FILE` - name of the configuration file. `TMS_CONFIG_FILE` is optional. If it is not provided, it is used default file name.
+
+* `TMS_PROXY` - it enables debug mode. `TMS_PROXY` is optional.
+
+* `TMS_CERT_VALIDATION` - it enables/disables certificate validation. `TMS_CERT_VALIDATION` is optional.
+
+#### Command line
+
+You also can use CLI variables, that sent to Robot Framework via `-v` option  (CLI variables take precedence over environment variables):
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
+* `tmsTestRunId` - ID of the created test-run in TMS instance. `tmsTestRunId` is optional. If it is not provided, it is created automatically.
+  
+* `tmsTestRunName` - name of the new test-run.`tmsTestRunName` is optional. If it is not provided, it is created automatically.
+  
+* `tmsConfigFile` - name of the configuration file. `tmsConfigFile` is optional. If it is not provided, it is used default file name.
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
+$ robot -v testgear <test directory>
+```
+
+Launch with command-line parameters (parameters are case-insensitive):
+
+```
+$ robot -v testgear -v tmsUrl:<url> -v tmsPrivateToken:<token> -v tmsProjectId:<id> -v tmsConfigurationId:<id> -v tmsTestRunId:<optional id> -v tmsTestRunName:<optional name> -v tmsProxy:'{"http":"http://localhost:8888","https":"http://localhost:8888"}' -v tmsConfigFile:<optional file> -v tmsCertValidation:<optional boolean> <test directory>
+```
+
+If you want to enable debug mode then see [How to enable debug logging?](https://github.com/testgear-tms/adapters-python/tree/main/testgear-python-commons)
+
+### Tags
+
+Tags can be used to specify information about autotest. Tags are space sensitive, use only one space between words.
+
+Description of tags:
+- `testgear.workItemsId` - linking an autotest to a test case
+- `testgear.displayName` - name of the autotest in the TMS system (default - name of test)
+- `testgear.externalId` - ID of the autotest within the project in the TMS System
+- `testgear.title` - title in the autotest card (default - name of test)
+- `testgear.description` - description in the autotest card (default - documentation of test)
+- `testgear.links` - links in the autotest card
+- `testgear.labels` - labels in the autotest card
+- `testgear.nameSpace` - directory in the TMS system (default - file's name of test)
+- `testgear.className` - subdirectory in the TMS system (default - class's name of test)
+
+Description of methods:
+- `Add Links` - links in the autotest result
+- `Add Link` - add one link in the autotest result
+- `Add Attachments` - uploading files in the autotest result
+- `Add Attachment` - upload given content with given filename in the autotest result
+- `Add Message` - information about autotest in the autotest result
+
+### Parallel execution
+
+You can also run your test in parallel with [Pabot](https://pabot.org/).
+
+```
+$ pabot --pabotlib -v testgear <test directory>
+```
+
+All other settings are the same as for standard execution.
+
+### Examples
+
+```robotframework
+*** Settings ***
+Documentation      Main Suite with examples
+Library            testgear_adapter_robotframework.TMSLibrary
+
+*** Variables ***
+&{SIMPLE_LINK}             url=http://google.com
+&{FULL_LINK}               url=http://google.co.uk   title=Google     type=Related   description=just a link
+
+@{LINKS}               ${SIMPLE_LINK}   ${FULL_LINK}
+
+
+*** Test Cases ***
+Simple Test
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as variable
+    [Tags]   testgear.links:${SIMPLE_LINK}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with link as dict
+    [Tags]   testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as string
+    [Tags]   testgear.workitemsID:123
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with WorkitemId as list
+    [Tags]   testgear.workitemsID:${{[123, '456']}}
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Simple Test with Title or Description or DisplayName with simple formatting
+    [Documentation]  Tags are space sensitive, use only one space between words
+    [Tags]   testgear.displayName:This works     testgear.title:'This also works'
+    ...    testgear.description:"This works too"
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Log  I'am a step
+    [Teardown]  Teardown
+
+Test With All Params
+    [Documentation]  It's better to use this kind of formatting for different data types in tags
+    [Tags]   testgear.externalID:123    testgear.title:${{'Different title'}}   testgear.displayName:${{'Different name'}}
+    ...     testgear.description:${{'Different description'}}    testgear.workitemsID:${{[123, '456']}}
+    ...     testgear.links:${{{'url': 'http://google.com', 'type':'Issue'}}}   testgear.labels:${{['smoke', 'lol']}}
+    [Setup]  Setup
+    Log    Something
+    Log    Another
+    [Teardown]  Teardown
+
+Test With Add Link
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Links    @{LINKS}
+#    You can also add one link (default type is Defect)
+    Add Link    http://ya.ru
+    Add Link    http://ya.ru    type=Issue
+    Add Link    ${SIMPLE_LINK}[url]
+    [Teardown]  Teardown
+
+Test With Add Attachment
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    ${V}   Get Variables
+    Add Attachment    '${V}'    file.txt
+    Add Attachments    images/banner.png     images/icon.png
+    [Teardown]  Teardown
+
+Test With Add Message
+    [Setup]  Setup
+    Do Something
+    Do Another Thing
+    Add Message    Wow, it's my error message!
+    Fail
+    [Teardown]  Teardown
+```
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testgear-tms/adapters-python/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testgear-tms/adapters-python/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testgear-tms/adapters-python/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testgear-adapter-robotframework-2.1.1/src/testgear_adapter_robotframework.egg-info/SOURCES.txt` & `testgear-adapter-robotframework-2.1.2/src/testgear_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

