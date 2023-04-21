# Comparing `tmp/pyquokka-0.2.5-py3-none-any.whl.zip` & `tmp/pyquokka-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 275647 bytes, number of entries: 34
+Zip file size: 275662 bytes, number of entries: 34
 -rw-rw-r--  2.0 unx      256 b- defN 23-Apr-15 21:15 pyquokka/__init__.py
 -rw-rw-r--  2.0 unx     4291 b- defN 23-Apr-19 05:39 pyquokka/catalog.py
 -rw-rw-r--  2.0 unx      372 b- defN 23-Apr-12 19:11 pyquokka/common_startup.sh
 -rw-rw-r--  2.0 unx    28239 b- defN 23-Apr-16 23:17 pyquokka/coordinator.py
 -rw-rw-r--  2.0 unx    48229 b- defN 23-Apr-16 23:13 pyquokka/core.py
 -rw-rw-r--  2.0 unx    48426 b- defN 23-Apr-19 05:39 pyquokka/dataset.py
 -rw-rw-r--  2.0 unx    96482 b- defN 23-Apr-19 18:58 pyquokka/datastream.py
@@ -22,15 +22,15 @@
 -rw-rw-r--  2.0 unx    19755 b- defN 23-Apr-14 04:33 pyquokka/quokka_runtime.py
 -rw-rw-r--  2.0 unx    93718 b- defN 22-Oct-04 03:50 pyquokka/redis.conf
 -rw-rw-r--  2.0 unx    16471 b- defN 23-Mar-27 22:47 pyquokka/sql_utils.py
 -rw-rw-r--  2.0 unx     2371 b- defN 22-Jul-15 20:59 pyquokka/state.py
 -rw-rw-r--  2.0 unx    11695 b- defN 23-Apr-09 03:05 pyquokka/tables.py
 -rw-rw-r--  2.0 unx     2351 b- defN 23-Jan-28 04:17 pyquokka/target_info.py
 -rw-rw-r--  2.0 unx     5752 b- defN 23-Mar-20 21:30 pyquokka/task.py
--rw-rw-r--  2.0 unx    29749 b- defN 23-Apr-20 23:44 pyquokka/utils.py
+-rw-rw-r--  2.0 unx    29805 b- defN 23-Apr-21 00:03 pyquokka/utils.py
 -rw-rw-r--  2.0 unx     4081 b- defN 23-Jan-25 17:17 pyquokka/windowtypes.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-20 23:45 pyquokka-0.2.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-20 23:45 pyquokka-0.2.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 23:45 pyquokka-0.2.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-20 23:45 pyquokka-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2659 b- defN 23-Apr-20 23:45 pyquokka-0.2.5.dist-info/RECORD
-34 files, 981484 bytes uncompressed, 271505 bytes compressed:  72.3%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1040 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2659 b- defN 23-Apr-21 00:04 pyquokka-0.2.6.dist-info/RECORD
+34 files, 981540 bytes uncompressed, 271520 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -81,23 +81,23 @@
 
 Filename: pyquokka/utils.py
 Comment: 
 
 Filename: pyquokka/windowtypes.py
 Comment: 
 
-Filename: pyquokka-0.2.5.dist-info/LICENSE
+Filename: pyquokka-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: pyquokka-0.2.5.dist-info/METADATA
+Filename: pyquokka-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: pyquokka-0.2.5.dist-info/WHEEL
+Filename: pyquokka-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: pyquokka-0.2.5.dist-info/top_level.txt
+Filename: pyquokka-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pyquokka-0.2.5.dist-info/RECORD
+Filename: pyquokka-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyquokka/utils.py

```diff
@@ -40,15 +40,18 @@
             self.leader_public_ip = docker_head_private_ip
         else:
             self.leader_public_ip = self.public_ips[0]
         self.leader_private_ip = self.private_ips[0]
         print("EC2 Cluster leader public IP", self.leader_public_ip, "private IP", self.leader_private_ip)
         pyquokka_loc = pyquokka.__file__.replace("__init__.py","")
         # connect to that ray cluster
-        ray.init(address='ray://' + str(self.leader_public_ip) + ':10001', 
+        if docker_head_private_ip is not None:
+            return 
+        else:
+            ray.init(address='ray://' + str(self.leader_public_ip) + ':10001', 
                  runtime_env={"py_modules":[pyquokka_loc]})
     
     def to_json(self, output = "cluster.json"):
 
         """
         Creates JSON representation of this cluster that can be used to connect to the cluster again.
 
@@ -132,14 +135,22 @@
         if self.redis_process is not None:
             self.redis_process.kill()
 
 
 def execute_script(key_location, x):
     return os.system("ssh -oStrictHostKeyChecking=no -i {} ubuntu@{} 'bash -s' < {}".format(key_location, x, pyquokka.__file__.replace("__init__.py", "common_startup.sh")))
 
+def get_cluster_from_docker_head(self, spill_dir = "/data"):
+    import socket
+    self_ip = socket.gethostbyname(socket.gethostname())
+    ray.init("ray://" + self_ip + ":10001")
+    private_ips = [name.split(":")[1] for name in ray.cluster_resources().keys() if "node" in name]
+    cpu_count = ray.cluster_resources()["CPU"] // len(private_ips)
+    return EC2Cluster([None] * len(private_ips), private_ips, [None] * len(private_ips), cpu_count, spill_dir, docker_head_private_ip=self_ip)
+
 class QuokkaClusterManager:
 
     def __init__(self, key_name = None, key_location = None, security_group= None) -> None:
         
         """
         Create a QuokkaClusterManager object. This object is used to create Ray clusters on AWS EC2 configured with Quokka or connecting to existing Ray clusters.
         This requires you to have an AWS key pair for logging into instances. 
@@ -544,23 +555,14 @@
 
         z = os.system("ssh -oStrictHostKeyChecking=no -i " + self.key_location + " ubuntu@" + public_ips[0] + " 'bash -s' < " + pyquokka.__file__.replace("__init__.py","leader_startup.sh"))
         print(z)
 
         self.copy_and_launch_flight(public_ips)
         return EC2Cluster(public_ips, private_ips, instance_ids, cpu_count, spill_dir)
 
-
-    def get_cluster_from_docker_head(self, spill_dir = "/data"):
-        import socket
-        self_ip = socket.gethostbyname(socket.gethostname())
-        ray.init("ray://" + self_ip + ":10001")
-        private_ips = [name.split(":")[1] for name in ray.cluster_resources().keys() if "node" in name]
-        cpu_count = ray.cluster_resources()["CPU"] // len(private_ips)
-        return EC2Cluster([None] * len(private_ips), private_ips, [None] * len(private_ips), cpu_count, spill_dir, docker_head_private_ip=self_ip)
-
     def get_cluster_from_docker_cluster(self, path_to_yaml, spill_dir = "/data", cluster_name = None):
 
         """
         """
 
         import yaml
         ec2 = boto3.client("ec2")
```

## Comparing `pyquokka-0.2.5.dist-info/LICENSE` & `pyquokka-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyquokka-0.2.5.dist-info/METADATA` & `pyquokka-0.2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquokka
-Version: 0.2.5
+Version: 0.2.6
 Summary: Quokka
 Author: Tony Wang
 Author-email: zihengw@stanford.edu
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `pyquokka-0.2.5.dist-info/RECORD` & `pyquokka-0.2.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 pyquokka/quokka_runtime.py,sha256=ADyM7i5KiJxERReBQdesm_kuYxGwPWccG5RiK4ywMK0,19755
 pyquokka/redis.conf,sha256=Hk0GU-BnDDpMZ6Gmit1-Ct_iyO7ttCvzyfz5PLFVkJY,93718
 pyquokka/sql_utils.py,sha256=1vWMrQft37so5KtOLlsqLk8MpaFB0XO9Ib9XwQEuw90,16471
 pyquokka/state.py,sha256=wGt5uh_ZS-xV-HqVgWmdTZUnQoabpvSOHiQXOejg7L4,2371
 pyquokka/tables.py,sha256=58vsFPBKOEKZ-7Ei7GbhXKsAgw6JguwdfQhayRJrjEI,11695
 pyquokka/target_info.py,sha256=RVldOYWGgxv9YXMSN3J3S-UbSEJxeUMoYY1LcHT3edg,2351
 pyquokka/task.py,sha256=_O_itxDxzXnjojys8___CKSaApTnEpUxVrAvWaU-AVI,5752
-pyquokka/utils.py,sha256=8gDI1Lbab0TR8hL4IKMpEsX-YddGcbTPS-KEgLjKR4o,29749
+pyquokka/utils.py,sha256=lkexwLiEKPbUMOEXyE1XtpUrDs0U7ilF5xwJVZyQA2o,29805
 pyquokka/windowtypes.py,sha256=zPh9QgwSQ3E00eNQM8jk2iQZNMuzAQ3eoaFDm1H5NGk,4081
-pyquokka-0.2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pyquokka-0.2.5.dist-info/METADATA,sha256=NIsFHBtrKkDr__ULXVirD1UzL8twuV1trDs9s2ozCL8,1040
-pyquokka-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyquokka-0.2.5.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
-pyquokka-0.2.5.dist-info/RECORD,,
+pyquokka-0.2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pyquokka-0.2.6.dist-info/METADATA,sha256=lYdk78FfHmUYsz9ikyincdBP2_4GD4QHLeQ9gsgI1WY,1040
+pyquokka-0.2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyquokka-0.2.6.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
+pyquokka-0.2.6.dist-info/RECORD,,
```

