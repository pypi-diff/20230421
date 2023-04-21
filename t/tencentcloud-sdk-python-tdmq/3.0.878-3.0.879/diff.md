# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.878.tar", last modified: Thu Apr 20 00:49:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.879.tar", last modified: Fri Apr 21 01:02:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.878.tar` & `tencentcloud-sdk-python-tdmq-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)    97986 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   359124 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:49:09.000000 tencentcloud-sdk-python-tdmq-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)    99909 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   372127 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1549,14 +1549,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribePulsarProInstanceDetail(self, request):
+        """获取Pulsar专业版集群实例信息
+
+        :param request: Request instance for DescribePulsarProInstanceDetail.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribePulsarProInstanceDetailRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribePulsarProInstanceDetailResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribePulsarProInstanceDetail", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribePulsarProInstanceDetailResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribePulsarProInstances(self, request):
+        """查询用户已购的Pulsar专业版实例列表
+
+        :param request: Request instance for DescribePulsarProInstances.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribePulsarProInstancesRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribePulsarProInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribePulsarProInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribePulsarProInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeRabbitMQNodeList(self, request):
         """RabbitMQ专享版查询节点列表
 
         :param request: Request instance for DescribeRabbitMQNodeList.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQNodeListRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.DescribeRabbitMQNodeListResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5228,14 +5228,145 @@
             for item in params.get("Publishers"):
                 obj = Publisher()
                 obj._deserialize(item)
                 self.Publishers.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribePulsarProInstanceDetailRequest(AbstractModel):
+    """DescribePulsarProInstanceDetail请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        """
+        self.ClusterId = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePulsarProInstanceDetailResponse(AbstractModel):
+    """DescribePulsarProInstanceDetail返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterInfo: 集群信息
+        :type ClusterInfo: :class:`tencentcloud.tdmq.v20200217.models.PulsarProClusterInfo`
+        :param NetworkAccessPointInfos: 集群网络接入点信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NetworkAccessPointInfos: list of PulsarNetworkAccessPointInfo
+        :param ClusterSpecInfo: 集群规格信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterSpecInfo: :class:`tencentcloud.tdmq.v20200217.models.PulsarProClusterSpecInfo`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ClusterInfo = None
+        self.NetworkAccessPointInfos = None
+        self.ClusterSpecInfo = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("ClusterInfo") is not None:
+            self.ClusterInfo = PulsarProClusterInfo()
+            self.ClusterInfo._deserialize(params.get("ClusterInfo"))
+        if params.get("NetworkAccessPointInfos") is not None:
+            self.NetworkAccessPointInfos = []
+            for item in params.get("NetworkAccessPointInfos"):
+                obj = PulsarNetworkAccessPointInfo()
+                obj._deserialize(item)
+                self.NetworkAccessPointInfos.append(obj)
+        if params.get("ClusterSpecInfo") is not None:
+            self.ClusterSpecInfo = PulsarProClusterSpecInfo()
+            self.ClusterSpecInfo._deserialize(params.get("ClusterSpecInfo"))
+        self.RequestId = params.get("RequestId")
+
+
+class DescribePulsarProInstancesRequest(AbstractModel):
+    """DescribePulsarProInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filters: 查询条件过滤器
+        :type Filters: list of Filter
+        :param Limit: 查询数目上限，默认20
+        :type Limit: int
+        :param Offset: 查询起始位置
+        :type Offset: int
+        """
+        self.Filters = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePulsarProInstancesResponse(AbstractModel):
+    """DescribePulsarProInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 未分页的总数目
+        :type TotalCount: int
+        :param Instances: 实例信息列表
+        :type Instances: list of PulsarProInstance
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Instances = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Instances") is not None:
+            self.Instances = []
+            for item in params.get("Instances"):
+                obj = PulsarProInstance()
+                obj._deserialize(item)
+                self.Instances.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeRabbitMQNodeListRequest(AbstractModel):
     """DescribeRabbitMQNodeList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7839,14 +7970,250 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class PulsarNetworkAccessPointInfo(AbstractModel):
+    """Pulsar 网络接入点信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcId: vpc的id，支撑网和公网接入点，该字段为空
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param SubnetId: 子网id，支撑网和公网接入点，该字段为空
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetId: str
+        :param Endpoint: 接入地址
+        :type Endpoint: str
+        :param InstanceId: 实例id
+        :type InstanceId: str
+        :param RouteType: 接入点类型：
+0：支撑网接入点 
+1：VPC接入点 
+2：公网接入点
+        :type RouteType: int
+        """
+        self.VpcId = None
+        self.SubnetId = None
+        self.Endpoint = None
+        self.InstanceId = None
+        self.RouteType = None
+
+
+    def _deserialize(self, params):
+        self.VpcId = params.get("VpcId")
+        self.SubnetId = params.get("SubnetId")
+        self.Endpoint = params.get("Endpoint")
+        self.InstanceId = params.get("InstanceId")
+        self.RouteType = params.get("RouteType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PulsarProClusterInfo(AbstractModel):
+    """Pulsar专业版集群信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群Id。
+        :type ClusterId: str
+        :param ClusterName: 集群名称。
+        :type ClusterName: str
+        :param Remark: 说明信息。
+        :type Remark: str
+        :param CreateTime: 创建时间
+        :type CreateTime: str
+        :param Status: 集群状态，0:创建中，1:正常，2:隔离
+        :type Status: int
+        :param Version: 集群版本
+        :type Version: str
+        :param NodeDistribution: 节点分布情况
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NodeDistribution: list of InstanceNodeDistribution
+        :param MaxStorage: 最大储存容量，单位：MB
+        :type MaxStorage: int
+        """
+        self.ClusterId = None
+        self.ClusterName = None
+        self.Remark = None
+        self.CreateTime = None
+        self.Status = None
+        self.Version = None
+        self.NodeDistribution = None
+        self.MaxStorage = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ClusterName = params.get("ClusterName")
+        self.Remark = params.get("Remark")
+        self.CreateTime = params.get("CreateTime")
+        self.Status = params.get("Status")
+        self.Version = params.get("Version")
+        if params.get("NodeDistribution") is not None:
+            self.NodeDistribution = []
+            for item in params.get("NodeDistribution"):
+                obj = InstanceNodeDistribution()
+                obj._deserialize(item)
+                self.NodeDistribution.append(obj)
+        self.MaxStorage = params.get("MaxStorage")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PulsarProClusterSpecInfo(AbstractModel):
+    """Pulsar专业版集群规格信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SpecName: 集群规格名称
+        :type SpecName: str
+        :param MaxTps: 峰值tps
+        :type MaxTps: int
+        :param MaxBandWidth: 峰值带宽。单位：mbps
+        :type MaxBandWidth: int
+        :param MaxNamespaces: 最大命名空间个数
+        :type MaxNamespaces: int
+        :param MaxTopics: 最大主题分区数
+        :type MaxTopics: int
+        :param ScalableTps: 规格外弹性TPS
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScalableTps: int
+        """
+        self.SpecName = None
+        self.MaxTps = None
+        self.MaxBandWidth = None
+        self.MaxNamespaces = None
+        self.MaxTopics = None
+        self.ScalableTps = None
+
+
+    def _deserialize(self, params):
+        self.SpecName = params.get("SpecName")
+        self.MaxTps = params.get("MaxTps")
+        self.MaxBandWidth = params.get("MaxBandWidth")
+        self.MaxNamespaces = params.get("MaxNamespaces")
+        self.MaxTopics = params.get("MaxTopics")
+        self.ScalableTps = params.get("ScalableTps")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PulsarProInstance(AbstractModel):
+    """Pulsar专业版实例信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例id
+        :type InstanceId: str
+        :param InstanceName: 实例名称
+        :type InstanceName: str
+        :param InstanceVersion: 实例版本
+        :type InstanceVersion: str
+        :param Status: 实例状态，0-创建中，1-正常，2-隔离中，3-已销毁，4 - 异常, 5 - 发货失败，6-变配中，7-变配失败
+        :type Status: int
+        :param ConfigDisplay: 实例配置规格名称
+        :type ConfigDisplay: str
+        :param MaxTps: 峰值TPS
+        :type MaxTps: int
+        :param MaxStorage: 存储容量，GB为单位
+        :type MaxStorage: int
+        :param ExpireTime: 实例到期时间，毫秒为单位
+        :type ExpireTime: int
+        :param AutoRenewFlag: 自动续费标记，0表示默认状态(用户未设置，即初始状态即手动续费)， 1表示自动续费，2表示明确不自动续费(用户设置)
+        :type AutoRenewFlag: int
+        :param PayMode: 0-后付费，1-预付费
+        :type PayMode: int
+        :param Remark: 备注信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Remark: str
+        :param SpecName: 实例配置ID
+        :type SpecName: str
+        :param ScalableTps: 规格外弹性TPS
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScalableTps: int
+        :param VpcId: VPC的id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param SubnetId: 子网id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetId: str
+        :param MaxBandWidth: 峰值带宽。单位：mbps
+        :type MaxBandWidth: int
+        """
+        self.InstanceId = None
+        self.InstanceName = None
+        self.InstanceVersion = None
+        self.Status = None
+        self.ConfigDisplay = None
+        self.MaxTps = None
+        self.MaxStorage = None
+        self.ExpireTime = None
+        self.AutoRenewFlag = None
+        self.PayMode = None
+        self.Remark = None
+        self.SpecName = None
+        self.ScalableTps = None
+        self.VpcId = None
+        self.SubnetId = None
+        self.MaxBandWidth = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.InstanceName = params.get("InstanceName")
+        self.InstanceVersion = params.get("InstanceVersion")
+        self.Status = params.get("Status")
+        self.ConfigDisplay = params.get("ConfigDisplay")
+        self.MaxTps = params.get("MaxTps")
+        self.MaxStorage = params.get("MaxStorage")
+        self.ExpireTime = params.get("ExpireTime")
+        self.AutoRenewFlag = params.get("AutoRenewFlag")
+        self.PayMode = params.get("PayMode")
+        self.Remark = params.get("Remark")
+        self.SpecName = params.get("SpecName")
+        self.ScalableTps = params.get("ScalableTps")
+        self.VpcId = params.get("VpcId")
+        self.SubnetId = params.get("SubnetId")
+        self.MaxBandWidth = params.get("MaxBandWidth")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class QueueQuota(AbstractModel):
     """queue使用配额信息
 
     """
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.879/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.878/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.879/setup.py`

 * *Files identical despite different names*

