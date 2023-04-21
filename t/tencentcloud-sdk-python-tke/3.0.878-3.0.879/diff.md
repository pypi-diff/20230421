# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.878.tar", last modified: Thu Apr 20 00:53:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.879.tar", last modified: Fri Apr 21 01:07:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.878.tar` & `tencentcloud-sdk-python-tke-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   177287 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19361 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   641750 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:53:47.000000 tencentcloud-sdk-python-tke-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   180345 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19361 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   649069 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:07:17.000000 tencentcloud-sdk-python-tke-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.878/README.rst` & `tencentcloud-sdk-python-tke-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateBackupStorageLocation(self, request):
+        """创建备份仓库，指定了存储仓库类型（如COS）、COS桶地区、名称等信息，当前最多允许创建100个仓库， 注意此接口当前是全局接口，多个地域的TKE集群如果要备份到相同的备份仓库中，不需要重复创建备份仓库
+
+        :param request: Request instance for CreateBackupStorageLocation.
+        :type request: :class:`tencentcloud.tke.v20180525.models.CreateBackupStorageLocationRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.CreateBackupStorageLocationResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateBackupStorageLocation", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateBackupStorageLocationResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateCluster(self, request):
         """创建集群
 
         :param request: Request instance for CreateCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.CreateClusterRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.CreateClusterResponse`
 
@@ -804,14 +827,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteBackupStorageLocation(self, request):
+        """删除备份仓库
+
+        :param request: Request instance for DeleteBackupStorageLocation.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DeleteBackupStorageLocationRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DeleteBackupStorageLocationResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteBackupStorageLocation", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteBackupStorageLocationResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteCluster(self, request):
         """删除集群(YUNAPI V3版本)
 
         :param request: Request instance for DeleteCluster.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteClusterRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.DeleteClusterResponse`
 
@@ -1446,14 +1492,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeBackupStorageLocations(self, request):
+        """查询备份仓库信息
+
+        :param request: Request instance for DescribeBackupStorageLocations.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DescribeBackupStorageLocationsRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DescribeBackupStorageLocationsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBackupStorageLocations", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBackupStorageLocationsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeClusterAsGroupOption(self, request):
         """集群弹性伸缩配置
 
         :param request: Request instance for DescribeClusterAsGroupOption.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeClusterAsGroupOptionRequest`
```

### Comparing `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.879/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,72 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BackupStorageLocation(AbstractModel):
+    """仓储仓库信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 备份仓库名称	
+        :type Name: str
+        :param StorageRegion: 存储仓库所属地域，比如COS广州(ap-guangzhou)	
+        :type StorageRegion: str
+        :param Provider: 存储服务提供方，默认腾讯云	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Provider: str
+        :param Bucket: 对象存储桶名称，如果是COS必须是tke-backup-前缀开头	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Bucket: str
+        :param Path: 对象存储桶路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Path: str
+        :param State: 存储仓库状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type State: str
+        :param Message: 详细状态信息	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param LastValidationTime: 最后一次检查时间	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LastValidationTime: str
+        """
+        self.Name = None
+        self.StorageRegion = None
+        self.Provider = None
+        self.Bucket = None
+        self.Path = None
+        self.State = None
+        self.Message = None
+        self.LastValidationTime = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.StorageRegion = params.get("StorageRegion")
+        self.Provider = params.get("Provider")
+        self.Bucket = params.get("Bucket")
+        self.Path = params.get("Path")
+        self.State = params.get("State")
+        self.Message = params.get("Message")
+        self.LastValidationTime = params.get("LastValidationTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CUDNN(AbstractModel):
     """cuDNN的版本信息
 
     """
 
     def __init__(self):
         r"""
@@ -1976,14 +2034,71 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CreateBackupStorageLocationRequest(AbstractModel):
+    """CreateBackupStorageLocation请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StorageRegion: 存储仓库所属地域，比如COS广州(ap-guangzhou)
+        :type StorageRegion: str
+        :param Bucket: 对象存储桶名称，如果是COS必须是tke-backup前缀开头
+        :type Bucket: str
+        :param Name: 备份仓库名称
+        :type Name: str
+        :param Provider: 存储服务提供方，默认腾讯云
+        :type Provider: str
+        :param Path: 对象存储桶路径
+        :type Path: str
+        """
+        self.StorageRegion = None
+        self.Bucket = None
+        self.Name = None
+        self.Provider = None
+        self.Path = None
+
+
+    def _deserialize(self, params):
+        self.StorageRegion = params.get("StorageRegion")
+        self.Bucket = params.get("Bucket")
+        self.Name = params.get("Name")
+        self.Provider = params.get("Provider")
+        self.Path = params.get("Path")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateBackupStorageLocationResponse(AbstractModel):
+    """CreateBackupStorageLocation返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CreateClusterEndpointRequest(AbstractModel):
     """CreateClusterEndpoint请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4013,14 +4128,55 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DeleteBackupStorageLocationRequest(AbstractModel):
+    """DeleteBackupStorageLocation请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 备份仓库名称
+        :type Name: str
+        """
+        self.Name = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteBackupStorageLocationResponse(AbstractModel):
+    """DeleteBackupStorageLocation返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteClusterAsGroupsRequest(AbstractModel):
     """DeleteClusterAsGroups请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5357,14 +5513,65 @@
     def _deserialize(self, params):
         self.Versions = params.get("Versions")
         self.EdgeVersionLatest = params.get("EdgeVersionLatest")
         self.EdgeVersionCurrent = params.get("EdgeVersionCurrent")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeBackupStorageLocationsRequest(AbstractModel):
+    """DescribeBackupStorageLocations请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Names: 多个备份仓库名称，如果不填写，默认返回当前地域所有存储仓库名称
+        :type Names: list of str
+        """
+        self.Names = None
+
+
+    def _deserialize(self, params):
+        self.Names = params.get("Names")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeBackupStorageLocationsResponse(AbstractModel):
+    """DescribeBackupStorageLocations返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BackupStorageLocationSet: 详细备份仓库信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BackupStorageLocationSet: list of BackupStorageLocation
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BackupStorageLocationSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("BackupStorageLocationSet") is not None:
+            self.BackupStorageLocationSet = []
+            for item in params.get("BackupStorageLocationSet"):
+                obj = BackupStorageLocation()
+                obj._deserialize(item)
+                self.BackupStorageLocationSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeClusterAsGroupOptionRequest(AbstractModel):
     """DescribeClusterAsGroupOption请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10480,14 +10687,17 @@
         :type Level: str
         :param AutoUpgradeClusterLevel: 是否支持自动提升集群配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type AutoUpgradeClusterLevel: bool
         :param ChargeType: 集群付费模式，支持POSTPAID_BY_HOUR或者PREPAID
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChargeType: str
+        :param EdgeVersion: 边缘集群组件的版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EdgeVersion: str
         """
         self.ClusterId = None
         self.ClusterName = None
         self.VpcId = None
         self.PodCIDR = None
         self.ServiceCIDR = None
         self.K8SVersion = None
@@ -10496,14 +10706,15 @@
         self.CreatedTime = None
         self.EdgeClusterVersion = None
         self.MaxNodePodNum = None
         self.ClusterAdvancedSettings = None
         self.Level = None
         self.AutoUpgradeClusterLevel = None
         self.ChargeType = None
+        self.EdgeVersion = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.VpcId = params.get("VpcId")
         self.PodCIDR = params.get("PodCIDR")
@@ -10516,14 +10727,15 @@
         self.MaxNodePodNum = params.get("MaxNodePodNum")
         if params.get("ClusterAdvancedSettings") is not None:
             self.ClusterAdvancedSettings = EdgeClusterAdvancedSettings()
             self.ClusterAdvancedSettings._deserialize(params.get("ClusterAdvancedSettings"))
         self.Level = params.get("Level")
         self.AutoUpgradeClusterLevel = params.get("AutoUpgradeClusterLevel")
         self.ChargeType = params.get("ChargeType")
+        self.EdgeVersion = params.get("EdgeVersion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11164,28 +11376,32 @@
         :type VpcCniType: str
         :param EnableStaticIp: 是否开启固定IP模式
         :type EnableStaticIp: bool
         :param Subnets: 使用的容器子网
         :type Subnets: list of str
         :param ExpiredSeconds: 在固定IP模式下，Pod销毁后退还IP的时间，传参必须大于300；不传默认IP永不销毁。
         :type ExpiredSeconds: int
+        :param SkipAddingNonMasqueradeCIDRs: 是否同步添加 vpc 网段到 ip-masq-agent-config 的 NonMasqueradeCIDRs 字段，默认 false 会同步添加
+        :type SkipAddingNonMasqueradeCIDRs: bool
         """
         self.ClusterId = None
         self.VpcCniType = None
         self.EnableStaticIp = None
         self.Subnets = None
         self.ExpiredSeconds = None
+        self.SkipAddingNonMasqueradeCIDRs = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.VpcCniType = params.get("VpcCniType")
         self.EnableStaticIp = params.get("EnableStaticIp")
         self.Subnets = params.get("Subnets")
         self.ExpiredSeconds = params.get("ExpiredSeconds")
+        self.SkipAddingNonMasqueradeCIDRs = params.get("SkipAddingNonMasqueradeCIDRs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tke-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.879/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.878'
+__version__ = '3.0.879'
```

### Comparing `tencentcloud-sdk-python-tke-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.878/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.879/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.878/setup.py` & `tencentcloud-sdk-python-tke-3.0.879/setup.py`

 * *Files identical despite different names*

