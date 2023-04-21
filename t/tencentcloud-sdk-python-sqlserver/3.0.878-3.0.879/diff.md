# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.878.tar", last modified: Thu Apr 20 00:41:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.879.tar", last modified: Fri Apr 21 00:59:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.878.tar` & `tencentcloud-sdk-python-sqlserver-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      755 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   104555 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334850 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-20 00:41:44.000000 tencentcloud-sdk-python-sqlserver-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:41:45.000000 tencentcloud-sdk-python-sqlserver-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   104570 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   335623 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:59:44.000000 tencentcloud-sdk-python-sqlserver-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2257,15 +2257,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RestoreInstance(self, request):
-        """本接口（RestoreInstance）用于根据备份文件恢复实例。
+        """本接口（RestoreInstance）用于按照备份集回档数据库。
 
         :param request: Request instance for RestoreInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RestoreInstanceRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.RestoreInstanceResponse`
 
         """
         try:
@@ -2280,15 +2280,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RollbackInstance(self, request):
-        """本接口（RollbackInstance）用于回档实例
+        """本接口（RollbackInstance）用于按照时间点回档实例
 
         :param request: Request instance for RollbackInstance.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.RollbackInstanceRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.RollbackInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2035,14 +2035,20 @@
         :param TimeZone: 系统时区，默认：China Standard Time
         :type TimeZone: str
         :param IsDrZone: 是否跨AZ
         :type IsDrZone: bool
         :param SlaveZones: 备可用区信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type SlaveZones: :class:`tencentcloud.sqlserver.v20180328.models.SlaveZones`
+        :param Architecture: 架构标识，SINGLE-单节点 DOUBLE-双节点 TRIPLE-三节点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Architecture: str
+        :param Style: 类型标识，EXCLUSIVE-独享型，SHARED-共享型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Style: str
         """
         self.InstanceId = None
         self.Name = None
         self.ProjectId = None
         self.RegionId = None
         self.ZoneId = None
         self.VpcId = None
@@ -2088,14 +2094,16 @@
         self.CrossBackupSaveDays = None
         self.DnsPodDomain = None
         self.TgwWanVPort = None
         self.Collation = None
         self.TimeZone = None
         self.IsDrZone = None
         self.SlaveZones = None
+        self.Architecture = None
+        self.Style = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.Name = params.get("Name")
         self.ProjectId = params.get("ProjectId")
         self.RegionId = params.get("RegionId")
@@ -2150,14 +2158,16 @@
         self.TgwWanVPort = params.get("TgwWanVPort")
         self.Collation = params.get("Collation")
         self.TimeZone = params.get("TimeZone")
         self.IsDrZone = params.get("IsDrZone")
         if params.get("SlaveZones") is not None:
             self.SlaveZones = SlaveZones()
             self.SlaveZones._deserialize(params.get("SlaveZones"))
+        self.Architecture = params.get("Architecture")
+        self.Style = params.get("Style")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8661,34 +8671,42 @@
         :type InstanceId: str
         :param BackupId: 备份文件ID，该ID可以通过DescribeBackups接口返回数据中的Id字段获得
         :type BackupId: int
         :param TargetInstanceId: 备份恢复到的同一个APPID下的实例ID，不填则恢复到原实例ID
         :type TargetInstanceId: str
         :param RenameRestore: 按照ReNameRestoreDatabase中的库进行恢复，并重命名，不填则按照默认方式命名恢复的库，且恢复所有的库。
         :type RenameRestore: list of RenameRestoreDatabase
-        :param GroupId: 备份任务组ID，在单库备份文件模式下，可通过[DescribeBackups](https://cloud.tencent.com/document/product/238/19943) 接口获得。
+        :param Type: 回档类型，0-覆盖方式；1-重命名方式，默认1
+        :type Type: int
+        :param DBList: 需要覆盖回档的数据库，只有覆盖回档时必填
+        :type DBList: list of str
+        :param GroupId: 备份任务组ID，在单库备份文件模式下
         :type GroupId: str
         """
         self.InstanceId = None
         self.BackupId = None
         self.TargetInstanceId = None
         self.RenameRestore = None
+        self.Type = None
+        self.DBList = None
         self.GroupId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.BackupId = params.get("BackupId")
         self.TargetInstanceId = params.get("TargetInstanceId")
         if params.get("RenameRestore") is not None:
             self.RenameRestore = []
             for item in params.get("RenameRestore"):
                 obj = RenameRestoreDatabase()
                 obj._deserialize(item)
                 self.RenameRestore.append(obj)
+        self.Type = params.get("Type")
+        self.DBList = params.get("DBList")
         self.GroupId = params.get("GroupId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -8723,36 +8741,36 @@
 
     def __init__(self):
         r"""
         :param InstanceId: 实例ID
         :type InstanceId: str
         :param Type: 回档类型，0-回档的数据库覆盖原库；1-回档的数据库以重命名的形式生成，不覆盖原库
         :type Type: int
-        :param DBs: 需要回档的数据库
-        :type DBs: list of str
         :param Time: 回档目标时间点
         :type Time: str
+        :param DBs: 需要回档的数据库
+        :type DBs: list of str
         :param TargetInstanceId: 备份恢复到的同一个APPID下的实例ID，不填则恢复到原实例ID
         :type TargetInstanceId: str
         :param RenameRestore: 按照ReNameRestoreDatabase中的库进行重命名，仅在Type = 1重命名回档方式有效；不填则按照默认方式命名库，DBs参数确定要恢复的库
         :type RenameRestore: list of RenameRestoreDatabase
         """
         self.InstanceId = None
         self.Type = None
-        self.DBs = None
         self.Time = None
+        self.DBs = None
         self.TargetInstanceId = None
         self.RenameRestore = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.Type = params.get("Type")
-        self.DBs = params.get("DBs")
         self.Time = params.get("Time")
+        self.DBs = params.get("DBs")
         self.TargetInstanceId = params.get("TargetInstanceId")
         if params.get("RenameRestore") is not None:
             self.RenameRestore = []
             for item in params.get("RenameRestore"):
                 obj = RenameRestoreDatabase()
                 obj._deserialize(item)
                 self.RenameRestore.append(obj)
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.879/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.879/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.878/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.879/setup.py`

 * *Files identical despite different names*

