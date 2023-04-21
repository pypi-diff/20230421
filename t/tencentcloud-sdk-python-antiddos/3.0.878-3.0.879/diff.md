# Comparing `tmp/tencentcloud-sdk-python-antiddos-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-antiddos-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.878.tar", last modified: Thu Apr 20 00:17:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-antiddos-3.0.879.tar", last modified: Fri Apr 21 00:27:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-antiddos-3.0.878.tar` & `tencentcloud-sdk-python-antiddos-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)    88167 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)   314064 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud_sdk_python_antiddos.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:17:48.000000 tencentcloud-sdk-python-antiddos-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)    88167 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   315539 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud_sdk_python_antiddos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud_sdk_python_antiddos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud_sdk_python_antiddos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud_sdk_python_antiddos.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-21 00:27:45.000000 tencentcloud-sdk-python-antiddos-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:27:46.000000 tencentcloud-sdk-python-antiddos-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/README.rst` & `tencentcloud-sdk-python-antiddos-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/antiddos/v20200309/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,17 +271,17 @@
 "idle"：正常状态(无攻击)
 "attacking"：攻击中
 "blocking"：封堵中
 "creating"：创建中
 "deblocking"：解封中
 "isolate"：回收隔离中
         :type Status: str
-        :param ExpiredTime: 购买时间
+        :param ExpiredTime: 到期时间
         :type ExpiredTime: str
-        :param CreatedTime: 到期时间
+        :param CreatedTime: 购买时间
         :type CreatedTime: str
         :param Name: 资产实例的名称
         :type Name: str
         :param PackInfo: 资产实例所属的套餐包信息，
 注意：当资产实例不是套餐包的实例时，此字段为null
 注意：此字段可能返回 null，表示取不到有效值。
         :type PackInfo: :class:`tencentcloud.antiddos.v20200309.models.PackInfo`
@@ -570,14 +570,17 @@
         :param Line: 网络线路
 注意：此字段可能返回 null，表示取不到有效值。
         :type Line: int
         :param ElasticServiceBandwidth: 弹性业务带宽开关
         :type ElasticServiceBandwidth: int
         :param GiftServiceBandWidth: 赠送的业务带宽
         :type GiftServiceBandWidth: int
+        :param ModifyTime: 修改时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifyTime: str
         """
         self.InstanceDetail = None
         self.SpecificationLimit = None
         self.Usage = None
         self.Region = None
         self.Status = None
         self.CreatedTime = None
@@ -590,14 +593,15 @@
         self.CCEnable = None
         self.TagInfoList = None
         self.IpCountNewFlag = None
         self.VitalityVersion = None
         self.Line = None
         self.ElasticServiceBandwidth = None
         self.GiftServiceBandWidth = None
+        self.ModifyTime = None
 
 
     def _deserialize(self, params):
         if params.get("InstanceDetail") is not None:
             self.InstanceDetail = InstanceRelation()
             self.InstanceDetail._deserialize(params.get("InstanceDetail"))
         if params.get("SpecificationLimit") is not None:
@@ -632,14 +636,15 @@
                 obj._deserialize(item)
                 self.TagInfoList.append(obj)
         self.IpCountNewFlag = params.get("IpCountNewFlag")
         self.VitalityVersion = params.get("VitalityVersion")
         self.Line = params.get("Line")
         self.ElasticServiceBandwidth = params.get("ElasticServiceBandwidth")
         self.GiftServiceBandWidth = params.get("GiftServiceBandWidth")
+        self.ModifyTime = params.get("ModifyTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3671,24 +3676,29 @@
         :type Id: str
         :param MetricName: 统计纬度，可取值connum, new_conn, inactive_conn, intraffic, outtraffic, inpkg, outpkg, qps
         :type MetricName: str
         :param Domain: 统计纬度为qps时，可选特定域名查询
         :type Domain: str
         :param ProtoInfo: 协议及端口列表，协议可取值TCP, UDP, HTTP, HTTPS，仅统计纬度为连接数时有效
         :type ProtoInfo: list of ProtocolPort
+        :param BusinessType: 业务类型可取值domain, port
+port：端口业务
+domain：域名业务
+        :type BusinessType: str
         """
         self.Statistics = None
         self.Business = None
         self.Period = None
         self.StartTime = None
         self.EndTime = None
         self.Id = None
         self.MetricName = None
         self.Domain = None
         self.ProtoInfo = None
+        self.BusinessType = None
 
 
     def _deserialize(self, params):
         self.Statistics = params.get("Statistics")
         self.Business = params.get("Business")
         self.Period = params.get("Period")
         self.StartTime = params.get("StartTime")
@@ -3698,14 +3708,15 @@
         self.Domain = params.get("Domain")
         if params.get("ProtoInfo") is not None:
             self.ProtoInfo = []
             for item in params.get("ProtoInfo"):
                 obj = ProtocolPort()
                 obj._deserialize(item)
                 self.ProtoInfo.append(obj)
+        self.BusinessType = params.get("BusinessType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3718,25 +3729,30 @@
 
     def __init__(self):
         r"""
         :param DataList: 曲线图各个时间点的值
         :type DataList: list of float
         :param MetricName: 统计纬度
         :type MetricName: str
+        :param MaxData: 返回DataList中的最大值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxData: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DataList = None
         self.MetricName = None
+        self.MaxData = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DataList = params.get("DataList")
         self.MetricName = params.get("MetricName")
+        self.MaxData = params.get("MaxData")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeBlackWhiteIpListRequest(AbstractModel):
     """DescribeBlackWhiteIpList请求参数结构体
 
     """
@@ -4900,14 +4916,16 @@
         :type FilterTag: :class:`tencentcloud.antiddos.v20200309.models.TagFilter`
         :param FilterTrialFlag: 试用资源搜索，1: 应急防护资源；2：PLG试用资源
         :type FilterTrialFlag: int
         :param FilterConvoy: 重保护航搜索
         :type FilterConvoy: int
         :param ExcludeAdvancedInfo: 默认false；接口传true，返回数据中不包含高级信息，高级信息包含：InstanceList[0].Usage。
         :type ExcludeAdvancedInfo: bool
+        :param FilterAssetIpList: 资产IP数组
+        :type FilterAssetIpList: list of str
         """
         self.Offset = None
         self.Limit = None
         self.FilterIp = None
         self.FilterInstanceId = None
         self.FilterRegion = None
         self.FilterName = None
@@ -4918,14 +4936,15 @@
         self.FilterEnterpriseFlag = None
         self.FilterLightFlag = None
         self.FilterChannelFlag = None
         self.FilterTag = None
         self.FilterTrialFlag = None
         self.FilterConvoy = None
         self.ExcludeAdvancedInfo = None
+        self.FilterAssetIpList = None
 
 
     def _deserialize(self, params):
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.FilterIp = params.get("FilterIp")
         self.FilterInstanceId = params.get("FilterInstanceId")
@@ -4940,14 +4959,15 @@
         self.FilterChannelFlag = params.get("FilterChannelFlag")
         if params.get("FilterTag") is not None:
             self.FilterTag = TagFilter()
             self.FilterTag._deserialize(params.get("FilterTag"))
         self.FilterTrialFlag = params.get("FilterTrialFlag")
         self.FilterConvoy = params.get("FilterConvoy")
         self.ExcludeAdvancedInfo = params.get("ExcludeAdvancedInfo")
+        self.FilterAssetIpList = params.get("FilterAssetIpList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5646,24 +5666,28 @@
         r"""
         :param Offset: 页起始偏移，取值为(页码-1)*一页条数
         :type Offset: int
         :param Limit: 一页条数，当Limit=0时，默认一页条数为20;最大取值为100
         :type Limit: int
         :param FilterDomain: 调度域名搜索
         :type FilterDomain: str
+        :param Status: 运行状态 0 代表未运行  1 正在运行  2 运行异常 
+        :type Status: str
         """
         self.Offset = None
         self.Limit = None
         self.FilterDomain = None
+        self.Status = None
 
 
     def _deserialize(self, params):
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.FilterDomain = params.get("FilterDomain")
+        self.Status = params.get("Status")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5998,44 +6022,44 @@
 class DescribeOverviewCCTrendRequest(AbstractModel):
     """DescribeOverviewCCTrend请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Business: 大禹子产品代号（bgpip表示高防IP；bgp-multip表示共享包；basic表示DDoS基础防护）
-        :type Business: str
         :param Period: 统计粒度，取值[300(5分钟)，3600(小时)，86400(天)]
         :type Period: int
         :param StartTime: 统计开始时间
         :type StartTime: str
         :param EndTime: 统计结束时间
         :type EndTime: str
         :param MetricName: 指标，取值[inqps(总请求峰值，dropqps(攻击请求峰值))，incount(请求次数), dropcount(攻击次数)]
         :type MetricName: str
+        :param Business: 大禹子产品代号（bgpip表示高防IP；bgp-multip表示共享包；basic表示DDoS基础防护）
+        :type Business: str
         :param IpList: 资源的IP
         :type IpList: list of str
         :param Id: 资源实例ID
         :type Id: str
         """
-        self.Business = None
         self.Period = None
         self.StartTime = None
         self.EndTime = None
         self.MetricName = None
+        self.Business = None
         self.IpList = None
         self.Id = None
 
 
     def _deserialize(self, params):
-        self.Business = params.get("Business")
         self.Period = params.get("Period")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.MetricName = params.get("MetricName")
+        self.Business = params.get("Business")
         self.IpList = params.get("IpList")
         self.Id = params.get("Id")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
@@ -6141,44 +6165,44 @@
 class DescribeOverviewDDoSTrendRequest(AbstractModel):
     """DescribeOverviewDDoSTrend请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Business: 大禹子产品代号（bgpip表示高防IP；bgp-multip表示高防包；basic表示DDoS基础防护）
-        :type Business: str
         :param Period: 统计粒度，取值[300(5分钟)，3600(小时)，86400(天)]
         :type Period: int
         :param StartTime: 统计开始时间
         :type StartTime: str
         :param EndTime: 统计结束时间
         :type EndTime: str
         :param MetricName: 指标，取值[bps(攻击流量带宽，pps(攻击包速率))]
         :type MetricName: str
+        :param Business: 大禹子产品代号（bgpip表示高防IP；bgp-multip表示高防包；basic表示DDoS基础防护）
+        :type Business: str
         :param IpList: 资源实例的IP列表
         :type IpList: list of str
         :param Id: 资源实例ID
         :type Id: str
         """
-        self.Business = None
         self.Period = None
         self.StartTime = None
         self.EndTime = None
         self.MetricName = None
+        self.Business = None
         self.IpList = None
         self.Id = None
 
 
     def _deserialize(self, params):
-        self.Business = params.get("Business")
         self.Period = params.get("Period")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.MetricName = params.get("MetricName")
+        self.Business = params.get("Business")
         self.IpList = params.get("IpList")
         self.Id = params.get("Id")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
@@ -6482,26 +6506,31 @@
 other(托管IP)
 ]
         :type BizType: str
         :param DeviceType: 云产品子类型，取值[cvm（CVM），lb（负载均衡器），eni（弹性网卡），vpngw（VPN），natgw（NAT），waf（WAF），fpc（金融），gaap（GAAP），other（托管IP），eip（黑石弹性IP）]
         :type DeviceType: str
         :param InstanceId: IP所属的云产品实例ID，例如是弹性网卡的IP，InstanceId为弹性网卡的ID(eni-*); 如果是托管IP没有对应的资源实例ID,InstanceId为""
         :type InstanceId: str
+        :param Domain: 域名化资产对应的域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Domain: str
         """
         self.Ip = None
         self.BizType = None
         self.DeviceType = None
         self.InstanceId = None
+        self.Domain = None
 
 
     def _deserialize(self, params):
         self.Ip = params.get("Ip")
         self.BizType = params.get("BizType")
         self.DeviceType = params.get("DeviceType")
         self.InstanceId = params.get("InstanceId")
+        self.Domain = params.get("Domain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6659,26 +6688,31 @@
         :type Type: str
         :param Eip: 线路IP
         :type Eip: str
         :param Cname: 实例对应的cname
         :type Cname: str
         :param ResourceFlag: 资源flag，0：高防包资源，1：高防IP资源，2：非高防资源IP
         :type ResourceFlag: int
+        :param Domain: 域名化资产对应的域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Domain: str
         """
         self.Type = None
         self.Eip = None
         self.Cname = None
         self.ResourceFlag = None
+        self.Domain = None
 
 
     def _deserialize(self, params):
         self.Type = params.get("Type")
         self.Eip = params.get("Eip")
         self.Cname = params.get("Cname")
         self.ResourceFlag = params.get("ResourceFlag")
+        self.Domain = params.get("Domain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.879/tencentcloud_sdk_python_antiddos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-antiddos-3.0.879/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-antiddos
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Antiddos SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-antiddos-3.0.878/setup.py` & `tencentcloud-sdk-python-antiddos-3.0.879/setup.py`

 * *Files identical despite different names*

