# Comparing `tmp/pygqlc-3.0.5.tar.gz` & `tmp/pygqlc-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygqlc-3.0.5.tar", last modified: Wed Feb 22 19:53:39 2023, max compression
+gzip compressed data, was "pygqlc-3.1.0.tar", last modified: Fri Apr 21 18:46:37 2023, max compression
```

## Comparing `pygqlc-3.0.5.tar` & `pygqlc-3.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-02-22 19:53:39.428344 pygqlc-3.0.5/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-12-22 16:29:04.000000 pygqlc-3.0.5/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       30 2023-02-14 17:33:49.000000 pygqlc-3.0.5/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     4702 2023-02-22 19:53:39.428195 pygqlc-3.0.5/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     4434 2023-02-10 19:11:02.000000 pygqlc-3.0.5/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-02-22 19:53:39.426649 pygqlc-3.0.5/pygqlc/
--rw-r--r--   0 baruc      (501) staff       (20)    25484 2023-02-17 23:04:23.000000 pygqlc-3.0.5/pygqlc/GraphQLClient.py
--rw-r--r--   0 baruc      (501) staff       (20)     4941 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/MutationBatch.py
--rw-r--r--   0 baruc      (501) staff       (20)     2795 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/MutationParser.py
--rw-r--r--   0 baruc      (501) staff       (20)        0 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/QueryBatch.py
--rw-r--r--   0 baruc      (501) staff       (20)      761 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/QueryParser.py
--rw-r--r--   0 baruc      (501) staff       (20)      124 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/SubscriptionParser.py
--rw-r--r--   0 baruc      (501) staff       (20)      338 2023-02-14 17:35:44.000000 pygqlc-3.0.5/pygqlc/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      338 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-02-22 19:53:02.000000 pygqlc-3.0.5/pygqlc/__version__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-02-22 19:53:39.428019 pygqlc-3.0.5/pygqlc/helper_modules/
--rw-r--r--   0 baruc      (501) staff       (20)      362 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/helper_modules/Singleton.py
--rw-r--r--   0 baruc      (501) staff       (20)        0 2021-12-22 16:29:04.000000 pygqlc-3.0.5/pygqlc/helper_modules/__init__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-02-22 19:53:39.427713 pygqlc-3.0.5/pygqlc.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     4702 2023-02-22 19:53:39.000000 pygqlc-3.0.5/pygqlc.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      523 2023-02-22 19:53:39.000000 pygqlc-3.0.5/pygqlc.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-22 19:53:39.000000 pygqlc-3.0.5/pygqlc.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       48 2023-02-22 19:53:39.000000 pygqlc-3.0.5/pygqlc.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-10 19:03:06.000000 pygqlc-3.0.5/pygqlc.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)       81 2023-02-22 19:53:39.000000 pygqlc-3.0.5/pygqlc.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)        7 2023-02-22 19:53:39.000000 pygqlc-3.0.5/pygqlc.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-02-22 19:53:39.428390 pygqlc-3.0.5/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     1914 2023-02-22 19:53:02.000000 pygqlc-3.0.5/setup.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.524084 pygqlc-3.1.0/
+-rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-12-22 16:29:04.000000 pygqlc-3.1.0/LICENCE
+-rw-r--r--   0 baruc      (501) staff       (20)       30 2023-02-14 17:33:49.000000 pygqlc-3.1.0/MANIFEST.in
+-rw-r--r--   0 baruc      (501) staff       (20)     4702 2023-04-21 18:46:37.523876 pygqlc-3.1.0/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)     4434 2023-02-10 19:11:02.000000 pygqlc-3.1.0/README.md
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.521825 pygqlc-3.1.0/pygqlc/
+-rw-r--r--   0 baruc      (501) staff       (20)    25872 2023-04-21 18:46:19.000000 pygqlc-3.1.0/pygqlc/GraphQLClient.py
+-rw-r--r--   0 baruc      (501) staff       (20)     4941 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/MutationBatch.py
+-rw-r--r--   0 baruc      (501) staff       (20)     2795 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/MutationParser.py
+-rw-r--r--   0 baruc      (501) staff       (20)        0 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/QueryBatch.py
+-rw-r--r--   0 baruc      (501) staff       (20)      761 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/QueryParser.py
+-rw-r--r--   0 baruc      (501) staff       (20)      124 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/SubscriptionParser.py
+-rw-r--r--   0 baruc      (501) staff       (20)      338 2023-02-14 17:35:44.000000 pygqlc-3.1.0/pygqlc/__init__.py
+-rw-r--r--   0 baruc      (501) staff       (20)      338 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/__main__.py
+-rw-r--r--   0 baruc      (501) staff       (20)       22 2023-04-21 18:46:19.000000 pygqlc-3.1.0/pygqlc/__version__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.523633 pygqlc-3.1.0/pygqlc/helper_modules/
+-rw-r--r--   0 baruc      (501) staff       (20)      362 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/helper_modules/Singleton.py
+-rw-r--r--   0 baruc      (501) staff       (20)        0 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/helper_modules/__init__.py
+drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.523254 pygqlc-3.1.0/pygqlc.egg-info/
+-rw-r--r--   0 baruc      (501) staff       (20)     4702 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/PKG-INFO
+-rw-r--r--   0 baruc      (501) staff       (20)      523 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/SOURCES.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/dependency_links.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       48 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/entry_points.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-10 19:03:06.000000 pygqlc-3.1.0/pygqlc.egg-info/not-zip-safe
+-rw-r--r--   0 baruc      (501) staff       (20)       81 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/requires.txt
+-rw-r--r--   0 baruc      (501) staff       (20)        7 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/top_level.txt
+-rw-r--r--   0 baruc      (501) staff       (20)       38 2023-04-21 18:46:37.524141 pygqlc-3.1.0/setup.cfg
+-rw-r--r--   0 baruc      (501) staff       (20)     1914 2023-02-22 19:53:02.000000 pygqlc-3.1.0/setup.py
```

### Comparing `pygqlc-3.0.5/LICENCE` & `pygqlc-3.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pygqlc-3.0.5/PKG-INFO` & `pygqlc-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygqlc
-Version: 3.0.5
+Version: 3.1.0
 Summary: GraphQL API Client for python language
 Home-page: https://github.com/valiot/pygqlc
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: pygqlc
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `pygqlc-3.0.5/README.md` & `pygqlc-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pygqlc-3.0.5/pygqlc/GraphQLClient.py` & `pygqlc-3.1.0/pygqlc/GraphQLClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import requests
 import json
 import time
 import threading
 import websocket
+import traceback
 import pydash as py_
 from pygqlc.helper_modules.Singleton import Singleton
 from tenacity import (
-  retry, 
-  retry_if_result, 
-  stop_after_attempt, 
+  retry,
+  retry_if_result,
+  stop_after_attempt,
   wait_random
 )
 """
 This module has the general purpose of defining the GraphQLClient class
 and all its methods.
 
 GQLResponse (type variable): [data[field(string)], errors[message(string),
@@ -25,15 +26,15 @@
 GQL_WS_SUBPROTOCOL = "graphql-transport-ws"
 
 def is_ws_payloadErrors_msg(message):
   errors = py_.get(message, 'payload.errors')
   if (errors):
     return True
   return False
-  
+
 def is_ws_connection_init_msg(message):
   data = py_.get(message, 'payload.data', {})
   if not data:
     return False # may have an error, but is not connection init message
   keys = list(data.keys())
   if (len(keys) > 0):
     body = data[keys[0]]
@@ -100,15 +101,15 @@
   else:
     return default
 
 
 class GraphQLClient(metaclass=Singleton):
   """The GraphQLClient class follows the singleton design pattern. It can
   make a query, mutation or subscription from an api.
-  
+
   Attributes:
       environments (dict): Dictonary with all envieroments. Defaults to
         empty dict.
       environment (dict): Dictionary with the data of the actual enviroment.
         Defaults to None.
       ws_url (string): String with the WSS url. Defaults to None.
       subs (dict): Dictionary with all active subscriptions in the instance.
@@ -121,15 +122,15 @@
         Defaults to False.
       closing (boolean): Checks if all subscriptions were successfully closed.
         Defaults to False.
       unsubscribing (boolean): Checks if all subscriptions were successfully
         canceled. Defaults to False.
       websocket_timeout (int): seconds of the websocket timeout. Defaults to
         60.
-  
+
   Examples:
       >>> <With> clause:
         '''
         client = GraphQLClient()
         with client.enterEnvironment('dev') as gql:
             data, errors = gql.query('{lines(limit:2){id}}')
             print(data, errors)
@@ -162,36 +163,36 @@
     self.sub_pingpong_thread = None
     self.wss_conn_halted = False
     self.closing = False
     self.unsubscribing = False
     self.websocket_timeout = 60
     self.pingIntervalTime = 15
     self.pingTimer = time.time()
-  
+
   # * with <Object> implementation
   def __enter__(self):
     return self
-  
+
   def __exit__(self, type, value, traceback):
     self.environment = self.save_env # restores environment
     return
-  
+
   def enterEnvironment(self, name):
     """This function makes a safe access to an environment.
 
     Args:
         name (string): Name of the environment.
 
     Returns:
         (self): Returns self instance for the use with `with` keyword.
     """
     self.save_env = self.environment
     self.environment = name
     return self # * for use with "with" keyword
-  
+
   # * HIGH LEVEL METHODS ---------------------------------
   # TODO: Implement tenacity in query, mutation and subscription methods
   # @retry(
   #   retry=(retry_if_result(has_errors)),
   #   stop=stop_after_attempt(5),
   #   wait=wait_random(min=0.25, max=0.5))
   # def query_wrapper(self, query, variables=None):
@@ -200,15 +201,15 @@
   #   try:
   #     result = self.execute(query, variables)
   #     data = result.get('data', None)
   #     errors = result.get('errors', [])
   #   except Exception as e:
   #     errors = [{'message': str(e)}]
   #   return data, errors
-  
+
   # * Query high level implementation
   def query(self, query, variables=None, flatten=True, single_child=False):
     """This function makes a query transaction to the actual environment.
 
     Args:
         query (string): Graphql query instructions.
         variables (string, optional): Query variables. Defaults to None.
@@ -244,15 +245,15 @@
         variables (string, optional): Query variables. Defaults to None.
 
 
     Returns:
         (GraphqlResponse): Returns the GraphqlResponse of the query.
     """
     return self.query(query, variables, flatten=True, single_child=True)
-  
+
   # * Mutation high level implementation
   def mutate(self, mutation, variables=None, flatten=True):
     """This function makes a mutation transaction to the actual environment.
 
     Args:
         mutation (string): Graphql mutation instructions.
         variables (string, optional): Mutation variables. Defaults to None.
@@ -319,30 +320,30 @@
     payload = {'query': query, 'variables': variables}
     self._start(payload, _id)
     # ! Create unsubscribe function for this specific thread:
     def unsubscribe():
       return self._unsubscribe(_id)
     self.subs[_id].update({'unsub': unsubscribe})
     return unsubscribe
-  
+
   def _unsubscribe(self, _id):
     if not self.subs.get(_id):
       print('Subscription already cleared')
       return
     self.unsubscribing = True
     self.subs[_id]['kill'] = True
     try:
       self._stop(_id)
     except BrokenPipeError as e:
       print('WSS Pipe broken, nothing to stop')
       print(f'original message: {e}')
     self.subs[_id]['thread'].join()
     self.subs[_id].update({'running': False})
     self.unsubscribing = False
-  
+
   def _sub_routing_loop(self):
     print('first subscription, starting routing loop')
     while not self.closing:
       if (self.wss_conn_halted):
         print('Connection halted, attempting reconnection...')
         if self._new_conn():
           self.wss_conn_halted = False
@@ -375,34 +376,34 @@
       except Exception as e:
         if not self.closing:
           print(f'Some error trying to receive WSS')
           print(f'original message: {e}')
           self.wss_conn_halted = True
         continue
 
-      if 'id' in message.keys(): 
+      if 'id' in message.keys():
         # if the message has an ID request, it will be handled by the _subscription_loop
         _id = py_.get(message, 'id')
         active_sub = self.subs.get(_id)
         # the connection may not be active due to:
         # 1. server error (incorrect ID sent)
-        # 2. race condition (we closed connection, but a message was already on its way here) 
+        # 2. race condition (we closed connection, but a message was already on its way here)
         if (not active_sub):
           continue
         active_sub['queue'].append(message)
       elif message['type'] == 'connection_ack':
         print('Connection Ack with the server.')
         pass
       elif message['type'] == 'pong':
         pass
       else:
         print(f'unknown msg type: {message}')
 
       time.sleep(0.01)
-  
+
   def _resubscribe_all(self):
     # first, clear every subscription thread running:
     for sub_id in self.subs.keys():
       self.subs[sub_id]['kill'] = True  # Signal threads to stop
     # wait for every thread to finish
     for sub_id in self.subs.keys():
       print(f'killing halted subscription (id={sub_id})')
@@ -414,15 +415,15 @@
         query=old_subs[sub_id]['query'],
         variables=old_subs[sub_id]['variables'],
         callback=old_subs[sub_id]['callback'],
         on_error_callback=old_subs[sub_id]['on_error_callback'],
         flatten=old_subs[sub_id]['flatten'],
         _id=sub_id,
       )
-  
+
   def _subscription_loop(self, _cb, _id, _ecb):
     self.subs[_id].update({'running': True, 'starting': False})
     while self.subs[_id]['running']:
       aborted = self.subs[_id]['kill']
       if aborted:
         print(f'stopping subscription id={_id} on Unsubscribe')
         break
@@ -452,22 +453,32 @@
           continue
         print('Subscription message has payload Errors')
         print(message)
       elif is_ws_connection_init_msg(message):
         print('Subscription successfully initialized')
       else:
         gql_msg = self._clean_sub_message(_id, message)
-        _cb(gql_msg) # execute callback function
-        self.subs[_id]['runs'] += 1 # take note of how many times this sub has been triggered   
+        try:
+          _cb(gql_msg) # execute callback function
+        except Exception as e:
+          print(f'Error on subscription callback: {e}')
+          sub_query = self.subs[_id].get('query')
+          sub_variables = self.subs[_id].get('variables')
+          if sub_query:
+            print(f'subscription document: \n\t{sub_query}')
+          if sub_variables:
+            print(f'subscription variables: \n\t{sub_variables}')
+          print(traceback.format_exc())
+          continue
+        self.subs[_id]['runs'] += 1 # take note of how many times this sub has been triggered
 
-      time.sleep(0.01)
     # ! subscription stopped, due to error or user event
     print(f'Subscription id={_id} stopped')
     self.subs[_id].update({'running': False, 'kill': True})
-  
+
   def _clean_sub_message(self, _id, message):
     data = py_.get(message, 'payload', {})
     return data_flatten(data) if self.subs[_id]['flatten'] else data
 
   def _new_conn(self):
     env = self.environments.get(self.environment, None)
     self.ws_url = env.get('wss')
@@ -497,15 +508,15 @@
     self.sub_pingpong_thread.join()
     self.sub_router_thread = None
     self.sub_pingpong_thread = None
     self._conn = None
     self.sub_counter = 0
     self.subs = {}
     self.closing = False
-  
+
   def _on_message(self, message):
     '''Dummy callback for subscription'''
     print(f'message received on subscription:')
     print(message)
 
   def _conn_init(self):
     env = self.environments.get(self.environment, None)
@@ -526,15 +537,15 @@
       self.sub_pingpong_thread = threading.Thread(target=self._ping_pong)
     if not self.sub_pingpong_thread.is_alive():
       self.sub_pingpong_thread.start()
 
   def _waiting_connection_ack(self):
     self._conn.settimeout(self.ack_timeout)
     # set timeout to raise Exception websocket.WebSocketTimeoutException
-    message = json.loads(self._conn.recv()) 
+    message = json.loads(self._conn.recv())
     if message['type'] == 'connection_ack':
       print('Connection Ack with the server.')
 
   def _ping_pong(self):
     self.pingTimer = time.time()
     while not self.closing:
       time.sleep(0.1)
@@ -552,15 +563,15 @@
 
   def _registerSub(self, _id=None):
     if not _id:
       self.sub_counter += 1
       _id = str(self.sub_counter)
     self.subs.update({_id: {'running': False, 'kill': False, 'starting': True}})
     return _id
-      
+
   def _start(self, payload, _id):
     frame = {'id': _id, 'type': 'subscribe', 'payload': payload}
     self._conn.send(json.dumps(frame))
 
   def _stop(self, _id):
     payload = {'id': _id, 'type': 'complete'}
     self._conn.send(json.dumps(payload))
@@ -570,18 +581,18 @@
 
     Returns:
         (boolean): Returns if the reconnection has been possible.
     """
     if not self.sub_router_thread:
       print('connection not stablished, nothing to reset')
       return False
-    if self.sub_router_thread.isAlive(): #check that _sub_routing_loop() is running
+    if self.sub_router_thread.is_alive(): #check that _sub_routing_loop() is running
       self._conn.close() # forces connection halted (wss_conn_halted)
       return True
-    # in case for some reason _sub_routing_loop() is not running 
+    # in case for some reason _sub_routing_loop() is not running
     if self._new_conn():
       print('WSS Reconnection succeeded, attempting resubscription to lost subs')
       self._resubscribe_all()
       print('finished resubscriptions')
       return True
     else:
       print('Reconnection has not been possible')
@@ -596,15 +607,15 @@
     Args:
         label (str, optional): Name of the mutation batch. Defaults to 'mutation'.
 
     Returns:
         (MutationBatch): Returns a MutationBatch Object.
     """
     return MutationBatch(client=self, label=label)
-  
+
   def batchQuery(self, label='query'):
     """This fuction makes a batchs of query transactions.
 
     Args:
         label (str, optional): Name of the query batch. Defaults to 'query'.
 
     Returns:
@@ -623,15 +634,15 @@
         wss (string, optional): URL of the WSS of the environment. Defaults to None.
         headers (dict, optional): A dictionary with the headers
          (like authorization). Defaults to {}.
         default (bool, optional): Checks if the new environment will be the
          default one of the instance. Defaults to False.
         timeoutWebsocket (int, optional): Seconds of the timeout of the
          websocket. Defaults to 60.
-        post_timeout (int, optional): Timeout in seconds for each post. 
+        post_timeout (int, optional): Timeout in seconds for each post.
          Defaults to 60.
     """
     self.environments.update({
       name: {
         'url': url,
         'wss': wss,
         'headers': headers,
@@ -649,27 +660,27 @@
         environment (string, optional): Name of the environment. Defaults to None.
         url (string, optional): New URL for the enviroment. Defaults to None.
     """
     # if environment is not selected, use current environment
     if not environment:
       environment = self.environment
     self.environments[environment].update({'url': url})
-  
+
   def setWss(self, environment=None, url=None):
     """This function sets a new WSS to an existing environment.
 
     Args:
         environment (string, optional): Name of the environment. Defaults to None.
         url (string, optional): New WSS URL for the environment. Defaults to None.
     """
     # if environment is not selected, use current environment
     if not environment:
       environment = self.environment
     self.environments[environment].update({'wss': url})
-  
+
   def addHeader(self, environment=None, header={}):
     """This function updates the header of an existing environment.
 
     Args:
         environment (string, optional): Name of the environment. Defaults to None.
         header (dict, optional): New headers to add. Defaults to {}.
     """
@@ -701,15 +712,15 @@
         seconds (int): Time for the timeout.
     """
     # if environment is not selected, use current environment
     if not environment:
       environment = self.environment
     self.environments[environment].update({'post_timeout': post_timeout})
 
-  
+
   def setTimeoutWebsocket(self, seconds):
     """This function sets the webscoket's timeout.
 
     Args:
         seconds (int): Time for the timeout.
     """
     self.websocket_timeout =  seconds
```

### Comparing `pygqlc-3.0.5/pygqlc/MutationBatch.py` & `pygqlc-3.1.0/pygqlc/MutationBatch.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.0.5/pygqlc/MutationParser.py` & `pygqlc-3.1.0/pygqlc/MutationParser.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.0.5/pygqlc/QueryParser.py` & `pygqlc-3.1.0/pygqlc/QueryParser.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.0.5/pygqlc.egg-info/PKG-INFO` & `pygqlc-3.1.0/pygqlc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygqlc
-Version: 3.0.5
+Version: 3.1.0
 Summary: GraphQL API Client for python language
 Home-page: https://github.com/valiot/pygqlc
 Author: Valiot
 Author-email: hiring@valiot.io
 Keywords: pygqlc
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `pygqlc-3.0.5/pygqlc.egg-info/SOURCES.txt` & `pygqlc-3.1.0/pygqlc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygqlc-3.0.5/setup.py` & `pygqlc-3.1.0/setup.py`

 * *Files identical despite different names*

