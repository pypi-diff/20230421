# Comparing `tmp/attini-cdk-lib-1.3.0.tar.gz` & `tmp/attini-cdk-lib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attini-cdk-lib-1.3.0.tar", last modified: Wed Mar 29 08:13:41 2023, max compression
+gzip compressed data, was "attini-cdk-lib-1.4.0.tar", last modified: Fri Apr 21 08:48:36 2023, max compression
```

## Comparing `attini-cdk-lib-1.3.0.tar` & `attini-cdk-lib-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/src/attini_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   143169 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/src/attini_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/src/attini_cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/src/attini_cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   250613 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/src/attini_cdk/_jsii/cdk@1.3.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:13:19.000000 attini-cdk-lib-1.3.0/src/attini_cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:41.796856 attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-29 08:13:41.000000 attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-29 08:13:41.000000 attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:13:41.000000 attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-29 08:13:41.000000 attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 08:13:41.000000 attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/attini_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   148861 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/attini_cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   251659 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/_jsii/cdk@1.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:48:23.000000 attini-cdk-lib-1.4.0/src/attini_cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:48:36.663416 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 08:48:36.000000 attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/top_level.txt
```

### Comparing `attini-cdk-lib-1.3.0/LICENSE` & `attini-cdk-lib-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attini-cdk-lib-1.3.0/PKG-INFO` & `attini-cdk-lib-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attini-cdk-lib
-Version: 1.3.0
+Version: 1.4.0
 Summary: Attini CDK Constructs
 Home-page: https://attini.io
 Author: oscarostrand<contact@attini.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/attini-cloud-solutions/attini-cdk-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `attini-cdk-lib-1.3.0/README.md` & `attini-cdk-lib-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `attini-cdk-lib-1.3.0/setup.py` & `attini-cdk-lib-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "attini-cdk-lib",
-    "version": "1.3.0",
+    "version": "1.4.0",
     "description": "Attini CDK Constructs",
     "license": "Apache-2.0",
     "url": "https://attini.io",
     "long_description_content_type": "text/markdown",
     "author": "oscarostrand<contact@attini.io>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "attini_cdk",
         "attini_cdk._jsii"
     ],
     "package_data": {
         "attini_cdk._jsii": [
-            "cdk@1.3.0.jsii.tgz"
+            "cdk@1.4.0.jsii.tgz"
         ],
         "attini_cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `attini-cdk-lib-1.3.0/src/attini_cdk/__init__.py` & `attini-cdk-lib-1.4.0/src/attini_cdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -876,40 +876,43 @@
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         aws_vpc_configuration: typing.Optional[typing.Union["AwsVpcConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
         container_name: typing.Optional[builtins.str] = None,
+        ec2_configuration: typing.Optional[typing.Union["Ec2Configuration", typing.Dict[builtins.str, typing.Any]]] = None,
         ecs_cluster: typing.Optional[builtins.str] = None,
         image: typing.Optional[builtins.str] = None,
         role_arn: typing.Optional[builtins.str] = None,
         runner_configuration: typing.Optional[typing.Union["RunnerConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
         startup: typing.Optional[typing.Union["Startup", typing.Dict[builtins.str, typing.Any]]] = None,
         task_definition_arn: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param aws_vpc_configuration: VPC configuration.
         :param container_name: The name of the container in the task definition. This is only required if a task definition with multiple containers is specified.
+        :param ec2_configuration: Configures an EC2 instance to host the Runner ECS task. By default, Attini Runners use Fargate, but you can use EC2 instead. This is useful if you want to start a container from the ECS container, which is currently not possible with Fargate.
         :param ecs_cluster: The name of the ECS Cluster to use. This is not mandatory if there is a default cluster in the account.
         :param image: A Container image that the runner should use. If you configure this value, Attini will configure a TaskDefinition for you. This configuration can not be combined with the {@link taskDefinitionArn} configuration.
         :param role_arn: The IAM Role the Runner should use. This IAM Role will override the IAM Role from the TaskDefinition. This IAM Role requires a basic execution policy that allows the runner to communicate with the deployment plan. Add the following execution policy to the IAM Role:: arn:aws:iam::${AccountId}:policy/attini-runner-basic-execution-policy-${Region}
         :param runner_configuration: Configuration for the runner.
         :param startup: Runner startup configuration.
-        :param task_definition_arn: Fargate ECS task definition that the Attini Runner should use. If omitted then Attini will use its default task definition.
+        :param task_definition_arn: Fargate ECS task definition that the Attini Runner should use. If omitted, then Attini will use its default task definition.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__660ed4052feaa95482efe568ab8ebc4f76163ce6d31bba60f75428748043a640)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = AttiniRunnerProps(
             aws_vpc_configuration=aws_vpc_configuration,
             container_name=container_name,
+            ec2_configuration=ec2_configuration,
             ecs_cluster=ecs_cluster,
             image=image,
             role_arn=role_arn,
             runner_configuration=runner_configuration,
             startup=startup,
             task_definition_arn=task_definition_arn,
         )
@@ -999,66 +1002,74 @@
 
 @jsii.data_type(
     jsii_type="@attini/cdk.AttiniRunnerProps",
     jsii_struct_bases=[],
     name_mapping={
         "aws_vpc_configuration": "awsVpcConfiguration",
         "container_name": "containerName",
+        "ec2_configuration": "ec2Configuration",
         "ecs_cluster": "ecsCluster",
         "image": "image",
         "role_arn": "roleArn",
         "runner_configuration": "runnerConfiguration",
         "startup": "startup",
         "task_definition_arn": "taskDefinitionArn",
     },
 )
 class AttiniRunnerProps:
     def __init__(
         self,
         *,
         aws_vpc_configuration: typing.Optional[typing.Union["AwsVpcConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
         container_name: typing.Optional[builtins.str] = None,
+        ec2_configuration: typing.Optional[typing.Union["Ec2Configuration", typing.Dict[builtins.str, typing.Any]]] = None,
         ecs_cluster: typing.Optional[builtins.str] = None,
         image: typing.Optional[builtins.str] = None,
         role_arn: typing.Optional[builtins.str] = None,
         runner_configuration: typing.Optional[typing.Union["RunnerConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
         startup: typing.Optional[typing.Union["Startup", typing.Dict[builtins.str, typing.Any]]] = None,
         task_definition_arn: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param aws_vpc_configuration: VPC configuration.
         :param container_name: The name of the container in the task definition. This is only required if a task definition with multiple containers is specified.
+        :param ec2_configuration: Configures an EC2 instance to host the Runner ECS task. By default, Attini Runners use Fargate, but you can use EC2 instead. This is useful if you want to start a container from the ECS container, which is currently not possible with Fargate.
         :param ecs_cluster: The name of the ECS Cluster to use. This is not mandatory if there is a default cluster in the account.
         :param image: A Container image that the runner should use. If you configure this value, Attini will configure a TaskDefinition for you. This configuration can not be combined with the {@link taskDefinitionArn} configuration.
         :param role_arn: The IAM Role the Runner should use. This IAM Role will override the IAM Role from the TaskDefinition. This IAM Role requires a basic execution policy that allows the runner to communicate with the deployment plan. Add the following execution policy to the IAM Role:: arn:aws:iam::${AccountId}:policy/attini-runner-basic-execution-policy-${Region}
         :param runner_configuration: Configuration for the runner.
         :param startup: Runner startup configuration.
-        :param task_definition_arn: Fargate ECS task definition that the Attini Runner should use. If omitted then Attini will use its default task definition.
+        :param task_definition_arn: Fargate ECS task definition that the Attini Runner should use. If omitted, then Attini will use its default task definition.
         '''
         if isinstance(aws_vpc_configuration, dict):
             aws_vpc_configuration = AwsVpcConfiguration(**aws_vpc_configuration)
+        if isinstance(ec2_configuration, dict):
+            ec2_configuration = Ec2Configuration(**ec2_configuration)
         if isinstance(runner_configuration, dict):
             runner_configuration = RunnerConfiguration(**runner_configuration)
         if isinstance(startup, dict):
             startup = Startup(**startup)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0fca31ef6f03939f00deed50f6175576696144f7d8eb08c3c6dab2f5143f2ff6)
             check_type(argname="argument aws_vpc_configuration", value=aws_vpc_configuration, expected_type=type_hints["aws_vpc_configuration"])
             check_type(argname="argument container_name", value=container_name, expected_type=type_hints["container_name"])
+            check_type(argname="argument ec2_configuration", value=ec2_configuration, expected_type=type_hints["ec2_configuration"])
             check_type(argname="argument ecs_cluster", value=ecs_cluster, expected_type=type_hints["ecs_cluster"])
             check_type(argname="argument image", value=image, expected_type=type_hints["image"])
             check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
             check_type(argname="argument runner_configuration", value=runner_configuration, expected_type=type_hints["runner_configuration"])
             check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             check_type(argname="argument task_definition_arn", value=task_definition_arn, expected_type=type_hints["task_definition_arn"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if aws_vpc_configuration is not None:
             self._values["aws_vpc_configuration"] = aws_vpc_configuration
         if container_name is not None:
             self._values["container_name"] = container_name
+        if ec2_configuration is not None:
+            self._values["ec2_configuration"] = ec2_configuration
         if ecs_cluster is not None:
             self._values["ecs_cluster"] = ecs_cluster
         if image is not None:
             self._values["image"] = image
         if role_arn is not None:
             self._values["role_arn"] = role_arn
         if runner_configuration is not None:
@@ -1080,14 +1091,24 @@
 
         This is only required if a task definition with multiple containers is specified.
         '''
         result = self._values.get("container_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def ec2_configuration(self) -> typing.Optional["Ec2Configuration"]:
+        '''Configures an EC2 instance to host the Runner ECS task.
+
+        By default, Attini Runners use Fargate, but you can use EC2 instead.
+        This is useful if you want to start a container from the ECS container, which is currently not possible with Fargate.
+        '''
+        result = self._values.get("ec2_configuration")
+        return typing.cast(typing.Optional["Ec2Configuration"], result)
+
+    @builtins.property
     def ecs_cluster(self) -> typing.Optional[builtins.str]:
         '''The name of the ECS Cluster to use.
 
         This is not mandatory if there is a default cluster in the account.
         '''
         result = self._values.get("ecs_cluster")
         return typing.cast(typing.Optional[builtins.str], result)
@@ -1129,15 +1150,15 @@
         result = self._values.get("startup")
         return typing.cast(typing.Optional["Startup"], result)
 
     @builtins.property
     def task_definition_arn(self) -> typing.Optional[builtins.str]:
         '''Fargate ECS task definition that the Attini Runner should use.
 
-        If omitted then Attini will use its default task definition.
+        If omitted, then Attini will use its default task definition.
         '''
         result = self._values.get("task_definition_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1754,14 +1775,90 @@
     def __repr__(self) -> str:
         return "DistributionSource(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="@attini/cdk.Ec2Configuration",
+    jsii_struct_bases=[],
+    name_mapping={
+        "instance_type": "instanceType",
+        "ami": "ami",
+        "instance_profile_name": "instanceProfileName",
+    },
+)
+class Ec2Configuration:
+    def __init__(
+        self,
+        *,
+        instance_type: builtins.str,
+        ami: typing.Optional[builtins.str] = None,
+        instance_profile_name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param instance_type: The instance type of the EC2 instance that will host the Runner.
+        :param ami: The AMI to use. Can be specified as an imageId, starting with "ami-", or a short hand name like, AmazonLinux2, AmazonLinux2_arm64 etc. For a complete list, please see the documentation. Will default to AmazonLinux2
+        :param instance_profile_name: The instance profile name for the EC2 instance. If omitted, then Attini will create an instance profile with the Runners default role.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d5fe3afe85450e047844f6a6337d6355f23baa3e5753c931e35ba3acba8a3c43)
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument ami", value=ami, expected_type=type_hints["ami"])
+            check_type(argname="argument instance_profile_name", value=instance_profile_name, expected_type=type_hints["instance_profile_name"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "instance_type": instance_type,
+        }
+        if ami is not None:
+            self._values["ami"] = ami
+        if instance_profile_name is not None:
+            self._values["instance_profile_name"] = instance_profile_name
+
+    @builtins.property
+    def instance_type(self) -> builtins.str:
+        '''The instance type of the EC2 instance that will host the Runner.'''
+        result = self._values.get("instance_type")
+        assert result is not None, "Required property 'instance_type' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def ami(self) -> typing.Optional[builtins.str]:
+        '''The AMI to use.
+
+        Can be specified as an imageId, starting with "ami-", or a short hand name like, AmazonLinux2, AmazonLinux2_arm64 etc.
+        For a complete list, please see the documentation.
+
+        Will default to AmazonLinux2
+        '''
+        result = self._values.get("ami")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def instance_profile_name(self) -> typing.Optional[builtins.str]:
+        '''The instance profile name for the EC2 instance.
+
+        If omitted, then Attini will create
+        an instance profile with the Runners default role.
+        '''
+        result = self._values.get("instance_profile_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "Ec2Configuration(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="@attini/cdk.Project",
     jsii_struct_bases=[],
     name_mapping={"path": "path", "build_dir": "buildDir", "template": "template"},
 )
 class Project:
     def __init__(
         self,
@@ -2576,14 +2673,15 @@
     "AttiniTask",
     "AwsVpcConfiguration",
     "CfnAction",
     "DeploymentPlan",
     "DeploymentPlanProps",
     "DiffProps",
     "DistributionSource",
+    "Ec2Configuration",
     "Project",
     "PropsUtil",
     "RunnerConfiguration",
     "S3Source",
     "SourceType",
     "StackConfigurationProps",
     "Startup",
@@ -2674,14 +2772,15 @@
 
 def _typecheckingstub__660ed4052feaa95482efe568ab8ebc4f76163ce6d31bba60f75428748043a640(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     aws_vpc_configuration: typing.Optional[typing.Union[AwsVpcConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
     container_name: typing.Optional[builtins.str] = None,
+    ec2_configuration: typing.Optional[typing.Union[Ec2Configuration, typing.Dict[builtins.str, typing.Any]]] = None,
     ecs_cluster: typing.Optional[builtins.str] = None,
     image: typing.Optional[builtins.str] = None,
     role_arn: typing.Optional[builtins.str] = None,
     runner_configuration: typing.Optional[typing.Union[RunnerConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
     startup: typing.Optional[typing.Union[Startup, typing.Dict[builtins.str, typing.Any]]] = None,
     task_definition_arn: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -2697,14 +2796,15 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0fca31ef6f03939f00deed50f6175576696144f7d8eb08c3c6dab2f5143f2ff6(
     *,
     aws_vpc_configuration: typing.Optional[typing.Union[AwsVpcConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
     container_name: typing.Optional[builtins.str] = None,
+    ec2_configuration: typing.Optional[typing.Union[Ec2Configuration, typing.Dict[builtins.str, typing.Any]]] = None,
     ecs_cluster: typing.Optional[builtins.str] = None,
     image: typing.Optional[builtins.str] = None,
     role_arn: typing.Optional[builtins.str] = None,
     runner_configuration: typing.Optional[typing.Union[RunnerConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
     startup: typing.Optional[typing.Union[Startup, typing.Dict[builtins.str, typing.Any]]] = None,
     task_definition_arn: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -2800,14 +2900,23 @@
 def _typecheckingstub__c396e701f6efcb92c096d07741726f7f6fc70b675aee75bbcc6a7683d7cf0396(
     *,
     name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__d5fe3afe85450e047844f6a6337d6355f23baa3e5753c931e35ba3acba8a3c43(
+    *,
+    instance_type: builtins.str,
+    ami: typing.Optional[builtins.str] = None,
+    instance_profile_name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__d0b5541fa7622b1155017a66dc54ea8b3d313290b55062564f73ff9a3a70e192(
     *,
     path: builtins.str,
     build_dir: typing.Optional[builtins.str] = None,
     template: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `attini-cdk-lib-1.3.0/src/attini_cdk_lib.egg-info/PKG-INFO` & `attini-cdk-lib-1.4.0/src/attini_cdk_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attini-cdk-lib
-Version: 1.3.0
+Version: 1.4.0
 Summary: Attini CDK Constructs
 Home-page: https://attini.io
 Author: oscarostrand<contact@attini.io>
 License: Apache-2.0
 Project-URL: Source, https://github.com/attini-cloud-solutions/attini-cdk-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

