# Comparing `tmp/blobfile-2.0.1-py3-none-any.whl.zip` & `tmp/blobfile-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 73529 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jan-10 07:25 blobfile/VERSION
--rw-rw-rw-  2.0 fat     1890 b- defN 22-May-05 23:14 blobfile/__init__.py
--rw-rw-rw-  2.0 fat    66272 b- defN 22-Sep-20 06:28 blobfile/_azure.py
--rw-rw-rw-  2.0 fat    42100 b- defN 23-Jan-10 06:19 blobfile/_common.py
--rw-rw-rw-  2.0 fat    61210 b- defN 22-Sep-30 02:59 blobfile/_context.py
+Zip file size: 74500 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-21 05:37 blobfile/VERSION
+-rw-rw-rw-  2.0 fat     1955 b- defN 23-Apr-21 05:37 blobfile/__init__.py
+-rw-rw-rw-  2.0 fat    67987 b- defN 23-Apr-21 05:37 blobfile/_azure.py
+-rw-rw-rw-  2.0 fat    42267 b- defN 23-Apr-21 05:37 blobfile/_common.py
+-rw-rw-rw-  2.0 fat    62882 b- defN 23-Apr-21 05:37 blobfile/_context.py
 -rw-rw-rw-  2.0 fat    27701 b- defN 22-Sep-04 17:28 blobfile/_gcp.py
--rw-rw-rw-  2.0 fat    14526 b- defN 22-Sep-30 03:00 blobfile/_ops.py
--rw-rw-rw-  2.0 fat    57956 b- defN 23-Jan-10 06:53 blobfile/_ops_test.py
+-rw-rw-rw-  2.0 fat    14898 b- defN 23-Apr-21 05:37 blobfile/_ops.py
+-rw-rw-rw-  2.0 fat    59052 b- defN 23-Apr-21 05:37 blobfile/_ops_test.py
 -rw-rw-rw-  2.0 fat     2776 b- defN 22-Sep-06 04:23 blobfile/_xml.py
 -rw-rw-rw-  2.0 fat     5094 b- defN 22-Sep-06 04:24 blobfile/_xml_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-May-05 23:14 blobfile/py.typed
--rw-rw-rw-  2.0 fat     1233 b- defN 23-Jan-10 07:26 blobfile-2.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14815 b- defN 23-Jan-10 07:26 blobfile-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jan-10 07:26 blobfile-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jan-10 07:26 blobfile-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1218 b- defN 23-Jan-10 07:26 blobfile-2.0.1.dist-info/RECORD
-16 files, 296902 bytes uncompressed, 71563 bytes compressed:  75.9%
+-rw-rw-rw-  2.0 fat     1233 b- defN 23-Apr-21 05:38 blobfile-2.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    14941 b- defN 23-Apr-21 05:38 blobfile-2.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-21 05:38 blobfile-2.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-21 05:38 blobfile-2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1218 b- defN 23-Apr-21 05:38 blobfile-2.0.2.dist-info/RECORD
+16 files, 302115 bytes uncompressed, 72534 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: blobfile/_xml_test.py
 Comment: 
 
 Filename: blobfile/py.typed
 Comment: 
 
-Filename: blobfile-2.0.1.dist-info/LICENSE
+Filename: blobfile-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: blobfile-2.0.1.dist-info/METADATA
+Filename: blobfile-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: blobfile-2.0.1.dist-info/WHEEL
+Filename: blobfile-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: blobfile-2.0.1.dist-info/top_level.txt
+Filename: blobfile-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: blobfile-2.0.1.dist-info/RECORD
+Filename: blobfile-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## blobfile/VERSION

```diff
@@ -1 +1 @@
-2.0.1
+2.0.2
```

## blobfile/__init__.py

```diff
@@ -29,14 +29,15 @@
 from blobfile._context import Context as Context, create_context as create_context
 from blobfile._common import (
     Request as Request,
     Error as Error,
     RequestFailure as RequestFailure,
     RestartableStreamingWriteFailure as RestartableStreamingWriteFailure,
     ConcurrentWriteFailure as ConcurrentWriteFailure,
+    VersionMismatch as VersionMismatch,
     DeadlineExceeded as DeadlineExceeded,
     Stat as Stat,
     DirEntry as DirEntry,
 )
 
 
 _SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
@@ -71,8 +72,9 @@
     "RestartableStreamingWriteFailure",
     "ConcurrentWriteFailure",
     "DeadlineExceeded",
     "Stat",
     "DirEntry",
     "Context",
     "create_context",
+    "VersionMismatch",
 ]
```

## blobfile/_azure.py

```diff
@@ -30,14 +30,15 @@
     Request,
     RequestFailure,
     Stat,
     TokenManager,
     path_join,
     strip_slashes,
     rng,
+    VersionMismatch,
 )
 
 SHARED_KEY = "shared_key"
 OAUTH_TOKEN = "oauth_token"
 ANONYMOUS = "anonymous"
 
 # it looks like azure signed urls cannot exceed the lifetime of the token used
@@ -859,15 +860,17 @@
 def _block_index_to_block_id(index: int, upload_id: int) -> str:
     assert index < 2 ** 17
     id_plus_index = (upload_id << 17) + index
     assert id_plus_index < 2 ** 64
     return base64.b64encode(id_plus_index.to_bytes(8, byteorder="big")).decode("utf8")
 
 
-def _clear_uncommitted_blocks(conf: Config, url: str, metadata: Dict[str, str]) -> None:
+def _clear_uncommitted_blocks(
+    conf: Config, url: str, metadata: Dict[str, str]
+) -> Optional[urllib3.HTTPResponse]:
     # to avoid leaking uncommitted blocks, we can do a Put Block List with
     # all the existing blocks for a file
     # this will change the last-modified timestamp and the etag
     req = Request(
         url=url, params=dict(comp="blocklist"), method="GET", success_codes=(200, 404)
     )
     resp = execute_api_request(conf, req)
@@ -891,33 +894,42 @@
         url=url,
         method="PUT",
         params=dict(comp="blocklist"),
         headers={**headers, "If-Match": metadata["etag"]},
         data=body,
         success_codes=(201, 404, 412),
     )
-    execute_api_request(conf, req)
+
+    return execute_api_request(conf, req)
 
 
 def _finalize_blob(
-    conf: Config, path: str, url: str, block_ids: List[str], md5_digest: Optional[bytes]
+    conf: Config,
+    path: str,
+    url: str,
+    block_ids: List[str],
+    md5_digest: Optional[bytes],
+    version: Optional[str],
 ) -> None:
     body = {"BlockList": {"Latest": block_ids}}
     headers = {}
     if md5_digest is not None:
         # azure does not calculate md5s for us, we have to do that manually
         # https://web.archive.org/web/20190118183153/https://blogs.msdn.microsoft.com/windowsazurestorage/2011/02/17/windows-azure-blob-md5-overview/
         headers["x-ms-blob-content-md5"] = base64.b64encode(md5_digest).decode("utf8")
+
+    if version is not None:
+        headers["If-Match"] = version
     req = Request(
         url=url,
         method="PUT",
         headers=headers,
         params=dict(comp="blocklist"),
         data=body,
-        success_codes=(201, 400, 404, INVALID_HOSTNAME_STATUS),
+        success_codes=(201, 400, 404, 412, INVALID_HOSTNAME_STATUS),
     )
     resp = execute_api_request(conf, req)
     if resp.status == 400:
         result = xml.parse(resp.data)
         if result["Error"]["Code"] == "InvalidBlockList":
             # the most likely way this could happen is if the file was deleted while
             # we were uploading, so assume that is what happened
@@ -931,14 +943,23 @@
         else:
             raise RequestFailure.create_from_request_response(
                 message=f"unexpected status {resp.status}", request=req, response=resp
             )
     elif resp.status == 404 or resp.status == INVALID_HOSTNAME_STATUS:
         # this can occur when using parallel upload
         raise FileNotFoundError(f"No such file or directory: '{path}'")
+    elif resp.status == 412:
+        if resp.headers["x-ms-error-code"] != "ConditionNotMet":
+            raise RequestFailure.create_from_request_response(
+                message=f"unexpected status {resp.status}", request=req, response=resp
+            )
+        else:
+            raise VersionMismatch.create_from_request_response(
+                message=f"etag mismatch", request=req, response=resp
+            )
 
 
 def isdir(conf: Config, path: str) -> bool:
     """
     Return true if a path is an existing directory
     """
     if not path.endswith("/"):
@@ -1034,15 +1055,15 @@
             preload_content=not streaming,
         )
         resp = execute_api_request(self._conf, req)
         return resp
 
 
 class StreamingWriteFile(BaseStreamingWriteFile):
-    def __init__(self, conf: Config, path: str) -> None:
+    def __init__(self, conf: Config, path: str, version: Optional[str]) -> None:
         self._path = path
         account, container, blob = split_path(path)
         self._url = build_url(
             account, "/{container}/{blob}", container=container, blob=blob
         )
         # block blobs let you upload up to 100,000 "uncommitted" blocks with user-chosen block ids
         # using the "Put Block" call
@@ -1116,41 +1137,58 @@
         # if blobs could automatically expire without having to add a container lifecycle rule
         #   then we could upload to a temp path, then copy to the final path (assuming copy is atomic)
         #   without automatic expiry, we'd leak temp files
         # we can use the lease system, but then we have to deal with leases
 
         self._upload_id = rng.randint(0, 2 ** 47 - 1)
         self._block_index = 0
+        self._version = version  # for azure, this is an etag
         # check to see if there is an existing blob at this location with the wrong type
         req = Request(
             url=self._url,
             method="HEAD",
-            success_codes=(200, 400, 404, INVALID_HOSTNAME_STATUS),
+            headers={"If-Match": self._version} if self._version else {},
+            success_codes=(200, 400, 404, 412, INVALID_HOSTNAME_STATUS),
         )
         resp = execute_api_request(conf, req)
         if resp.status == 200:
             if resp.headers["x-ms-blob-type"] == "BlockBlob":
                 # because we delete all the uncommitted blocks, any concurrent writers will fail
                 # but they would fail anyway since the first writer to finish would end up
                 # deleting all uncommitted blocks
                 # this means that the last writer to start is likely to win, the others should fail
                 # with ConcurrentWriteFailure
-                _clear_uncommitted_blocks(conf, self._url, resp.headers)
+                resp = _clear_uncommitted_blocks(conf, self._url, resp.headers)
+                if resp:
+                    self._version = resp.headers[
+                        "ETag"
+                    ]  # update the version according to new etag
             else:
                 # if the existing blob type is not compatible with the block blob we are about to write
                 # we have to delete the file before writing our block blob or else we will get a 409
                 # error when putting the first block
                 remove(conf, path)
         elif resp.status in (400, INVALID_HOSTNAME_STATUS) or (
             resp.status == 404
             and resp.headers["x-ms-error-code"] == "ContainerNotFound"
         ):
             raise FileNotFoundError(
                 f"No such file or container/account does not exist: '{path}'"
             )
+        elif resp.status == 412:
+            if resp.headers["x-ms-error-code"] != "ConditionNotMet":
+                raise RequestFailure.create_from_request_response(
+                    message=f"unexpected status {resp.status}",
+                    request=req,
+                    response=resp,
+                )
+            else:
+                raise VersionMismatch.create_from_request_response(
+                    message=f"etag mismatch", request=req, response=resp
+                )
         self._md5 = hashlib.md5()
         super().__init__(conf=conf, chunk_size=conf.azure_write_chunk_size)
 
     def _upload_chunk(self, chunk: memoryview, finalize: bool) -> None:
         start = 0
         while start < len(chunk):
             # premium block blob storage supports block blobs and append blobs
@@ -1195,14 +1233,15 @@
             ]
             _finalize_blob(
                 conf=self._conf,
                 path=self._path,
                 url=self._url,
                 block_ids=block_ids,
                 md5_digest=self._md5.digest(),
+                version=self._version,
             )
 
 
 def _upload_chunk(
     conf: Config, path: str, start: int, size: int, url: str, block_id: str
 ) -> None:
     req = Request(
@@ -1222,14 +1261,15 @@
 
 def parallel_upload(
     conf: Config,
     executor: concurrent.futures.Executor,
     src: str,
     dst: str,
     return_md5: bool,
+    dst_version: Optional[str],
 ) -> Optional[str]:
     with open(src, "rb") as f:
         md5_digest = common.block_md5(f)
 
     account, container, blob = split_path(dst)
     dst_url = build_url(account, "/{container}/{blob}", container=container, blob=blob)
 
@@ -1259,15 +1299,20 @@
         block_ids.append(block_id)
         i += 1
         start += part_size
     for future in futures:
         future.result()
 
     _finalize_blob(
-        conf=conf, path=dst, url=dst_url, block_ids=block_ids, md5_digest=md5_digest
+        conf=conf,
+        path=dst,
+        url=dst_url,
+        block_ids=block_ids,
+        md5_digest=md5_digest,
+        version=dst_version,
     )
     return binascii.hexlify(md5_digest).decode("utf8") if return_md5 else None
 
 
 def maybe_stat(conf: Config, path: str) -> Optional[Stat]:
     account, container, blob = split_path(path)
     if blob == "":
@@ -1622,14 +1667,15 @@
 
 def parallel_remote_copy(
     conf: Config,
     executor: concurrent.futures.Executor,
     src: str,
     dst: str,
     return_md5: bool,
+    dst_version: Optional[str],
 ) -> Optional[str]:
     # for whatever reason, put block from url is faster than copy blob when you run multiple requests in parallel
     # https://docs.microsoft.com/en-us/rest/api/storageservices/put-block-from-url
 
     st = maybe_stat(conf, src)
     if st is None:
         raise FileNotFoundError(f"The system cannot find the path specified: '{src}'")
@@ -1665,15 +1711,20 @@
 
     dst_account, dst_container, dst_blob = split_path(dst)
     dst_url = build_url(
         dst_account, "/{container}/{blob}", container=dst_container, blob=dst_blob
     )
 
     _finalize_blob(
-        conf=conf, path=dst, url=dst_url, block_ids=block_ids, md5_digest=md5_digest
+        conf=conf,
+        path=dst,
+        url=dst_url,
+        block_ids=block_ids,
+        md5_digest=md5_digest,
+        version=dst_version,
     )
     return (
         binascii.hexlify(md5_digest).decode("utf8")
         if (return_md5 and md5_digest is not None)
         else None
     )
```

## blobfile/_common.py

```diff
@@ -240,14 +240,22 @@
     """
     A read failed after the deadline was exceeded
     """
 
     pass
 
 
+class VersionMismatch(RequestFailure):
+    """
+    A write failed due to a version mismatch, using ETag for azure or generation for gcloud
+    """
+
+    pass
+
+
 class Stat(NamedTuple):
     size: int
     mtime: float
     ctime: float
     md5: Optional[str]
     version: Optional[str]
```

## blobfile/_context.py

```diff
@@ -1,12 +1,11 @@
 # https://mypy.readthedocs.io/en/stable/common_issues.html#using-classes-that-are-generic-in-stubs-but-not-at-runtime
 from __future__ import annotations
 
 import binascii
-import stat as stat_module
 import collections
 import concurrent.futures
 import contextlib
 import hashlib
 import io
 import itertools
 import math
@@ -14,14 +13,15 @@
 import os
 import re
 import shutil
 import stat as stat_module
 import tempfile
 import time
 import urllib.parse
+from functools import partial
 from types import ModuleType
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Callable,
     Iterator,
@@ -91,46 +91,54 @@
         self,
         src: str,
         dst: str,
         overwrite: bool = False,
         parallel: bool = False,
         parallel_executor: Optional[concurrent.futures.Executor] = None,
         return_md5: bool = False,
+        dst_version: Optional[str] = None,
     ) -> Optional[str]:
         # it would be best to check isdir() for remote paths, but that would
         # involve 2 extra network requests, so just do this test instead
         if _guess_isdir(src):
             raise IsADirectoryError(f"Is a directory: '{src}'")
         if _guess_isdir(dst):
             raise IsADirectoryError(f"Is a directory: '{dst}'")
 
         if not overwrite:
             if self.exists(dst):
                 raise FileExistsError(
                     f"Destination '{dst}' already exists and overwrite is disabled"
                 )
 
+        if dst_version is not None:
+            assert _is_azure_path(
+                dst
+            ), f"Destination version was specified, but destination path {dst} does not support a version check"
+
         if parallel:
             copy_fn = None
             if (_is_azure_path(src) or _is_gcp_path(src)) and _is_local_path(dst):
                 copy_fn = _parallel_download
 
             if _is_local_path(src) and _is_azure_path(dst):
-                copy_fn = azure.parallel_upload
+                copy_fn = partial(azure.parallel_upload, dst_version=dst_version)
 
             if _is_local_path(src) and _is_gcp_path(dst):
                 copy_fn = gcp.parallel_upload
 
             if _is_azure_path(src) and _is_azure_path(dst):
                 src_account, _, _ = azure.split_path(src)
                 dst_account, _, _ = azure.split_path(dst)
                 if src_account != dst_account:
                     # normal remote copy is pretty fast and doesn't benefit from parallelization when used within
                     # a storage account
-                    copy_fn = azure.parallel_remote_copy
+                    copy_fn = partial(
+                        azure.parallel_remote_copy, dst_version=dst_version
+                    )
 
             if copy_fn is not None:
                 if parallel_executor is None:
                     with concurrent.futures.ProcessPoolExecutor(
                         mp_context=mp.get_context(
                             self._conf.multiprocessing_start_method
                         )
@@ -144,22 +152,26 @@
                     )
 
         # special case cloud to cloud copy, don't download the file
         if _is_gcp_path(src) and _is_gcp_path(dst):
             return gcp.remote_copy(self._conf, src=src, dst=dst, return_md5=return_md5)
 
         if _is_azure_path(src) and _is_azure_path(dst):
+            # support could be added here for this but it's currently missing
+            assert (
+                dst_version is None
+            ), f"Destination version was specified, but destination path {dst} does not support a version check"
             return azure.remote_copy(
                 self._conf, src=src, dst=dst, return_md5=return_md5
             )
 
         for attempt, backoff in enumerate(common.exponential_sleep_generator()):
             try:
                 with self.BlobFile(src, "rb", streaming=True) as src_f, self.BlobFile(
-                    dst, "wb", streaming=True
+                    dst, "wb", streaming=True, version=dst_version
                 ) as dst_f:
                     m = hashlib.md5()
                     while True:
                         block = src_f.read(CHUNK_SIZE)
                         if block == b"":
                             break
                         if return_md5:
@@ -815,69 +827,85 @@
         self,
         path: str,
         mode: Literal["rb", "wb", "ab"],
         streaming: Optional[bool] = ...,
         buffer_size: int = ...,
         cache_dir: Optional[str] = ...,
         file_size: Optional[int] = None,
+        version: Optional[str] = None,
     ) -> BinaryIO:
         ...
 
     @overload
     def BlobFile(
         self,
         path: str,
         mode: Literal["r", "w", "a"] = ...,
         streaming: Optional[bool] = ...,
         buffer_size: int = ...,
         cache_dir: Optional[str] = ...,
         file_size: Optional[int] = None,
+        version: Optional[str] = None,
     ) -> TextIO:
         ...
 
     def BlobFile(
         self,
         path: str,
         mode: Literal["r", "rb", "w", "wb", "a", "ab"] = "r",
         streaming: Optional[bool] = None,
         buffer_size: Optional[int] = None,
         cache_dir: Optional[str] = None,
         file_size: Optional[int] = None,
+        version: Optional[str] = None,
     ):
         """
         Open a local or remote file for reading or writing
 
         Args:
-            path local or remote path
+            path: local or remote path
             mode: one of "r", "rb", "w", "wb", "a", "ab" indicating the mode to open the file in
             streaming: the default for `streaming` is `True` when `mode` is in `"r", "rb"` and `False` when `mode` is in `"w", "wb", "a", "ab"`.
                 * `streaming=True`:
                     * Reading is done without downloading the entire remote file.
                     * Writing is done to the remote file directly, but only in chunks of a few MB in size. `flush()` will not cause an early write.
                     * Appending is not implemented.
                 * `streaming=False`:
                     * Reading is done by downloading the remote file to a local file during the constructor.
                     * Writing is done by uploading the file on `close()` or during destruction.
                     * Appending is done by downloading the file during construction and uploading on `close()` or during destruction.
             buffer_size: number of bytes to buffer, this can potentially make reading more efficient.
             cache_dir: a directory in which to cache files for reading, only valid if `streaming=False` and `mode` is in `"r", "rb"`.   You are reponsible for cleaning up the cache directory.
             file_size: size of the file being opened, can be specified directly to avoid checking the file size when opening the file.  While this will avoid a network request, it also means that you may get an error when first reading a file that does not exist rather than when opening it.  Only valid for modes "r" and "rb".  This valid will be ignored for local files.
+            version: a version number of the file being opened, used to prevent overwriting a file that has changed since it was opened.  Only valid for modes "w", "wb", "a", "ab"
 
         Returns:
             A file-like object
         """
         if _guess_isdir(path):
             raise IsADirectoryError(f"Is a directory: '{path}'")
 
         if streaming is None:
             streaming = mode in ("r", "rb")
 
         if file_size is not None:
             assert mode in ("r", "rb"), "Can only specify file_size when reading"
 
+        if version:
+            assert mode in (
+                "w",
+                "wb",
+                "a",
+                "ab",
+            ), "Can only specify version when writing"
+            assert not _is_local_path(
+                path
+            ), "Cannot specify version when writing to local file"
+            # we check for gcp later to raise a NotImplementedError instead
+
         if _is_local_path(path) and "w" in mode:
             # local filesystems require that intermediate directories exist, but this is not required by the
             # remote filesystems
             # for consistency, automatically create local intermediate directories
             if self.dirname(path) != "":
                 self.makedirs(self.dirname(path))
 
@@ -892,24 +920,26 @@
             if _is_local_path(path):
                 f = io.FileIO(path, mode=mode)
                 if "r" in mode:
                     f = io.BufferedReader(f, buffer_size=buffer_size)
                 else:
                     f = io.BufferedWriter(f, buffer_size=buffer_size)
             elif _is_gcp_path(path):
+                if version:
+                    raise NotImplementedError("Cannot specify version for GCP files")
                 if mode in ("w", "wb"):
                     f = gcp.StreamingWriteFile(self._conf, path)
                 elif mode in ("r", "rb"):
                     f = gcp.StreamingReadFile(self._conf, path, size=file_size)
                     f = io.BufferedReader(f, buffer_size=buffer_size)
                 else:
                     raise Error(f"Unsupported mode: '{mode}'")
             elif _is_azure_path(path):
                 if mode in ("w", "wb"):
-                    f = azure.StreamingWriteFile(self._conf, path)
+                    f = azure.StreamingWriteFile(self._conf, path, version)
                 elif mode in ("r", "rb"):
                     f = azure.StreamingReadFile(self._conf, path, size=file_size)
                     f = io.BufferedReader(f, buffer_size=buffer_size)
                 else:
                     raise Error(f"Unsupported mode: '{mode}'")
             else:
                 raise Error(f"Unrecognized path: '{path}'")
@@ -1052,14 +1082,15 @@
 
             f = _ProxyFile(
                 ctx=self,
                 local_path=local_path,
                 mode=mode,
                 tmp_dir=tmp_dir,
                 remote_path=remote_path,
+                version=version,
             )
             if "r" in mode:
                 f = io.BufferedReader(f, buffer_size=buffer_size)
             else:
                 f = io.BufferedWriter(f, buffer_size=buffer_size)
             binary_f = cast(BinaryIO, f)
             if "b" in mode:
@@ -1469,31 +1500,38 @@
     def __init__(
         self,
         ctx: Context,
         local_path: str,
         mode: 'Literal["r", "rb", "w", "wb", "a", "ab"]',
         tmp_dir: Optional[str],
         remote_path: Optional[str],
+        version: Optional[str],
     ) -> None:
         super().__init__(local_path, mode=mode)
         self._ctx = ctx
         self._mode = mode
         self._tmp_dir = tmp_dir
         self._local_path = local_path
         self._remote_path = remote_path
         self._closed = False
+        self._version = version
 
     def close(self) -> None:
         if not hasattr(self, "_closed") or self._closed:
             return
 
         super().close()
         try:
             if self._remote_path is not None and self._mode in ("w", "wb", "a", "ab"):
-                self._ctx.copy(self._local_path, self._remote_path, overwrite=True)
+                self._ctx.copy(
+                    self._local_path,
+                    self._remote_path,
+                    overwrite=True,
+                    dst_version=self._version,
+                )
         finally:
             # if the copy fails, still cleanup our local temp file so it is not leaked
             if self._tmp_dir is not None:
                 os.remove(self._local_path)
                 os.rmdir(self._tmp_dir)
         self._closed = True
```

## blobfile/_ops.py

```diff
@@ -106,14 +106,15 @@
 def copy(
     src: str,
     dst: str,
     overwrite: bool = False,
     parallel: bool = False,
     parallel_executor: Optional[concurrent.futures.Executor] = None,
     return_md5: bool = False,
+    dst_version: Optional[str] = None,
 ) -> Optional[str]:
     """
     Copy a file from one path to another
 
     If both paths are on the same blob storage, this will perform a remote copy operation without downloading
     the contents locally.
 
@@ -122,22 +123,25 @@
 
     If `parallel` is `True`, use multiple processes to dowload or upload the file.  For this to work, one path must be on blob storage and the other path must be local.  This can be faster on cloud machines but is not in general guaranteed to be faster than using serial copy.  The default is `False`.
 
     If `parallel_executor` is set to a `concurrent.futures.Executor` and `parallel` is set to `True`, the provided executor will be used instead of creating a new one for each call to `copy()`.
 
     If `return_md5` is set to `True`, an md5 will be calculated during the copy and returned if available,
     or else None will be returned.
+
+    If `dst_version` is set to a version string, the copy will fail if the destination path does not have this version (versions can be retrieved with `stat()`)
     """
     return default_context.copy(
         src=src,
         dst=dst,
         overwrite=overwrite,
         parallel=parallel,
         parallel_executor=parallel_executor,
         return_md5=return_md5,
+        dst_version=dst_version,
     )
 
 
 def exists(path: str) -> bool:
     """
     Return true if that path exists (either as a file or a directory)
     """
@@ -307,37 +311,40 @@
 def BlobFile(
     path: str,
     mode: Literal["rb", "wb", "ab"],
     streaming: Optional[bool] = ...,
     buffer_size: int = ...,
     cache_dir: Optional[str] = ...,
     file_size: Optional[int] = None,
+    version: Optional[str] = None,
 ) -> BinaryIO:
     ...
 
 
 @overload
 def BlobFile(
     path: str,
     mode: Literal["r", "w", "a"] = ...,
     streaming: Optional[bool] = ...,
     buffer_size: int = ...,
     cache_dir: Optional[str] = ...,
     file_size: Optional[int] = None,
+    version: Optional[str] = None,
 ) -> TextIO:
     ...
 
 
 def BlobFile(
     path: str,
     mode: Literal["r", "rb", "w", "wb", "a", "ab"] = "r",
     streaming: Optional[bool] = None,
     buffer_size: Optional[int] = None,
     cache_dir: Optional[str] = None,
     file_size: Optional[int] = None,
+    version: Optional[str] = None,
 ):
     """
     Open a local or remote file for reading or writing
 
     Args:
         path local or remote path
         mode: one of "r", "rb", "w", "wb", "a", "ab" indicating the mode to open the file in
@@ -359,8 +366,9 @@
     return default_context.BlobFile(
         path=path,
         mode=mode,
         streaming=streaming,
         buffer_size=buffer_size,
         cache_dir=cache_dir,
         file_size=file_size,
+        version=version,
     )
```

## blobfile/_ops_test.py

```diff
@@ -1469,14 +1469,46 @@
         assert st.md5 == purr_hash
         bf.remove(path)
         assert not azure.maybe_update_md5(
             ops.default_context._conf, path, st.version, meow_hash
         )
 
 
+@pytest.mark.parametrize("ctx", [_get_temp_as_path])
+def test_azure_etags(ctx):
+    contents = b"bark!"
+    alternative_contents = b"ruff"
+
+    with ctx() as path:
+        bf.BlobFile(path, "wb").write(contents)
+        version = bf.stat(path).version
+
+        # test can write a bunch of times on correct version
+        with bf.BlobFile(path, "wb", version=version) as f:
+            # first time should work
+            for _ in range(1000):
+                f.write(alternative_contents)
+
+        version = bf.stat(path).version
+        with bf.BlobFile(path, "wb", version=version) as f:
+            # overwrite it again to match with later in test
+            f.write(alternative_contents)
+
+        new_version = bf.stat(path).version
+        assert new_version != version
+        with pytest.raises(bf.VersionMismatch):
+            with bf.BlobFile(path, "wb", version=version) as f:
+                # second time should fail
+                f.write(contents)
+
+        assert bf.BlobFile(path, "rb").read() == alternative_contents
+
+        bf.remove(path)
+
+
 def test_azure_timestamp_parsing():
     timestamp = "Sun, 27 Sep 2009 18:41:57 GMT"
 
     def ref_parse_timestamp(text: str) -> float:
         return datetime.datetime.strptime(
             text.replace("GMT", "Z"), "%a, %d %b %Y %H:%M:%S %z"
         ).timestamp()
```

## Comparing `blobfile-2.0.1.dist-info/LICENSE` & `blobfile-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `blobfile-2.0.1.dist-info/METADATA` & `blobfile-2.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobfile
-Version: 2.0.1
+Version: 2.0.2
 Summary: Read GCS, ABS and local paths with the same interface, clone of tensorflow.io.gfile
 Home-page: https://github.com/christopher-hesse/blobfile
 Author: Christopher Hesse
 License: Public Domain
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -150,14 +150,15 @@
 
 ## Errors
 
 * `Error` - base class for library-specific exceptions
 * `RequestFailure(Error)` - a request has failed permanently, the status code can be found in the property `response_status:int` and an error code, if available, is in `error:Optional[str]`.
 * `RestartableStreamingWriteFailure(RequestFailure)` - a streaming write has failed permanently, which requires restarting from the beginning of the stream.
 * `ConcurrentWriteFailure(RequestFailure)` - a write failed because another process was writing to the same file at the same time.
+* `VersionMismatch(RequestFailure)` - a write failed because the remote file did not match the version specified by the user.
 * The following generic exceptions are raised from some functions to make the behavior similar to the original versions: `FileNotFoundError`, `FileExistsError`, `IsADirectoryError`, `NotADirectoryError`, `OSError`, `ValueError`, `io.UnsupportedOperation`
 
 ## Logging
 
 `blobfile` will keep retrying transient errors until they succeed or a permanent error is encountered (which will raise an exception).  In order to make diagnosing stalls easier, `blobfile` will log when retrying requests.
 
 To route those log lines, use `configure(log_callback=<fn>)` to set a callback function which will be called whenever a log line should be printed.  The default callback prints to stdout with the prefix `blobfile:`.
```

