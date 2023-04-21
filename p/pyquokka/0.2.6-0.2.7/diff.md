# Comparing `tmp/pyquokka-0.2.6-py3-none-any.whl.zip` & `tmp/pyquokka-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -22,15 +22,15 @@
 -rw-rw-r--  2.0 unx    19755 b- defN 23-Apr-14 04:33 pyquokka/quokka_runtime.py
 -rw-rw-r--  2.0 unx    93718 b- defN 22-Oct-04 03:50 pyquokka/redis.conf
 -rw-rw-r--  2.0 unx    16471 b- defN 23-Mar-27 22:47 pyquokka/sql_utils.py
 -rw-rw-r--  2.0 unx     2371 b- defN 22-Jul-15 20:59 pyquokka/state.py
 -rw-rw-r--  2.0 unx    11695 b- defN 23-Apr-09 03:05 pyquokka/tables.py
 -rw-rw-r--  2.0 unx     2351 b- defN 23-Jan-28 04:17 pyquokka/target_info.py
 -rw-rw-r--  2.0 unx     5752 b- defN 23-Mar-20 21:30 pyquokka/task.py
--rw-rw-r--  2.0 unx    29805 b- defN 23-Apr-21 00:03 pyquokka/utils.py
+-rw-rw-r--  2.0 unx    29799 b- defN 23-Apr-21 00:29 pyquokka/utils.py
 -rw-rw-r--  2.0 unx     4081 b- defN 23-Jan-25 17:17 pyquokka/windowtypes.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2659 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/RECORD
-34 files, 981540 bytes uncompressed, 271520 bytes compressed:  72.3%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-21 00:31 pyquokka-0.2.7.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-21 00:31 pyquokka-0.2.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 00:31 pyquokka-0.2.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-21 00:31 pyquokka-0.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2659 b- defN 23-Apr-21 00:31 pyquokka-0.2.7.dist-info/RECORD
+34 files, 981534 bytes uncompressed, 271520 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -81,23 +81,23 @@
 
 Filename: pyquokka/utils.py
 Comment: 
 
 Filename: pyquokka/windowtypes.py
 Comment: 
 
-Filename: pyquokka-0.2.6.dist-info/LICENSE
+Filename: pyquokka-0.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: pyquokka-0.2.6.dist-info/METADATA
+Filename: pyquokka-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: pyquokka-0.2.6.dist-info/WHEEL
+Filename: pyquokka-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyquokka-0.2.6.dist-info/top_level.txt
+Filename: pyquokka-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyquokka-0.2.6.dist-info/RECORD
+Filename: pyquokka-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyquokka/utils.py

```diff
@@ -135,15 +135,15 @@
         if self.redis_process is not None:
             self.redis_process.kill()
 
 
 def execute_script(key_location, x):
     return os.system("ssh -oStrictHostKeyChecking=no -i {} ubuntu@{} 'bash -s' < {}".format(key_location, x, pyquokka.__file__.replace("__init__.py", "common_startup.sh")))
 
-def get_cluster_from_docker_head(self, spill_dir = "/data"):
+def get_cluster_from_docker_head(spill_dir = "/data"):
     import socket
     self_ip = socket.gethostbyname(socket.gethostname())
     ray.init("ray://" + self_ip + ":10001")
     private_ips = [name.split(":")[1] for name in ray.cluster_resources().keys() if "node" in name]
     cpu_count = ray.cluster_resources()["CPU"] // len(private_ips)
     return EC2Cluster([None] * len(private_ips), private_ips, [None] * len(private_ips), cpu_count, spill_dir, docker_head_private_ip=self_ip)
```

## Comparing `pyquokka-0.2.6.dist-info/LICENSE` & `pyquokka-0.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyquokka-0.2.6.dist-info/METADATA` & `pyquokka-0.2.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquokka
-Version: 0.2.6
+Version: 0.2.7
 Summary: Quokka
 Author: Tony Wang
 Author-email: zihengw@stanford.edu
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `pyquokka-0.2.6.dist-info/RECORD` & `pyquokka-0.2.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 pyquokka/quokka_runtime.py,sha256=ADyM7i5KiJxERReBQdesm_kuYxGwPWccG5RiK4ywMK0,19755
 pyquokka/redis.conf,sha256=Hk0GU-BnDDpMZ6Gmit1-Ct_iyO7ttCvzyfz5PLFVkJY,93718
 pyquokka/sql_utils.py,sha256=1vWMrQft37so5KtOLlsqLk8MpaFB0XO9Ib9XwQEuw90,16471
 pyquokka/state.py,sha256=wGt5uh_ZS-xV-HqVgWmdTZUnQoabpvSOHiQXOejg7L4,2371
 pyquokka/tables.py,sha256=58vsFPBKOEKZ-7Ei7GbhXKsAgw6JguwdfQhayRJrjEI,11695
 pyquokka/target_info.py,sha256=RVldOYWGgxv9YXMSN3J3S-UbSEJxeUMoYY1LcHT3edg,2351
 pyquokka/task.py,sha256=_O_itxDxzXnjojys8___CKSaApTnEpUxVrAvWaU-AVI,5752
-pyquokka/utils.py,sha256=lkexwLiEKPbUMOEXyE1XtpUrDs0U7ilF5xwJVZyQA2o,29805
+pyquokka/utils.py,sha256=cECTzW_EKCcOja-BAWRP-4XBzrPGGZUhMqdekcSUwW4,29799
 pyquokka/windowtypes.py,sha256=zPh9QgwSQ3E00eNQM8jk2iQZNMuzAQ3eoaFDm1H5NGk,4081
-pyquokka-0.2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pyquokka-0.2.6.dist-info/METADATA,sha256=lYdk78FfHmUYsz9ikyincdBP2_4GD4QHLeQ9gsgI1WY,1040
-pyquokka-0.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyquokka-0.2.6.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
-pyquokka-0.2.6.dist-info/RECORD,,
+pyquokka-0.2.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pyquokka-0.2.7.dist-info/METADATA,sha256=4ijqKpojmvB4u2VZ4QxX0rtogwDFoCj2nAa3Kxz-H1k,1040
+pyquokka-0.2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyquokka-0.2.7.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
+pyquokka-0.2.7.dist-info/RECORD,,
```

