# Comparing `tmp/pangea_sdk-1.7.0.tar.gz` & `tmp/pangea_sdk-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_sdk-1.7.0.tar", max compression
+gzip compressed data, was "pangea_sdk-1.8.0.tar", max compression
```

## Comparing `pangea_sdk-1.7.0.tar` & `pangea_sdk-1.8.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     7767 2023-03-20 14:38:05.057755 pangea_sdk-1.7.0/README.md
--rw-r--r--   0        0        0      146 2023-04-10 17:17:45.138097 pangea_sdk-1.7.0/pangea/__init__.py
--rw-r--r--   0        0        0     3778 2023-03-14 20:28:21.418701 pangea_sdk-1.7.0/pangea/audit_logger.py
--rw-r--r--   0        0        0     1055 2023-03-30 18:27:54.782177 pangea_sdk-1.7.0/pangea/config.py
--rw-r--r--   0        0        0     8741 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/deep_verify.py
--rw-r--r--   0        0        0      604 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/deprecated.py
--rw-r--r--   0        0        0     6511 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/dump_audit.py
--rw-r--r--   0        0        0     4458 2023-04-10 12:18:10.328825 pangea_sdk-1.7.0/pangea/exceptions.py
--rw-r--r--   0        0        0     9874 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/request.py
--rw-r--r--   0        0        0     3895 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/response.py
--rw-r--r--   0        0        0      190 2023-04-10 17:23:24.030383 pangea_sdk-1.7.0/pangea/services/__init__.py
--rw-r--r--   0        0        0    24615 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/services/audit/audit.py
--rw-r--r--   0        0        0      451 2023-03-14 20:28:21.418701 pangea_sdk-1.7.0/pangea/services/audit/exceptions.py
--rw-r--r--   0        0        0    12230 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/services/audit/models.py
--rw-r--r--   0        0        0     5635 2023-04-10 17:24:06.407418 pangea_sdk-1.7.0/pangea/services/audit/signing.py
--rw-r--r--   0        0        0     8533 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/audit/util.py
--rw-r--r--   0        0        0     1037 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/base.py
--rw-r--r--   0        0        0     5565 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/embargo.py
--rw-r--r--   0        0        0    33733 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/intel.py
--rw-r--r--   0        0        0     7253 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/redact.py
--rw-r--r--   0        0        0     1450 2023-03-14 20:28:21.418701 pangea_sdk-1.7.0/pangea/services/vault/models/asymmetric.py
--rw-r--r--   0        0        0     7847 2023-03-28 15:10:30.783526 pangea_sdk-1.7.0/pangea/services/vault/models/common.py
--rw-r--r--   0        0        0      481 2023-03-14 20:28:21.422701 pangea_sdk-1.7.0/pangea/services/vault/models/secret.py
--rw-r--r--   0        0        0     1260 2023-03-14 20:28:21.422701 pangea_sdk-1.7.0/pangea/services/vault/models/symmetric.py
--rw-r--r--   0        0        0    43335 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/services/vault/vault.py
--rw-r--r--   0        0        0     5472 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/tools.py
--rw-r--r--   0        0        0      554 2023-03-28 15:10:30.783526 pangea_sdk-1.7.0/pangea/utils.py
--rw-r--r--   0        0        0    10606 2023-04-10 17:24:06.411419 pangea_sdk-1.7.0/pangea/verify_audit.py
--rw-r--r--   0        0        0      840 2023-04-10 17:17:45.138097 pangea_sdk-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7767 2023-03-20 14:36:50.582052 pangea_sdk-1.8.0/README.md
+-rw-r--r--   0        0        0      146 2023-04-21 21:23:31.675163 pangea_sdk-1.8.0/pangea/__init__.py
+-rw-r--r--   0        0        0     3778 2023-03-14 20:29:54.979893 pangea_sdk-1.8.0/pangea/audit_logger.py
+-rw-r--r--   0        0        0     1055 2023-03-30 18:28:00.245753 pangea_sdk-1.8.0/pangea/config.py
+-rw-r--r--   0        0        0     8741 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/deep_verify.py
+-rw-r--r--   0        0        0      604 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/deprecated.py
+-rw-r--r--   0        0        0     6511 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/dump_audit.py
+-rw-r--r--   0        0        0     4458 2023-04-10 12:19:13.490833 pangea_sdk-1.8.0/pangea/exceptions.py
+-rw-r--r--   0        0        0     9874 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/request.py
+-rw-r--r--   0        0        0     3891 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/response.py
+-rw-r--r--   0        0        0      221 2023-04-18 15:23:55.985948 pangea_sdk-1.8.0/pangea/services/__init__.py
+-rw-r--r--   0        0        0    24321 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/audit.py
+-rw-r--r--   0        0        0      451 2023-03-14 20:29:54.979893 pangea_sdk-1.8.0/pangea/services/audit/exceptions.py
+-rw-r--r--   0        0        0    12093 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/models.py
+-rw-r--r--   0        0        0     5635 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/signing.py
+-rw-r--r--   0        0        0     8533 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/audit/util.py
+-rw-r--r--   0        0        0    37620 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/authn/authn.py
+-rw-r--r--   0        0        0    16741 2023-04-19 18:36:20.317300 pangea_sdk-1.8.0/pangea/services/authn/models.py
+-rw-r--r--   0        0        0     1037 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/base.py
+-rw-r--r--   0        0        0     5565 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/embargo.py
+-rw-r--r--   0        0        0    33733 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/intel.py
+-rw-r--r--   0        0        0     7253 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/redact.py
+-rw-r--r--   0        0        0     1450 2023-03-14 20:29:54.983893 pangea_sdk-1.8.0/pangea/services/vault/models/asymmetric.py
+-rw-r--r--   0        0        0     7847 2023-04-12 15:07:35.002848 pangea_sdk-1.8.0/pangea/services/vault/models/common.py
+-rw-r--r--   0        0        0      481 2023-03-14 20:29:54.983893 pangea_sdk-1.8.0/pangea/services/vault/models/secret.py
+-rw-r--r--   0        0        0     1260 2023-04-12 15:07:35.002848 pangea_sdk-1.8.0/pangea/services/vault/models/symmetric.py
+-rw-r--r--   0        0        0    43335 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/services/vault/vault.py
+-rw-r--r--   0        0        0     5472 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/tools.py
+-rw-r--r--   0        0        0      554 2023-04-18 15:23:55.985948 pangea_sdk-1.8.0/pangea/utils.py
+-rw-r--r--   0        0        0    10606 2023-04-21 21:24:04.426975 pangea_sdk-1.8.0/pangea/verify_audit.py
+-rw-r--r--   0        0        0      840 2023-04-21 21:23:31.675163 pangea_sdk-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.8.0/PKG-INFO
```

### Comparing `pangea_sdk-1.7.0/README.md` & `pangea_sdk-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/audit_logger.py` & `pangea_sdk-1.8.0/pangea/audit_logger.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/config.py` & `pangea_sdk-1.8.0/pangea/config.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/deep_verify.py` & `pangea_sdk-1.8.0/pangea/deep_verify.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/deprecated.py` & `pangea_sdk-1.8.0/pangea/deprecated.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/dump_audit.py` & `pangea_sdk-1.8.0/pangea/dump_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/exceptions.py` & `pangea_sdk-1.8.0/pangea/exceptions.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/request.py` & `pangea_sdk-1.8.0/pangea/request.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/response.py` & `pangea_sdk-1.8.0/pangea/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         }
 
 
 class PangeaResponseResult(APIResponseModel):
     pass
 
 
-class ErrorField(PangeaResponseResult):
+class ErrorField(APIResponseModel):
     """
     Field errors denote errors in fields provided in request payloads
 
     Fields:
         code(str): The field code
         detail(str): A human readable detail explaining the error
         source(str): A JSON pointer where the error occurred
```

### Comparing `pangea_sdk-1.7.0/pangea/services/audit/audit.py` & `pangea_sdk-1.8.0/pangea/services/audit/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,14 @@
         old: Optional[Union[str, dict]] = None,
         source: Optional[str] = None,
         status: Optional[str] = None,
         target: Optional[str] = None,
         timestamp: Optional[datetime.datetime] = None,
         verify: bool = False,
         signing: EventSigning = EventSigning.NONE,
-        signature_key_id: Optional[str] = None,
-        signature_key_version: Optional[str] = None,
         verbose: Optional[bool] = None,
     ) -> PangeaResponse[LogResult]:
         """
         Log an entry
 
         Create a log entry in the Secure Audit Log.
         Args:
@@ -170,19 +168,14 @@
                 input.signature = signature
             else:
                 raise AuditException("Error: failure signing message")
 
             # Add public key value to public key info and serialize
             self.set_public_key(input, self.signer, self.public_key_info)
 
-        elif signing == EventSigning.VAULT:
-            input.sign = True
-            input.signature_key_id = signature_key_id
-            input.signature_key_version = signature_key_version
-
         if verify:
             input.verbose = True
             if self.prev_unpublished_root_hash:
                 input.prev_root = self.prev_unpublished_root_hash
 
         response = self.request.post(endpoint_name, data=input.dict(exclude_none=True))
         return self.handle_log_response(response, verify=verify)
```

### Comparing `pangea_sdk-1.7.0/pangea/services/audit/models.py` & `pangea_sdk-1.8.0/pangea/services/audit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     def __repr__(self):
         return str(self.value)
 
 
 class EventSigning(enum.Enum):
     NONE = 0
     LOCAL = 1
-    VAULT = 2
 
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return str(self.value)
 
@@ -124,17 +123,14 @@
     """
 
     event: Event
     verbose: Optional[bool] = None
     signature: Optional[str] = None
     public_key: Optional[str] = None
     prev_root: Optional[str] = None
-    sign: Optional[bool] = None
-    signature_key_id: Optional[str] = None
-    signature_key_version: Optional[str] = None
 
 
 class LogResult(PangeaResponseResult):
     """
     Result class after an audit log action
 
     envelope -- Event envelope information.
```

### Comparing `pangea_sdk-1.7.0/pangea/services/audit/signing.py` & `pangea_sdk-1.8.0/pangea/services/audit/signing.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/audit/util.py` & `pangea_sdk-1.8.0/pangea/services/audit/util.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/base.py` & `pangea_sdk-1.8.0/pangea/services/base.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/embargo.py` & `pangea_sdk-1.8.0/pangea/services/embargo.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/intel.py` & `pangea_sdk-1.8.0/pangea/services/intel.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/redact.py` & `pangea_sdk-1.8.0/pangea/services/redact.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/vault/models/asymmetric.py` & `pangea_sdk-1.8.0/pangea/services/vault/models/asymmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/vault/models/common.py` & `pangea_sdk-1.8.0/pangea/services/vault/models/common.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/vault/models/symmetric.py` & `pangea_sdk-1.8.0/pangea/services/vault/models/symmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/services/vault/vault.py` & `pangea_sdk-1.8.0/pangea/services/vault/vault.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/tools.py` & `pangea_sdk-1.8.0/pangea/tools.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/utils.py` & `pangea_sdk-1.8.0/pangea/utils.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pangea/verify_audit.py` & `pangea_sdk-1.8.0/pangea/verify_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.7.0/pyproject.toml` & `pangea_sdk-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pangea-sdk"
-version = "1.7.0"
+version = "1.8.0"
 description = "Pangea API SDK"
 authors = ["Glenn Gallien <glenn.gallien@pangea.cloud>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = ""
 keywords = ["Pangea", "SDK", "Audit"]
```

### Comparing `pangea_sdk-1.7.0/PKG-INFO` & `pangea_sdk-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangea-sdk
-Version: 1.7.0
+Version: 1.8.0
 Summary: Pangea API SDK
 License: MIT
 Keywords: Pangea,SDK,Audit
 Author: Glenn Gallien
 Author-email: glenn.gallien@pangea.cloud
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

