# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.16.0.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.16.0.tar", last modified: Thu Apr 20 22:24:22 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.16.1.tar", last modified: Fri Apr 21 03:05:06 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.16.0.tar` & `aws_prototyping_sdk.type_safe_api-0.16.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:24:22.365283 aws_prototyping_sdk.type_safe_api-0.16.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-20 22:24:22.361283 aws_prototyping_sdk.type_safe_api-0.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    53263 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:24:22.365283 aws_prototyping_sdk.type_safe_api-0.16.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:24:22.349283 aws_prototyping_sdk.type_safe_api-0.16.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:24:22.349283 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:24:22.357283 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   275121 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:24:22.361283 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   841643 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.16.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:24:04.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:24:22.357283 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54204 2023-04-20 22:24:22.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-20 22:24:22.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:24:22.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-20 22:24:22.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 22:24:22.000000 aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:05:06.418392 aws_prototyping_sdk.type_safe_api-0.16.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    54094 2023-04-21 03:05:06.418392 aws_prototyping_sdk.type_safe_api-0.16.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53153 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:05:06.418392 aws_prototyping_sdk.type_safe_api-0.16.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:05:06.410392 aws_prototyping_sdk.type_safe_api-0.16.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:05:06.410392 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:05:06.414392 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   285917 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:05:06.418392 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   851219 2023-04-21 03:04:49.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.16.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:04:50.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:05:06.414392 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54094 2023-04-21 03:05:06.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-21 03:05:06.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:05:06.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 03:05:06.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 03:05:06.000000 aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.16.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.16.0
+Version: 0.16.1
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -1115,16 +1115,15 @@
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
-lambdas.addDependency(`${api.runtime.python!.name}@{path="${path.relative(lambdas.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(lambdas, api.runtime.python!);
+monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
 lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
 lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
 lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
 lambdas.gitignore.addPatterns('lambda-dist');
@@ -1139,20 +1138,17 @@
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
 
 // The infrastructure project depends on the python types, python infrastructure, and the lambda package
-infra.addDependency(`${api.runtime.python!.name}@{path="${path.relative(infra.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.runtime.python!);
-infra.addDependency(`${api.infrastructure.python!.name}@{path="${path.relative(infra.outdir, api.infrastructure.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.infrastructure.python!);
-infra.addDependency(`${lambdas.name}@{path="${path.relative(infra.outdir, lambdas.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, lambdas);
+monorepo.addPythonPoetryDependency(infra, api.runtime.python!);
+monorepo.addPythonPoetryDependency(infra, api.infrastructure.python!);
+monorepo.addPythonPoetryDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
 In your CDK application, consume the `Api` construct, vended from the generated Python infrastructure package.
@@ -1265,20 +1261,15 @@
   outdir: 'packages/lambdas',
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
-lambdas.addDependency(`${api.runtime.java!.pom.groupId}/${api.runtime.java!.pom.artifactId}@${api.runtime.java!.pom.version}`);
-lambdas.pom.addRepository({
-  url: `file://${path.relative(lambdas.outdir, api.runtime.java!.outdir)}/dist/java`,
-  id: 'java-api-runtime',
-});
-monorepo.addImplicitDependency(lambdas, api.runtime.java!);
+monorepo.addJavaDependency(lambdas, api.runtime.java!);
 
 // Use the maven shade plugin to build a "super jar" which we can deploy to AWS Lambda
 lambdas.pom.addPlugin("org.apache.maven.plugins/maven-shade-plugin@3.3.0", {
   configuration: {
     createDependencyReducedPom: false,
   },
   executions: [
@@ -1298,20 +1289,15 @@
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
 
 // Add a dependency on the generated CDK infrastructure
-infra.addDependency(`${api.infrastructure.java!.pom.groupId}/${api.infrastructure.java!.pom.artifactId}@${api.infrastructure.java!.pom.version}`);
-infra.pom.addRepository({
-  url: `file://${path.relative(infra.outdir, api.infrastructure.java!.outdir)}/dist/java`,
-  id: 'java-api-infra',
-});
-monorepo.addImplicitDependency(infra, api.infrastructure.java!);
+monorepo.addJavaDependency(infra, api.infrastructure.java!);
 
 // Make sure the java lambda builds before our CDK infra
 monorepo.addImplicitDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
@@ -1470,7 +1456,39 @@
 When multiple tags are used, the "first" tag is considered to be the API that the operation belongs to, so in the generated client, the above example operation would be included in the `PetsApi` client but not the `UsersApi` client.
 
 Multiple tags are still useful for documentation generation, for example `DocumentationFormat.HTML_REDOC` will group operations by tag in the side navigation bar.
 
 If you would like to introduce tags without breaking existing clients, we recommend first adding a tag named `default` to all operations.
 
 ⚠️ **Important Note**: Smithy versions below `1.28.0` sort tags in alphabetical order and so the "first" tag will be the earliest in the alphabet. Therefore, if using tags with older versions of Smithy, we recommend prefixing your desired first tag with an underscore (for example `_default`). This is rectified in `1.28.0`, where tag order from the `@tags` trait is preserved.
+
+#### Smithy Model Libraries and Dependencies
+
+You can instantiate the TypeSafeApiModelProject on its own to create a standalone Smithy model library.
+
+You can consume the library using the `addSmithyDeps` method, which adds a local file dependency on the built Smithy jar.
+
+```python
+// Standalone model project, used as our model library
+const shapes = new TypeSafeApiModelProject({
+  name: "shapes",
+  parent: monorepo,
+  outdir: "packages/shapes",
+  modelLanguage: ModelLanguage.SMITHY,
+  modelOptions: {
+    smithy: {
+      serviceName: {
+        namespace: "com.my.shared.shapes",
+        serviceName: "Ignored",
+      },
+    },
+  },
+});
+
+const api = new TypeSafeApiProject({ ... });
+
+// Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
+monorepo.addImplicitDependency(api.model, shapes);
+
+// Add a local file dependency on the built shapes jar
+api.model.smithy!.addSmithyDeps(shapes.smithy!);
+```
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/README.md` & `aws_prototyping_sdk.type_safe_api-0.16.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1091,16 +1091,15 @@
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
-lambdas.addDependency(`${api.runtime.python!.name}@{path="${path.relative(lambdas.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(lambdas, api.runtime.python!);
+monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
 lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
 lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
 lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
 lambdas.gitignore.addPatterns('lambda-dist');
@@ -1115,20 +1114,17 @@
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
 
 // The infrastructure project depends on the python types, python infrastructure, and the lambda package
-infra.addDependency(`${api.runtime.python!.name}@{path="${path.relative(infra.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.runtime.python!);
-infra.addDependency(`${api.infrastructure.python!.name}@{path="${path.relative(infra.outdir, api.infrastructure.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.infrastructure.python!);
-infra.addDependency(`${lambdas.name}@{path="${path.relative(infra.outdir, lambdas.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, lambdas);
+monorepo.addPythonPoetryDependency(infra, api.runtime.python!);
+monorepo.addPythonPoetryDependency(infra, api.infrastructure.python!);
+monorepo.addPythonPoetryDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
 In your CDK application, consume the `Api` construct, vended from the generated Python infrastructure package.
@@ -1241,20 +1237,15 @@
   outdir: 'packages/lambdas',
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
-lambdas.addDependency(`${api.runtime.java!.pom.groupId}/${api.runtime.java!.pom.artifactId}@${api.runtime.java!.pom.version}`);
-lambdas.pom.addRepository({
-  url: `file://${path.relative(lambdas.outdir, api.runtime.java!.outdir)}/dist/java`,
-  id: 'java-api-runtime',
-});
-monorepo.addImplicitDependency(lambdas, api.runtime.java!);
+monorepo.addJavaDependency(lambdas, api.runtime.java!);
 
 // Use the maven shade plugin to build a "super jar" which we can deploy to AWS Lambda
 lambdas.pom.addPlugin("org.apache.maven.plugins/maven-shade-plugin@3.3.0", {
   configuration: {
     createDependencyReducedPom: false,
   },
   executions: [
@@ -1274,20 +1265,15 @@
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
 
 // Add a dependency on the generated CDK infrastructure
-infra.addDependency(`${api.infrastructure.java!.pom.groupId}/${api.infrastructure.java!.pom.artifactId}@${api.infrastructure.java!.pom.version}`);
-infra.pom.addRepository({
-  url: `file://${path.relative(infra.outdir, api.infrastructure.java!.outdir)}/dist/java`,
-  id: 'java-api-infra',
-});
-monorepo.addImplicitDependency(infra, api.infrastructure.java!);
+monorepo.addJavaDependency(infra, api.infrastructure.java!);
 
 // Make sure the java lambda builds before our CDK infra
 monorepo.addImplicitDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
@@ -1446,7 +1432,39 @@
 When multiple tags are used, the "first" tag is considered to be the API that the operation belongs to, so in the generated client, the above example operation would be included in the `PetsApi` client but not the `UsersApi` client.
 
 Multiple tags are still useful for documentation generation, for example `DocumentationFormat.HTML_REDOC` will group operations by tag in the side navigation bar.
 
 If you would like to introduce tags without breaking existing clients, we recommend first adding a tag named `default` to all operations.
 
 ⚠️ **Important Note**: Smithy versions below `1.28.0` sort tags in alphabetical order and so the "first" tag will be the earliest in the alphabet. Therefore, if using tags with older versions of Smithy, we recommend prefixing your desired first tag with an underscore (for example `_default`). This is rectified in `1.28.0`, where tag order from the `@tags` trait is preserved.
+
+#### Smithy Model Libraries and Dependencies
+
+You can instantiate the TypeSafeApiModelProject on its own to create a standalone Smithy model library.
+
+You can consume the library using the `addSmithyDeps` method, which adds a local file dependency on the built Smithy jar.
+
+```python
+// Standalone model project, used as our model library
+const shapes = new TypeSafeApiModelProject({
+  name: "shapes",
+  parent: monorepo,
+  outdir: "packages/shapes",
+  modelLanguage: ModelLanguage.SMITHY,
+  modelOptions: {
+    smithy: {
+      serviceName: {
+        namespace: "com.my.shared.shapes",
+        serviceName: "Ignored",
+      },
+    },
+  },
+});
+
+const api = new TypeSafeApiProject({ ... });
+
+// Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
+monorepo.addImplicitDependency(api.model, shapes);
+
+// Add a local file dependency on the built shapes jar
+api.model.smithy!.addSmithyDeps(shapes.smithy!);
+```
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/setup.py` & `aws_prototyping_sdk.type_safe_api-0.16.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.16.0",
+    "version": "0.16.1",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.16.0.jsii.tgz"
+            "type-safe-api@0.16.1.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1092,16 +1092,15 @@
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
-lambdas.addDependency(`${api.runtime.python!.name}@{path="${path.relative(lambdas.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(lambdas, api.runtime.python!);
+monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
 lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
 lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
 lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
 lambdas.gitignore.addPatterns('lambda-dist');
@@ -1116,20 +1115,17 @@
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
 
 // The infrastructure project depends on the python types, python infrastructure, and the lambda package
-infra.addDependency(`${api.runtime.python!.name}@{path="${path.relative(infra.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.runtime.python!);
-infra.addDependency(`${api.infrastructure.python!.name}@{path="${path.relative(infra.outdir, api.infrastructure.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.infrastructure.python!);
-infra.addDependency(`${lambdas.name}@{path="${path.relative(infra.outdir, lambdas.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, lambdas);
+monorepo.addPythonPoetryDependency(infra, api.runtime.python!);
+monorepo.addPythonPoetryDependency(infra, api.infrastructure.python!);
+monorepo.addPythonPoetryDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
 In your CDK application, consume the `Api` construct, vended from the generated Python infrastructure package.
@@ -1242,20 +1238,15 @@
   outdir: 'packages/lambdas',
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
-lambdas.addDependency(`${api.runtime.java!.pom.groupId}/${api.runtime.java!.pom.artifactId}@${api.runtime.java!.pom.version}`);
-lambdas.pom.addRepository({
-  url: `file://${path.relative(lambdas.outdir, api.runtime.java!.outdir)}/dist/java`,
-  id: 'java-api-runtime',
-});
-monorepo.addImplicitDependency(lambdas, api.runtime.java!);
+monorepo.addJavaDependency(lambdas, api.runtime.java!);
 
 // Use the maven shade plugin to build a "super jar" which we can deploy to AWS Lambda
 lambdas.pom.addPlugin("org.apache.maven.plugins/maven-shade-plugin@3.3.0", {
   configuration: {
     createDependencyReducedPom: false,
   },
   executions: [
@@ -1275,20 +1266,15 @@
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
 
 // Add a dependency on the generated CDK infrastructure
-infra.addDependency(`${api.infrastructure.java!.pom.groupId}/${api.infrastructure.java!.pom.artifactId}@${api.infrastructure.java!.pom.version}`);
-infra.pom.addRepository({
-  url: `file://${path.relative(infra.outdir, api.infrastructure.java!.outdir)}/dist/java`,
-  id: 'java-api-infra',
-});
-monorepo.addImplicitDependency(infra, api.infrastructure.java!);
+monorepo.addJavaDependency(infra, api.infrastructure.java!);
 
 // Make sure the java lambda builds before our CDK infra
 monorepo.addImplicitDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
@@ -1447,14 +1433,46 @@
 When multiple tags are used, the "first" tag is considered to be the API that the operation belongs to, so in the generated client, the above example operation would be included in the `PetsApi` client but not the `UsersApi` client.
 
 Multiple tags are still useful for documentation generation, for example `DocumentationFormat.HTML_REDOC` will group operations by tag in the side navigation bar.
 
 If you would like to introduce tags without breaking existing clients, we recommend first adding a tag named `default` to all operations.
 
 ⚠️ **Important Note**: Smithy versions below `1.28.0` sort tags in alphabetical order and so the "first" tag will be the earliest in the alphabet. Therefore, if using tags with older versions of Smithy, we recommend prefixing your desired first tag with an underscore (for example `_default`). This is rectified in `1.28.0`, where tag order from the `@tags` trait is preserved.
+
+#### Smithy Model Libraries and Dependencies
+
+You can instantiate the TypeSafeApiModelProject on its own to create a standalone Smithy model library.
+
+You can consume the library using the `addSmithyDeps` method, which adds a local file dependency on the built Smithy jar.
+
+```python
+// Standalone model project, used as our model library
+const shapes = new TypeSafeApiModelProject({
+  name: "shapes",
+  parent: monorepo,
+  outdir: "packages/shapes",
+  modelLanguage: ModelLanguage.SMITHY,
+  modelOptions: {
+    smithy: {
+      serviceName: {
+        namespace: "com.my.shared.shapes",
+        serviceName: "Ignored",
+      },
+    },
+  },
+});
+
+const api = new TypeSafeApiProject({ ... });
+
+// Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
+monorepo.addImplicitDependency(api.model, shapes);
+
+// Add a local file dependency on the built shapes jar
+api.model.smithy!.addSmithyDeps(shapes.smithy!);
+```
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -3394,14 +3412,101 @@
     def __init__(self) -> None:
         '''
         :stability: experimental
         '''
         jsii.create(self.__class__, self, [])
 
 
+class OpenApiDefinition(
+    _projen_04054675.Component,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-prototyping-sdk/type-safe-api.OpenApiDefinition",
+):
+    '''(experimental) The OpenAPI Spec.
+
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        project: "TypeSafeApiModelProject",
+        *,
+        open_api_options: typing.Union["OpenApiModelOptions", typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''
+        :param project: -
+        :param open_api_options: (experimental) Options for the openapi model.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__370ebffac0840359674dee761aaeaa906d40299ef3ec2d6323f2214155e1db2d)
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+        options = OpenApiDefinitionOptions(open_api_options=open_api_options)
+
+        jsii.create(self.__class__, self, [project, options])
+
+    @builtins.property
+    @jsii.member(jsii_name="openApiSpecificationPath")
+    def open_api_specification_path(self) -> builtins.str:
+        '''(experimental) Path to the root OpenAPI specification file.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "openApiSpecificationPath"))
+
+
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.OpenApiDefinitionOptions",
+    jsii_struct_bases=[],
+    name_mapping={"open_api_options": "openApiOptions"},
+)
+class OpenApiDefinitionOptions:
+    def __init__(
+        self,
+        *,
+        open_api_options: typing.Union["OpenApiModelOptions", typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''(experimental) Options for the OpenAPI Spec.
+
+        :param open_api_options: (experimental) Options for the openapi model.
+
+        :stability: experimental
+        '''
+        if isinstance(open_api_options, dict):
+            open_api_options = OpenApiModelOptions(**open_api_options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__591f8c9caef1c0f0144c3c8f46e6c9515a9b59283a269f9a55ff68f0655c28bd)
+            check_type(argname="argument open_api_options", value=open_api_options, expected_type=type_hints["open_api_options"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "open_api_options": open_api_options,
+        }
+
+    @builtins.property
+    def open_api_options(self) -> "OpenApiModelOptions":
+        '''(experimental) Options for the openapi model.
+
+        :stability: experimental
+        '''
+        result = self._values.get("open_api_options")
+        assert result is not None, "Required property 'open_api_options' is missing"
+        return typing.cast("OpenApiModelOptions", result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "OpenApiDefinitionOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.OpenApiModelOptions",
     jsii_struct_bases=[],
     name_mapping={"title": "title"},
 )
 class OpenApiModelOptions:
     def __init__(self, *, title: builtins.str) -> None:
@@ -3562,14 +3667,136 @@
 
     def __repr__(self) -> str:
         return "SmithyCommon(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class SmithyDefinition(
+    _projen_04054675.Component,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@aws-prototyping-sdk/type-safe-api.SmithyDefinition",
+):
+    '''(experimental) Creates a project which transforms a Smithy model to OpenAPI.
+
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        project: "TypeSafeApiModelProject",
+        *,
+        smithy_options: typing.Union["SmithyModelOptions", typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''
+        :param project: -
+        :param smithy_options: (experimental) Smithy engine options.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__da45c4bac118e04412e8a56eb9f701f415202aec168d3c649824a65a789cbdbd)
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+        options = SmithyDefinitionOptions(smithy_options=smithy_options)
+
+        jsii.create(self.__class__, self, [project, options])
+
+    @jsii.member(jsii_name="addDeps")
+    def add_deps(self, *deps: builtins.str) -> None:
+        '''(experimental) Add maven-style or local file dependencies to the smithy model project.
+
+        :param deps: dependencies to add, eg "software.amazon.smithy:smithy-validation-model:1.27.2" or "file://../some/path/build/lib/my-shapes.jar.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__671cc8c9571996d8a6bd6cffe56aa2f3c23025d1e0f1b630b4a312786ae8d84a)
+            check_type(argname="argument deps", value=deps, expected_type=typing.Tuple[type_hints["deps"], ...]) # pyright: ignore [reportGeneralTypeIssues]
+        return typing.cast(None, jsii.invoke(self, "addDeps", [*deps]))
+
+    @jsii.member(jsii_name="addSmithyDeps")
+    def add_smithy_deps(self, *deps: "SmithyDefinition") -> None:
+        '''(experimental) Add dependencies on other smithy models, such that their shapes can be imported in this project.
+
+        :param deps: smithy definitions to depend on.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2b4739ed02d1dd3269fca1e6cf1c9dda195085fbcf4af8a48df5573dbe28ee82)
+            check_type(argname="argument deps", value=deps, expected_type=typing.Tuple[type_hints["deps"], ...]) # pyright: ignore [reportGeneralTypeIssues]
+        return typing.cast(None, jsii.invoke(self, "addSmithyDeps", [*deps]))
+
+    @builtins.property
+    @jsii.member(jsii_name="gradleProjectName")
+    def gradle_project_name(self) -> builtins.str:
+        '''(experimental) Name of the gradle project.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "gradleProjectName"))
+
+    @builtins.property
+    @jsii.member(jsii_name="openApiSpecificationPath")
+    def open_api_specification_path(self) -> builtins.str:
+        '''(experimental) Path to the generated OpenAPI specification, relative to the project outdir.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.get(self, "openApiSpecificationPath"))
+
+
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.SmithyDefinitionOptions",
+    jsii_struct_bases=[],
+    name_mapping={"smithy_options": "smithyOptions"},
+)
+class SmithyDefinitionOptions:
+    def __init__(
+        self,
+        *,
+        smithy_options: typing.Union["SmithyModelOptions", typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''(experimental) Options for a smithy build project.
+
+        :param smithy_options: (experimental) Smithy engine options.
+
+        :stability: experimental
+        '''
+        if isinstance(smithy_options, dict):
+            smithy_options = SmithyModelOptions(**smithy_options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__036ba6d3e9b28066c60f4c0d3d8829c325d7b35770e1fe8c5d663bd4c2a2ce63)
+            check_type(argname="argument smithy_options", value=smithy_options, expected_type=type_hints["smithy_options"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "smithy_options": smithy_options,
+        }
+
+    @builtins.property
+    def smithy_options(self) -> "SmithyModelOptions":
+        '''(experimental) Smithy engine options.
+
+        :stability: experimental
+        '''
+        result = self._values.get("smithy_options")
+        assert result is not None, "Required property 'smithy_options' is missing"
+        return typing.cast("SmithyModelOptions", result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SmithyDefinitionOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.SmithyMavenConfiguration",
     jsii_struct_bases=[],
     name_mapping={"dependencies": "dependencies", "repository_urls": "repositoryUrls"},
 )
 class SmithyMavenConfiguration:
     def __init__(
@@ -4109,27 +4336,51 @@
         )
 
         jsii.create(self.__class__, self, [options])
 
     @builtins.property
     @jsii.member(jsii_name="generateTask")
     def generate_task(self) -> _projen_04054675.Task:
-        '''
+        '''(experimental) Reference to the task used for generating the final bundled OpenAPI specification.
+
         :stability: experimental
         '''
         return typing.cast(_projen_04054675.Task, jsii.get(self, "generateTask"))
 
     @builtins.property
     @jsii.member(jsii_name="parsedSpecFile")
     def parsed_spec_file(self) -> builtins.str:
-        '''
+        '''(experimental) Name of the final bundled OpenAPI specification.
+
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "parsedSpecFile"))
 
+    @builtins.property
+    @jsii.member(jsii_name="openapi")
+    def openapi(self) -> typing.Optional[OpenApiDefinition]:
+        '''(experimental) Reference to the OpenAPI definition component.
+
+        Will be defined if the model language is OpenAPI
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[OpenApiDefinition], jsii.get(self, "openapi"))
+
+    @builtins.property
+    @jsii.member(jsii_name="smithy")
+    def smithy(self) -> typing.Optional[SmithyDefinition]:
+        '''(experimental) Reference to the Smithy definition component.
+
+        Will be defined if the model language is Smithy
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[SmithyDefinition], jsii.get(self, "smithy"))
+
 
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.TypeSafeApiModelProjectOptions",
     jsii_struct_bases=[_projen_04054675.ProjectOptions],
     name_mapping={
         "name": "name",
         "commit_generated": "commitGenerated",
@@ -4592,14 +4843,23 @@
         Only the property corresponding to ``infrastructure.language`` will be defined.
 
         :stability: experimental
         '''
         return typing.cast(GeneratedCodeProjects, jsii.get(self, "infrastructure"))
 
     @builtins.property
+    @jsii.member(jsii_name="model")
+    def model(self) -> TypeSafeApiModelProject:
+        '''(experimental) Project for the api model.
+
+        :stability: experimental
+        '''
+        return typing.cast(TypeSafeApiModelProject, jsii.get(self, "model"))
+
+    @builtins.property
     @jsii.member(jsii_name="runtime")
     def runtime(self) -> GeneratedCodeProjects:
         '''(experimental) Generated runtime projects.
 
         When ``runtime.languages`` includes the corresponding language, the project can be
         assumed to be defined.
 
@@ -5866,18 +6126,22 @@
     "Language",
     "ManagedRule",
     "MethodAndPath",
     "ModelConfiguration",
     "ModelLanguage",
     "ModelOptions",
     "NoneAuthorizer",
+    "OpenApiDefinition",
+    "OpenApiDefinitionOptions",
     "OpenApiModelOptions",
     "RuntimeConfiguration",
     "SmithyBuildOptions",
     "SmithyCommon",
+    "SmithyDefinition",
+    "SmithyDefinitionOptions",
     "SmithyMavenConfiguration",
     "SmithyModelOptions",
     "SmithyPlugin",
     "SmithyProjection",
     "SmithyServiceName",
     "SmithyTransform",
     "TypeSafeApiIntegration",
@@ -6047,14 +6311,29 @@
     *,
     openapi: typing.Optional[typing.Union[OpenApiModelOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     smithy: typing.Optional[typing.Union[SmithyModelOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__370ebffac0840359674dee761aaeaa906d40299ef3ec2d6323f2214155e1db2d(
+    project: TypeSafeApiModelProject,
+    *,
+    open_api_options: typing.Union[OpenApiModelOptions, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__591f8c9caef1c0f0144c3c8f46e6c9515a9b59283a269f9a55ff68f0655c28bd(
+    *,
+    open_api_options: typing.Union[OpenApiModelOptions, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__4384c14a609de971de6d097c833aea11812d657157670113cb85f7eeca095985(
     *,
     title: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -6070,14 +6349,41 @@
     *,
     imports: typing.Optional[typing.Sequence[builtins.str]] = None,
     plugins: typing.Optional[typing.Mapping[builtins.str, typing.Union[SmithyPlugin, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__da45c4bac118e04412e8a56eb9f701f415202aec168d3c649824a65a789cbdbd(
+    project: TypeSafeApiModelProject,
+    *,
+    smithy_options: typing.Union[SmithyModelOptions, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__671cc8c9571996d8a6bd6cffe56aa2f3c23025d1e0f1b630b4a312786ae8d84a(
+    *deps: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2b4739ed02d1dd3269fca1e6cf1c9dda195085fbcf4af8a48df5573dbe28ee82(
+    *deps: SmithyDefinition,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__036ba6d3e9b28066c60f4c0d3d8829c325d7b35770e1fe8c5d663bd4c2a2ce63(
+    *,
+    smithy_options: typing.Union[SmithyModelOptions, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__0658a2f7e63bc2e040803cf6247a71762da6c3f26d27fc3438d10efa0c2b0014(
     *,
     dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
     repository_urls: typing.Optional[typing.Sequence[builtins.str]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.16.0
+Version: 0.16.1
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -1115,16 +1115,15 @@
   moduleName: "lambdas",
   version: "1.0.0",
   // Poetry is used to simplify local python dependencies
   poetry: true,
 });
 
 // Add a local dependency on the generated python runtime
-lambdas.addDependency(`${api.runtime.python!.name}@{path="${path.relative(lambdas.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(lambdas, api.runtime.python!);
+monorepo.addPythonPoetryDependency(lambdas, api.runtime.python!);
 
 // Add commands to the lambda project's package task to create a distributable which can be deployed to AWS Lambda
 lambdas.packageTask.exec(`mkdir -p lambda-dist && rm -rf lambda-dist/*`);
 lambdas.packageTask.exec(`cp -r ${lambdas.moduleName} lambda-dist/${lambdas.moduleName}`);
 lambdas.packageTask.exec(`poetry export --without-hashes --format=requirements.txt > lambda-dist/requirements.txt`);
 lambdas.packageTask.exec(`pip install -r lambda-dist/requirements.txt --target lambda-dist --upgrade`);
 lambdas.gitignore.addPatterns('lambda-dist');
@@ -1139,20 +1138,17 @@
   cdkVersion: "2.0.0",
   moduleName: "infra",
   version: "1.0.0",
   poetry: true,
 });
 
 // The infrastructure project depends on the python types, python infrastructure, and the lambda package
-infra.addDependency(`${api.runtime.python!.name}@{path="${path.relative(infra.outdir, api.runtime.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.runtime.python!);
-infra.addDependency(`${api.infrastructure.python!.name}@{path="${path.relative(infra.outdir, api.infrastructure.python!.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, api.infrastructure.python!);
-infra.addDependency(`${lambdas.name}@{path="${path.relative(infra.outdir, lambdas.outdir)}", develop=true}`);
-monorepo.addImplicitDependency(infra, lambdas);
+monorepo.addPythonPoetryDependency(infra, api.runtime.python!);
+monorepo.addPythonPoetryDependency(infra, api.infrastructure.python!);
+monorepo.addPythonPoetryDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
 #### Use the CDK Construct
 
 In your CDK application, consume the `Api` construct, vended from the generated Python infrastructure package.
@@ -1265,20 +1261,15 @@
   outdir: 'packages/lambdas',
   artifactId: "lambdas",
   groupId: "com.my.api",
   version: "1.0.0",
 });
 
 // The lambdas package needs a dependency on the generated java runtime
-lambdas.addDependency(`${api.runtime.java!.pom.groupId}/${api.runtime.java!.pom.artifactId}@${api.runtime.java!.pom.version}`);
-lambdas.pom.addRepository({
-  url: `file://${path.relative(lambdas.outdir, api.runtime.java!.outdir)}/dist/java`,
-  id: 'java-api-runtime',
-});
-monorepo.addImplicitDependency(lambdas, api.runtime.java!);
+monorepo.addJavaDependency(lambdas, api.runtime.java!);
 
 // Use the maven shade plugin to build a "super jar" which we can deploy to AWS Lambda
 lambdas.pom.addPlugin("org.apache.maven.plugins/maven-shade-plugin@3.3.0", {
   configuration: {
     createDependencyReducedPom: false,
   },
   executions: [
@@ -1298,20 +1289,15 @@
   groupId: "com.my.api",
   mainClass: "com.my.api.MyApp",
   version: "1.0.0",
   cdkVersion: "2.0.0",
 });
 
 // Add a dependency on the generated CDK infrastructure
-infra.addDependency(`${api.infrastructure.java!.pom.groupId}/${api.infrastructure.java!.pom.artifactId}@${api.infrastructure.java!.pom.version}`);
-infra.pom.addRepository({
-  url: `file://${path.relative(infra.outdir, api.infrastructure.java!.outdir)}/dist/java`,
-  id: 'java-api-infra',
-});
-monorepo.addImplicitDependency(infra, api.infrastructure.java!);
+monorepo.addJavaDependency(infra, api.infrastructure.java!);
 
 // Make sure the java lambda builds before our CDK infra
 monorepo.addImplicitDependency(infra, lambdas);
 
 monorepo.synth();
 ```
 
@@ -1470,7 +1456,39 @@
 When multiple tags are used, the "first" tag is considered to be the API that the operation belongs to, so in the generated client, the above example operation would be included in the `PetsApi` client but not the `UsersApi` client.
 
 Multiple tags are still useful for documentation generation, for example `DocumentationFormat.HTML_REDOC` will group operations by tag in the side navigation bar.
 
 If you would like to introduce tags without breaking existing clients, we recommend first adding a tag named `default` to all operations.
 
 ⚠️ **Important Note**: Smithy versions below `1.28.0` sort tags in alphabetical order and so the "first" tag will be the earliest in the alphabet. Therefore, if using tags with older versions of Smithy, we recommend prefixing your desired first tag with an underscore (for example `_default`). This is rectified in `1.28.0`, where tag order from the `@tags` trait is preserved.
+
+#### Smithy Model Libraries and Dependencies
+
+You can instantiate the TypeSafeApiModelProject on its own to create a standalone Smithy model library.
+
+You can consume the library using the `addSmithyDeps` method, which adds a local file dependency on the built Smithy jar.
+
+```python
+// Standalone model project, used as our model library
+const shapes = new TypeSafeApiModelProject({
+  name: "shapes",
+  parent: monorepo,
+  outdir: "packages/shapes",
+  modelLanguage: ModelLanguage.SMITHY,
+  modelOptions: {
+    smithy: {
+      serviceName: {
+        namespace: "com.my.shared.shapes",
+        serviceName: "Ignored",
+      },
+    },
+  },
+});
+
+const api = new TypeSafeApiProject({ ... });
+
+// Add the implicit monorepo dependency (if using the nx-monorepo) to ensure the shape library is built before the api model
+monorepo.addImplicitDependency(api.model, shapes);
+
+// Add a local file dependency on the built shapes jar
+api.model.smithy!.addSmithyDeps(shapes.smithy!);
+```
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.16.0/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.16.1/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.16.0.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.16.1.jsii.tgz
```

