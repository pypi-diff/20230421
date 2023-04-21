# Comparing `tmp/pye2-0.3.5.tar.gz` & `tmp/pye2-0.3.6.tar.gz`

## Comparing `pye2-0.3.5.tar` & `pye2-0.3.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.3.5/TODOs.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.3.5/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pye2-0.3.5/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.3.5/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/__init__.py
--rw-r--r--   0        0        0    21169 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/logger.py
--rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/pipeline.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/default/__init__.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.3.5/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/.example_env
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/attach_example.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/ex1.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/hello.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/remote_exec.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.3.5/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.3.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.3.5/LICENSE
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pye2-0.3.5/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pye2-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 pye2-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.3.6/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.3.6/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pye2-0.3.6/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.3.6/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.3.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    22284 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.3.6/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/.example_env
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/ex1.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/hello.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.3.6/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.3.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.3.6/LICENSE
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pye2-0.3.6/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pye2-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 pye2-0.3.6/PKG-INFO
```

### Comparing `pye2-0.3.5/.github/workflows/python-publish.yml` & `pye2-0.3.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/base/__init__.py` & `pye2-0.3.6/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/base/generic_session.py` & `pye2-0.3.6/PyE2/base/generic_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,19 +47,19 @@
       },
       "PAYLOADS_CHANNEL": {
           "TOPIC": "lummetry/payloads"
       },
       "QOS": 0
   }
 
-  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, log=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
+  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
     """
-  A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
-  A Session manages `Pipelines` and handles all messages received from the communication server.
-  The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
+    A Session is a connection to a communication server which provides the channel to interact with nodes from the AiXpand network.
+    A Session manages `Pipelines` and handles all messages received from the communication server.
+    The Session handles all callbacks that are user-defined and passed as arguments in the API calls.  
 
     Parameters
     ----------
     host : str
         The hostname of the server
     port : int
         The port
@@ -71,28 +71,33 @@
         The name of this connection, used to identify owned pipelines on a specific AiXpand node.
         The name will be used as `INITIATOR_ID` and `SESSION_ID` when communicating with AiXp nodes, by default 'pySDK'
     config : dict, optional
         Configures the names of the channels this session will connect to.
         If using a Mqtt server, these channels are in fact topics.
         Modify this if you are absolutely certain of what you are doing.
         By default {}
+    filter_workers: list, optional
+        If set, process the messages that come only from the nodes from this list. 
+        Defaults to None
     log : Logger, optional
         A logger object which implements basic logging functionality and some other utils stuff. Can be ignored for now.
         In the future, the documentation for the Logger base class will be available and developers will be able to use
         custom-made Loggers. 
-    on_notification : Callable[[Session, dict], None], optional
+    on_notification : Callable[[Session, str, dict], None], optional
         Callback that handles notifications received from this network. 
-        As arguments, it has a reference to this Pipeline object, along with the payload itself. 
+        As arguments, it has a reference to this Session object, the node name and the notification payload. 
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
         This callback will be called when there are notifications related to the node itself, e.g. when the node runs
         low on memory. 
         Defaults to None.
-    on_heartbeat : Callable[[Session, dict], None], optional
-        Callback that handles heartbeats received from this network, by default None
+    on_heartbeat : Callable[[Session, str, dict], None], optional
+        Callback that handles heartbeats received from this network.
+        As arguments, it has a reference to this Session object, the node name and the heartbeat payload.
+        Defaults to None.
     silent : bool, optional
         This flag will disable debug logs, set to 'False` for a more verbose log, by default True
     """
     if log is None:
       log = Logger()
 
     super(GenericSession, self).__init__()
@@ -101,14 +106,17 @@
 
     # maybe read config from file?
     self._config = {**self.default_config, **config}
     self.log = log
     self.name = name
 
     self._online_boxes = {}
+    self._last_seen_boxes = {}
+    self.online_timeout = 60
+    self.filter_workers = filter_workers
 
     self._fill_config(host, port, user, pwd, name)
 
     self.custom_on_heartbeat = on_heartbeat
     self.custom_on_notification = on_notification
 
     self.on_payload = self._on_payload_default
@@ -153,70 +161,93 @@
   def _parse_message(self, dict_msg: dict):
     formatter = self.formatter_wrapper \
         .get_required_formatter_from_payload(dict_msg)
     if formatter is not None:
       dict_msg = formatter.decode_output(dict_msg)
     return dict_msg
 
+  def _maybe_ignore_message(self, e2id):
+    return self.filter_workers is not None and e2id not in self.filter_workers
+
+  def _track_online_node(self, e2id):
+    self._last_seen_boxes[e2id] = tm()
+    return
+
   def _on_heartbeat_default(self, dict_msg: dict):
+    # extract relevant data from the message
     msg_eeid = dict_msg['EE_ID']
     msg_active_configs = dict_msg['CONFIG_STREAMS']
 
     # default action
-    # TODO: print stuff
-    self.D("Received hb from: {}".format(msg_eeid))
+    self._track_online_node(msg_eeid)
     self._online_boxes[msg_eeid] = {
         config['NAME']: config for config in msg_active_configs}
 
-    # call the pipeline defined callbacks, if any
-    for pipeline, callback in self.heartbeat_pipeline_callbacks:
-      if msg_eeid == pipeline.e2id:
-        callback(pipeline, dict_msg)
+    if self._maybe_ignore_message(msg_eeid):
+      return
+
+    self.D("Received hb from: {}".format(msg_eeid))
 
     # call the custom callback, if defined
     if self.custom_on_heartbeat is not None:
-      self.custom_on_heartbeat(self, dict_msg)
+      self.custom_on_heartbeat(self, msg_eeid, dict_msg)
 
     return
 
   def _on_notification_default(self, dict_msg: dict):
+    # extract relevant data from the message
     msg_eeid = dict_msg['EE_ID']
     msg_stream = dict_msg.get('STREAM_NAME', None)
     notification_type = dict_msg.get("NOTIFICATION_TYPE")
     notification = dict_msg.get("NOTIFICATION")
 
+    # default action
+    self._track_online_node(msg_eeid)
+
+    if self._maybe_ignore_message(msg_eeid):
+      return
+
+    color = None
+    if notification_type != "NORMAL":
+      color = 'r'
+    self.D("Received notification {} from <{}/{}>: {}"
+           .format(
+              notification_type,
+              msg_eeid,
+              msg_stream,
+              notification),
+           color=color)
+
     # call the pipeline defined callbacks, if any
     for pipeline, callback in self.notification_pipeline_callbacks:
       if msg_eeid == pipeline.e2id and msg_stream == pipeline.name:
         callback(pipeline, dict_msg)
 
     # call the custom callback, if defined
     if self.custom_on_notification is not None:
-      self.custom_on_notification(self, dict_msg)
-
-    # call default action on notif
-    # TODO: maybe print stuff
-    color = None
-    if notification_type != "NORMAL":
-      color = 'r'
-    self.D("Received notification {} from <{}/{}>: {}".format(notification_type,
-           msg_eeid, msg_stream, notification), color=color)
+      self.custom_on_notification(self, msg_eeid, dict_msg)
 
     return
 
   # TODO: maybe convert dict_msg to Payload object
   #       also maybe strip the dict from useless info for the user of the sdk
   #       Add try-except + sleep
   def _on_payload_default(self, dict_msg: dict) -> None:
-    msg_stream = dict_msg.get('STREAM', None)
+    # extract relevant data from the message
     msg_eeid = dict_msg['EE_ID']
+    msg_stream = dict_msg.get('STREAM', None)
     msg_signature = dict_msg.get('SIGNATURE', '').upper()
     msg_instance = dict_msg.get('INSTANCE_ID', None)
     msg_data = dict_msg
 
+    self._track_online_node(msg_eeid)
+
+    if self._maybe_ignore_message(msg_eeid):
+      return
+
     for pipeline, callback in self.payload_pipeline_callbacks:
       if msg_eeid == pipeline.e2id and msg_stream == pipeline.name:
         callback(pipeline, msg_signature, msg_instance, msg_data)
 
     for pipeline, signature, instance, callback in self.payload_instance_callbacks:
       if msg_eeid == pipeline.e2id and msg_stream == pipeline.name and msg_signature == signature and msg_instance == instance:
         callback(pipeline, msg_data)
@@ -344,15 +375,16 @@
         Name of the AiXpand node that will handle this pipeline.  
     name : str
         Name of the pipeline. This is good to be kept unique, as it allows multiple parties to overwrite each others configurations.
     data_source : str
         This is the name of the DCT plugin, which resembles the desired functionality of the acquisition.
     on_data : Callable[[Pipeline, str, str, dict], None]
         Callback that handles messages received from any plugin instance. 
-        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+        As arguments, it has a reference to this Pipeline object, the signature and the instance of the plugin
+        that sent the message and the payload itself.
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
     plugins : list
         List of dictionaries which contain the configurations of each plugin instance that is desired to run on the box. Defaults to []. Should be left [], and instances should be created with the api.
     config : dict, optional
         This is the dictionary that contains the configuration of the acquisition source, by default {}
     on_notification : Callable[[Pipeline, dict], None], optional
@@ -433,15 +465,15 @@
 
     Returns
     -------
     list
         List of names of all the AiXp nodes that are considered online
 
     """
-    return list(self._online_boxes.keys())
+    return [k for k, v in self._last_seen_boxes.items() if tm() - v > self.online_timeout]
 
   def get_active_pipelines(self, e2id):
     """
     Get a dictionary with all the pipelines that are active on this AiXp node
 
     Parameters
     ----------
@@ -450,15 +482,15 @@
 
     Returns
     -------
     dict
         The key is the name of the pipeline, and the value is the entire config dictionary of that pipeline.
 
     """
-    return self._online_boxes.get(e2id, None)
+    return self._online_boxes.get(e2id, None) if e2id in self.get_active_nodes() else None
 
   def attach_to_pipeline(self, e2id, pipeline_name, on_data, on_notification=None, max_wait_time=0, **kwargs) -> Pipeline:
     """
     Create a Pipeline object and attach to an existing pipeline on an AiXpand node.
     Useful when one wants to treat an existing pipeline as one of his own,
     or when one wants to attach callbacks to various events (on_data, on_notification).
 
@@ -485,15 +517,16 @@
     ----------
     e2id : str
         Name of the AiXpand node that handles this pipeline.  
     pipeline_name : str
         Name of the existing pipeline.
     on_data : Callable[[Pipeline, str, str, dict], None]
         Callback that handles messages received from any plugin instance. 
-        As arguments, it has a reference to this Pipeline object, along with the payload itself.
+        As arguments, it has a reference to this Pipeline object, the signature and the instance of the plugin
+        that sent the message and the payload itself.
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
     on_notification : Callable[[Pipeline, dict], None], optional
         Callback that handles notifications received from any plugin instance. 
         As arguments, it has a reference to this Pipeline object, along with the payload itself. 
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
@@ -519,15 +552,15 @@
     _start = tm()
     while (tm() - _start) < max_wait_time:
       avail_workers = self.get_active_nodes()
       if e2id in avail_workers:
         break
       sleep(0.1)
 
-    if e2id not in self._online_boxes:
+    if e2id not in self.get_active_nodes():
       raise Exception("Unable to attach to pipeline. Node does not exist")
 
     if pipeline_name not in self._online_boxes[e2id]:
       raise Exception("Unable to attach to pipeline. Pipeline does not exist")
 
     pipeline_config = {
         k.lower(): v for k, v in self._online_boxes[e2id][pipeline_name].items()}
```

### Comparing `pye2-0.3.5/PyE2/base/logger.py` & `pye2-0.3.6/PyE2/base/logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/base/pipeline.py` & `pye2-0.3.6/PyE2/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/base/payload/payload.py` & `pye2-0.3.6/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/comm/__init__.py` & `pye2-0.3.6/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/comm/amqp_wrapper.py` & `pye2-0.3.6/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/comm/mqtt_wrapper.py` & `pye2-0.3.6/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/const/__init__.py` & `pye2-0.3.6/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/const/base.py` & `pye2-0.3.6/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/const/comms.py` & `pye2-0.3.6/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/const/heartbeat.py` & `pye2-0.3.6/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/const/misc.py` & `pye2-0.3.6/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/const/payload.py` & `pye2-0.3.6/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/default/mqtt_session.py` & `pye2-0.3.6/PyE2/default/mqtt_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from ..comm import MQTTWrapper
 from ..base import GenericSession
 
 
 # TODO: implement send_command, send_payload,
 #       to be used by the Pipeline class
 class MqttSession(GenericSession):
-  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, log=None, on_notification=None, on_heartbeat=None, silent=False, **kwargs) -> None:
-    super(MqttSession, self).__init__(host=host, port=port, user=user, pwd=pwd, name=name, config=config,
+  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_notification=None, on_heartbeat=None, silent=False, **kwargs) -> None:
+    super(MqttSession, self).__init__(host=host, port=port, user=user, pwd=pwd, name=name, config=config, filter_workers=filter_workers,
                                       log=log, on_notification=on_notification, on_heartbeat=on_heartbeat, silent=silent, **kwargs)
 
     self._payload_messages = deque()
     self._default_communicator = MQTTWrapper(
         log=self.log,
         config=self._config,
         send_channel_name=comm_ct.COMMUNICATION_CONFIG_CHANNEL,
```

### Comparing `pye2-0.3.5/PyE2/io_formatter/__init__.py` & `pye2-0.3.6/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/consts.py` & `pye2-0.3.6/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.3.6/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/base/__init__.py` & `pye2-0.3.6/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.3.6/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/default/__init__.py` & `pye2-0.3.6/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.3.6/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/default/cavi2.py` & `pye2-0.3.6/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.3.6/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/utils/code.py` & `pye2-0.3.6/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/PyE2/utils/code_exec.py` & `pye2-0.3.6/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/xperimental/attach_example.py` & `pye2-0.3.6/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/xperimental/ex1.py` & `pye2-0.3.6/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/xperimental/remote_exec.py` & `pye2-0.3.6/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/xperimental/decentralized/dedist_example.py` & `pye2-0.3.6/xperimental/decentralized/dedist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.3.6/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/.gitignore` & `pye2-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/LICENSE` & `pye2-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/README.md` & `pye2-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pye2-0.3.5/pyproject.toml` & `pye2-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.3.5/PKG-INFO` & `pye2-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyE2
-Version: 0.3.5
+Version: 0.3.6
 Summary: PyE2 is an SDK used to communicate with the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@global-technical.com>, Cristan Bleotiu <cristan.bleotiu@global-technical.com>, Andrei Ionut Damian <andrei.damian@lummetry.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

