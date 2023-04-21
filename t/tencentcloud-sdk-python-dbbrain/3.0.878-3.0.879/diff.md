# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.878.tar", last modified: Thu Apr 20 00:26:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.879.tar", last modified: Fri Apr 21 00:42:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.878.tar` & `tencentcloud-sdk-python-dbbrain-3.0.879.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    45821 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   172014 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111297 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:26:02.000000 tencentcloud-sdk-python-dbbrain-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   182383 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   111297 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-21 00:42:33.000000 tencentcloud-sdk-python-dbbrain-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:42:34.000000 tencentcloud-sdk-python-dbbrain-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateAuditLogFile(self, request):
+        """用于创建云数据库实例的审计日志文件，最多下载600w审计日志。
+
+        :param request: Request instance for CreateAuditLogFile.
+        :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateAuditLogFileRequest`
+        :rtype: :class:`tencentcloud.dbbrain.v20210527.models.CreateAuditLogFileResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateAuditLogFile", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateAuditLogFileResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateDBDiagReportTask(self, request):
         """创建健康报告，并可以选择是否发送邮件。
 
         :param request: Request instance for CreateDBDiagReportTask.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateDBDiagReportTaskRequest`
         :rtype: :class:`tencentcloud.dbbrain.v20210527.models.CreateDBDiagReportTaskResponse`
 
@@ -252,14 +275,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteAuditLogFile(self, request):
+        """用于删除云数据库实例的审计日志文件。
+
+        :param request: Request instance for DeleteAuditLogFile.
+        :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteAuditLogFileRequest`
+        :rtype: :class:`tencentcloud.dbbrain.v20210527.models.DeleteAuditLogFileResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteAuditLogFile", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteAuditLogFileResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteDBDiagReportTasks(self, request):
         """根据任务id删除健康报告生成任务
 
         :param request: Request instance for DeleteDBDiagReportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteDBDiagReportTasksRequest`
         :rtype: :class:`tencentcloud.dbbrain.v20210527.models.DeleteDBDiagReportTasksResponse`
 
@@ -365,14 +411,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeAuditLogFiles(self, request):
+        """用于创建云数据库实例的审计日志文件
+
+        :param request: Request instance for DescribeAuditLogFiles.
+        :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeAuditLogFilesRequest`
+        :rtype: :class:`tencentcloud.dbbrain.v20210527.models.DescribeAuditLogFilesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAuditLogFiles", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAuditLogFilesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDBDiagEvent(self, request):
         """获取实例异常诊断事件的详情信息。
 
         :param request: Request instance for DescribeDBDiagEvent.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeDBDiagEventRequest`
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,7 +66,10 @@
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# 该时间范围内的审计日志已下载
+UNSUPPORTEDOPERATION_HASDUPLICATEDTASK = 'UnsupportedOperation.HasDuplicatedTask'
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,120 @@
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.RequestId = params.get("RequestId")
 
 
+class AuditLogFile(AbstractModel):
+    """审计日志文件
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AsyncRequestId: 审计日志文件生成异步任务ID。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncRequestId: int
+        :param FileName: 审计日志文件名称。
+        :type FileName: str
+        :param CreateTime: 审计日志文件创建时间。格式为 : "2019-03-20 17:09:13"。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param Status: 文件状态值。可能返回的值为：
+"creating" - 生成中;
+"failed" - 创建失败;
+"success" - 已生成;
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param FileSize: 文件大小，单位为 KB。
+        :type FileSize: float
+        :param DownloadUrl: 审计日志下载地址。
+        :type DownloadUrl: str
+        :param ErrMsg: 错误信息。
+        :type ErrMsg: str
+        :param Progress: 文件生成进度。
+        :type Progress: float
+        :param FinishTime: 文件生成成功时间。
+        :type FinishTime: str
+        """
+        self.AsyncRequestId = None
+        self.FileName = None
+        self.CreateTime = None
+        self.Status = None
+        self.FileSize = None
+        self.DownloadUrl = None
+        self.ErrMsg = None
+        self.Progress = None
+        self.FinishTime = None
+
+
+    def _deserialize(self, params):
+        self.AsyncRequestId = params.get("AsyncRequestId")
+        self.FileName = params.get("FileName")
+        self.CreateTime = params.get("CreateTime")
+        self.Status = params.get("Status")
+        self.FileSize = params.get("FileSize")
+        self.DownloadUrl = params.get("DownloadUrl")
+        self.ErrMsg = params.get("ErrMsg")
+        self.Progress = params.get("Progress")
+        self.FinishTime = params.get("FinishTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AuditLogFilter(AbstractModel):
+    """过滤条件。可按设置的过滤条件过滤日志。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Host: 客户端地址。
+        :type Host: list of str
+        :param DBName: 数据库名称。
+        :type DBName: list of str
+        :param User: 用户名。
+        :type User: list of str
+        :param SentRows: 返回行数。表示筛选返回行数大于该值的审计日志。
+        :type SentRows: int
+        :param AffectRows: 影响行数。表示筛选影响行数大于该值的审计日志。
+        :type AffectRows: int
+        :param ExecTime: 执行时间。单位为：µs。表示筛选执行时间大于该值的审计日志。
+        :type ExecTime: int
+        """
+        self.Host = None
+        self.DBName = None
+        self.User = None
+        self.SentRows = None
+        self.AffectRows = None
+        self.ExecTime = None
+
+
+    def _deserialize(self, params):
+        self.Host = params.get("Host")
+        self.DBName = params.get("DBName")
+        self.User = params.get("User")
+        self.SentRows = params.get("SentRows")
+        self.AffectRows = params.get("AffectRows")
+        self.ExecTime = params.get("ExecTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CancelKillTaskRequest(AbstractModel):
     """CancelKillTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -148,14 +254,81 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CreateAuditLogFileRequest(AbstractModel):
+    """CreateAuditLogFile请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB for MariaDB。
+        :type Product: str
+        :param NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"
+        :type NodeRequestType: str
+        :param InstanceId: 实例 ID 。
+        :type InstanceId: str
+        :param StartTime: 开始时间，如“2019-09-10 12:13:14”。	
+        :type StartTime: str
+        :param EndTime: 截止时间，如“2019-09-11 10:13:14”。
+        :type EndTime: str
+        :param Filter: 过滤条件。可按设置的过滤条件过滤日志。
+        :type Filter: :class:`tencentcloud.dbbrain.v20210527.models.AuditLogFilter`
+        """
+        self.Product = None
+        self.NodeRequestType = None
+        self.InstanceId = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Filter = None
+
+
+    def _deserialize(self, params):
+        self.Product = params.get("Product")
+        self.NodeRequestType = params.get("NodeRequestType")
+        self.InstanceId = params.get("InstanceId")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        if params.get("Filter") is not None:
+            self.Filter = AuditLogFilter()
+            self.Filter._deserialize(params.get("Filter"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateAuditLogFileResponse(AbstractModel):
+    """CreateAuditLogFile返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AsyncRequestId: 审计日志文件下载的任务ID
+        :type AsyncRequestId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.AsyncRequestId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.AsyncRequestId = params.get("AsyncRequestId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateDBDiagReportTaskRequest(AbstractModel):
     """CreateDBDiagReportTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -653,14 +826,67 @@
 
 
     def _deserialize(self, params):
         self.FilterId = params.get("FilterId")
         self.RequestId = params.get("RequestId")
 
 
+class DeleteAuditLogFileRequest(AbstractModel):
+    """DeleteAuditLogFile请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB for MariaDB。
+        :type Product: str
+        :param NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"	
+        :type NodeRequestType: str
+        :param InstanceId: 实例 ID 。
+        :type InstanceId: str
+        :param AsyncRequestId: 审计日志文件生成异步任务ID。
+        :type AsyncRequestId: int
+        """
+        self.Product = None
+        self.NodeRequestType = None
+        self.InstanceId = None
+        self.AsyncRequestId = None
+
+
+    def _deserialize(self, params):
+        self.Product = params.get("Product")
+        self.NodeRequestType = params.get("NodeRequestType")
+        self.InstanceId = params.get("InstanceId")
+        self.AsyncRequestId = params.get("AsyncRequestId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteAuditLogFileResponse(AbstractModel):
+    """DeleteAuditLogFile返回参数结构体
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
 class DeleteDBDiagReportTasksRequest(AbstractModel):
     """DeleteDBDiagReportTasks请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -923,14 +1149,86 @@
             for item in params.get("Groups"):
                 obj = GroupItem()
                 obj._deserialize(item)
                 self.Groups.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeAuditLogFilesRequest(AbstractModel):
+    """DescribeAuditLogFiles请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB for MariaDB。
+        :type Product: str
+        :param NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"
+        :type NodeRequestType: str
+        :param InstanceId: 实例 ID 。
+        :type InstanceId: str
+        :param Offset: 偏移量，默认为0。
+        :type Offset: int
+        :param Limit: 查询数目，默认为20，最大为100。
+        :type Limit: int
+        """
+        self.Product = None
+        self.NodeRequestType = None
+        self.InstanceId = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.Product = params.get("Product")
+        self.NodeRequestType = params.get("NodeRequestType")
+        self.InstanceId = params.get("InstanceId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAuditLogFilesResponse(AbstractModel):
+    """DescribeAuditLogFiles返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 符合条件的审计日志文件个数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param Items: 审计日志文件详情。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Items: list of AuditLogFile
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Items = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Items") is not None:
+            self.Items = []
+            for item in params.get("Items"):
+                obj = AuditLogFile()
+                obj._deserialize(item)
+                self.Items.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDBDiagEventRequest(AbstractModel):
     """DescribeDBDiagEvent请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.879/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.879/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.878/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.879/setup.py`

 * *Files identical despite different names*

