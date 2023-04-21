# Comparing `tmp/kafka_slurm_agent-1.0.0-py3-none-any.whl.zip` & `tmp/kafka_slurm_agent-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 29769 bytes, number of entries: 18
+Zip file size: 29840 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      164 b- defN 21-Nov-07 16:55 kafka_slurm_agent/__init__.py
 -rw-rw-r--  2.0 unx     4083 b- defN 23-Jan-18 12:51 kafka_slurm_agent/cluster_agent.py
 -rw-rw-r--  2.0 unx     4929 b- defN 22-Oct-13 22:44 kafka_slurm_agent/command.py
 -rw-rw-r--  2.0 unx    11318 b- defN 21-Nov-04 13:26 kafka_slurm_agent/config_module.py
--rw-rw-r--  2.0 unx    26970 b- defN 23-Jan-18 12:51 kafka_slurm_agent/kafka_modules.py
+-rw-rw-r--  2.0 unx    27136 b- defN 23-Apr-21 08:14 kafka_slurm_agent/kafka_modules.py
 -rw-rw-r--  2.0 unx     4686 b- defN 22-Oct-21 17:16 kafka_slurm_agent/monitor_agent.py
 -rw-rw-r--  2.0 unx     7406 b- defN 22-Oct-21 21:16 kafka_slurm_agent/runner.py
 -rw-rw-r--  2.0 unx     3463 b- defN 22-Oct-28 08:05 kafka_slurm_agent/worker_agent.py
--rwxrwxr-x  2.0 unx     2007 b- defN 22-Oct-21 21:14 kafka_slurm_agent-1.0.0.data/data/cluster_agent
--rw-rw-r--  2.0 unx     2016 b- defN 23-Jan-18 12:50 kafka_slurm_agent-1.0.0.data/data/kafkaslurm_cfg.py__
--rwxrwxr-x  2.0 unx     1991 b- defN 22-Oct-21 21:00 kafka_slurm_agent-1.0.0.data/data/monitor_agent
--rwxrwxr-x  2.0 unx     2011 b- defN 22-Oct-21 20:58 kafka_slurm_agent-1.0.0.data/data/worker_agent
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jan-18 12:53 kafka_slurm_agent-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2069 b- defN 23-Jan-18 12:53 kafka_slurm_agent-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       86 b- defN 23-Jan-18 12:53 kafka_slurm_agent-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       62 b- defN 23-Jan-18 12:53 kafka_slurm_agent-1.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Jan-18 12:53 kafka_slurm_agent-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1673 b- defN 23-Jan-18 12:53 kafka_slurm_agent-1.0.0.dist-info/RECORD
-18 files, 86309 bytes uncompressed, 26969 bytes compressed:  68.8%
+-rwxrwxr-x  2.0 unx     2007 b- defN 22-Oct-21 21:14 kafka_slurm_agent-1.0.1.data/data/cluster_agent
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Apr-21 08:14 kafka_slurm_agent-1.0.1.data/data/kafkaslurm_cfg.py__
+-rwxrwxr-x  2.0 unx     1991 b- defN 22-Oct-21 21:00 kafka_slurm_agent-1.0.1.data/data/monitor_agent
+-rwxrwxr-x  2.0 unx     2011 b- defN 22-Oct-21 20:58 kafka_slurm_agent-1.0.1.data/data/worker_agent
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-21 08:16 kafka_slurm_agent-1.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2069 b- defN 23-Apr-21 08:16 kafka_slurm_agent-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       86 b- defN 23-Apr-21 08:16 kafka_slurm_agent-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       62 b- defN 23-Apr-21 08:16 kafka_slurm_agent-1.0.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-21 08:16 kafka_slurm_agent-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Apr-21 08:16 kafka_slurm_agent-1.0.1.dist-info/RECORD
+18 files, 86542 bytes uncompressed, 27040 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -18,38 +18,38 @@
 
 Filename: kafka_slurm_agent/runner.py
 Comment: 
 
 Filename: kafka_slurm_agent/worker_agent.py
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.data/data/cluster_agent
+Filename: kafka_slurm_agent-1.0.1.data/data/cluster_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.data/data/kafkaslurm_cfg.py__
+Filename: kafka_slurm_agent-1.0.1.data/data/kafkaslurm_cfg.py__
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.data/data/monitor_agent
+Filename: kafka_slurm_agent-1.0.1.data/data/monitor_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.data/data/worker_agent
+Filename: kafka_slurm_agent-1.0.1.data/data/worker_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.dist-info/LICENSE
+Filename: kafka_slurm_agent-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.dist-info/METADATA
+Filename: kafka_slurm_agent-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.dist-info/WHEEL
+Filename: kafka_slurm_agent-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.dist-info/entry_points.txt
+Filename: kafka_slurm_agent-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.dist-info/top_level.txt
+Filename: kafka_slurm_agent-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.0.dist-info/RECORD
+Filename: kafka_slurm_agent-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kafka_slurm_agent/kafka_modules.py

```diff
@@ -350,15 +350,18 @@
         tfile = tempfile.NamedTemporaryFile(dir=config['SHARED_TMP'], mode="w+", delete=False)
         json.dump(job_config, tfile)
         tfile.flush()
         return tfile.name
 
     def get_runner_batch_cmd(self, input_job_id, script, msg=None, job_id=None):
         # TODO - override the method according to your needs
-        cmd = os.path.join(config['PREFIX'], 'venv', 'bin', 'python') + ' ' + script + ' ' + str(input_job_id)
+        if 'PYTHON_VENV' in config:
+            cmd = os.path.join(config['PYTHON_VENV'], 'bin', 'python') + ' ' + script + ' ' + str(input_job_id)
+        else:
+            cmd = os.path.join(config['PREFIX'], 'venv', 'bin', 'python') + ' ' + script + ' ' + str(input_job_id)
         time_out = None
         if msg:
             if 'TIMEOUT' in msg['slurm_pars']:
                 time_out = int(msg['slurm_pars']['TIMEOUT'])
             cmd += ' cfg_file=' + self.write_job_config(msg)
         if job_id:
             cmd += ' job_id=' + str(job_id)
```

## Comparing `kafka_slurm_agent-1.0.0.data/data/cluster_agent` & `kafka_slurm_agent-1.0.1.data/data/cluster_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.0.data/data/kafkaslurm_cfg.py__` & `kafka_slurm_agent-1.0.1.data/data/kafkaslurm_cfg.py__`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 MONITOR_AGENT_NEW_GROUP = socket.gethostname() + '_monitor_agent_new'
 WORKER_NAME = 'my_worker_' + socket.gethostname()
 WORKER_AGENT_CLASS = 'my_worker_agent.MyWorkerAgent'
 WORKER_AGENT_MAX_WORKERS = 4
 WORKER_JOB_TIMEOUT = 360000 # in seconds
 CLUSTER_JOB_TIMEOUT = 360000 # in seconds
 HEARTBEAT_INTERVAL = 300.0 # in seconds, set to 0 to disable heartbeat
+#PYTHON_VENV = # if set overrides the default PREFIX/venv location
 
 # / The parameters below are used to run a command directly on Kafka to query for new and waiting jobs
 BOOTSTRAP_SERVERS_LOCAL = 'localhost:9092'
 KAFKA_HOME = '/opt/kafka'
 # /
 
 #POLL_INTERVAL = 20.0,
```

## Comparing `kafka_slurm_agent-1.0.0.data/data/monitor_agent` & `kafka_slurm_agent-1.0.1.data/data/monitor_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.0.data/data/worker_agent` & `kafka_slurm_agent-1.0.1.data/data/worker_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.0.dist-info/LICENSE` & `kafka_slurm_agent-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.0.dist-info/METADATA` & `kafka_slurm_agent-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-slurm-agent
-Version: 1.0.0
+Version: 1.0.1
 Summary: The Kafka Slurm Agent is a tool for submitting computing tasks to the Slurm queues on multiple clusters. It uses Kafka to asynchronously communicate with an agent installed on the cluster.It contains a monitoring tool and a job submitter.
 Home-page: https://github.com/prubach/kafka-slurm-agent
 Author: Paweł Rubach
 Author-email: pawel.rubach@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `kafka_slurm_agent-1.0.0.dist-info/RECORD` & `kafka_slurm_agent-1.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kafka_slurm_agent/__init__.py,sha256=Z443N5Cv9w8TrZFQ5WxjHvLpZBks7iokln6SLAsEk74,164
 kafka_slurm_agent/cluster_agent.py,sha256=bdnMxGvnJPzVfZAR9YH7u5XVc9vxV7B7ZikAMp7ULwI,4083
 kafka_slurm_agent/command.py,sha256=lAFVoo1V15SdpBuLBac8mmTmILxfHV9oGxXw0rcLZJw,4929
 kafka_slurm_agent/config_module.py,sha256=1JnZTmvrj08tdprZROST7RkYp2UlCRL3CdgRre-mYKs,11318
-kafka_slurm_agent/kafka_modules.py,sha256=j_LKjH65UlAhySLTdTN3hhvRbZ5XDPaEDOtMyAz5DL0,26970
+kafka_slurm_agent/kafka_modules.py,sha256=bhUf-LI9qz6uBw463gYb74WWHFTbImTZprxKsZaNVL4,27136
 kafka_slurm_agent/monitor_agent.py,sha256=UVAQqAJT8Cpzx1-V-mzXkTJ0vULOhzTL-7wIiKKAlPM,4686
 kafka_slurm_agent/runner.py,sha256=3xKS_DUtbFXdmFC17qwXKpuqWzeW6GRFTA_H9tgOWe8,7406
 kafka_slurm_agent/worker_agent.py,sha256=qS4ymnvnfdLozzj88Wf3CV1IaAfmdulWGFZXJmrnEic,3463
-kafka_slurm_agent-1.0.0.data/data/cluster_agent,sha256=1tsn3OhOaReuH42EkkotbpO2TRjfiemKazr5g-c_JAE,2007
-kafka_slurm_agent-1.0.0.data/data/kafkaslurm_cfg.py__,sha256=TA5HUgpMMI5VvAJ9HT1XnFO9SmuVYTxwzHikaXlEuSM,2016
-kafka_slurm_agent-1.0.0.data/data/monitor_agent,sha256=nzf6GYqA45xaPkOSrMKLhZXLmqvrEPJ-lcgI_PRp1VQ,1991
-kafka_slurm_agent-1.0.0.data/data/worker_agent,sha256=s6mcqKJLJlSxclFzWv6FbnBRHQtYaNCOWotLaKQTG7o,2011
-kafka_slurm_agent-1.0.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-kafka_slurm_agent-1.0.0.dist-info/METADATA,sha256=Tm2FAFupJrWjyvoMaATfJcOBOcjFHACv897u2Z09RLE,2069
-kafka_slurm_agent-1.0.0.dist-info/WHEEL,sha256=BLqeAEDufjK4U17YM0Cbp3qk07uloSGcRE6RzzoGn5o,86
-kafka_slurm_agent-1.0.0.dist-info/entry_points.txt,sha256=pZiTuEXiq16U2FWuWE49x2_2xLoxtgGlzB9Mc389kmg,62
-kafka_slurm_agent-1.0.0.dist-info/top_level.txt,sha256=ot5Idwc6vKowyJdvWhOZepKDqtzCTFN52Oe7iIrtfVQ,18
-kafka_slurm_agent-1.0.0.dist-info/RECORD,,
+kafka_slurm_agent-1.0.1.data/data/cluster_agent,sha256=1tsn3OhOaReuH42EkkotbpO2TRjfiemKazr5g-c_JAE,2007
+kafka_slurm_agent-1.0.1.data/data/kafkaslurm_cfg.py__,sha256=YSLNEz9u_jP7xkJt4A0IebdfSs7YFg3DbqwEFHy1dis,2083
+kafka_slurm_agent-1.0.1.data/data/monitor_agent,sha256=nzf6GYqA45xaPkOSrMKLhZXLmqvrEPJ-lcgI_PRp1VQ,1991
+kafka_slurm_agent-1.0.1.data/data/worker_agent,sha256=s6mcqKJLJlSxclFzWv6FbnBRHQtYaNCOWotLaKQTG7o,2011
+kafka_slurm_agent-1.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+kafka_slurm_agent-1.0.1.dist-info/METADATA,sha256=n94bGx94LOwVDNPm-J_16fTKfmHNuo2EKayzuEMnZDU,2069
+kafka_slurm_agent-1.0.1.dist-info/WHEEL,sha256=yYV-D90-NW-UlZINH_90hGjz3BXXubiZbvu2N2r2uFU,86
+kafka_slurm_agent-1.0.1.dist-info/entry_points.txt,sha256=pZiTuEXiq16U2FWuWE49x2_2xLoxtgGlzB9Mc389kmg,62
+kafka_slurm_agent-1.0.1.dist-info/top_level.txt,sha256=ot5Idwc6vKowyJdvWhOZepKDqtzCTFN52Oe7iIrtfVQ,18
+kafka_slurm_agent-1.0.1.dist-info/RECORD,,
```

