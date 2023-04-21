# Comparing `tmp/esdbclient-0.8.tar.gz` & `tmp/esdbclient-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdbclient-0.8.tar", max compression
+gzip compressed data, was "esdbclient-0.9.tar", max compression
```

## Comparing `esdbclient-0.8.tar` & `esdbclient-0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-0.8/LICENSE
--rw-r--r--   0        0        0    43411 2023-02-11 18:37:22.810902 esdbclient-0.8/README.md
--rw-r--r--   0        0        0      182 2022-06-23 14:19:18.317724 esdbclient-0.8/esdbclient/__init__.py
--rw-r--r--   0        0        0     7297 2023-02-11 18:13:50.593476 esdbclient-0.8/esdbclient/client.py
--rw-r--r--   0        0        0    18197 2023-02-11 18:13:50.594271 esdbclient-0.8/esdbclient/esdbapi.py
--rw-r--r--   0        0        0      574 2023-02-11 18:13:50.594724 esdbclient-0.8/esdbclient/events.py
--rw-r--r--   0        0        0      710 2022-06-23 14:19:18.318601 esdbclient-0.8/esdbclient/exceptions.py
--rw-r--r--   0        0        0     1790 2023-01-23 18:02:35.248448 esdbclient-0.8/esdbclient/protos/Grpc/code_pb2.py
--rw-r--r--   0        0        0    13555 2023-01-23 18:02:35.249448 esdbclient-0.8/esdbclient/protos/Grpc/code_pb2.pyi
--rw-r--r--   0        0        0      158 2022-11-06 16:49:34.017453 esdbclient-0.8/esdbclient/protos/Grpc/code_pb2_grpc.py
--rw-r--r--   0        0        0    43977 2023-01-31 13:52:51.273428 esdbclient-0.8/esdbclient/protos/Grpc/persistent_pb2.py
--rw-r--r--   0        0        0    73085 2023-01-31 13:52:51.274163 esdbclient-0.8/esdbclient/protos/Grpc/persistent_pb2.pyi
--rw-r--r--   0        0        0    15771 2023-01-31 13:52:51.274680 esdbclient-0.8/esdbclient/protos/Grpc/persistent_pb2_grpc.py
--rw-r--r--   0        0        0     3782 2023-01-23 18:02:35.250362 esdbclient-0.8/esdbclient/protos/Grpc/shared_pb2.py
--rw-r--r--   0        0        0     9874 2023-01-23 18:02:35.251226 esdbclient-0.8/esdbclient/protos/Grpc/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2022-11-06 16:49:34.030872 esdbclient-0.8/esdbclient/protos/Grpc/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1686 2023-01-23 18:02:35.252048 esdbclient-0.8/esdbclient/protos/Grpc/status_pb2.py
--rw-r--r--   0        0        0     2838 2023-01-23 18:02:35.252880 esdbclient-0.8/esdbclient/protos/Grpc/status_pb2.pyi
--rw-r--r--   0        0        0      158 2022-11-06 16:49:34.040459 esdbclient-0.8/esdbclient/protos/Grpc/status_pb2_grpc.py
--rw-r--r--   0        0        0    19933 2023-01-23 18:02:35.254530 esdbclient-0.8/esdbclient/protos/Grpc/streams_pb2.py
--rw-r--r--   0        0        0    71744 2023-01-23 18:02:35.257256 esdbclient-0.8/esdbclient/protos/Grpc/streams_pb2.pyi
--rw-r--r--   0        0        0     9787 2022-11-06 16:49:34.163884 esdbclient-0.8/esdbclient/protos/Grpc/streams_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-0.8/esdbclient/py.typed
--rw-r--r--   0        0        0     2536 2023-02-11 18:56:08.019539 esdbclient-0.8/pyproject.toml
--rw-r--r--   0        0        0    45473 1970-01-01 00:00:00.000000 esdbclient-0.8/setup.py
--rw-r--r--   0        0        0    44703 1970-01-01 00:00:00.000000 esdbclient-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-0.9/LICENSE
+-rw-r--r--   0        0        0    48510 2023-02-12 01:08:46.249759 esdbclient-0.9/README.md
+-rw-r--r--   0        0        0      434 2023-02-12 00:54:11.519980 esdbclient-0.9/esdbclient/__init__.py
+-rw-r--r--   0        0        0     7519 2023-02-12 01:03:15.566450 esdbclient-0.9/esdbclient/client.py
+-rw-r--r--   0        0        0    18582 2023-02-12 00:54:11.835919 esdbclient-0.9/esdbclient/esdbapi.py
+-rw-r--r--   0        0        0      800 2023-02-12 00:54:11.521056 esdbclient-0.9/esdbclient/events.py
+-rw-r--r--   0        0        0      710 2022-06-23 14:19:18.318601 esdbclient-0.9/esdbclient/exceptions.py
+-rw-r--r--   0        0        0     1790 2023-01-23 18:02:35.248448 esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.py
+-rw-r--r--   0        0        0    13555 2023-01-23 18:02:35.249448 esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2022-11-06 16:49:34.017453 esdbclient-0.9/esdbclient/protos/Grpc/code_pb2_grpc.py
+-rw-r--r--   0        0        0    43977 2023-01-31 13:52:51.273428 esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.py
+-rw-r--r--   0        0        0    73085 2023-01-31 13:52:51.274163 esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.pyi
+-rw-r--r--   0        0        0    15771 2023-01-31 13:52:51.274680 esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0     3782 2023-01-23 18:02:35.250362 esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.py
+-rw-r--r--   0        0        0     9874 2023-01-23 18:02:35.251226 esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2022-11-06 16:49:34.030872 esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1686 2023-01-23 18:02:35.252048 esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.py
+-rw-r--r--   0        0        0     2838 2023-01-23 18:02:35.252880 esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2022-11-06 16:49:34.040459 esdbclient-0.9/esdbclient/protos/Grpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0    19933 2023-01-23 18:02:35.254530 esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.py
+-rw-r--r--   0        0        0    71744 2023-01-23 18:02:35.257256 esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.pyi
+-rw-r--r--   0        0        0     9787 2022-11-06 16:49:34.163884 esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-0.9/esdbclient/py.typed
+-rw-r--r--   0        0        0     2536 2023-02-12 01:12:22.638342 esdbclient-0.9/pyproject.toml
+-rw-r--r--   0        0        0    50700 1970-01-01 00:00:00.000000 esdbclient-0.9/setup.py
+-rw-r--r--   0        0        0    49802 1970-01-01 00:00:00.000000 esdbclient-0.9/PKG-INFO
```

### Comparing `esdbclient-0.8/LICENSE` & `esdbclient-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/README.md` & `esdbclient-0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   * [Start EventStoreDB](#start-eventstoredb)
   * [Stop EventStoreDB](#stop-eventstoredb)
 * [Client](#client)
 * [Streams](#streams)
   * [Append events](#append-events)
   * [Get current stream position](#get-current-stream-position)
   * [Read stream events](#read-stream-events)
+  * [Idempotent writes](#idempotent-writes)
   * [Read all recorded events](#read-all-recorded-events)
   * [Get current commit position](#get-current-commit-position)
 * [Subscriptions](#subscriptions)
   * [Catch-up subscriptions](#catch-up-subscriptions)
   * [Persistent subscriptions](#persistent-subscriptions)
 * [Notes](#notes)
   * [Regular expression filters](#regular-expression-filters)
@@ -172,23 +173,22 @@
 Please note, the append events operation is atomic, so that either all
 or none of the given new events will be recorded. By design, it is only
 possible with EventStoreDB to atomically record new events in one stream.
 
 In the example below, a new event is appended to a new stream.
 
 ```python
-from uuid import uuid4
+from uuid import UUID, uuid4
 
 from esdbclient import NewEvent
 
 # Construct new event object.
 event1 = NewEvent(
     type='OrderCreated',
     data=b'data1',
-    metadata=b'{}'
 )
 
 # Define stream name.
 stream_name1 = str(uuid4())
 
 # Append list of events to new stream.
 commit_position1 = client.append_events(
@@ -201,20 +201,18 @@
 In the example below, two subsequent events are appended to an existing
 stream.
 
 ```python
 event2 = NewEvent(
     type='OrderUpdated',
     data=b'data2',
-    metadata=b'{}',
 )
 event3 = NewEvent(
     type='OrderDeleted',
     data=b'data3',
-    metadata=b'{}',
 )
 
 commit_position2 = client.append_events(
     stream_name=stream_name1,
     expected_position=0,
     events=[event2, event3],
 )
@@ -222,26 +220,31 @@
 
 If the append operation is successful, this method returns an integer
 representing the overall "commit position" as it was when the operation
 was completed. Otherwise, an exception will be raised.
 
 A "commit position" is a monotonically increasing integer representing
 the position of the recorded event in a "total order" of all recorded
-events in the database across all streams. The sequence of commit positions
-is not gapless. It represents the position of the event record on disk, and
-there are usually large differences between successive commits.
-
-The "commit position" returned in this way can be used to wait for a
-downstream component to have processed the newly appended events.
-For example, after a user interface command that results in the recording
-of new events, and before a query is issued that depends on an eventually
-consistent materialized view in a downstream component that would be stale
-if those newly appended events have not yet been processed, the user interface
-can poll the downstream component, to see if it has processed an event at that
-commit position, before executing a query for that materialized view.
+events in the database across all streams. It is the actual position
+of the event record on disk, and there are usually large differences
+between successive commits. The sequence of commit positions
+is NOT gapless.
+
+The "commit position" returned by `append_events()` is that of the last
+recorded event in the given sequence of new events.
+
+The "commit position" returned in this way can therefore be used to wait
+for a downstream component to have processed all the events that were recorded.
+
+For example, consider a user interface command that results in the recording
+of new events, and a query into an eventually consistent materialized
+view in a downstream component that is updated from these events. If the new
+events have not yet been processed, the view would be stale. The "commit position"
+can be used by the user interface to poll the downstream component until it has
+processed the new events, after which time the view will not be stale.
 
 ### Get current stream position
 
 The client has a `get_stream_position()` method, which can be used to
 get the current "stream position" of a stream (the position in the
 stream of the last recorded event in that stream).
 
@@ -445,14 +448,75 @@
 
 assert events[0].stream_name == stream_name1
 assert events[0].stream_position == 2
 assert events[0].type == event3.type
 assert events[0].data == event3.data
 ```
 
+### Idempotent writes
+
+Now that we can both append events and read from a stream, we can demonstrate
+the idempotent nature of the `append_events()` operation.
+
+Sometimes it may happen that a new event is successfully recorded and then somehow
+the connection to the database gets interrupted before the successful call can return
+successfully to the client. In case of an error when appending an event, it may be
+desirable to retry appending the same event at the same position. If the event was
+in fact successfully recorded, it is convenient for the retry to return successfully
+without raising an error due to optimistic concurrency control (as described above).
+
+The example below shows the `append_events()` method being called again with
+`event3` and `expected_position=2`.
+
+```python
+# Retry appending event3.
+commit_position_retry = client.append_events(
+    stream_name=stream_name1,
+    expected_position=0,
+    events=[event2, event3],
+)
+```
+
+We can see that the same commit position is returned as above.
+
+```python
+assert commit_position_retry == commit_position2
+```
+
+This works because the `NewEvent` class has an `id` attribute that
+is supplied with a new version-4 UUID when an instance is constructed.
+
+```python
+assert isinstance(event1.id, UUID)
+assert isinstance(event2.id, UUID)
+assert isinstance(event3.id, UUID)
+
+assert event1.id != event2.id
+assert event2.id != event3.id
+```
+
+It is possible to provide an `id` value when constructing instances of
+`NewEvent`, but in the examples above we have been using the default behaviour.
+
+We can see that the `append_events()` method returns successfully, and
+that the stream has been unchanged by calling the method twice with the
+same arguments.
+
+```python
+response = client.read_stream_events(
+    stream_name=stream_name1
+)
+
+events = list(response)
+assert events[0].id == event1.id
+assert events[1].id == event2.id
+assert events[2].id == event3.id
+```
+
+
 ### Read all recorded events
 
 The method `read_all_events()` can be used to read all recorded events
 in the database in the order they were recorded. An iterable object of
 recorded events is returned. This iterable object will stop when it has
 yielded the last recorded event.
 
@@ -622,14 +686,16 @@
 assert len(events) == 1
 
 assert events[0].commit_position < commit_position2
 ```
 
 ### Get current commit position
 
+*only supported in EventStoreDB version >= 22.10*
+
 The method `get_commit_position()` can be used to get the current
 commit position of the database.
 
 ```python
 commit_position = client.get_commit_position()
 ```
 
@@ -706,25 +772,22 @@
 commit_position = client.get_commit_position()
 
 # Append three events to another stream.
 stream_name2 = str(uuid4())
 event4 = NewEvent(
     type='OrderCreated',
     data=b'data4',
-    metadata=b'{}',
 )
 event5 = NewEvent(
     type='OrderUpdated',
     data=b'data5',
-    metadata=b'{}',
 )
 event6 = NewEvent(
     type='OrderDeleted',
     data=b'data6',
-    metadata=b'{}',
 )
 client.append_events(
     stream_name=stream_name2,
     expected_position=None,
     events=[event4, event5, event6],
 )
 
@@ -746,25 +809,22 @@
 
 
 # Append three more events.
 stream_name3 = str(uuid4())
 event7 = NewEvent(
     type='OrderCreated',
     data=b'data7',
-    metadata=b'{}',
 )
 event8 = NewEvent(
     type='OrderUpdated',
     data=b'data8',
-    metadata=b'{}',
 )
 event9 = NewEvent(
     type='OrderDeleted',
     data=b'data9',
-    metadata=b'{}',
 )
 
 client.append_events(
     stream_name=stream_name3,
     expected_position=None,
     events=[event7, event8, event9],
 )
@@ -840,14 +900,22 @@
 the subscription should receive events. Please note, the recorded event
 at the specified commit position MAY be included in the recorded events
 received by the group of consumers.
 
 If neither `from_end` or `position` are specified, the group of consumers
 of the subscription will receive all recorded events.
 
+This method also takes option `filter_exclude`, `filter_include`
+arguments, which work in the same way as they do in the `subscribe_all_events()`
+method.
+
+This method also takes an optional `timeout` argument, that
+is expected to be a Python `float`, which sets a deadline
+for the completion of the gRPC operation.
+
 The method `create_subscription()` does not return a value, because
 recorded events are obtained by the group of consumers of the subscription
 using the `read_subscription()` method.
 
 In the example below, a persistent subscription is created.
 
 ```python
@@ -859,14 +927,18 @@
 The method `read_subscription()` can be used by a group of consumers to receive
 recorded events from a persistent subscription created using `create_subscription`.
 
 This method takes a required `group_name` argument, which is
 the name of a "group" of consumers of the subscription specified
 when `create_subscription()` was called.
 
+This method also takes an optional `timeout` argument, that
+is expected to be a Python `float`, which sets a deadline
+for the completion of the gRPC operation.
+
 This method returns a 2-tuple: a "read request" object and a "read response" object.
 
 ```python
 read_req, read_resp = client.read_subscription(group_name=group_name)
 ```
 
 The "read response" object is an iterator that yields recorded events from
@@ -1007,89 +1079,136 @@
 the same transaction), and making these records unique so that transactions will be
 rolled back preventing the results of reprocessing the event being committed.
 
 ## Notes
 
 ### Regular expression filters
 
-The `filter_exclude` and `filter_include` arguments in `read_all_events()` and
-`subscribe_all_events()` are applied to the `type` attribute of recorded events.
+The filter arguments in `read_all_events()`, `subscribe_all_events()`,
+`create_subscription()` and `commit_position()` are applied to the `type`
+attribute of recorded events.
 
 The default value of the `filter_exclude` arguments is designed to exclude
-EventStoreDB "system events", which otherwise would be included. System
-events, by convention in EventStoreDB, all have `type` strings that
-start with the `$` sign.
-
-Please note, characters that have a special meaning in regular expressions
-will need to be escaped (with double-backslash) when matching these characters
-in type strings.
-
-For example, to match EventStoreDB system events, use the sequence `['\\$.*']`.
-Please note, the constant `ESDB_EVENTS_REGEX` is set to `'\\$.*'`. You
-can import this value (`from esdbclient import ESDB_EVENTS_REGEX`) and use
-it when building longer sequences of regular expressions. For example,
-to exclude system events and snapshots, you might use the sequence
-`[ESDB_EVENTS_REGEX, '.*Snapshot']` as the value of the `filter_exclude`
-argument.
-
+EventStoreDB "system" and "persistence subscription config" events, which
+otherwise would be included. System events generated by EventStoreDB all
+have `type` strings that start with the `$` sign. Persistence subscription
+events generated when manipulating persistence subscriptions all have `type`
+strings that start with `PersistentConfig`.
+
+For example, to match the type of EventStoreDB system events, use the regular
+expression `r'\$.+'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is
+set to `r'\$.+'`. You can import this value
+(`from esdbclient import ESDB_SYSTEM_EVENTS_REGEX`) and use
+it when building longer sequences of regular expressions.
+
+Similarly, to match the type of EventStoreDB persistence subscription events, use the
+regular expression `r'PersistentConfig\d+'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`
+is set to `r'PersistentConfig\d+'`. You can also import this value
+(`from esdbclient import ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`) and use it when building
+longer sequences of regular expressions.
+
+The constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that match
+the events that EventStoreDB generates internally, events that are extraneous to those
+which you append using the `append_events()` method.
+
+For example, to exclude system events and persistence subscription configuration events,
+and snapshots, you might use the sequence `DEFAULT_EXCLUDE_FILTER + ['.*Snapshot']` as
+the value of the `filter_exclude` argument when calling `read_all_events()`,
+`subscribe_all_events()`, `create_subscription()` or `get_commit_position()`.
 
 ### The NewEvent class
 
-The `NewEvent` class can be used to define new events.
+The `NewEvent` class is used when appending events.
+
+The required argument `type` is a Python `str` object, used to indicate the type of
+the event that will be recorded.
+
+The required argument `data` is a Python `bytes` object, used to indicate the data of
+the event that will be recorded.
 
-The attribute `type` is a unicode string, used to specify the type of the event
-to be recorded.
+The optional argument `metadata` is a Python `bytes` object, used to indicate any
+metadata of the event that will be recorded. The default value is an empty `bytes`
+object.
 
-The attribute `data` is a byte string, used to specify the data of the event
-to be recorded. Please note, in this version of this Python client,
-writing JSON event data to EventStoreDB isn't supported, but it might be in
-a future version.
+The optional argument `content_type` is a Python `str` object, used to indicate the
+type of the data that will be recorded for this event. The default value is
+`application/json`, which indicates that the `data` was serialised using JSON.
+An alternative value for this argument is `application/octet-stream`.
 
-The attribute `metadata` is a byte string, used to specify metadata for the event
-to be recorded.
+The optional argument `id` is a Python `UUID` object, used to specify the unique ID
+of the event that will be recorded. This value will default to a new version-4 UUID.
 
 ```python
-new_event = NewEvent(
+new_event1 = NewEvent(
     type='OrderCreated',
-    data=b'{}',
-    metadata=b'{}',
+    data=b'{"name": "Greg"}',
 )
+assert new_event1.type == 'OrderCreated'
+assert new_event1.data == b'{"name": "Greg"}'
+assert new_event1.metadata == b''
+assert new_event1.content_type == 'application/json'
+assert isinstance(new_event1.id, UUID)
+
+event_id = uuid4()
+new_event2 = NewEvent(
+    type='ImageCreated',
+    data=b'01010101010101',
+    metadata=b'{"a": 1}',
+    content_type='application/octet-stream',
+    id=event_id,
+)
+assert new_event2.type == 'ImageCreated'
+assert new_event2.data == b'01010101010101'
+assert new_event2.metadata == b'{"a": 1}'
+assert new_event2.content_type == 'application/octet-stream'
+assert new_event2.id == event_id
 ```
 
 ### The RecordedEvent class
 
-The `RecordedEvent` class is used when reading recorded events.
+The `RecordedEvent` class is used when reading events.
 
-The attribute `type` is a unicode string, used to indicate the type of the event
+The attribute `type` is a Python `str` object, used to indicate the type of event
 that was recorded.
 
-The attribute `data` is a byte string, used to indicate the data of the event
-that was recorded.
+The attribute `data` is a Python `bytes` object, used to indicate the data of the
+event that was recorded.
 
-The attribute `metadata` is a byte string, used to indicate metadata for the event
-that was recorded.
+The attribute `metadata` is a Python `bytes` object, used to indicate the metadata of
+the event that was recorded.
 
-The attribute `stream_name` is a unicode string, used to indicate the type of
-the name of the stream in which the event was recorded.
+The attribute `content_type` is a Python `str` object, used to indicate the type of
+data that was recorded for this event (usually `application/json` to indicate that
+this data can be parsed as JSON, but alternatively `application/octet-stream` to
+indicate that it is something else).
+
+The attribute `id` is a Python `UUID` object, used to indicate the unique ID of the
+event that was recorded. Please note, when recorded events are returned from a call
+to `read_stream_events()` in EventStoreDB v21.10, the commit position is not actually
+set in the response. For this reason, this attribute is actually typed as an optional
+value (`Optional[UUID]`), and this case the value of this attribute will be `None`.
 
-The attribute `stream_position` is an integer, used to indicate
-the position in the stream at which the event was recorded.
+The attribute `stream_name` is a Python `str` object, used to indicate the name of the
+stream in which the event was recorded.
 
-The attribute `commit_position` is an integer, used to indicate
-the position in total order of all recorded events at which the
-event was recorded.
+The attribute `stream_position` is a Python `int`, used to indicate the position in the
+stream at which the event was recorded.
+
+The attribute `commit_position` is a Python `int`, used to indicate the commit position
+at which the event was recorded.
 
 ```python
 from esdbclient.events import RecordedEvent
 
 recorded_event = RecordedEvent(
-    id=uuid4(),
     type='OrderCreated',
     data=b'{}',
-    metadata=b'{}',
+    metadata=b'',
+    content_type='application/json',
+    id=uuid4(),
     stream_name='stream1',
     stream_position=0,
     commit_position=512,
 )
 ```
 
 ## Contributors
```

### Comparing `esdbclient-0.8/esdbclient/client.py` & `esdbclient-0.9/esdbclient/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,20 @@
     SubscriptionReadResponse,
     Subscriptions,
     handle_rpc_error,
 )
 from esdbclient.events import NewEvent, RecordedEvent
 from esdbclient.exceptions import StreamNotFound
 
-ESDB_EVENTS_REGEX = "\\$.*"  # Matches the 'type' of system events.
+# Matches the 'type' of "system" events.
+ESDB_SYSTEM_EVENTS_REGEX = r"\$.+"
+# Matches the 'type' of "PersistentConfig" events.
+ESDB_PERSISTENT_CONFIG_EVENTS_REGEX = r"PersistentConfig\d+"
+
+DEFAULT_EXCLUDE_FILTER = (ESDB_SYSTEM_EVENTS_REGEX, ESDB_PERSISTENT_CONFIG_EVENTS_REGEX)
 
 
 class EsdbClient:
     """
     Encapsulates the EventStoreDB gRPC API.
     """
 
@@ -98,15 +103,15 @@
             credentials=self._call_credentials,
         )
 
     def read_all_events(
         self,
         commit_position: Optional[int] = None,
         backwards: bool = False,
-        filter_exclude: Sequence[str] = (ESDB_EVENTS_REGEX,),
+        filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
     ) -> Iterable[RecordedEvent]:
         """
         Reads recorded events in "all streams" in the database.
         """
@@ -142,34 +147,35 @@
             return None
         else:
             return last_event.stream_position
 
     def get_commit_position(
         self,
         timeout: Optional[float] = None,
-        filter_exclude: Sequence[str] = (ESDB_EVENTS_REGEX,),
+        filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
     ) -> int:
         """
         Returns the current commit position of the database.
         """
         recorded_events = self.read_all_events(
             backwards=True,
             filter_exclude=filter_exclude,
             limit=1,
             timeout=timeout,
         )
         commit_position = 0
         for ev in recorded_events:
+            assert ev.commit_position is not None
             commit_position = ev.commit_position
         return commit_position
 
     def subscribe_all_events(
         self,
         commit_position: Optional[int] = None,
-        filter_exclude: Sequence[str] = (ESDB_EVENTS_REGEX,),
+        filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         timeout: Optional[float] = None,
     ) -> Iterator[RecordedEvent]:
         """
         Returns a catch-up subscription, from which recorded
         events in "all streams" in the database can be received.
         """
@@ -184,16 +190,15 @@
         return CatchupSubscription(read_resp=read_resp)
 
     def create_subscription(
         self,
         group_name: str,
         from_end: bool = False,
         commit_position: Optional[int] = None,
-        # filter_exclude: Sequence[str] = (ESDB_EVENTS_REGEX,),
-        filter_exclude: Sequence[str] = (),
+        filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         timeout: Optional[float] = None,
     ) -> None:
         self._subscriptions.create(
             group_name=group_name,
             from_end=from_end,
             commit_position=commit_position,
```

### Comparing `esdbclient-0.8/esdbclient/esdbapi.py` & `esdbclient-0.9/esdbclient/esdbapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import sys
 from base64 import b64encode
 from queue import Empty, Queue
 from typing import Iterable, Optional, Sequence, Tuple, overload
-from uuid import UUID, uuid4
+from uuid import UUID
 
 import grpc
 from grpc import (
     AuthMetadataContext,
     AuthMetadataPluginCallback,
     Call,
     CallCredentials,
@@ -212,22 +212,28 @@
             for response in self._stub.Read(
                 read_req, timeout=timeout, credentials=credentials
             ):
                 assert isinstance(response, grpc_streams.ReadResp)
                 content_attribute_name = response.WhichOneof("content")
                 if content_attribute_name == "event":
                     event = response.event.event
+                    if response.event.WhichOneof("position") == "commit_position":
+                        commit_position = response.event.commit_position
+                    else:
+                        commit_position = None  # pragma: no cover
+
                     yield RecordedEvent(
                         id=UUID(event.id.string),
                         type=event.metadata["type"],
                         data=event.data,
+                        content_type=event.metadata["content-type"],
                         metadata=event.custom_metadata,
                         stream_name=event.stream_identifier.stream_name.decode("utf8"),
                         stream_position=event.stream_revision,
-                        commit_position=response.event.commit_position,
+                        commit_position=commit_position,
                     )
                 elif content_attribute_name == "stream_not_found":
                     raise StreamNotFound(f"Stream {stream_name!r} not found")
         except RpcError as e:
             raise handle_rpc_error(e) from e
 
     def append(
@@ -271,18 +277,18 @@
                 ),
             )
         ]
         for event in events:
             requests.append(
                 grpc_streams.AppendReq(
                     proposed_message=grpc_streams.AppendReq.ProposedMessage(
-                        id=grpc_shared.UUID(string=str(uuid4())),
+                        id=grpc_shared.UUID(string=str(event.id)),
                         metadata={
                             "type": event.type,
-                            "content-type": "application/octet-stream",
+                            "content-type": event.content_type,
                         },
                         custom_metadata=event.metadata,
                         data=event.data,
                     )
                 )
             )
 
@@ -359,25 +365,26 @@
 
     def __next__(self) -> RecordedEvent:
         while True:
             response = next(self.resp)
             assert isinstance(response, grpc_persistent.ReadResp)
             if response.WhichOneof("content") == "event":
                 event = response.event.event
-                stream_name = event.stream_identifier.stream_name.decode("utf8")
-                if stream_name.startswith("$"):
-                    continue
+                assert response.event.WhichOneof("position") == "commit_position"
+                commit_position = response.event.commit_position
+
                 return RecordedEvent(
                     id=UUID(event.id.string),
-                    type=event.metadata["type"],
+                    type=event.metadata.get("type", ""),
                     data=event.data,
                     metadata=event.custom_metadata,
-                    stream_name=stream_name,
+                    content_type=event.metadata.get("content-type", ""),
+                    stream_name=event.stream_identifier.stream_name.decode("utf8"),
                     stream_position=event.stream_revision,
-                    commit_position=response.event.commit_position,
+                    commit_position=commit_position,
                 )
 
 
 class Subscriptions:
     """
     Encapsulates the 'Subscriptions' gRPC service.
     """
```

### Comparing `esdbclient-0.8/esdbclient/exceptions.py` & `esdbclient-0.9/esdbclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/code_pb2.py` & `esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/code_pb2.pyi` & `esdbclient-0.9/esdbclient/protos/Grpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/persistent_pb2.py` & `esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/persistent_pb2.pyi` & `esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/persistent_pb2_grpc.py` & `esdbclient-0.9/esdbclient/protos/Grpc/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/shared_pb2.py` & `esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/shared_pb2.pyi` & `esdbclient-0.9/esdbclient/protos/Grpc/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/status_pb2.py` & `esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/status_pb2.pyi` & `esdbclient-0.9/esdbclient/protos/Grpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/streams_pb2.py` & `esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/streams_pb2.pyi` & `esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/esdbclient/protos/Grpc/streams_pb2_grpc.py` & `esdbclient-0.9/esdbclient/protos/Grpc/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-0.8/pyproject.toml` & `esdbclient-0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdbclient"
-version = "0.8"
+version = "0.9"
 description = "Python gRPC Client for EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `esdbclient-0.8/setup.py` & `esdbclient-0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,1353 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: esdbclient
+Version: 0.9
+Summary: Python gRPC Client for EventStoreDB
+Home-page: https://github.com/pyeventsourcing/esdbclient
+License: BSD 3-Clause
+Author: John Bywater
+Author-email: john.bywater@appropriatesoftware.net
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: grpcio (>=1.51.0,<1.52.0)
+Requires-Dist: protobuf (>=4.21.0,<5.0.0)
+Requires-Dist: typing_extensions
+Project-URL: Repository, https://github.com/pyeventsourcing/esdbclient
+Description-Content-Type: text/markdown
 
-packages = \
-['esdbclient', 'esdbclient.protos.Grpc']
+# Python gRPC Client for EventStoreDB
 
-package_data = \
-{'': ['*']}
+This package provides a Python gRPC client for
+[EventStoreDB](https://www.eventstore.com/).
 
-install_requires = \
-['grpcio>=1.51.0,<1.52.0', 'protobuf>=4.21.0,<5.0.0', 'typing_extensions']
-
-setup_kwargs = {
-    'name': 'esdbclient',
-    'version': '0.8',
-    'description': 'Python gRPC Client for EventStoreDB',
-    'long_description': '# Python gRPC Client for EventStoreDB\n\nThis package provides a Python gRPC client for\n[EventStoreDB](https://www.eventstore.com/).\n\nThis client has been developed and tested to work with EventStoreDB LTS\nversions 21.10 and 21.10, without and without SSL/TLS enabled on both\nthese versions, and with Python versions 3.7, 3.8, 3.9, 3.10, and 3.11\nacross all of the above. The test coverage is 100% including branch coverage.\n\nAll the code in this package has typing annotations. The static typing\nannotations checked relatively strictly with mypy.\n\nNot all the features of the EventStoreDB API are presented\nby this client in its current form, however many of the most\nuseful aspects are presented in an easy-to-use interface (see below).\nFor an example of usage, see the [eventsourcing-eventstoredb](\nhttps://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.\n\n## Table of contents\n\n<!-- TOC -->\n* [Installation](#installation)\n* [Server](#server)\n  * [Start EventStoreDB](#start-eventstoredb)\n  * [Stop EventStoreDB](#stop-eventstoredb)\n* [Client](#client)\n* [Streams](#streams)\n  * [Append events](#append-events)\n  * [Get current stream position](#get-current-stream-position)\n  * [Read stream events](#read-stream-events)\n  * [Read all recorded events](#read-all-recorded-events)\n  * [Get current commit position](#get-current-commit-position)\n* [Subscriptions](#subscriptions)\n  * [Catch-up subscriptions](#catch-up-subscriptions)\n  * [Persistent subscriptions](#persistent-subscriptions)\n* [Notes](#notes)\n  * [Regular expression filters](#regular-expression-filters)\n  * [The NewEvent class](#the-newevent-class)\n  * [The RecordedEvent class](#the-recordedevent-class)\n* [Contributors](#contributors)\n  * [Install Poetry](#install-poetry)\n  * [Setup for PyCharm users](#setup-for-pycharm-users)\n  * [Setup from command line](#setup-from-command-line)\n  * [Project Makefile commands](#project-makefile-commands)\n<!-- TOC -->\n\n## Installation\n\nUse pip to install this package from\n[the Python Package Index](https://pypi.org/project/esdbclient/).\n\n    $ pip install esdbclient\n\nIt is recommended to install Python packages into a Python virtual environment.\n\n\n## Server\n\n### Start EventStoreDB\n\nUse Docker to run EventStoreDB using the official Docker container image on DockerHub.\n\nFor development, you can start a "secure" server locally on port 2113 using the following command.\n\n    $ docker run -d --name my-eventstoredb -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:22.10.0-buster-slim --dev\n\nAlternatively, you can start an "insecure" server locally on port 2113 using the following command.\n\n    $ docker run -d --name my-eventstoredb -it -p 2113:2113 eventstore/eventstore:22.10.0-buster-slim --insecure\n\nTo connect to the "insecure" local server using the client in this package, you just need\nto know the local hostname and the port number. To connect to the "secure" local\ndevelopment server, you will also need to know that the username is "admin" and\nthe password is "changeit". You will also need to get the SSL/TLS certificate from\nthe server. You can get the server certificate with the following command.\n\n    $ python -c "import ssl; print(get_server_certificate(addr=(\'localhost\', 2113)))"\n\n\n### Stop EventStoreDB\n\nTo stop and remove the `my-eventstoredb` container created above, use the following Docker commands.\n\n    $ docker stop my-eventstoredb\n\t$ docker rm my-eventstoredb\n\n\n## Client\n\nThe `EsdbClient` class can be imported from the `esdbclient` package.\n\n```python\nfrom esdbclient import EsdbClient\n```\n\nThe `EsdbClient` class can be constructed with `host` and `port` arguments.\nThe `host` and `port` arguments indicate the hostname and port number of the\nEventStoreDB server.\n\nIf the EventStoreDB server is "secure", then also use the `server_cert`,\n`username` and `password` arguments.\n\nThe `host` argument is expected to be a Python `str`. The `port` argument is expected\nto be a Python `int`. The `server_cert` is expected to be a Python `str` containing\nthe PEM encoded SSL/TLS server certificate. Both `username` and `password` are expected\nto be a Python `str`.\n\nIn the example below, the constructor argument values are taken from the operating\nsystem environment, because the examples in this document are tested with both\na "secure" and an "insecure" server.\n\n```python\nimport os\n\nclient = EsdbClient(\n    host=os.getenv("ESDB_HOST"),\n    port=int(os.getenv("ESDB_PORT")),\n    server_cert=os.getenv("ESDB_SERVER_CERT"),\n    username=os.getenv("ESDB_USERNAME"),\n    password=os.getenv("ESDB_PASSWORD"),\n)\n```\n\n## Streams\n\nIn EventStoreDB, a "stream" is a sequence of recorded events that all have\nthe same "stream name". Each recorded event has a "position" in its stream.\nThe positions of the recorded events in a stream is a gapless sequence starting\nfrom zero.\n\n### Append events\n\nThe client has an `append_events()` method, which can be used to append\nnew events to a "stream".\n\nThree arguments are required, `stream_name`, `expected_position`\nand `events`.\n\nThe `stream_name` argument is required, and is expected to be a Python\n`str` object that uniquely identifies the stream in the database.\n\nThe `expected_position` argument is required, is expected to be: either `None`\nif new events are being appended to a new stream, or an integer equal to the\nposition the last recorded event in the stream.\n\nThe stream positions of recorded events start from zero. And so, when appending\nthe second new event to a stream that has one recorded event, the correct value\nof the `expected_position` argument is `0`. Similarly, when appending the third\nnew event to a stream that has two recorded events, the correct value\nof the `expected_position` argument is `1`.\n\nStreams are created by appending events. The correct value of the `expected_position`\nargument when appending the first event of a new stream (a stream with zero recorded\nevents) is `None`. Please note, it is not possible to create an "empty" stream in\nEventStoreDB.\n\nIf there is a mismatch between the given value of the `expected_position` argument\nand the position of the last recorded event in a stream, then an `ExpectedPositionError`\nexception will be raised. This effectively accomplishes optimistic concurrency control.\n\nIf you wish to disable optimistic concurrency control when appending new events, you\ncan set the `expected_position` to a negative integer.\n\nIf you need to discover the current position of the last recorded event in a stream,\nyou can use the `get_stream_position()` method (see below).\n\nThe `events` argument is required, and is expected to be a sequence of new\nevent objects to be appended to the named stream. The `NewEvent` class should\nbe used to construct new event objects (see below).\n\nPlease note, the append events operation is atomic, so that either all\nor none of the given new events will be recorded. By design, it is only\npossible with EventStoreDB to atomically record new events in one stream.\n\nIn the example below, a new event is appended to a new stream.\n\n```python\nfrom uuid import uuid4\n\nfrom esdbclient import NewEvent\n\n# Construct new event object.\nevent1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'data1\',\n    metadata=b\'{}\'\n)\n\n# Define stream name.\nstream_name1 = str(uuid4())\n\n# Append list of events to new stream.\ncommit_position1 = client.append_events(\n    stream_name=stream_name1,\n    expected_position=None,\n    events=[event1],\n)\n```\n\nIn the example below, two subsequent events are appended to an existing\nstream.\n\n```python\nevent2 = NewEvent(\n    type=\'OrderUpdated\',\n    data=b\'data2\',\n    metadata=b\'{}\',\n)\nevent3 = NewEvent(\n    type=\'OrderDeleted\',\n    data=b\'data3\',\n    metadata=b\'{}\',\n)\n\ncommit_position2 = client.append_events(\n    stream_name=stream_name1,\n    expected_position=0,\n    events=[event2, event3],\n)\n```\n\nIf the append operation is successful, this method returns an integer\nrepresenting the overall "commit position" as it was when the operation\nwas completed. Otherwise, an exception will be raised.\n\nA "commit position" is a monotonically increasing integer representing\nthe position of the recorded event in a "total order" of all recorded\nevents in the database across all streams. The sequence of commit positions\nis not gapless. It represents the position of the event record on disk, and\nthere are usually large differences between successive commits.\n\nThe "commit position" returned in this way can be used to wait for a\ndownstream component to have processed the newly appended events.\nFor example, after a user interface command that results in the recording\nof new events, and before a query is issued that depends on an eventually\nconsistent materialized view in a downstream component that would be stale\nif those newly appended events have not yet been processed, the user interface\ncan poll the downstream component, to see if it has processed an event at that\ncommit position, before executing a query for that materialized view.\n\n### Get current stream position\n\nThe client has a `get_stream_position()` method, which can be used to\nget the current "stream position" of a stream (the position in the\nstream of the last recorded event in that stream).\n\nThis method has a `stream_name` argument, which is required.\n\nThis method also takes an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe sequence of positions in a stream is gapless. It is zero-based,\nso that a stream with one recorded event has a current stream\nposition of `0`. The current stream position is `1` when a stream has\ntwo events, and it is `2` when there are events, and so on.\n\nIn the example below, the current stream position is obtained of the\nstream to which events were appended in the examples above.\nBecause the sequence of stream positions is zero-based, and because\nthree events were appended, so the current stream position is `2`.\n\n```python\nstream_position = client.get_stream_position(\n    stream_name=stream_name1\n)\n\nassert stream_position == 2\n```\n\nIf a stream does not exist, the returned stream position value is `None`,\nwhich matches the required expected position when appending the first event\nof a new stream (see above).\n\n```python\nstream_position = client.get_stream_position(\n    stream_name=str(uuid4())\n)\n\nassert stream_position == None\n```\n\nThis method takes an optional argument `timeout` which is a float that sets\na deadline for the completion of the gRPC operation.\n\n\n### Read stream events\n\nThe client has a `read_stream_events()` method, which can be used to read\nthe events of a stream.\n\nThis method returns nn iterable object that yields recorded event objects.\nThese recorded event objects are instances of the `RecordedEvent` class (see below)\n\nThis method has one required argument, `stream_name`, which is the name of\nthe stream to be read. By default, the recorded events in the stream\nare returned in the order they were recorded.\n\nThe example below shows how to read the recorded events of a stream\nforwards from the start of the stream to the end of the stream. The\nname of a stream is given when calling the method. In this example,\nthe iterable response object is converted into a Python `list`, which\ncontains all the recorded event objects that were read from the stream.\n\n```python\nresponse = client.read_stream_events(\n    stream_name=stream_name1\n)\n\nevents = list(response)\n```\n\nNow that we have a list of event objects, we can check we got the\nthree events that were appended to the stream, and that they are\nordered exactly as they were appended.\n\n```python\nassert len(events) == 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n\nassert events[2].stream_name == stream_name1\nassert events[2].stream_position == 2\nassert events[2].type == event3.type\nassert events[2].data == event3.data\n```\n\nThe method `read_stream_events()` also supports four optional arguments,\n`position`, `backwards`, `limit`, and `timeout`.\n\nThe optional `position` argument is an optional integer that can be used to indicate\nthe position in the stream from which to start reading. This argument is `None`\nby default, which means the stream will be read either from the start of the\nstream (the default behaviour), or from the end of the stream if `backwards` is\n`True` (see below). When reading a stream from a specific position in the stream, the\nrecorded event at that position WILL be included, both when reading forwards\nfrom that position, and when reading backwards from that position.\n\nThe optional argument `backwards` is a boolean, by default `False`, which means the\nstream will be read forwards by default, so that events are returned in the\norder they were appended, If `backwards` is `True`, the stream will be read\nbackwards, so that events are returned in reverse order.\n\nThe optional argument `limit` is an integer which limits the number of events that will\nbe returned. The default value is `sys.maxint`.\n\nThe optional argument `timeout` is a float which sets a deadline for the completion of\nthe gRPC operation.\n\nThe example below shows how to read recorded events in a stream forwards from\na specific stream position to the end of the stream.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        position=1,\n    )\n)\n\nassert len(events) == 2\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 1\nassert events[0].type == event2.type\nassert events[0].data == event2.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 2\nassert events[1].type == event3.type\nassert events[1].data == event3.data\n```\n\nThe example below shows how to read the recorded events in a stream backwards from\nthe end of the stream to the start of the stream.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        backwards=True,\n    )\n)\n\nassert len(events) == 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n```\n\nThe example below shows how to read a limited number (two) of the recorded events\nin a stream forwards from the start of the stream.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        limit=2,\n    )\n)\n\nassert len(events) == 2\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n```\n\nThe example below shows how to read a limited number (one) of the recorded\nevents in a stream backwards from a given stream position.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        position=2,\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n```\n\n### Read all recorded events\n\nThe method `read_all_events()` can be used to read all recorded events\nin the database in the order they were recorded. An iterable object of\nrecorded events is returned. This iterable object will stop when it has\nyielded the last recorded event.\n\nThe method `read_stream_events()` supports six optional arguments,\n`commit_position`, `backwards`, `filter_exclude`, `filter_include`, `limit`,\nand `timeout`.\n\nThe optional argument `position` is an optional integer that can be used to specify\nthe commit position from which to start reading. This argument is `None` by\ndefault, meaning that all the events will be read either from the start, or\nfrom the end if `backwards` is `True` (see below). Please note, if specified,\nthe specified position must be an actually existing commit position, because\nany other number will result in a server error (at least in EventStoreDB v21.10).\n\nPlease also note, when reading forwards from a specific commit position, the event\nat the specified position WILL be included. However, when reading backwards, the\nevent at the specified position will NOT be included. (This non-inclusive behaviour\nof excluding the specified commit position when reading all streams differs from the\nbehaviour when reading a named stream backwards from a specific stream position, I\'m\nnot sure why.)\n\nThe optional argument `backwards` is a boolean which is by default `False` meaning the\nevents will be read forwards by default, so that events are returned in the\norder they were committed, If `backwards` is `True`, the events will be read\nbackwards, so that events are returned in reverse order.\n\nThe optional argument `filter_exclude` is a sequence of regular expressions that\nmatch the type strings of recorded events that should not be included. By default,\nthis argument will match "system events", so that they will not be included.\nThis argument is ignored if `filter_include` is set to a non-empty sequence.\n\nThe optional argument `filter_include` is a sequence of regular expressions\nthat match the type strings of recorded events that should be included. By\ndefault, this argument is an empty tuple. If this argument is set to a\nnon-empty sequence, the `filter_exclude` argument is ignored.\n\nPlease note, the filtering happens on the EventStoreDB server, and the\n`limit` argument is applied on the server after filtering. See below for\nmore information about filter regular expressions.\n\nThe optional argument `limit` is an integer which limits the number of events that will\nbe returned. The default value is `sys.maxint`.\n\nThe optional argument `timeout` is a float which sets a deadline for the completion of\nthe gRPC operation.\n\nThe example below shows how to read all events in the database in the\norder they were recorded.\n\n```python\nevents = list(client.read_all_events())\n\nassert len(events) >= 3\n```\n\nThe example below shows how to read all recorded events from a particular commit position.\n\n```python\nevents = list(\n    client.read_all_events(\n        commit_position=commit_position1\n    )\n)\n\nassert len(events) == 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n\nassert events[2].stream_name == stream_name1\nassert events[2].stream_position == 2\nassert events[2].type == event3.type\nassert events[2].data == event3.data\n```\n\nThe example below shows how to read all recorded events in reverse order.\n\n```python\nevents = list(\n    client.read_all_events(\n        backwards=True\n    )\n)\n\nassert len(events) >= 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n\nassert events[2].stream_name == stream_name1\nassert events[2].stream_position == 0\nassert events[2].type == event1.type\nassert events[2].data == event1.data\n```\n\nThe example below shows how to read a limited number (one) of the recorded events\nin the database forwards from a specific commit position. Please note, when reading\nall events forwards from a specific commit position, the event at the specified\nposition WILL be included.\n\n\n```python\nevents = list(\n    client.read_all_events(\n        commit_position=commit_position1,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[0].commit_position == commit_position1\n```\n\nThe example below shows how to read a limited number (one) of the recorded events\nin the database backwards from the end. This gives the last recorded event.\n\n```python\nevents = list(\n    client.read_all_events(\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n```\n\nThe example below shows how to read a limited number (one) of the recorded events\nin the database backwards from a specific commit position. Please note, when reading\nall events backwards from a specific commit position, the event at the specified\nposition WILL NOT be included.\n\n```python\nevents = list(\n    client.read_all_events(\n        commit_position=commit_position2,\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].commit_position < commit_position2\n```\n\n### Get current commit position\n\nThe method `get_commit_position()` can be used to get the current\ncommit position of the database.\n\n```python\ncommit_position = client.get_commit_position()\n```\n\nThis method takes an optional argument `timeout` which is a float that sets\na deadline for the completion of the gRPC operation.\n\nThis method can be useful to measure progress of a downstream component\nthat is processing all recorded events, by comparing the current commit\nposition with the recorded commit position of the last successfully processed\nevent in a downstream component.\n\nThe value of the `commit_position` argument when reading events either by using\nthe `read_all_events()` method or by using a catch-up subscription would usually\nbe determined by the recorded commit position of the last successfully processed\nevent in a downstream component.\n\n## Subscriptions\n\n### Catch-up subscriptions\n\nThe client has a `subscribe_all_events()` method, which can be used\nto start a "catch-up" subscription.\n\nMany catch-up subscriptions can be created, concurrently or\nsuccessively, and all will receive all the events they are\nsubscribed to receive.\n\nThis method returns an iterator object which yields recorded events,\nincluding events that are recorded after the subscription was created.\nThis iterator object will therefore not stop, unless the connection\nto the database is lost. The connection will be closed when the\niterator object is deleted from memory, which will happen when the\niterator object goes out of scope is explicitly deleted (see below),\nand the connection may be closed by the server.\n\nThis method takes an optional `commit_position` argument, which can be\nused to specify a commit position from which to subscribe for\nrecorded events. The default value is `None`, which means\nthe subscription will operate from the first recorded event\nin the database. If a commit position is given, it must match\nan actually existing commit position in the database. The events\nthat are obtained will not include the event recorded at that commit\nposition.\n\nThis method also takes three other optional arguments, `filter_exclude`,\n`filter_include`, and `timeout`.\n\nThe argument `filter_exclude` is a sequence of regular expressions matching\nthe type strings of recorded events that should be excluded. By default,\nthis argument will match "system events", so that they will not be included.\nThis argument is ignored if `filter_include` is set to a non-empty sequence.\n\nThe argument `filter_include` is a sequence of regular expressions\nmatching the type strings of recorded events that should be included. By\ndefault, this argument is an empty tuple. If this argument is set to a\nnon-empty sequence, the `filter_exclude` argument is ignored.\n\nPlease note, the filtering happens on the EventStoreDB server, and the\n`limit` argument is applied on the server after filtering. See below for\nmore information about filter regular expressions.\n\nThe argument `timeout` is a float which sets a deadline for the completion of\nthe gRPC operation. This probably isn\'t very useful, but is included for\ncompleteness and consistency with the other methods.\n\nThe example below shows how to subscribe to receive all recorded\nevents from a specific commit position. Three already-recorded\nevents are received, and then three new events are recorded, which\nare then received via the subscription.\n\n```python\n\n# Get the commit position (usually from database of materialised views).\ncommit_position = client.get_commit_position()\n\n# Append three events to another stream.\nstream_name2 = str(uuid4())\nevent4 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'data4\',\n    metadata=b\'{}\',\n)\nevent5 = NewEvent(\n    type=\'OrderUpdated\',\n    data=b\'data5\',\n    metadata=b\'{}\',\n)\nevent6 = NewEvent(\n    type=\'OrderDeleted\',\n    data=b\'data6\',\n    metadata=b\'{}\',\n)\nclient.append_events(\n    stream_name=stream_name2,\n    expected_position=None,\n    events=[event4, event5, event6],\n)\n\n# Subscribe from the commit position.\nsubscription = client.subscribe_all_events(\n    commit_position=commit_position\n)\n\n# Catch up by receiving the three events from the subscription.\nevents = []\nfor event in subscription:\n    events.append(event)\n    if event.data == event6.data and event.stream_name:\n        break\n\nassert events[0].data == event4.data\nassert events[1].data == event5.data\nassert events[2].data == event6.data\n\n\n# Append three more events.\nstream_name3 = str(uuid4())\nevent7 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'data7\',\n    metadata=b\'{}\',\n)\nevent8 = NewEvent(\n    type=\'OrderUpdated\',\n    data=b\'data8\',\n    metadata=b\'{}\',\n)\nevent9 = NewEvent(\n    type=\'OrderDeleted\',\n    data=b\'data9\',\n    metadata=b\'{}\',\n)\n\nclient.append_events(\n    stream_name=stream_name3,\n    expected_position=None,\n    events=[event7, event8, event9],\n)\n\n# Receive the three new events from the same subscription.\nfor event in subscription:\n    # Check the stream name.\n    events.append(event)\n    if event.stream_name == stream_name3:\n        if event.data == event9.data:\n            break\n\nassert events[3].data == event7.data\nassert events[4].data == event8.data\nassert events[5].data == event9.data\n```\n\nCatch-up subscriptions are not registered in EventStoreDB (they are not\n"persistent" subscriptions). It is simply a streaming gRPC call which is\nkept open by the server, with newly recorded events sent to the client\nas the client iterates over the subscription. This kind of subscription\nis closed as soon as the subscription object goes out of memory.\n\n```python\n# End the subscription.\ndel subscription\n```\n\nPlease note, when processing events in a downstream component, the commit position of\nthe last successfully processed event is usefully recorded by the downstream component\nso that the commit position can be determined by the downstream component from its own\nrecorded when it is restarted. This commit position can be used to specify the commit\nposition from which to subscribe. Since this commit position represents the position of\nthe last successfully processed event in a downstream component, so it will be usual to\nwant the next event after this position, because that is the next event that needs to\nbe processed. When subscribing for events using a catchup-subscription\nin EventStoreDB, the event at the specified commit position will NOT be included in\nthe sequence of recorded events.\n\nTo accomplish "exactly once" processing of the events, the commit position\nof a recorded event should be recorded atomically and uniquely along with\nthe result of processing recorded events, for example in the same database\nas materialised views when implementing eventually-consistent CQRS, or in\nthe same database as a downstream analytics or reporting or archiving\napplication. This avoids "dual writing" in the processing of events.\n\nRecorded events received from a catch-up subscription cannot be acknowledged back\nto the EventStoreDB server (there is no need to do this). Acknowledging events is\nan aspect of "persistent subscriptions" (see below).\n\nThe subscription object might be used directly when processing events. It might\nalso be used within a thread dedicated to receiving events, with recorded events\nput on a queue for processing in a different thread. This package doesn\'t provide\nsuch thread or queue objects, you would need to do that yourself. Just make sure\nto reconstruct the subscription (and the queue) using your last recorded commit\nposition when resuming the subscription after an error, to be sure all events\nare processed once.\n\n### Persistent subscriptions\n\nThe method `create_subscription()` can be used to create a\n"persistent subscription" to EventStoreDB.\n\nThis method takes a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription.\n\nThis method takes an optional `from_end` argument, which can be\nused to specify that the group of consumers of the subscription should\nonly receive events that were recorded after the subscription was created.\n\nThis method takes an optional `commit_position` argument, which can be\nused to specify a commit position from which the group of consumers of\nthe subscription should receive events. Please note, the recorded event\nat the specified commit position MAY be included in the recorded events\nreceived by the group of consumers.\n\nIf neither `from_end` or `position` are specified, the group of consumers\nof the subscription will receive all recorded events.\n\nThe method `create_subscription()` does not return a value, because\nrecorded events are obtained by the group of consumers of the subscription\nusing the `read_subscription()` method.\n\nIn the example below, a persistent subscription is created.\n\n```python\n# Create a persistent subscription.\ngroup_name = f"group-{uuid4()}"\nclient.create_subscription(group_name=group_name)\n```\n\nThe method `read_subscription()` can be used by a group of consumers to receive\nrecorded events from a persistent subscription created using `create_subscription`.\n\nThis method takes a required `group_name` argument, which is\nthe name of a "group" of consumers of the subscription specified\nwhen `create_subscription()` was called.\n\nThis method returns a 2-tuple: a "read request" object and a "read response" object.\n\n```python\nread_req, read_resp = client.read_subscription(group_name=group_name)\n```\n\nThe "read response" object is an iterator that yields recorded events from\nthe specified commit position.\n\nThe "read request" object has an `ack()` method that can be used by a consumer\nin a group to acknowledge to the server that it has received and successfully\nprocessed a recorded event. This will prevent that recorded event being received\nby another consumer in the same group. The `ack()` method takes an `event_id`\nargument, which is the ID of the recorded event that has been received.\n\nThe example below iterates over the "read response" object, and calls `ack()`\non the "read response" object. The for loop breaks when we have received\nthe last event, so that we can continue with the examples below.\n\n```python\nevents = []\nfor event in read_resp:\n    events.append(event)\n\n    # Acknowledge the received event.\n    read_req.ack(event_id=event.id)\n\n    # Break when the last event has been received.\n    if event.stream_name == stream_name3:\n        if event.data == event9.data:\n            break\n```\n\nThe received events are the events we appended above.\n\n```python\nassert events[-9].data == event1.data\nassert events[-8].data == event2.data\nassert events[-7].data == event3.data\nassert events[-6].data == event4.data\nassert events[-5].data == event5.data\nassert events[-4].data == event6.data\nassert events[-3].data == event7.data\nassert events[-2].data == event8.data\nassert events[-1].data == event9.data\n```\n\nThe "read request" object also has an `nack()` method that can be used by a consumer\nin a group to acknowledge to the server that it has failed successfully to\nprocess a recorded event. This will allow that recorded event to be received\nby this or another consumer in the same group.\n\nIt might be more useful to encapsulate the request and response objects and to iterate\nover the "read response" in a separate thread, to call back to a handler function when\na recorded event is received, and call `ack()` if the handler does not raise an\nexception, and to call `nack()` if an exception is raised. The example below shows how\nthis might be done.\n\n```python\nfrom threading import Thread\n\n\nclass SubscriptionReader:\n    def __init__(self, client, group_name, callback):\n        self.client = client\n        self.group_name = group_name\n        self.callback = callback\n        self.thread = Thread(target=self.read_subscription, daemon=True)\n        self.error = None\n\n    def start(self):\n        self.thread.start()\n\n    def join(self):\n        self.thread.join()\n\n    def read_subscription(self):\n        req, resp = self.client.read_subscription(group_name=self.group_name)\n        for event in resp:\n            try:\n                self.callback(event)\n            except Exception as e:\n                # req.nack(event.id)  # not yet implemented....\n                self.error = e\n                break\n            else:\n                req.ack(event.id)\n\n\n# Create another persistent subscription.\ngroup_name = f"group-{uuid4()}"\nclient.create_subscription(group_name=group_name)\n\nevents = []\n\ndef handle_event(event):\n    events.append(event)\n    if event.stream_name == stream_name3:\n        if event.data == event9.data:\n            raise Exception()\n\n\nreader = SubscriptionReader(\n    client=client,\n    group_name=group_name,\n    callback=handle_event\n)\n\nreader.start()\nreader.join()\n\nassert events[-1].data == event9.data\n```\n\nPlease note, when processing events in a downstream component, the commit position of\nthe last successfully processed event is usefully recorded by the downstream component\nso that the commit position can be determined by the downstream component from its own\nrecorded when it is restarted. This commit position can be used to specify the commit\nposition from which to subscribe. Since this commit position represents the position of\nthe last successfully processed event in a downstream component, so it will be usual to\nwant to read from the next event after this position, because that is the next event\nthat needs to be processed. However, when subscribing for events using a persistent\nsubscription in EventStoreDB, the event at the specified commit position MAY be returned\nas the first event in the received sequence of recorded events, and so it may\nbe necessary to check the commit position of the received events and to discard\nany  recorded event object that has a commit position equal to the commit position\nspecified in the request.\n\nWhilst there are some advantages of persistent subscriptions, by tracking in the\nupstream server the position in the commit sequence of events that have been processed,\nthere is a danger of "dual writing" in the consumption of events. The danger is that if\nan event is successfully processed but then the acknowledgment fails, the event may be\nreceived more than once. On the other hand, if the acknowledgment is successful but\nthen the processing fails, the event may effectively not be been processed. By either\nprocessing an events more than once, or failing to process an event, the resulting state\nof the processing of the recorded events might be inaccurate, or possibly\ninconsistent, and perhaps catastrophically so. Any relatively minor consequences may or\nmay not matter in your situation. But sometimes inconsistencies may halt processing\nuntil the issue is resolved. You can avoid "dual writing" in the consumption of events\nby atomically recording the commit position of an event that has been processed along\nwith the results of processing that event (that is, with both things being recorded in\nthe same transaction), and making these records unique so that transactions will be\nrolled back preventing the results of reprocessing the event being committed.\n\n## Notes\n\n### Regular expression filters\n\nThe `filter_exclude` and `filter_include` arguments in `read_all_events()` and\n`subscribe_all_events()` are applied to the `type` attribute of recorded events.\n\nThe default value of the `filter_exclude` arguments is designed to exclude\nEventStoreDB "system events", which otherwise would be included. System\nevents, by convention in EventStoreDB, all have `type` strings that\nstart with the `$` sign.\n\nPlease note, characters that have a special meaning in regular expressions\nwill need to be escaped (with double-backslash) when matching these characters\nin type strings.\n\nFor example, to match EventStoreDB system events, use the sequence `[\'\\\\$.*\']`.\nPlease note, the constant `ESDB_EVENTS_REGEX` is set to `\'\\\\$.*\'`. You\ncan import this value (`from esdbclient import ESDB_EVENTS_REGEX`) and use\nit when building longer sequences of regular expressions. For example,\nto exclude system events and snapshots, you might use the sequence\n`[ESDB_EVENTS_REGEX, \'.*Snapshot\']` as the value of the `filter_exclude`\nargument.\n\n\n### The NewEvent class\n\nThe `NewEvent` class can be used to define new events.\n\nThe attribute `type` is a unicode string, used to specify the type of the event\nto be recorded.\n\nThe attribute `data` is a byte string, used to specify the data of the event\nto be recorded. Please note, in this version of this Python client,\nwriting JSON event data to EventStoreDB isn\'t supported, but it might be in\na future version.\n\nThe attribute `metadata` is a byte string, used to specify metadata for the event\nto be recorded.\n\n```python\nnew_event = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'{}\',\n    metadata=b\'{}\',\n)\n```\n\n### The RecordedEvent class\n\nThe `RecordedEvent` class is used when reading recorded events.\n\nThe attribute `type` is a unicode string, used to indicate the type of the event\nthat was recorded.\n\nThe attribute `data` is a byte string, used to indicate the data of the event\nthat was recorded.\n\nThe attribute `metadata` is a byte string, used to indicate metadata for the event\nthat was recorded.\n\nThe attribute `stream_name` is a unicode string, used to indicate the type of\nthe name of the stream in which the event was recorded.\n\nThe attribute `stream_position` is an integer, used to indicate\nthe position in the stream at which the event was recorded.\n\nThe attribute `commit_position` is an integer, used to indicate\nthe position in total order of all recorded events at which the\nevent was recorded.\n\n```python\nfrom esdbclient.events import RecordedEvent\n\nrecorded_event = RecordedEvent(\n    id=uuid4(),\n    type=\'OrderCreated\',\n    data=b\'{}\',\n    metadata=b\'{}\',\n    stream_name=\'stream1\',\n    stream_position=0,\n    commit_position=512,\n)\n```\n\n## Contributors\n\n### Install Poetry\n\nThe first thing is to check you have Poetry installed.\n\n    $ poetry --version\n\nIf you don\'t, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\n    $ curl -sSL https://install.python-poetry.org | python3 -\n\nIt will help to make sure Poetry\'s bin directory is in your `PATH` environment variable.\n\nBut in any case, make sure you know the path to the `poetry` executable. The Poetry\ninstaller tells you where it has been installed, and how to configure your shell.\n\nPlease refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on\nusing Poetry.\n\n### Setup for PyCharm users\n\nYou can easily obtain the project files using PyCharm (menu "Git > Clone...").\nPyCharm will then usually prompt you to open the project.\n\nOpen the project in a new window. PyCharm will then usually prompt you to create\na new virtual environment.\n\nCreate a new Poetry virtual environment for the project. If PyCharm doesn\'t already\nknow where your `poetry` executable is, then set the path to your `poetry` executable\nin the "New Poetry Environment" form input field labelled "Poetry executable". In the\n"New Poetry Environment" form, you will also have the opportunity to select which\nPython executable will be used by the virtual environment.\n\nPyCharm will then create a new Poetry virtual environment for your project, using\na particular version of Python, and also install into this virtual environment the\nproject\'s package dependencies according to the `pyproject.toml` file, or the\n`poetry.lock` file if that exists in the project files.\n\nYou can add different Poetry environments for different Python versions, and switch\nbetween them using the "Python Interpreter" settings of PyCharm. If you want to use\na version of Python that isn\'t installed, either use your favourite package manager,\nor install Python by downloading an installer for recent versions of Python directly\nfrom the [Python website](https://www.python.org/downloads/).\n\nOnce project dependencies have been installed, you should be able to run tests\nfrom within PyCharm (right-click on the `tests` folder and select the \'Run\' option).\n\nBecause of a conflict between pytest and PyCharm\'s debugger and the coverage tool,\nyou may need to add ``--no-cov`` as an option to the test runner template. Alternatively,\njust use the Python Standard Library\'s ``unittest`` module.\n\nYou should also be able to open a terminal window in PyCharm, and run the project\'s\nMakefile commands from the command line (see below).\n\n### Setup from command line\n\nObtain the project files, using Git or suitable alternative.\n\nIn a terminal application, change your current working directory\nto the root folder of the project files. There should be a Makefile\nin this folder.\n\nUse the Makefile to create a new Poetry virtual environment for the\nproject and install the project\'s package dependencies into it,\nusing the following command.\n\n    $ make install-packages\n\nIt\'s also possible to also install the project in \'editable mode\'.\n\n    $ make install\n\nPlease note, if you create the virtual environment in this way, and then try to\nopen the project in PyCharm and configure the project to use this virtual\nenvironment as an "Existing Poetry Environment", PyCharm sometimes has some\nissues (don\'t know why) which might be problematic. If you encounter such\nissues, you can resolve these issues by deleting the virtual environment\nand creating the Poetry virtual environment using PyCharm (see above).\n\n### Project Makefile commands\n\nYou can start EventStoreDB using the following command.\n\n    $ make start-eventstoredb\n\nYou can run tests using the following command (needs EventStoreDB to be running).\n\n    $ make test\n\nYou can stop EventStoreDB using the following command.\n\n    $ make stop-eventstoredb\n\nYou can check the formatting of the code using the following command.\n\n    $ make lint\n\nYou can reformat the code using the following command.\n\n    $ make fmt\n\nTests belong in `./tests`. Code-under-test belongs in `./esdbclient`.\n\nEdit package dependencies in `pyproject.toml`. Update installed packages (and the\n`poetry.lock` file) using the following command.\n\n    $ make update-packages\n',
-    'author': 'John Bywater',
-    'author_email': 'john.bywater@appropriatesoftware.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pyeventsourcing/esdbclient',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+This client has been developed and tested to work with EventStoreDB LTS
+versions 21.10 and 21.10, without and without SSL/TLS enabled on both
+these versions, and with Python versions 3.7, 3.8, 3.9, 3.10, and 3.11
+across all of the above. The test coverage is 100% including branch coverage.
 
+All the code in this package has typing annotations. The static typing
+annotations checked relatively strictly with mypy.
+
+Not all the features of the EventStoreDB API are presented
+by this client in its current form, however many of the most
+useful aspects are presented in an easy-to-use interface (see below).
+For an example of usage, see the [eventsourcing-eventstoredb](
+https://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.
+
+## Table of contents
+
+<!-- TOC -->
+* [Installation](#installation)
+* [Server](#server)
+  * [Start EventStoreDB](#start-eventstoredb)
+  * [Stop EventStoreDB](#stop-eventstoredb)
+* [Client](#client)
+* [Streams](#streams)
+  * [Append events](#append-events)
+  * [Get current stream position](#get-current-stream-position)
+  * [Read stream events](#read-stream-events)
+  * [Idempotent writes](#idempotent-writes)
+  * [Read all recorded events](#read-all-recorded-events)
+  * [Get current commit position](#get-current-commit-position)
+* [Subscriptions](#subscriptions)
+  * [Catch-up subscriptions](#catch-up-subscriptions)
+  * [Persistent subscriptions](#persistent-subscriptions)
+* [Notes](#notes)
+  * [Regular expression filters](#regular-expression-filters)
+  * [The NewEvent class](#the-newevent-class)
+  * [The RecordedEvent class](#the-recordedevent-class)
+* [Contributors](#contributors)
+  * [Install Poetry](#install-poetry)
+  * [Setup for PyCharm users](#setup-for-pycharm-users)
+  * [Setup from command line](#setup-from-command-line)
+  * [Project Makefile commands](#project-makefile-commands)
+<!-- TOC -->
+
+## Installation
+
+Use pip to install this package from
+[the Python Package Index](https://pypi.org/project/esdbclient/).
+
+    $ pip install esdbclient
+
+It is recommended to install Python packages into a Python virtual environment.
+
+
+## Server
+
+### Start EventStoreDB
+
+Use Docker to run EventStoreDB using the official Docker container image on DockerHub.
+
+For development, you can start a "secure" server locally on port 2113 using the following command.
+
+    $ docker run -d --name my-eventstoredb -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:22.10.0-buster-slim --dev
+
+Alternatively, you can start an "insecure" server locally on port 2113 using the following command.
+
+    $ docker run -d --name my-eventstoredb -it -p 2113:2113 eventstore/eventstore:22.10.0-buster-slim --insecure
+
+To connect to the "insecure" local server using the client in this package, you just need
+to know the local hostname and the port number. To connect to the "secure" local
+development server, you will also need to know that the username is "admin" and
+the password is "changeit". You will also need to get the SSL/TLS certificate from
+the server. You can get the server certificate with the following command.
+
+    $ python -c "import ssl; print(get_server_certificate(addr=('localhost', 2113)))"
+
+
+### Stop EventStoreDB
+
+To stop and remove the `my-eventstoredb` container created above, use the following Docker commands.
+
+    $ docker stop my-eventstoredb
+	$ docker rm my-eventstoredb
+
+
+## Client
+
+The `EsdbClient` class can be imported from the `esdbclient` package.
+
+```python
+from esdbclient import EsdbClient
+```
+
+The `EsdbClient` class can be constructed with `host` and `port` arguments.
+The `host` and `port` arguments indicate the hostname and port number of the
+EventStoreDB server.
+
+If the EventStoreDB server is "secure", then also use the `server_cert`,
+`username` and `password` arguments.
+
+The `host` argument is expected to be a Python `str`. The `port` argument is expected
+to be a Python `int`. The `server_cert` is expected to be a Python `str` containing
+the PEM encoded SSL/TLS server certificate. Both `username` and `password` are expected
+to be a Python `str`.
+
+In the example below, the constructor argument values are taken from the operating
+system environment, because the examples in this document are tested with both
+a "secure" and an "insecure" server.
+
+```python
+import os
+
+client = EsdbClient(
+    host=os.getenv("ESDB_HOST"),
+    port=int(os.getenv("ESDB_PORT")),
+    server_cert=os.getenv("ESDB_SERVER_CERT"),
+    username=os.getenv("ESDB_USERNAME"),
+    password=os.getenv("ESDB_PASSWORD"),
+)
+```
+
+## Streams
+
+In EventStoreDB, a "stream" is a sequence of recorded events that all have
+the same "stream name". Each recorded event has a "position" in its stream.
+The positions of the recorded events in a stream is a gapless sequence starting
+from zero.
+
+### Append events
+
+The client has an `append_events()` method, which can be used to append
+new events to a "stream".
+
+Three arguments are required, `stream_name`, `expected_position`
+and `events`.
+
+The `stream_name` argument is required, and is expected to be a Python
+`str` object that uniquely identifies the stream in the database.
+
+The `expected_position` argument is required, is expected to be: either `None`
+if new events are being appended to a new stream, or an integer equal to the
+position the last recorded event in the stream.
+
+The stream positions of recorded events start from zero. And so, when appending
+the second new event to a stream that has one recorded event, the correct value
+of the `expected_position` argument is `0`. Similarly, when appending the third
+new event to a stream that has two recorded events, the correct value
+of the `expected_position` argument is `1`.
+
+Streams are created by appending events. The correct value of the `expected_position`
+argument when appending the first event of a new stream (a stream with zero recorded
+events) is `None`. Please note, it is not possible to create an "empty" stream in
+EventStoreDB.
+
+If there is a mismatch between the given value of the `expected_position` argument
+and the position of the last recorded event in a stream, then an `ExpectedPositionError`
+exception will be raised. This effectively accomplishes optimistic concurrency control.
+
+If you wish to disable optimistic concurrency control when appending new events, you
+can set the `expected_position` to a negative integer.
+
+If you need to discover the current position of the last recorded event in a stream,
+you can use the `get_stream_position()` method (see below).
+
+The `events` argument is required, and is expected to be a sequence of new
+event objects to be appended to the named stream. The `NewEvent` class should
+be used to construct new event objects (see below).
+
+Please note, the append events operation is atomic, so that either all
+or none of the given new events will be recorded. By design, it is only
+possible with EventStoreDB to atomically record new events in one stream.
+
+In the example below, a new event is appended to a new stream.
+
+```python
+from uuid import UUID, uuid4
+
+from esdbclient import NewEvent
+
+# Construct new event object.
+event1 = NewEvent(
+    type='OrderCreated',
+    data=b'data1',
+)
+
+# Define stream name.
+stream_name1 = str(uuid4())
+
+# Append list of events to new stream.
+commit_position1 = client.append_events(
+    stream_name=stream_name1,
+    expected_position=None,
+    events=[event1],
+)
+```
+
+In the example below, two subsequent events are appended to an existing
+stream.
+
+```python
+event2 = NewEvent(
+    type='OrderUpdated',
+    data=b'data2',
+)
+event3 = NewEvent(
+    type='OrderDeleted',
+    data=b'data3',
+)
+
+commit_position2 = client.append_events(
+    stream_name=stream_name1,
+    expected_position=0,
+    events=[event2, event3],
+)
+```
+
+If the append operation is successful, this method returns an integer
+representing the overall "commit position" as it was when the operation
+was completed. Otherwise, an exception will be raised.
+
+A "commit position" is a monotonically increasing integer representing
+the position of the recorded event in a "total order" of all recorded
+events in the database across all streams. It is the actual position
+of the event record on disk, and there are usually large differences
+between successive commits. The sequence of commit positions
+is NOT gapless.
+
+The "commit position" returned by `append_events()` is that of the last
+recorded event in the given sequence of new events.
+
+The "commit position" returned in this way can therefore be used to wait
+for a downstream component to have processed all the events that were recorded.
+
+For example, consider a user interface command that results in the recording
+of new events, and a query into an eventually consistent materialized
+view in a downstream component that is updated from these events. If the new
+events have not yet been processed, the view would be stale. The "commit position"
+can be used by the user interface to poll the downstream component until it has
+processed the new events, after which time the view will not be stale.
+
+### Get current stream position
+
+The client has a `get_stream_position()` method, which can be used to
+get the current "stream position" of a stream (the position in the
+stream of the last recorded event in that stream).
+
+This method has a `stream_name` argument, which is required.
+
+This method also takes an optional `timeout` argument, that
+is expected to be a Python `float`, which sets a deadline
+for the completion of the gRPC operation.
+
+The sequence of positions in a stream is gapless. It is zero-based,
+so that a stream with one recorded event has a current stream
+position of `0`. The current stream position is `1` when a stream has
+two events, and it is `2` when there are events, and so on.
+
+In the example below, the current stream position is obtained of the
+stream to which events were appended in the examples above.
+Because the sequence of stream positions is zero-based, and because
+three events were appended, so the current stream position is `2`.
+
+```python
+stream_position = client.get_stream_position(
+    stream_name=stream_name1
+)
+
+assert stream_position == 2
+```
+
+If a stream does not exist, the returned stream position value is `None`,
+which matches the required expected position when appending the first event
+of a new stream (see above).
+
+```python
+stream_position = client.get_stream_position(
+    stream_name=str(uuid4())
+)
+
+assert stream_position == None
+```
+
+This method takes an optional argument `timeout` which is a float that sets
+a deadline for the completion of the gRPC operation.
+
+
+### Read stream events
+
+The client has a `read_stream_events()` method, which can be used to read
+the events of a stream.
+
+This method returns nn iterable object that yields recorded event objects.
+These recorded event objects are instances of the `RecordedEvent` class (see below)
+
+This method has one required argument, `stream_name`, which is the name of
+the stream to be read. By default, the recorded events in the stream
+are returned in the order they were recorded.
+
+The example below shows how to read the recorded events of a stream
+forwards from the start of the stream to the end of the stream. The
+name of a stream is given when calling the method. In this example,
+the iterable response object is converted into a Python `list`, which
+contains all the recorded event objects that were read from the stream.
+
+```python
+response = client.read_stream_events(
+    stream_name=stream_name1
+)
+
+events = list(response)
+```
+
+Now that we have a list of event objects, we can check we got the
+three events that were appended to the stream, and that they are
+ordered exactly as they were appended.
+
+```python
+assert len(events) == 3
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 0
+assert events[0].type == event1.type
+assert events[0].data == event1.data
+
+assert events[1].stream_name == stream_name1
+assert events[1].stream_position == 1
+assert events[1].type == event2.type
+assert events[1].data == event2.data
+
+assert events[2].stream_name == stream_name1
+assert events[2].stream_position == 2
+assert events[2].type == event3.type
+assert events[2].data == event3.data
+```
+
+The method `read_stream_events()` also supports four optional arguments,
+`position`, `backwards`, `limit`, and `timeout`.
+
+The optional `position` argument is an optional integer that can be used to indicate
+the position in the stream from which to start reading. This argument is `None`
+by default, which means the stream will be read either from the start of the
+stream (the default behaviour), or from the end of the stream if `backwards` is
+`True` (see below). When reading a stream from a specific position in the stream, the
+recorded event at that position WILL be included, both when reading forwards
+from that position, and when reading backwards from that position.
+
+The optional argument `backwards` is a boolean, by default `False`, which means the
+stream will be read forwards by default, so that events are returned in the
+order they were appended, If `backwards` is `True`, the stream will be read
+backwards, so that events are returned in reverse order.
+
+The optional argument `limit` is an integer which limits the number of events that will
+be returned. The default value is `sys.maxint`.
+
+The optional argument `timeout` is a float which sets a deadline for the completion of
+the gRPC operation.
+
+The example below shows how to read recorded events in a stream forwards from
+a specific stream position to the end of the stream.
+
+```python
+events = list(
+    client.read_stream_events(
+        stream_name=stream_name1,
+        position=1,
+    )
+)
+
+assert len(events) == 2
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 1
+assert events[0].type == event2.type
+assert events[0].data == event2.data
+
+assert events[1].stream_name == stream_name1
+assert events[1].stream_position == 2
+assert events[1].type == event3.type
+assert events[1].data == event3.data
+```
+
+The example below shows how to read the recorded events in a stream backwards from
+the end of the stream to the start of the stream.
+
+```python
+events = list(
+    client.read_stream_events(
+        stream_name=stream_name1,
+        backwards=True,
+    )
+)
+
+assert len(events) == 3
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 2
+assert events[0].type == event3.type
+assert events[0].data == event3.data
+
+assert events[1].stream_name == stream_name1
+assert events[1].stream_position == 1
+assert events[1].type == event2.type
+assert events[1].data == event2.data
+```
+
+The example below shows how to read a limited number (two) of the recorded events
+in a stream forwards from the start of the stream.
+
+```python
+events = list(
+    client.read_stream_events(
+        stream_name=stream_name1,
+        limit=2,
+    )
+)
+
+assert len(events) == 2
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 0
+assert events[0].type == event1.type
+assert events[0].data == event1.data
+
+assert events[1].stream_name == stream_name1
+assert events[1].stream_position == 1
+assert events[1].type == event2.type
+assert events[1].data == event2.data
+```
+
+The example below shows how to read a limited number (one) of the recorded
+events in a stream backwards from a given stream position.
+
+```python
+events = list(
+    client.read_stream_events(
+        stream_name=stream_name1,
+        position=2,
+        backwards=True,
+        limit=1,
+    )
+)
+
+assert len(events) == 1
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 2
+assert events[0].type == event3.type
+assert events[0].data == event3.data
+```
+
+### Idempotent writes
+
+Now that we can both append events and read from a stream, we can demonstrate
+the idempotent nature of the `append_events()` operation.
+
+Sometimes it may happen that a new event is successfully recorded and then somehow
+the connection to the database gets interrupted before the successful call can return
+successfully to the client. In case of an error when appending an event, it may be
+desirable to retry appending the same event at the same position. If the event was
+in fact successfully recorded, it is convenient for the retry to return successfully
+without raising an error due to optimistic concurrency control (as described above).
+
+The example below shows the `append_events()` method being called again with
+`event3` and `expected_position=2`.
+
+```python
+# Retry appending event3.
+commit_position_retry = client.append_events(
+    stream_name=stream_name1,
+    expected_position=0,
+    events=[event2, event3],
+)
+```
+
+We can see that the same commit position is returned as above.
+
+```python
+assert commit_position_retry == commit_position2
+```
+
+This works because the `NewEvent` class has an `id` attribute that
+is supplied with a new version-4 UUID when an instance is constructed.
+
+```python
+assert isinstance(event1.id, UUID)
+assert isinstance(event2.id, UUID)
+assert isinstance(event3.id, UUID)
+
+assert event1.id != event2.id
+assert event2.id != event3.id
+```
+
+It is possible to provide an `id` value when constructing instances of
+`NewEvent`, but in the examples above we have been using the default behaviour.
+
+We can see that the `append_events()` method returns successfully, and
+that the stream has been unchanged by calling the method twice with the
+same arguments.
+
+```python
+response = client.read_stream_events(
+    stream_name=stream_name1
+)
+
+events = list(response)
+assert events[0].id == event1.id
+assert events[1].id == event2.id
+assert events[2].id == event3.id
+```
+
+
+### Read all recorded events
+
+The method `read_all_events()` can be used to read all recorded events
+in the database in the order they were recorded. An iterable object of
+recorded events is returned. This iterable object will stop when it has
+yielded the last recorded event.
+
+The method `read_stream_events()` supports six optional arguments,
+`commit_position`, `backwards`, `filter_exclude`, `filter_include`, `limit`,
+and `timeout`.
+
+The optional argument `position` is an optional integer that can be used to specify
+the commit position from which to start reading. This argument is `None` by
+default, meaning that all the events will be read either from the start, or
+from the end if `backwards` is `True` (see below). Please note, if specified,
+the specified position must be an actually existing commit position, because
+any other number will result in a server error (at least in EventStoreDB v21.10).
+
+Please also note, when reading forwards from a specific commit position, the event
+at the specified position WILL be included. However, when reading backwards, the
+event at the specified position will NOT be included. (This non-inclusive behaviour
+of excluding the specified commit position when reading all streams differs from the
+behaviour when reading a named stream backwards from a specific stream position, I'm
+not sure why.)
+
+The optional argument `backwards` is a boolean which is by default `False` meaning the
+events will be read forwards by default, so that events are returned in the
+order they were committed, If `backwards` is `True`, the events will be read
+backwards, so that events are returned in reverse order.
+
+The optional argument `filter_exclude` is a sequence of regular expressions that
+match the type strings of recorded events that should not be included. By default,
+this argument will match "system events", so that they will not be included.
+This argument is ignored if `filter_include` is set to a non-empty sequence.
+
+The optional argument `filter_include` is a sequence of regular expressions
+that match the type strings of recorded events that should be included. By
+default, this argument is an empty tuple. If this argument is set to a
+non-empty sequence, the `filter_exclude` argument is ignored.
+
+Please note, the filtering happens on the EventStoreDB server, and the
+`limit` argument is applied on the server after filtering. See below for
+more information about filter regular expressions.
+
+The optional argument `limit` is an integer which limits the number of events that will
+be returned. The default value is `sys.maxint`.
+
+The optional argument `timeout` is a float which sets a deadline for the completion of
+the gRPC operation.
+
+The example below shows how to read all events in the database in the
+order they were recorded.
+
+```python
+events = list(client.read_all_events())
+
+assert len(events) >= 3
+```
+
+The example below shows how to read all recorded events from a particular commit position.
+
+```python
+events = list(
+    client.read_all_events(
+        commit_position=commit_position1
+    )
+)
+
+assert len(events) == 3
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 0
+assert events[0].type == event1.type
+assert events[0].data == event1.data
+
+assert events[1].stream_name == stream_name1
+assert events[1].stream_position == 1
+assert events[1].type == event2.type
+assert events[1].data == event2.data
+
+assert events[2].stream_name == stream_name1
+assert events[2].stream_position == 2
+assert events[2].type == event3.type
+assert events[2].data == event3.data
+```
+
+The example below shows how to read all recorded events in reverse order.
+
+```python
+events = list(
+    client.read_all_events(
+        backwards=True
+    )
+)
+
+assert len(events) >= 3
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 2
+assert events[0].type == event3.type
+assert events[0].data == event3.data
+
+assert events[1].stream_name == stream_name1
+assert events[1].stream_position == 1
+assert events[1].type == event2.type
+assert events[1].data == event2.data
+
+assert events[2].stream_name == stream_name1
+assert events[2].stream_position == 0
+assert events[2].type == event1.type
+assert events[2].data == event1.data
+```
+
+The example below shows how to read a limited number (one) of the recorded events
+in the database forwards from a specific commit position. Please note, when reading
+all events forwards from a specific commit position, the event at the specified
+position WILL be included.
+
+
+```python
+events = list(
+    client.read_all_events(
+        commit_position=commit_position1,
+        limit=1,
+    )
+)
+
+assert len(events) == 1
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 0
+assert events[0].type == event1.type
+assert events[0].data == event1.data
+
+assert events[0].commit_position == commit_position1
+```
+
+The example below shows how to read a limited number (one) of the recorded events
+in the database backwards from the end. This gives the last recorded event.
+
+```python
+events = list(
+    client.read_all_events(
+        backwards=True,
+        limit=1,
+    )
+)
+
+assert len(events) == 1
+
+assert events[0].stream_name == stream_name1
+assert events[0].stream_position == 2
+assert events[0].type == event3.type
+assert events[0].data == event3.data
+```
+
+The example below shows how to read a limited number (one) of the recorded events
+in the database backwards from a specific commit position. Please note, when reading
+all events backwards from a specific commit position, the event at the specified
+position WILL NOT be included.
+
+```python
+events = list(
+    client.read_all_events(
+        commit_position=commit_position2,
+        backwards=True,
+        limit=1,
+    )
+)
+
+assert len(events) == 1
+
+assert events[0].commit_position < commit_position2
+```
+
+### Get current commit position
+
+*only supported in EventStoreDB version >= 22.10*
+
+The method `get_commit_position()` can be used to get the current
+commit position of the database.
+
+```python
+commit_position = client.get_commit_position()
+```
+
+This method takes an optional argument `timeout` which is a float that sets
+a deadline for the completion of the gRPC operation.
+
+This method can be useful to measure progress of a downstream component
+that is processing all recorded events, by comparing the current commit
+position with the recorded commit position of the last successfully processed
+event in a downstream component.
+
+The value of the `commit_position` argument when reading events either by using
+the `read_all_events()` method or by using a catch-up subscription would usually
+be determined by the recorded commit position of the last successfully processed
+event in a downstream component.
+
+## Subscriptions
+
+### Catch-up subscriptions
+
+The client has a `subscribe_all_events()` method, which can be used
+to start a "catch-up" subscription.
+
+Many catch-up subscriptions can be created, concurrently or
+successively, and all will receive all the events they are
+subscribed to receive.
+
+This method returns an iterator object which yields recorded events,
+including events that are recorded after the subscription was created.
+This iterator object will therefore not stop, unless the connection
+to the database is lost. The connection will be closed when the
+iterator object is deleted from memory, which will happen when the
+iterator object goes out of scope is explicitly deleted (see below),
+and the connection may be closed by the server.
+
+This method takes an optional `commit_position` argument, which can be
+used to specify a commit position from which to subscribe for
+recorded events. The default value is `None`, which means
+the subscription will operate from the first recorded event
+in the database. If a commit position is given, it must match
+an actually existing commit position in the database. The events
+that are obtained will not include the event recorded at that commit
+position.
+
+This method also takes three other optional arguments, `filter_exclude`,
+`filter_include`, and `timeout`.
+
+The argument `filter_exclude` is a sequence of regular expressions matching
+the type strings of recorded events that should be excluded. By default,
+this argument will match "system events", so that they will not be included.
+This argument is ignored if `filter_include` is set to a non-empty sequence.
+
+The argument `filter_include` is a sequence of regular expressions
+matching the type strings of recorded events that should be included. By
+default, this argument is an empty tuple. If this argument is set to a
+non-empty sequence, the `filter_exclude` argument is ignored.
+
+Please note, the filtering happens on the EventStoreDB server, and the
+`limit` argument is applied on the server after filtering. See below for
+more information about filter regular expressions.
+
+The argument `timeout` is a float which sets a deadline for the completion of
+the gRPC operation. This probably isn't very useful, but is included for
+completeness and consistency with the other methods.
+
+The example below shows how to subscribe to receive all recorded
+events from a specific commit position. Three already-recorded
+events are received, and then three new events are recorded, which
+are then received via the subscription.
+
+```python
+
+# Get the commit position (usually from database of materialised views).
+commit_position = client.get_commit_position()
+
+# Append three events to another stream.
+stream_name2 = str(uuid4())
+event4 = NewEvent(
+    type='OrderCreated',
+    data=b'data4',
+)
+event5 = NewEvent(
+    type='OrderUpdated',
+    data=b'data5',
+)
+event6 = NewEvent(
+    type='OrderDeleted',
+    data=b'data6',
+)
+client.append_events(
+    stream_name=stream_name2,
+    expected_position=None,
+    events=[event4, event5, event6],
+)
+
+# Subscribe from the commit position.
+subscription = client.subscribe_all_events(
+    commit_position=commit_position
+)
+
+# Catch up by receiving the three events from the subscription.
+events = []
+for event in subscription:
+    events.append(event)
+    if event.data == event6.data and event.stream_name:
+        break
+
+assert events[0].data == event4.data
+assert events[1].data == event5.data
+assert events[2].data == event6.data
+
+
+# Append three more events.
+stream_name3 = str(uuid4())
+event7 = NewEvent(
+    type='OrderCreated',
+    data=b'data7',
+)
+event8 = NewEvent(
+    type='OrderUpdated',
+    data=b'data8',
+)
+event9 = NewEvent(
+    type='OrderDeleted',
+    data=b'data9',
+)
+
+client.append_events(
+    stream_name=stream_name3,
+    expected_position=None,
+    events=[event7, event8, event9],
+)
+
+# Receive the three new events from the same subscription.
+for event in subscription:
+    # Check the stream name.
+    events.append(event)
+    if event.stream_name == stream_name3:
+        if event.data == event9.data:
+            break
+
+assert events[3].data == event7.data
+assert events[4].data == event8.data
+assert events[5].data == event9.data
+```
+
+Catch-up subscriptions are not registered in EventStoreDB (they are not
+"persistent" subscriptions). It is simply a streaming gRPC call which is
+kept open by the server, with newly recorded events sent to the client
+as the client iterates over the subscription. This kind of subscription
+is closed as soon as the subscription object goes out of memory.
+
+```python
+# End the subscription.
+del subscription
+```
+
+Please note, when processing events in a downstream component, the commit position of
+the last successfully processed event is usefully recorded by the downstream component
+so that the commit position can be determined by the downstream component from its own
+recorded when it is restarted. This commit position can be used to specify the commit
+position from which to subscribe. Since this commit position represents the position of
+the last successfully processed event in a downstream component, so it will be usual to
+want the next event after this position, because that is the next event that needs to
+be processed. When subscribing for events using a catchup-subscription
+in EventStoreDB, the event at the specified commit position will NOT be included in
+the sequence of recorded events.
+
+To accomplish "exactly once" processing of the events, the commit position
+of a recorded event should be recorded atomically and uniquely along with
+the result of processing recorded events, for example in the same database
+as materialised views when implementing eventually-consistent CQRS, or in
+the same database as a downstream analytics or reporting or archiving
+application. This avoids "dual writing" in the processing of events.
+
+Recorded events received from a catch-up subscription cannot be acknowledged back
+to the EventStoreDB server (there is no need to do this). Acknowledging events is
+an aspect of "persistent subscriptions" (see below).
+
+The subscription object might be used directly when processing events. It might
+also be used within a thread dedicated to receiving events, with recorded events
+put on a queue for processing in a different thread. This package doesn't provide
+such thread or queue objects, you would need to do that yourself. Just make sure
+to reconstruct the subscription (and the queue) using your last recorded commit
+position when resuming the subscription after an error, to be sure all events
+are processed once.
+
+### Persistent subscriptions
+
+The method `create_subscription()` can be used to create a
+"persistent subscription" to EventStoreDB.
+
+This method takes a required `group_name` argument, which is the
+name of a "group" of consumers of the subscription.
+
+This method takes an optional `from_end` argument, which can be
+used to specify that the group of consumers of the subscription should
+only receive events that were recorded after the subscription was created.
+
+This method takes an optional `commit_position` argument, which can be
+used to specify a commit position from which the group of consumers of
+the subscription should receive events. Please note, the recorded event
+at the specified commit position MAY be included in the recorded events
+received by the group of consumers.
+
+If neither `from_end` or `position` are specified, the group of consumers
+of the subscription will receive all recorded events.
+
+This method also takes option `filter_exclude`, `filter_include`
+arguments, which work in the same way as they do in the `subscribe_all_events()`
+method.
+
+This method also takes an optional `timeout` argument, that
+is expected to be a Python `float`, which sets a deadline
+for the completion of the gRPC operation.
+
+The method `create_subscription()` does not return a value, because
+recorded events are obtained by the group of consumers of the subscription
+using the `read_subscription()` method.
+
+In the example below, a persistent subscription is created.
+
+```python
+# Create a persistent subscription.
+group_name = f"group-{uuid4()}"
+client.create_subscription(group_name=group_name)
+```
+
+The method `read_subscription()` can be used by a group of consumers to receive
+recorded events from a persistent subscription created using `create_subscription`.
+
+This method takes a required `group_name` argument, which is
+the name of a "group" of consumers of the subscription specified
+when `create_subscription()` was called.
+
+This method also takes an optional `timeout` argument, that
+is expected to be a Python `float`, which sets a deadline
+for the completion of the gRPC operation.
+
+This method returns a 2-tuple: a "read request" object and a "read response" object.
+
+```python
+read_req, read_resp = client.read_subscription(group_name=group_name)
+```
+
+The "read response" object is an iterator that yields recorded events from
+the specified commit position.
+
+The "read request" object has an `ack()` method that can be used by a consumer
+in a group to acknowledge to the server that it has received and successfully
+processed a recorded event. This will prevent that recorded event being received
+by another consumer in the same group. The `ack()` method takes an `event_id`
+argument, which is the ID of the recorded event that has been received.
+
+The example below iterates over the "read response" object, and calls `ack()`
+on the "read response" object. The for loop breaks when we have received
+the last event, so that we can continue with the examples below.
+
+```python
+events = []
+for event in read_resp:
+    events.append(event)
+
+    # Acknowledge the received event.
+    read_req.ack(event_id=event.id)
+
+    # Break when the last event has been received.
+    if event.stream_name == stream_name3:
+        if event.data == event9.data:
+            break
+```
+
+The received events are the events we appended above.
+
+```python
+assert events[-9].data == event1.data
+assert events[-8].data == event2.data
+assert events[-7].data == event3.data
+assert events[-6].data == event4.data
+assert events[-5].data == event5.data
+assert events[-4].data == event6.data
+assert events[-3].data == event7.data
+assert events[-2].data == event8.data
+assert events[-1].data == event9.data
+```
+
+The "read request" object also has an `nack()` method that can be used by a consumer
+in a group to acknowledge to the server that it has failed successfully to
+process a recorded event. This will allow that recorded event to be received
+by this or another consumer in the same group.
+
+It might be more useful to encapsulate the request and response objects and to iterate
+over the "read response" in a separate thread, to call back to a handler function when
+a recorded event is received, and call `ack()` if the handler does not raise an
+exception, and to call `nack()` if an exception is raised. The example below shows how
+this might be done.
+
+```python
+from threading import Thread
+
+
+class SubscriptionReader:
+    def __init__(self, client, group_name, callback):
+        self.client = client
+        self.group_name = group_name
+        self.callback = callback
+        self.thread = Thread(target=self.read_subscription, daemon=True)
+        self.error = None
+
+    def start(self):
+        self.thread.start()
+
+    def join(self):
+        self.thread.join()
+
+    def read_subscription(self):
+        req, resp = self.client.read_subscription(group_name=self.group_name)
+        for event in resp:
+            try:
+                self.callback(event)
+            except Exception as e:
+                # req.nack(event.id)  # not yet implemented....
+                self.error = e
+                break
+            else:
+                req.ack(event.id)
+
+
+# Create another persistent subscription.
+group_name = f"group-{uuid4()}"
+client.create_subscription(group_name=group_name)
+
+events = []
+
+def handle_event(event):
+    events.append(event)
+    if event.stream_name == stream_name3:
+        if event.data == event9.data:
+            raise Exception()
+
+
+reader = SubscriptionReader(
+    client=client,
+    group_name=group_name,
+    callback=handle_event
+)
+
+reader.start()
+reader.join()
+
+assert events[-1].data == event9.data
+```
+
+Please note, when processing events in a downstream component, the commit position of
+the last successfully processed event is usefully recorded by the downstream component
+so that the commit position can be determined by the downstream component from its own
+recorded when it is restarted. This commit position can be used to specify the commit
+position from which to subscribe. Since this commit position represents the position of
+the last successfully processed event in a downstream component, so it will be usual to
+want to read from the next event after this position, because that is the next event
+that needs to be processed. However, when subscribing for events using a persistent
+subscription in EventStoreDB, the event at the specified commit position MAY be returned
+as the first event in the received sequence of recorded events, and so it may
+be necessary to check the commit position of the received events and to discard
+any  recorded event object that has a commit position equal to the commit position
+specified in the request.
+
+Whilst there are some advantages of persistent subscriptions, by tracking in the
+upstream server the position in the commit sequence of events that have been processed,
+there is a danger of "dual writing" in the consumption of events. The danger is that if
+an event is successfully processed but then the acknowledgment fails, the event may be
+received more than once. On the other hand, if the acknowledgment is successful but
+then the processing fails, the event may effectively not be been processed. By either
+processing an events more than once, or failing to process an event, the resulting state
+of the processing of the recorded events might be inaccurate, or possibly
+inconsistent, and perhaps catastrophically so. Any relatively minor consequences may or
+may not matter in your situation. But sometimes inconsistencies may halt processing
+until the issue is resolved. You can avoid "dual writing" in the consumption of events
+by atomically recording the commit position of an event that has been processed along
+with the results of processing that event (that is, with both things being recorded in
+the same transaction), and making these records unique so that transactions will be
+rolled back preventing the results of reprocessing the event being committed.
+
+## Notes
+
+### Regular expression filters
+
+The filter arguments in `read_all_events()`, `subscribe_all_events()`,
+`create_subscription()` and `commit_position()` are applied to the `type`
+attribute of recorded events.
+
+The default value of the `filter_exclude` arguments is designed to exclude
+EventStoreDB "system" and "persistence subscription config" events, which
+otherwise would be included. System events generated by EventStoreDB all
+have `type` strings that start with the `$` sign. Persistence subscription
+events generated when manipulating persistence subscriptions all have `type`
+strings that start with `PersistentConfig`.
+
+For example, to match the type of EventStoreDB system events, use the regular
+expression `r'\$.+'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is
+set to `r'\$.+'`. You can import this value
+(`from esdbclient import ESDB_SYSTEM_EVENTS_REGEX`) and use
+it when building longer sequences of regular expressions.
+
+Similarly, to match the type of EventStoreDB persistence subscription events, use the
+regular expression `r'PersistentConfig\d+'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`
+is set to `r'PersistentConfig\d+'`. You can also import this value
+(`from esdbclient import ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`) and use it when building
+longer sequences of regular expressions.
+
+The constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that match
+the events that EventStoreDB generates internally, events that are extraneous to those
+which you append using the `append_events()` method.
+
+For example, to exclude system events and persistence subscription configuration events,
+and snapshots, you might use the sequence `DEFAULT_EXCLUDE_FILTER + ['.*Snapshot']` as
+the value of the `filter_exclude` argument when calling `read_all_events()`,
+`subscribe_all_events()`, `create_subscription()` or `get_commit_position()`.
+
+### The NewEvent class
+
+The `NewEvent` class is used when appending events.
+
+The required argument `type` is a Python `str` object, used to indicate the type of
+the event that will be recorded.
+
+The required argument `data` is a Python `bytes` object, used to indicate the data of
+the event that will be recorded.
+
+The optional argument `metadata` is a Python `bytes` object, used to indicate any
+metadata of the event that will be recorded. The default value is an empty `bytes`
+object.
+
+The optional argument `content_type` is a Python `str` object, used to indicate the
+type of the data that will be recorded for this event. The default value is
+`application/json`, which indicates that the `data` was serialised using JSON.
+An alternative value for this argument is `application/octet-stream`.
+
+The optional argument `id` is a Python `UUID` object, used to specify the unique ID
+of the event that will be recorded. This value will default to a new version-4 UUID.
+
+```python
+new_event1 = NewEvent(
+    type='OrderCreated',
+    data=b'{"name": "Greg"}',
+)
+assert new_event1.type == 'OrderCreated'
+assert new_event1.data == b'{"name": "Greg"}'
+assert new_event1.metadata == b''
+assert new_event1.content_type == 'application/json'
+assert isinstance(new_event1.id, UUID)
+
+event_id = uuid4()
+new_event2 = NewEvent(
+    type='ImageCreated',
+    data=b'01010101010101',
+    metadata=b'{"a": 1}',
+    content_type='application/octet-stream',
+    id=event_id,
+)
+assert new_event2.type == 'ImageCreated'
+assert new_event2.data == b'01010101010101'
+assert new_event2.metadata == b'{"a": 1}'
+assert new_event2.content_type == 'application/octet-stream'
+assert new_event2.id == event_id
+```
+
+### The RecordedEvent class
+
+The `RecordedEvent` class is used when reading events.
+
+The attribute `type` is a Python `str` object, used to indicate the type of event
+that was recorded.
+
+The attribute `data` is a Python `bytes` object, used to indicate the data of the
+event that was recorded.
+
+The attribute `metadata` is a Python `bytes` object, used to indicate the metadata of
+the event that was recorded.
+
+The attribute `content_type` is a Python `str` object, used to indicate the type of
+data that was recorded for this event (usually `application/json` to indicate that
+this data can be parsed as JSON, but alternatively `application/octet-stream` to
+indicate that it is something else).
+
+The attribute `id` is a Python `UUID` object, used to indicate the unique ID of the
+event that was recorded. Please note, when recorded events are returned from a call
+to `read_stream_events()` in EventStoreDB v21.10, the commit position is not actually
+set in the response. For this reason, this attribute is actually typed as an optional
+value (`Optional[UUID]`), and this case the value of this attribute will be `None`.
+
+The attribute `stream_name` is a Python `str` object, used to indicate the name of the
+stream in which the event was recorded.
+
+The attribute `stream_position` is a Python `int`, used to indicate the position in the
+stream at which the event was recorded.
+
+The attribute `commit_position` is a Python `int`, used to indicate the commit position
+at which the event was recorded.
+
+```python
+from esdbclient.events import RecordedEvent
+
+recorded_event = RecordedEvent(
+    type='OrderCreated',
+    data=b'{}',
+    metadata=b'',
+    content_type='application/json',
+    id=uuid4(),
+    stream_name='stream1',
+    stream_position=0,
+    commit_position=512,
+)
+```
+
+## Contributors
+
+### Install Poetry
+
+The first thing is to check you have Poetry installed.
+
+    $ poetry --version
+
+If you don't, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).
+
+    $ curl -sSL https://install.python-poetry.org | python3 -
+
+It will help to make sure Poetry's bin directory is in your `PATH` environment variable.
+
+But in any case, make sure you know the path to the `poetry` executable. The Poetry
+installer tells you where it has been installed, and how to configure your shell.
+
+Please refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on
+using Poetry.
+
+### Setup for PyCharm users
+
+You can easily obtain the project files using PyCharm (menu "Git > Clone...").
+PyCharm will then usually prompt you to open the project.
+
+Open the project in a new window. PyCharm will then usually prompt you to create
+a new virtual environment.
+
+Create a new Poetry virtual environment for the project. If PyCharm doesn't already
+know where your `poetry` executable is, then set the path to your `poetry` executable
+in the "New Poetry Environment" form input field labelled "Poetry executable". In the
+"New Poetry Environment" form, you will also have the opportunity to select which
+Python executable will be used by the virtual environment.
+
+PyCharm will then create a new Poetry virtual environment for your project, using
+a particular version of Python, and also install into this virtual environment the
+project's package dependencies according to the `pyproject.toml` file, or the
+`poetry.lock` file if that exists in the project files.
+
+You can add different Poetry environments for different Python versions, and switch
+between them using the "Python Interpreter" settings of PyCharm. If you want to use
+a version of Python that isn't installed, either use your favourite package manager,
+or install Python by downloading an installer for recent versions of Python directly
+from the [Python website](https://www.python.org/downloads/).
+
+Once project dependencies have been installed, you should be able to run tests
+from within PyCharm (right-click on the `tests` folder and select the 'Run' option).
+
+Because of a conflict between pytest and PyCharm's debugger and the coverage tool,
+you may need to add ``--no-cov`` as an option to the test runner template. Alternatively,
+just use the Python Standard Library's ``unittest`` module.
+
+You should also be able to open a terminal window in PyCharm, and run the project's
+Makefile commands from the command line (see below).
+
+### Setup from command line
+
+Obtain the project files, using Git or suitable alternative.
+
+In a terminal application, change your current working directory
+to the root folder of the project files. There should be a Makefile
+in this folder.
+
+Use the Makefile to create a new Poetry virtual environment for the
+project and install the project's package dependencies into it,
+using the following command.
+
+    $ make install-packages
+
+It's also possible to also install the project in 'editable mode'.
+
+    $ make install
+
+Please note, if you create the virtual environment in this way, and then try to
+open the project in PyCharm and configure the project to use this virtual
+environment as an "Existing Poetry Environment", PyCharm sometimes has some
+issues (don't know why) which might be problematic. If you encounter such
+issues, you can resolve these issues by deleting the virtual environment
+and creating the Poetry virtual environment using PyCharm (see above).
+
+### Project Makefile commands
+
+You can start EventStoreDB using the following command.
+
+    $ make start-eventstoredb
+
+You can run tests using the following command (needs EventStoreDB to be running).
+
+    $ make test
+
+You can stop EventStoreDB using the following command.
+
+    $ make stop-eventstoredb
+
+You can check the formatting of the code using the following command.
+
+    $ make lint
+
+You can reformat the code using the following command.
+
+    $ make fmt
+
+Tests belong in `./tests`. Code-under-test belongs in `./esdbclient`.
+
+Edit package dependencies in `pyproject.toml`. Update installed packages (and the
+`poetry.lock` file) using the following command.
+
+    $ make update-packages
 
-setup(**setup_kwargs)
```

### Comparing `esdbclient-0.8/PKG-INFO` & `esdbclient-0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1234 +1,30 @@
-Metadata-Version: 2.1
-Name: esdbclient
-Version: 0.8
-Summary: Python gRPC Client for EventStoreDB
-Home-page: https://github.com/pyeventsourcing/esdbclient
-License: BSD 3-Clause
-Author: John Bywater
-Author-email: john.bywater@appropriatesoftware.net
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: grpcio (>=1.51.0,<1.52.0)
-Requires-Dist: protobuf (>=4.21.0,<5.0.0)
-Requires-Dist: typing_extensions
-Project-URL: Repository, https://github.com/pyeventsourcing/esdbclient
-Description-Content-Type: text/markdown
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-# Python gRPC Client for EventStoreDB
+packages = \
+['esdbclient', 'esdbclient.protos.Grpc']
 
-This package provides a Python gRPC client for
-[EventStoreDB](https://www.eventstore.com/).
+package_data = \
+{'': ['*']}
 
-This client has been developed and tested to work with EventStoreDB LTS
-versions 21.10 and 21.10, without and without SSL/TLS enabled on both
-these versions, and with Python versions 3.7, 3.8, 3.9, 3.10, and 3.11
-across all of the above. The test coverage is 100% including branch coverage.
+install_requires = \
+['grpcio>=1.51.0,<1.52.0', 'protobuf>=4.21.0,<5.0.0', 'typing_extensions']
+
+setup_kwargs = {
+    'name': 'esdbclient',
+    'version': '0.9',
+    'description': 'Python gRPC Client for EventStoreDB',
+    'long_description': '# Python gRPC Client for EventStoreDB\n\nThis package provides a Python gRPC client for\n[EventStoreDB](https://www.eventstore.com/).\n\nThis client has been developed and tested to work with EventStoreDB LTS\nversions 21.10 and 21.10, without and without SSL/TLS enabled on both\nthese versions, and with Python versions 3.7, 3.8, 3.9, 3.10, and 3.11\nacross all of the above. The test coverage is 100% including branch coverage.\n\nAll the code in this package has typing annotations. The static typing\nannotations checked relatively strictly with mypy.\n\nNot all the features of the EventStoreDB API are presented\nby this client in its current form, however many of the most\nuseful aspects are presented in an easy-to-use interface (see below).\nFor an example of usage, see the [eventsourcing-eventstoredb](\nhttps://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.\n\n## Table of contents\n\n<!-- TOC -->\n* [Installation](#installation)\n* [Server](#server)\n  * [Start EventStoreDB](#start-eventstoredb)\n  * [Stop EventStoreDB](#stop-eventstoredb)\n* [Client](#client)\n* [Streams](#streams)\n  * [Append events](#append-events)\n  * [Get current stream position](#get-current-stream-position)\n  * [Read stream events](#read-stream-events)\n  * [Idempotent writes](#idempotent-writes)\n  * [Read all recorded events](#read-all-recorded-events)\n  * [Get current commit position](#get-current-commit-position)\n* [Subscriptions](#subscriptions)\n  * [Catch-up subscriptions](#catch-up-subscriptions)\n  * [Persistent subscriptions](#persistent-subscriptions)\n* [Notes](#notes)\n  * [Regular expression filters](#regular-expression-filters)\n  * [The NewEvent class](#the-newevent-class)\n  * [The RecordedEvent class](#the-recordedevent-class)\n* [Contributors](#contributors)\n  * [Install Poetry](#install-poetry)\n  * [Setup for PyCharm users](#setup-for-pycharm-users)\n  * [Setup from command line](#setup-from-command-line)\n  * [Project Makefile commands](#project-makefile-commands)\n<!-- TOC -->\n\n## Installation\n\nUse pip to install this package from\n[the Python Package Index](https://pypi.org/project/esdbclient/).\n\n    $ pip install esdbclient\n\nIt is recommended to install Python packages into a Python virtual environment.\n\n\n## Server\n\n### Start EventStoreDB\n\nUse Docker to run EventStoreDB using the official Docker container image on DockerHub.\n\nFor development, you can start a "secure" server locally on port 2113 using the following command.\n\n    $ docker run -d --name my-eventstoredb -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:22.10.0-buster-slim --dev\n\nAlternatively, you can start an "insecure" server locally on port 2113 using the following command.\n\n    $ docker run -d --name my-eventstoredb -it -p 2113:2113 eventstore/eventstore:22.10.0-buster-slim --insecure\n\nTo connect to the "insecure" local server using the client in this package, you just need\nto know the local hostname and the port number. To connect to the "secure" local\ndevelopment server, you will also need to know that the username is "admin" and\nthe password is "changeit". You will also need to get the SSL/TLS certificate from\nthe server. You can get the server certificate with the following command.\n\n    $ python -c "import ssl; print(get_server_certificate(addr=(\'localhost\', 2113)))"\n\n\n### Stop EventStoreDB\n\nTo stop and remove the `my-eventstoredb` container created above, use the following Docker commands.\n\n    $ docker stop my-eventstoredb\n\t$ docker rm my-eventstoredb\n\n\n## Client\n\nThe `EsdbClient` class can be imported from the `esdbclient` package.\n\n```python\nfrom esdbclient import EsdbClient\n```\n\nThe `EsdbClient` class can be constructed with `host` and `port` arguments.\nThe `host` and `port` arguments indicate the hostname and port number of the\nEventStoreDB server.\n\nIf the EventStoreDB server is "secure", then also use the `server_cert`,\n`username` and `password` arguments.\n\nThe `host` argument is expected to be a Python `str`. The `port` argument is expected\nto be a Python `int`. The `server_cert` is expected to be a Python `str` containing\nthe PEM encoded SSL/TLS server certificate. Both `username` and `password` are expected\nto be a Python `str`.\n\nIn the example below, the constructor argument values are taken from the operating\nsystem environment, because the examples in this document are tested with both\na "secure" and an "insecure" server.\n\n```python\nimport os\n\nclient = EsdbClient(\n    host=os.getenv("ESDB_HOST"),\n    port=int(os.getenv("ESDB_PORT")),\n    server_cert=os.getenv("ESDB_SERVER_CERT"),\n    username=os.getenv("ESDB_USERNAME"),\n    password=os.getenv("ESDB_PASSWORD"),\n)\n```\n\n## Streams\n\nIn EventStoreDB, a "stream" is a sequence of recorded events that all have\nthe same "stream name". Each recorded event has a "position" in its stream.\nThe positions of the recorded events in a stream is a gapless sequence starting\nfrom zero.\n\n### Append events\n\nThe client has an `append_events()` method, which can be used to append\nnew events to a "stream".\n\nThree arguments are required, `stream_name`, `expected_position`\nand `events`.\n\nThe `stream_name` argument is required, and is expected to be a Python\n`str` object that uniquely identifies the stream in the database.\n\nThe `expected_position` argument is required, is expected to be: either `None`\nif new events are being appended to a new stream, or an integer equal to the\nposition the last recorded event in the stream.\n\nThe stream positions of recorded events start from zero. And so, when appending\nthe second new event to a stream that has one recorded event, the correct value\nof the `expected_position` argument is `0`. Similarly, when appending the third\nnew event to a stream that has two recorded events, the correct value\nof the `expected_position` argument is `1`.\n\nStreams are created by appending events. The correct value of the `expected_position`\nargument when appending the first event of a new stream (a stream with zero recorded\nevents) is `None`. Please note, it is not possible to create an "empty" stream in\nEventStoreDB.\n\nIf there is a mismatch between the given value of the `expected_position` argument\nand the position of the last recorded event in a stream, then an `ExpectedPositionError`\nexception will be raised. This effectively accomplishes optimistic concurrency control.\n\nIf you wish to disable optimistic concurrency control when appending new events, you\ncan set the `expected_position` to a negative integer.\n\nIf you need to discover the current position of the last recorded event in a stream,\nyou can use the `get_stream_position()` method (see below).\n\nThe `events` argument is required, and is expected to be a sequence of new\nevent objects to be appended to the named stream. The `NewEvent` class should\nbe used to construct new event objects (see below).\n\nPlease note, the append events operation is atomic, so that either all\nor none of the given new events will be recorded. By design, it is only\npossible with EventStoreDB to atomically record new events in one stream.\n\nIn the example below, a new event is appended to a new stream.\n\n```python\nfrom uuid import UUID, uuid4\n\nfrom esdbclient import NewEvent\n\n# Construct new event object.\nevent1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'data1\',\n)\n\n# Define stream name.\nstream_name1 = str(uuid4())\n\n# Append list of events to new stream.\ncommit_position1 = client.append_events(\n    stream_name=stream_name1,\n    expected_position=None,\n    events=[event1],\n)\n```\n\nIn the example below, two subsequent events are appended to an existing\nstream.\n\n```python\nevent2 = NewEvent(\n    type=\'OrderUpdated\',\n    data=b\'data2\',\n)\nevent3 = NewEvent(\n    type=\'OrderDeleted\',\n    data=b\'data3\',\n)\n\ncommit_position2 = client.append_events(\n    stream_name=stream_name1,\n    expected_position=0,\n    events=[event2, event3],\n)\n```\n\nIf the append operation is successful, this method returns an integer\nrepresenting the overall "commit position" as it was when the operation\nwas completed. Otherwise, an exception will be raised.\n\nA "commit position" is a monotonically increasing integer representing\nthe position of the recorded event in a "total order" of all recorded\nevents in the database across all streams. It is the actual position\nof the event record on disk, and there are usually large differences\nbetween successive commits. The sequence of commit positions\nis NOT gapless.\n\nThe "commit position" returned by `append_events()` is that of the last\nrecorded event in the given sequence of new events.\n\nThe "commit position" returned in this way can therefore be used to wait\nfor a downstream component to have processed all the events that were recorded.\n\nFor example, consider a user interface command that results in the recording\nof new events, and a query into an eventually consistent materialized\nview in a downstream component that is updated from these events. If the new\nevents have not yet been processed, the view would be stale. The "commit position"\ncan be used by the user interface to poll the downstream component until it has\nprocessed the new events, after which time the view will not be stale.\n\n### Get current stream position\n\nThe client has a `get_stream_position()` method, which can be used to\nget the current "stream position" of a stream (the position in the\nstream of the last recorded event in that stream).\n\nThis method has a `stream_name` argument, which is required.\n\nThis method also takes an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe sequence of positions in a stream is gapless. It is zero-based,\nso that a stream with one recorded event has a current stream\nposition of `0`. The current stream position is `1` when a stream has\ntwo events, and it is `2` when there are events, and so on.\n\nIn the example below, the current stream position is obtained of the\nstream to which events were appended in the examples above.\nBecause the sequence of stream positions is zero-based, and because\nthree events were appended, so the current stream position is `2`.\n\n```python\nstream_position = client.get_stream_position(\n    stream_name=stream_name1\n)\n\nassert stream_position == 2\n```\n\nIf a stream does not exist, the returned stream position value is `None`,\nwhich matches the required expected position when appending the first event\nof a new stream (see above).\n\n```python\nstream_position = client.get_stream_position(\n    stream_name=str(uuid4())\n)\n\nassert stream_position == None\n```\n\nThis method takes an optional argument `timeout` which is a float that sets\na deadline for the completion of the gRPC operation.\n\n\n### Read stream events\n\nThe client has a `read_stream_events()` method, which can be used to read\nthe events of a stream.\n\nThis method returns nn iterable object that yields recorded event objects.\nThese recorded event objects are instances of the `RecordedEvent` class (see below)\n\nThis method has one required argument, `stream_name`, which is the name of\nthe stream to be read. By default, the recorded events in the stream\nare returned in the order they were recorded.\n\nThe example below shows how to read the recorded events of a stream\nforwards from the start of the stream to the end of the stream. The\nname of a stream is given when calling the method. In this example,\nthe iterable response object is converted into a Python `list`, which\ncontains all the recorded event objects that were read from the stream.\n\n```python\nresponse = client.read_stream_events(\n    stream_name=stream_name1\n)\n\nevents = list(response)\n```\n\nNow that we have a list of event objects, we can check we got the\nthree events that were appended to the stream, and that they are\nordered exactly as they were appended.\n\n```python\nassert len(events) == 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n\nassert events[2].stream_name == stream_name1\nassert events[2].stream_position == 2\nassert events[2].type == event3.type\nassert events[2].data == event3.data\n```\n\nThe method `read_stream_events()` also supports four optional arguments,\n`position`, `backwards`, `limit`, and `timeout`.\n\nThe optional `position` argument is an optional integer that can be used to indicate\nthe position in the stream from which to start reading. This argument is `None`\nby default, which means the stream will be read either from the start of the\nstream (the default behaviour), or from the end of the stream if `backwards` is\n`True` (see below). When reading a stream from a specific position in the stream, the\nrecorded event at that position WILL be included, both when reading forwards\nfrom that position, and when reading backwards from that position.\n\nThe optional argument `backwards` is a boolean, by default `False`, which means the\nstream will be read forwards by default, so that events are returned in the\norder they were appended, If `backwards` is `True`, the stream will be read\nbackwards, so that events are returned in reverse order.\n\nThe optional argument `limit` is an integer which limits the number of events that will\nbe returned. The default value is `sys.maxint`.\n\nThe optional argument `timeout` is a float which sets a deadline for the completion of\nthe gRPC operation.\n\nThe example below shows how to read recorded events in a stream forwards from\na specific stream position to the end of the stream.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        position=1,\n    )\n)\n\nassert len(events) == 2\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 1\nassert events[0].type == event2.type\nassert events[0].data == event2.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 2\nassert events[1].type == event3.type\nassert events[1].data == event3.data\n```\n\nThe example below shows how to read the recorded events in a stream backwards from\nthe end of the stream to the start of the stream.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        backwards=True,\n    )\n)\n\nassert len(events) == 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n```\n\nThe example below shows how to read a limited number (two) of the recorded events\nin a stream forwards from the start of the stream.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        limit=2,\n    )\n)\n\nassert len(events) == 2\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n```\n\nThe example below shows how to read a limited number (one) of the recorded\nevents in a stream backwards from a given stream position.\n\n```python\nevents = list(\n    client.read_stream_events(\n        stream_name=stream_name1,\n        position=2,\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n```\n\n### Idempotent writes\n\nNow that we can both append events and read from a stream, we can demonstrate\nthe idempotent nature of the `append_events()` operation.\n\nSometimes it may happen that a new event is successfully recorded and then somehow\nthe connection to the database gets interrupted before the successful call can return\nsuccessfully to the client. In case of an error when appending an event, it may be\ndesirable to retry appending the same event at the same position. If the event was\nin fact successfully recorded, it is convenient for the retry to return successfully\nwithout raising an error due to optimistic concurrency control (as described above).\n\nThe example below shows the `append_events()` method being called again with\n`event3` and `expected_position=2`.\n\n```python\n# Retry appending event3.\ncommit_position_retry = client.append_events(\n    stream_name=stream_name1,\n    expected_position=0,\n    events=[event2, event3],\n)\n```\n\nWe can see that the same commit position is returned as above.\n\n```python\nassert commit_position_retry == commit_position2\n```\n\nThis works because the `NewEvent` class has an `id` attribute that\nis supplied with a new version-4 UUID when an instance is constructed.\n\n```python\nassert isinstance(event1.id, UUID)\nassert isinstance(event2.id, UUID)\nassert isinstance(event3.id, UUID)\n\nassert event1.id != event2.id\nassert event2.id != event3.id\n```\n\nIt is possible to provide an `id` value when constructing instances of\n`NewEvent`, but in the examples above we have been using the default behaviour.\n\nWe can see that the `append_events()` method returns successfully, and\nthat the stream has been unchanged by calling the method twice with the\nsame arguments.\n\n```python\nresponse = client.read_stream_events(\n    stream_name=stream_name1\n)\n\nevents = list(response)\nassert events[0].id == event1.id\nassert events[1].id == event2.id\nassert events[2].id == event3.id\n```\n\n\n### Read all recorded events\n\nThe method `read_all_events()` can be used to read all recorded events\nin the database in the order they were recorded. An iterable object of\nrecorded events is returned. This iterable object will stop when it has\nyielded the last recorded event.\n\nThe method `read_stream_events()` supports six optional arguments,\n`commit_position`, `backwards`, `filter_exclude`, `filter_include`, `limit`,\nand `timeout`.\n\nThe optional argument `position` is an optional integer that can be used to specify\nthe commit position from which to start reading. This argument is `None` by\ndefault, meaning that all the events will be read either from the start, or\nfrom the end if `backwards` is `True` (see below). Please note, if specified,\nthe specified position must be an actually existing commit position, because\nany other number will result in a server error (at least in EventStoreDB v21.10).\n\nPlease also note, when reading forwards from a specific commit position, the event\nat the specified position WILL be included. However, when reading backwards, the\nevent at the specified position will NOT be included. (This non-inclusive behaviour\nof excluding the specified commit position when reading all streams differs from the\nbehaviour when reading a named stream backwards from a specific stream position, I\'m\nnot sure why.)\n\nThe optional argument `backwards` is a boolean which is by default `False` meaning the\nevents will be read forwards by default, so that events are returned in the\norder they were committed, If `backwards` is `True`, the events will be read\nbackwards, so that events are returned in reverse order.\n\nThe optional argument `filter_exclude` is a sequence of regular expressions that\nmatch the type strings of recorded events that should not be included. By default,\nthis argument will match "system events", so that they will not be included.\nThis argument is ignored if `filter_include` is set to a non-empty sequence.\n\nThe optional argument `filter_include` is a sequence of regular expressions\nthat match the type strings of recorded events that should be included. By\ndefault, this argument is an empty tuple. If this argument is set to a\nnon-empty sequence, the `filter_exclude` argument is ignored.\n\nPlease note, the filtering happens on the EventStoreDB server, and the\n`limit` argument is applied on the server after filtering. See below for\nmore information about filter regular expressions.\n\nThe optional argument `limit` is an integer which limits the number of events that will\nbe returned. The default value is `sys.maxint`.\n\nThe optional argument `timeout` is a float which sets a deadline for the completion of\nthe gRPC operation.\n\nThe example below shows how to read all events in the database in the\norder they were recorded.\n\n```python\nevents = list(client.read_all_events())\n\nassert len(events) >= 3\n```\n\nThe example below shows how to read all recorded events from a particular commit position.\n\n```python\nevents = list(\n    client.read_all_events(\n        commit_position=commit_position1\n    )\n)\n\nassert len(events) == 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n\nassert events[2].stream_name == stream_name1\nassert events[2].stream_position == 2\nassert events[2].type == event3.type\nassert events[2].data == event3.data\n```\n\nThe example below shows how to read all recorded events in reverse order.\n\n```python\nevents = list(\n    client.read_all_events(\n        backwards=True\n    )\n)\n\nassert len(events) >= 3\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n\nassert events[1].stream_name == stream_name1\nassert events[1].stream_position == 1\nassert events[1].type == event2.type\nassert events[1].data == event2.data\n\nassert events[2].stream_name == stream_name1\nassert events[2].stream_position == 0\nassert events[2].type == event1.type\nassert events[2].data == event1.data\n```\n\nThe example below shows how to read a limited number (one) of the recorded events\nin the database forwards from a specific commit position. Please note, when reading\nall events forwards from a specific commit position, the event at the specified\nposition WILL be included.\n\n\n```python\nevents = list(\n    client.read_all_events(\n        commit_position=commit_position1,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 0\nassert events[0].type == event1.type\nassert events[0].data == event1.data\n\nassert events[0].commit_position == commit_position1\n```\n\nThe example below shows how to read a limited number (one) of the recorded events\nin the database backwards from the end. This gives the last recorded event.\n\n```python\nevents = list(\n    client.read_all_events(\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].stream_name == stream_name1\nassert events[0].stream_position == 2\nassert events[0].type == event3.type\nassert events[0].data == event3.data\n```\n\nThe example below shows how to read a limited number (one) of the recorded events\nin the database backwards from a specific commit position. Please note, when reading\nall events backwards from a specific commit position, the event at the specified\nposition WILL NOT be included.\n\n```python\nevents = list(\n    client.read_all_events(\n        commit_position=commit_position2,\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].commit_position < commit_position2\n```\n\n### Get current commit position\n\n*only supported in EventStoreDB version >= 22.10*\n\nThe method `get_commit_position()` can be used to get the current\ncommit position of the database.\n\n```python\ncommit_position = client.get_commit_position()\n```\n\nThis method takes an optional argument `timeout` which is a float that sets\na deadline for the completion of the gRPC operation.\n\nThis method can be useful to measure progress of a downstream component\nthat is processing all recorded events, by comparing the current commit\nposition with the recorded commit position of the last successfully processed\nevent in a downstream component.\n\nThe value of the `commit_position` argument when reading events either by using\nthe `read_all_events()` method or by using a catch-up subscription would usually\nbe determined by the recorded commit position of the last successfully processed\nevent in a downstream component.\n\n## Subscriptions\n\n### Catch-up subscriptions\n\nThe client has a `subscribe_all_events()` method, which can be used\nto start a "catch-up" subscription.\n\nMany catch-up subscriptions can be created, concurrently or\nsuccessively, and all will receive all the events they are\nsubscribed to receive.\n\nThis method returns an iterator object which yields recorded events,\nincluding events that are recorded after the subscription was created.\nThis iterator object will therefore not stop, unless the connection\nto the database is lost. The connection will be closed when the\niterator object is deleted from memory, which will happen when the\niterator object goes out of scope is explicitly deleted (see below),\nand the connection may be closed by the server.\n\nThis method takes an optional `commit_position` argument, which can be\nused to specify a commit position from which to subscribe for\nrecorded events. The default value is `None`, which means\nthe subscription will operate from the first recorded event\nin the database. If a commit position is given, it must match\nan actually existing commit position in the database. The events\nthat are obtained will not include the event recorded at that commit\nposition.\n\nThis method also takes three other optional arguments, `filter_exclude`,\n`filter_include`, and `timeout`.\n\nThe argument `filter_exclude` is a sequence of regular expressions matching\nthe type strings of recorded events that should be excluded. By default,\nthis argument will match "system events", so that they will not be included.\nThis argument is ignored if `filter_include` is set to a non-empty sequence.\n\nThe argument `filter_include` is a sequence of regular expressions\nmatching the type strings of recorded events that should be included. By\ndefault, this argument is an empty tuple. If this argument is set to a\nnon-empty sequence, the `filter_exclude` argument is ignored.\n\nPlease note, the filtering happens on the EventStoreDB server, and the\n`limit` argument is applied on the server after filtering. See below for\nmore information about filter regular expressions.\n\nThe argument `timeout` is a float which sets a deadline for the completion of\nthe gRPC operation. This probably isn\'t very useful, but is included for\ncompleteness and consistency with the other methods.\n\nThe example below shows how to subscribe to receive all recorded\nevents from a specific commit position. Three already-recorded\nevents are received, and then three new events are recorded, which\nare then received via the subscription.\n\n```python\n\n# Get the commit position (usually from database of materialised views).\ncommit_position = client.get_commit_position()\n\n# Append three events to another stream.\nstream_name2 = str(uuid4())\nevent4 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'data4\',\n)\nevent5 = NewEvent(\n    type=\'OrderUpdated\',\n    data=b\'data5\',\n)\nevent6 = NewEvent(\n    type=\'OrderDeleted\',\n    data=b\'data6\',\n)\nclient.append_events(\n    stream_name=stream_name2,\n    expected_position=None,\n    events=[event4, event5, event6],\n)\n\n# Subscribe from the commit position.\nsubscription = client.subscribe_all_events(\n    commit_position=commit_position\n)\n\n# Catch up by receiving the three events from the subscription.\nevents = []\nfor event in subscription:\n    events.append(event)\n    if event.data == event6.data and event.stream_name:\n        break\n\nassert events[0].data == event4.data\nassert events[1].data == event5.data\nassert events[2].data == event6.data\n\n\n# Append three more events.\nstream_name3 = str(uuid4())\nevent7 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'data7\',\n)\nevent8 = NewEvent(\n    type=\'OrderUpdated\',\n    data=b\'data8\',\n)\nevent9 = NewEvent(\n    type=\'OrderDeleted\',\n    data=b\'data9\',\n)\n\nclient.append_events(\n    stream_name=stream_name3,\n    expected_position=None,\n    events=[event7, event8, event9],\n)\n\n# Receive the three new events from the same subscription.\nfor event in subscription:\n    # Check the stream name.\n    events.append(event)\n    if event.stream_name == stream_name3:\n        if event.data == event9.data:\n            break\n\nassert events[3].data == event7.data\nassert events[4].data == event8.data\nassert events[5].data == event9.data\n```\n\nCatch-up subscriptions are not registered in EventStoreDB (they are not\n"persistent" subscriptions). It is simply a streaming gRPC call which is\nkept open by the server, with newly recorded events sent to the client\nas the client iterates over the subscription. This kind of subscription\nis closed as soon as the subscription object goes out of memory.\n\n```python\n# End the subscription.\ndel subscription\n```\n\nPlease note, when processing events in a downstream component, the commit position of\nthe last successfully processed event is usefully recorded by the downstream component\nso that the commit position can be determined by the downstream component from its own\nrecorded when it is restarted. This commit position can be used to specify the commit\nposition from which to subscribe. Since this commit position represents the position of\nthe last successfully processed event in a downstream component, so it will be usual to\nwant the next event after this position, because that is the next event that needs to\nbe processed. When subscribing for events using a catchup-subscription\nin EventStoreDB, the event at the specified commit position will NOT be included in\nthe sequence of recorded events.\n\nTo accomplish "exactly once" processing of the events, the commit position\nof a recorded event should be recorded atomically and uniquely along with\nthe result of processing recorded events, for example in the same database\nas materialised views when implementing eventually-consistent CQRS, or in\nthe same database as a downstream analytics or reporting or archiving\napplication. This avoids "dual writing" in the processing of events.\n\nRecorded events received from a catch-up subscription cannot be acknowledged back\nto the EventStoreDB server (there is no need to do this). Acknowledging events is\nan aspect of "persistent subscriptions" (see below).\n\nThe subscription object might be used directly when processing events. It might\nalso be used within a thread dedicated to receiving events, with recorded events\nput on a queue for processing in a different thread. This package doesn\'t provide\nsuch thread or queue objects, you would need to do that yourself. Just make sure\nto reconstruct the subscription (and the queue) using your last recorded commit\nposition when resuming the subscription after an error, to be sure all events\nare processed once.\n\n### Persistent subscriptions\n\nThe method `create_subscription()` can be used to create a\n"persistent subscription" to EventStoreDB.\n\nThis method takes a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription.\n\nThis method takes an optional `from_end` argument, which can be\nused to specify that the group of consumers of the subscription should\nonly receive events that were recorded after the subscription was created.\n\nThis method takes an optional `commit_position` argument, which can be\nused to specify a commit position from which the group of consumers of\nthe subscription should receive events. Please note, the recorded event\nat the specified commit position MAY be included in the recorded events\nreceived by the group of consumers.\n\nIf neither `from_end` or `position` are specified, the group of consumers\nof the subscription will receive all recorded events.\n\nThis method also takes option `filter_exclude`, `filter_include`\narguments, which work in the same way as they do in the `subscribe_all_events()`\nmethod.\n\nThis method also takes an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe method `create_subscription()` does not return a value, because\nrecorded events are obtained by the group of consumers of the subscription\nusing the `read_subscription()` method.\n\nIn the example below, a persistent subscription is created.\n\n```python\n# Create a persistent subscription.\ngroup_name = f"group-{uuid4()}"\nclient.create_subscription(group_name=group_name)\n```\n\nThe method `read_subscription()` can be used by a group of consumers to receive\nrecorded events from a persistent subscription created using `create_subscription`.\n\nThis method takes a required `group_name` argument, which is\nthe name of a "group" of consumers of the subscription specified\nwhen `create_subscription()` was called.\n\nThis method also takes an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method returns a 2-tuple: a "read request" object and a "read response" object.\n\n```python\nread_req, read_resp = client.read_subscription(group_name=group_name)\n```\n\nThe "read response" object is an iterator that yields recorded events from\nthe specified commit position.\n\nThe "read request" object has an `ack()` method that can be used by a consumer\nin a group to acknowledge to the server that it has received and successfully\nprocessed a recorded event. This will prevent that recorded event being received\nby another consumer in the same group. The `ack()` method takes an `event_id`\nargument, which is the ID of the recorded event that has been received.\n\nThe example below iterates over the "read response" object, and calls `ack()`\non the "read response" object. The for loop breaks when we have received\nthe last event, so that we can continue with the examples below.\n\n```python\nevents = []\nfor event in read_resp:\n    events.append(event)\n\n    # Acknowledge the received event.\n    read_req.ack(event_id=event.id)\n\n    # Break when the last event has been received.\n    if event.stream_name == stream_name3:\n        if event.data == event9.data:\n            break\n```\n\nThe received events are the events we appended above.\n\n```python\nassert events[-9].data == event1.data\nassert events[-8].data == event2.data\nassert events[-7].data == event3.data\nassert events[-6].data == event4.data\nassert events[-5].data == event5.data\nassert events[-4].data == event6.data\nassert events[-3].data == event7.data\nassert events[-2].data == event8.data\nassert events[-1].data == event9.data\n```\n\nThe "read request" object also has an `nack()` method that can be used by a consumer\nin a group to acknowledge to the server that it has failed successfully to\nprocess a recorded event. This will allow that recorded event to be received\nby this or another consumer in the same group.\n\nIt might be more useful to encapsulate the request and response objects and to iterate\nover the "read response" in a separate thread, to call back to a handler function when\na recorded event is received, and call `ack()` if the handler does not raise an\nexception, and to call `nack()` if an exception is raised. The example below shows how\nthis might be done.\n\n```python\nfrom threading import Thread\n\n\nclass SubscriptionReader:\n    def __init__(self, client, group_name, callback):\n        self.client = client\n        self.group_name = group_name\n        self.callback = callback\n        self.thread = Thread(target=self.read_subscription, daemon=True)\n        self.error = None\n\n    def start(self):\n        self.thread.start()\n\n    def join(self):\n        self.thread.join()\n\n    def read_subscription(self):\n        req, resp = self.client.read_subscription(group_name=self.group_name)\n        for event in resp:\n            try:\n                self.callback(event)\n            except Exception as e:\n                # req.nack(event.id)  # not yet implemented....\n                self.error = e\n                break\n            else:\n                req.ack(event.id)\n\n\n# Create another persistent subscription.\ngroup_name = f"group-{uuid4()}"\nclient.create_subscription(group_name=group_name)\n\nevents = []\n\ndef handle_event(event):\n    events.append(event)\n    if event.stream_name == stream_name3:\n        if event.data == event9.data:\n            raise Exception()\n\n\nreader = SubscriptionReader(\n    client=client,\n    group_name=group_name,\n    callback=handle_event\n)\n\nreader.start()\nreader.join()\n\nassert events[-1].data == event9.data\n```\n\nPlease note, when processing events in a downstream component, the commit position of\nthe last successfully processed event is usefully recorded by the downstream component\nso that the commit position can be determined by the downstream component from its own\nrecorded when it is restarted. This commit position can be used to specify the commit\nposition from which to subscribe. Since this commit position represents the position of\nthe last successfully processed event in a downstream component, so it will be usual to\nwant to read from the next event after this position, because that is the next event\nthat needs to be processed. However, when subscribing for events using a persistent\nsubscription in EventStoreDB, the event at the specified commit position MAY be returned\nas the first event in the received sequence of recorded events, and so it may\nbe necessary to check the commit position of the received events and to discard\nany  recorded event object that has a commit position equal to the commit position\nspecified in the request.\n\nWhilst there are some advantages of persistent subscriptions, by tracking in the\nupstream server the position in the commit sequence of events that have been processed,\nthere is a danger of "dual writing" in the consumption of events. The danger is that if\nan event is successfully processed but then the acknowledgment fails, the event may be\nreceived more than once. On the other hand, if the acknowledgment is successful but\nthen the processing fails, the event may effectively not be been processed. By either\nprocessing an events more than once, or failing to process an event, the resulting state\nof the processing of the recorded events might be inaccurate, or possibly\ninconsistent, and perhaps catastrophically so. Any relatively minor consequences may or\nmay not matter in your situation. But sometimes inconsistencies may halt processing\nuntil the issue is resolved. You can avoid "dual writing" in the consumption of events\nby atomically recording the commit position of an event that has been processed along\nwith the results of processing that event (that is, with both things being recorded in\nthe same transaction), and making these records unique so that transactions will be\nrolled back preventing the results of reprocessing the event being committed.\n\n## Notes\n\n### Regular expression filters\n\nThe filter arguments in `read_all_events()`, `subscribe_all_events()`,\n`create_subscription()` and `commit_position()` are applied to the `type`\nattribute of recorded events.\n\nThe default value of the `filter_exclude` arguments is designed to exclude\nEventStoreDB "system" and "persistence subscription config" events, which\notherwise would be included. System events generated by EventStoreDB all\nhave `type` strings that start with the `$` sign. Persistence subscription\nevents generated when manipulating persistence subscriptions all have `type`\nstrings that start with `PersistentConfig`.\n\nFor example, to match the type of EventStoreDB system events, use the regular\nexpression `r\'\\$.+\'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is\nset to `r\'\\$.+\'`. You can import this value\n(`from esdbclient import ESDB_SYSTEM_EVENTS_REGEX`) and use\nit when building longer sequences of regular expressions.\n\nSimilarly, to match the type of EventStoreDB persistence subscription events, use the\nregular expression `r\'PersistentConfig\\d+\'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`\nis set to `r\'PersistentConfig\\d+\'`. You can also import this value\n(`from esdbclient import ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`) and use it when building\nlonger sequences of regular expressions.\n\nThe constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that match\nthe events that EventStoreDB generates internally, events that are extraneous to those\nwhich you append using the `append_events()` method.\n\nFor example, to exclude system events and persistence subscription configuration events,\nand snapshots, you might use the sequence `DEFAULT_EXCLUDE_FILTER + [\'.*Snapshot\']` as\nthe value of the `filter_exclude` argument when calling `read_all_events()`,\n`subscribe_all_events()`, `create_subscription()` or `get_commit_position()`.\n\n### The NewEvent class\n\nThe `NewEvent` class is used when appending events.\n\nThe required argument `type` is a Python `str` object, used to indicate the type of\nthe event that will be recorded.\n\nThe required argument `data` is a Python `bytes` object, used to indicate the data of\nthe event that will be recorded.\n\nThe optional argument `metadata` is a Python `bytes` object, used to indicate any\nmetadata of the event that will be recorded. The default value is an empty `bytes`\nobject.\n\nThe optional argument `content_type` is a Python `str` object, used to indicate the\ntype of the data that will be recorded for this event. The default value is\n`application/json`, which indicates that the `data` was serialised using JSON.\nAn alternative value for this argument is `application/octet-stream`.\n\nThe optional argument `id` is a Python `UUID` object, used to specify the unique ID\nof the event that will be recorded. This value will default to a new version-4 UUID.\n\n```python\nnew_event1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'{"name": "Greg"}\',\n)\nassert new_event1.type == \'OrderCreated\'\nassert new_event1.data == b\'{"name": "Greg"}\'\nassert new_event1.metadata == b\'\'\nassert new_event1.content_type == \'application/json\'\nassert isinstance(new_event1.id, UUID)\n\nevent_id = uuid4()\nnew_event2 = NewEvent(\n    type=\'ImageCreated\',\n    data=b\'01010101010101\',\n    metadata=b\'{"a": 1}\',\n    content_type=\'application/octet-stream\',\n    id=event_id,\n)\nassert new_event2.type == \'ImageCreated\'\nassert new_event2.data == b\'01010101010101\'\nassert new_event2.metadata == b\'{"a": 1}\'\nassert new_event2.content_type == \'application/octet-stream\'\nassert new_event2.id == event_id\n```\n\n### The RecordedEvent class\n\nThe `RecordedEvent` class is used when reading events.\n\nThe attribute `type` is a Python `str` object, used to indicate the type of event\nthat was recorded.\n\nThe attribute `data` is a Python `bytes` object, used to indicate the data of the\nevent that was recorded.\n\nThe attribute `metadata` is a Python `bytes` object, used to indicate the metadata of\nthe event that was recorded.\n\nThe attribute `content_type` is a Python `str` object, used to indicate the type of\ndata that was recorded for this event (usually `application/json` to indicate that\nthis data can be parsed as JSON, but alternatively `application/octet-stream` to\nindicate that it is something else).\n\nThe attribute `id` is a Python `UUID` object, used to indicate the unique ID of the\nevent that was recorded. Please note, when recorded events are returned from a call\nto `read_stream_events()` in EventStoreDB v21.10, the commit position is not actually\nset in the response. For this reason, this attribute is actually typed as an optional\nvalue (`Optional[UUID]`), and this case the value of this attribute will be `None`.\n\nThe attribute `stream_name` is a Python `str` object, used to indicate the name of the\nstream in which the event was recorded.\n\nThe attribute `stream_position` is a Python `int`, used to indicate the position in the\nstream at which the event was recorded.\n\nThe attribute `commit_position` is a Python `int`, used to indicate the commit position\nat which the event was recorded.\n\n```python\nfrom esdbclient.events import RecordedEvent\n\nrecorded_event = RecordedEvent(\n    type=\'OrderCreated\',\n    data=b\'{}\',\n    metadata=b\'\',\n    content_type=\'application/json\',\n    id=uuid4(),\n    stream_name=\'stream1\',\n    stream_position=0,\n    commit_position=512,\n)\n```\n\n## Contributors\n\n### Install Poetry\n\nThe first thing is to check you have Poetry installed.\n\n    $ poetry --version\n\nIf you don\'t, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\n    $ curl -sSL https://install.python-poetry.org | python3 -\n\nIt will help to make sure Poetry\'s bin directory is in your `PATH` environment variable.\n\nBut in any case, make sure you know the path to the `poetry` executable. The Poetry\ninstaller tells you where it has been installed, and how to configure your shell.\n\nPlease refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on\nusing Poetry.\n\n### Setup for PyCharm users\n\nYou can easily obtain the project files using PyCharm (menu "Git > Clone...").\nPyCharm will then usually prompt you to open the project.\n\nOpen the project in a new window. PyCharm will then usually prompt you to create\na new virtual environment.\n\nCreate a new Poetry virtual environment for the project. If PyCharm doesn\'t already\nknow where your `poetry` executable is, then set the path to your `poetry` executable\nin the "New Poetry Environment" form input field labelled "Poetry executable". In the\n"New Poetry Environment" form, you will also have the opportunity to select which\nPython executable will be used by the virtual environment.\n\nPyCharm will then create a new Poetry virtual environment for your project, using\na particular version of Python, and also install into this virtual environment the\nproject\'s package dependencies according to the `pyproject.toml` file, or the\n`poetry.lock` file if that exists in the project files.\n\nYou can add different Poetry environments for different Python versions, and switch\nbetween them using the "Python Interpreter" settings of PyCharm. If you want to use\na version of Python that isn\'t installed, either use your favourite package manager,\nor install Python by downloading an installer for recent versions of Python directly\nfrom the [Python website](https://www.python.org/downloads/).\n\nOnce project dependencies have been installed, you should be able to run tests\nfrom within PyCharm (right-click on the `tests` folder and select the \'Run\' option).\n\nBecause of a conflict between pytest and PyCharm\'s debugger and the coverage tool,\nyou may need to add ``--no-cov`` as an option to the test runner template. Alternatively,\njust use the Python Standard Library\'s ``unittest`` module.\n\nYou should also be able to open a terminal window in PyCharm, and run the project\'s\nMakefile commands from the command line (see below).\n\n### Setup from command line\n\nObtain the project files, using Git or suitable alternative.\n\nIn a terminal application, change your current working directory\nto the root folder of the project files. There should be a Makefile\nin this folder.\n\nUse the Makefile to create a new Poetry virtual environment for the\nproject and install the project\'s package dependencies into it,\nusing the following command.\n\n    $ make install-packages\n\nIt\'s also possible to also install the project in \'editable mode\'.\n\n    $ make install\n\nPlease note, if you create the virtual environment in this way, and then try to\nopen the project in PyCharm and configure the project to use this virtual\nenvironment as an "Existing Poetry Environment", PyCharm sometimes has some\nissues (don\'t know why) which might be problematic. If you encounter such\nissues, you can resolve these issues by deleting the virtual environment\nand creating the Poetry virtual environment using PyCharm (see above).\n\n### Project Makefile commands\n\nYou can start EventStoreDB using the following command.\n\n    $ make start-eventstoredb\n\nYou can run tests using the following command (needs EventStoreDB to be running).\n\n    $ make test\n\nYou can stop EventStoreDB using the following command.\n\n    $ make stop-eventstoredb\n\nYou can check the formatting of the code using the following command.\n\n    $ make lint\n\nYou can reformat the code using the following command.\n\n    $ make fmt\n\nTests belong in `./tests`. Code-under-test belongs in `./esdbclient`.\n\nEdit package dependencies in `pyproject.toml`. Update installed packages (and the\n`poetry.lock` file) using the following command.\n\n    $ make update-packages\n',
+    'author': 'John Bywater',
+    'author_email': 'john.bywater@appropriatesoftware.net',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/pyeventsourcing/esdbclient',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.7,<4.0',
+}
 
-All the code in this package has typing annotations. The static typing
-annotations checked relatively strictly with mypy.
-
-Not all the features of the EventStoreDB API are presented
-by this client in its current form, however many of the most
-useful aspects are presented in an easy-to-use interface (see below).
-For an example of usage, see the [eventsourcing-eventstoredb](
-https://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.
-
-## Table of contents
-
-<!-- TOC -->
-* [Installation](#installation)
-* [Server](#server)
-  * [Start EventStoreDB](#start-eventstoredb)
-  * [Stop EventStoreDB](#stop-eventstoredb)
-* [Client](#client)
-* [Streams](#streams)
-  * [Append events](#append-events)
-  * [Get current stream position](#get-current-stream-position)
-  * [Read stream events](#read-stream-events)
-  * [Read all recorded events](#read-all-recorded-events)
-  * [Get current commit position](#get-current-commit-position)
-* [Subscriptions](#subscriptions)
-  * [Catch-up subscriptions](#catch-up-subscriptions)
-  * [Persistent subscriptions](#persistent-subscriptions)
-* [Notes](#notes)
-  * [Regular expression filters](#regular-expression-filters)
-  * [The NewEvent class](#the-newevent-class)
-  * [The RecordedEvent class](#the-recordedevent-class)
-* [Contributors](#contributors)
-  * [Install Poetry](#install-poetry)
-  * [Setup for PyCharm users](#setup-for-pycharm-users)
-  * [Setup from command line](#setup-from-command-line)
-  * [Project Makefile commands](#project-makefile-commands)
-<!-- TOC -->
-
-## Installation
-
-Use pip to install this package from
-[the Python Package Index](https://pypi.org/project/esdbclient/).
-
-    $ pip install esdbclient
-
-It is recommended to install Python packages into a Python virtual environment.
-
-
-## Server
-
-### Start EventStoreDB
-
-Use Docker to run EventStoreDB using the official Docker container image on DockerHub.
-
-For development, you can start a "secure" server locally on port 2113 using the following command.
-
-    $ docker run -d --name my-eventstoredb -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:22.10.0-buster-slim --dev
-
-Alternatively, you can start an "insecure" server locally on port 2113 using the following command.
-
-    $ docker run -d --name my-eventstoredb -it -p 2113:2113 eventstore/eventstore:22.10.0-buster-slim --insecure
-
-To connect to the "insecure" local server using the client in this package, you just need
-to know the local hostname and the port number. To connect to the "secure" local
-development server, you will also need to know that the username is "admin" and
-the password is "changeit". You will also need to get the SSL/TLS certificate from
-the server. You can get the server certificate with the following command.
-
-    $ python -c "import ssl; print(get_server_certificate(addr=('localhost', 2113)))"
-
-
-### Stop EventStoreDB
-
-To stop and remove the `my-eventstoredb` container created above, use the following Docker commands.
-
-    $ docker stop my-eventstoredb
-	$ docker rm my-eventstoredb
-
-
-## Client
-
-The `EsdbClient` class can be imported from the `esdbclient` package.
-
-```python
-from esdbclient import EsdbClient
-```
-
-The `EsdbClient` class can be constructed with `host` and `port` arguments.
-The `host` and `port` arguments indicate the hostname and port number of the
-EventStoreDB server.
-
-If the EventStoreDB server is "secure", then also use the `server_cert`,
-`username` and `password` arguments.
-
-The `host` argument is expected to be a Python `str`. The `port` argument is expected
-to be a Python `int`. The `server_cert` is expected to be a Python `str` containing
-the PEM encoded SSL/TLS server certificate. Both `username` and `password` are expected
-to be a Python `str`.
-
-In the example below, the constructor argument values are taken from the operating
-system environment, because the examples in this document are tested with both
-a "secure" and an "insecure" server.
-
-```python
-import os
-
-client = EsdbClient(
-    host=os.getenv("ESDB_HOST"),
-    port=int(os.getenv("ESDB_PORT")),
-    server_cert=os.getenv("ESDB_SERVER_CERT"),
-    username=os.getenv("ESDB_USERNAME"),
-    password=os.getenv("ESDB_PASSWORD"),
-)
-```
-
-## Streams
-
-In EventStoreDB, a "stream" is a sequence of recorded events that all have
-the same "stream name". Each recorded event has a "position" in its stream.
-The positions of the recorded events in a stream is a gapless sequence starting
-from zero.
-
-### Append events
-
-The client has an `append_events()` method, which can be used to append
-new events to a "stream".
-
-Three arguments are required, `stream_name`, `expected_position`
-and `events`.
-
-The `stream_name` argument is required, and is expected to be a Python
-`str` object that uniquely identifies the stream in the database.
-
-The `expected_position` argument is required, is expected to be: either `None`
-if new events are being appended to a new stream, or an integer equal to the
-position the last recorded event in the stream.
-
-The stream positions of recorded events start from zero. And so, when appending
-the second new event to a stream that has one recorded event, the correct value
-of the `expected_position` argument is `0`. Similarly, when appending the third
-new event to a stream that has two recorded events, the correct value
-of the `expected_position` argument is `1`.
-
-Streams are created by appending events. The correct value of the `expected_position`
-argument when appending the first event of a new stream (a stream with zero recorded
-events) is `None`. Please note, it is not possible to create an "empty" stream in
-EventStoreDB.
-
-If there is a mismatch between the given value of the `expected_position` argument
-and the position of the last recorded event in a stream, then an `ExpectedPositionError`
-exception will be raised. This effectively accomplishes optimistic concurrency control.
-
-If you wish to disable optimistic concurrency control when appending new events, you
-can set the `expected_position` to a negative integer.
-
-If you need to discover the current position of the last recorded event in a stream,
-you can use the `get_stream_position()` method (see below).
-
-The `events` argument is required, and is expected to be a sequence of new
-event objects to be appended to the named stream. The `NewEvent` class should
-be used to construct new event objects (see below).
-
-Please note, the append events operation is atomic, so that either all
-or none of the given new events will be recorded. By design, it is only
-possible with EventStoreDB to atomically record new events in one stream.
-
-In the example below, a new event is appended to a new stream.
-
-```python
-from uuid import uuid4
-
-from esdbclient import NewEvent
-
-# Construct new event object.
-event1 = NewEvent(
-    type='OrderCreated',
-    data=b'data1',
-    metadata=b'{}'
-)
-
-# Define stream name.
-stream_name1 = str(uuid4())
-
-# Append list of events to new stream.
-commit_position1 = client.append_events(
-    stream_name=stream_name1,
-    expected_position=None,
-    events=[event1],
-)
-```
-
-In the example below, two subsequent events are appended to an existing
-stream.
-
-```python
-event2 = NewEvent(
-    type='OrderUpdated',
-    data=b'data2',
-    metadata=b'{}',
-)
-event3 = NewEvent(
-    type='OrderDeleted',
-    data=b'data3',
-    metadata=b'{}',
-)
-
-commit_position2 = client.append_events(
-    stream_name=stream_name1,
-    expected_position=0,
-    events=[event2, event3],
-)
-```
-
-If the append operation is successful, this method returns an integer
-representing the overall "commit position" as it was when the operation
-was completed. Otherwise, an exception will be raised.
-
-A "commit position" is a monotonically increasing integer representing
-the position of the recorded event in a "total order" of all recorded
-events in the database across all streams. The sequence of commit positions
-is not gapless. It represents the position of the event record on disk, and
-there are usually large differences between successive commits.
-
-The "commit position" returned in this way can be used to wait for a
-downstream component to have processed the newly appended events.
-For example, after a user interface command that results in the recording
-of new events, and before a query is issued that depends on an eventually
-consistent materialized view in a downstream component that would be stale
-if those newly appended events have not yet been processed, the user interface
-can poll the downstream component, to see if it has processed an event at that
-commit position, before executing a query for that materialized view.
-
-### Get current stream position
-
-The client has a `get_stream_position()` method, which can be used to
-get the current "stream position" of a stream (the position in the
-stream of the last recorded event in that stream).
-
-This method has a `stream_name` argument, which is required.
-
-This method also takes an optional `timeout` argument, that
-is expected to be a Python `float`, which sets a deadline
-for the completion of the gRPC operation.
-
-The sequence of positions in a stream is gapless. It is zero-based,
-so that a stream with one recorded event has a current stream
-position of `0`. The current stream position is `1` when a stream has
-two events, and it is `2` when there are events, and so on.
-
-In the example below, the current stream position is obtained of the
-stream to which events were appended in the examples above.
-Because the sequence of stream positions is zero-based, and because
-three events were appended, so the current stream position is `2`.
-
-```python
-stream_position = client.get_stream_position(
-    stream_name=stream_name1
-)
-
-assert stream_position == 2
-```
-
-If a stream does not exist, the returned stream position value is `None`,
-which matches the required expected position when appending the first event
-of a new stream (see above).
-
-```python
-stream_position = client.get_stream_position(
-    stream_name=str(uuid4())
-)
-
-assert stream_position == None
-```
-
-This method takes an optional argument `timeout` which is a float that sets
-a deadline for the completion of the gRPC operation.
-
-
-### Read stream events
-
-The client has a `read_stream_events()` method, which can be used to read
-the events of a stream.
-
-This method returns nn iterable object that yields recorded event objects.
-These recorded event objects are instances of the `RecordedEvent` class (see below)
-
-This method has one required argument, `stream_name`, which is the name of
-the stream to be read. By default, the recorded events in the stream
-are returned in the order they were recorded.
-
-The example below shows how to read the recorded events of a stream
-forwards from the start of the stream to the end of the stream. The
-name of a stream is given when calling the method. In this example,
-the iterable response object is converted into a Python `list`, which
-contains all the recorded event objects that were read from the stream.
-
-```python
-response = client.read_stream_events(
-    stream_name=stream_name1
-)
-
-events = list(response)
-```
-
-Now that we have a list of event objects, we can check we got the
-three events that were appended to the stream, and that they are
-ordered exactly as they were appended.
-
-```python
-assert len(events) == 3
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 0
-assert events[0].type == event1.type
-assert events[0].data == event1.data
-
-assert events[1].stream_name == stream_name1
-assert events[1].stream_position == 1
-assert events[1].type == event2.type
-assert events[1].data == event2.data
-
-assert events[2].stream_name == stream_name1
-assert events[2].stream_position == 2
-assert events[2].type == event3.type
-assert events[2].data == event3.data
-```
-
-The method `read_stream_events()` also supports four optional arguments,
-`position`, `backwards`, `limit`, and `timeout`.
-
-The optional `position` argument is an optional integer that can be used to indicate
-the position in the stream from which to start reading. This argument is `None`
-by default, which means the stream will be read either from the start of the
-stream (the default behaviour), or from the end of the stream if `backwards` is
-`True` (see below). When reading a stream from a specific position in the stream, the
-recorded event at that position WILL be included, both when reading forwards
-from that position, and when reading backwards from that position.
-
-The optional argument `backwards` is a boolean, by default `False`, which means the
-stream will be read forwards by default, so that events are returned in the
-order they were appended, If `backwards` is `True`, the stream will be read
-backwards, so that events are returned in reverse order.
-
-The optional argument `limit` is an integer which limits the number of events that will
-be returned. The default value is `sys.maxint`.
-
-The optional argument `timeout` is a float which sets a deadline for the completion of
-the gRPC operation.
-
-The example below shows how to read recorded events in a stream forwards from
-a specific stream position to the end of the stream.
-
-```python
-events = list(
-    client.read_stream_events(
-        stream_name=stream_name1,
-        position=1,
-    )
-)
-
-assert len(events) == 2
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 1
-assert events[0].type == event2.type
-assert events[0].data == event2.data
-
-assert events[1].stream_name == stream_name1
-assert events[1].stream_position == 2
-assert events[1].type == event3.type
-assert events[1].data == event3.data
-```
-
-The example below shows how to read the recorded events in a stream backwards from
-the end of the stream to the start of the stream.
-
-```python
-events = list(
-    client.read_stream_events(
-        stream_name=stream_name1,
-        backwards=True,
-    )
-)
-
-assert len(events) == 3
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 2
-assert events[0].type == event3.type
-assert events[0].data == event3.data
-
-assert events[1].stream_name == stream_name1
-assert events[1].stream_position == 1
-assert events[1].type == event2.type
-assert events[1].data == event2.data
-```
-
-The example below shows how to read a limited number (two) of the recorded events
-in a stream forwards from the start of the stream.
-
-```python
-events = list(
-    client.read_stream_events(
-        stream_name=stream_name1,
-        limit=2,
-    )
-)
-
-assert len(events) == 2
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 0
-assert events[0].type == event1.type
-assert events[0].data == event1.data
-
-assert events[1].stream_name == stream_name1
-assert events[1].stream_position == 1
-assert events[1].type == event2.type
-assert events[1].data == event2.data
-```
-
-The example below shows how to read a limited number (one) of the recorded
-events in a stream backwards from a given stream position.
-
-```python
-events = list(
-    client.read_stream_events(
-        stream_name=stream_name1,
-        position=2,
-        backwards=True,
-        limit=1,
-    )
-)
-
-assert len(events) == 1
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 2
-assert events[0].type == event3.type
-assert events[0].data == event3.data
-```
-
-### Read all recorded events
-
-The method `read_all_events()` can be used to read all recorded events
-in the database in the order they were recorded. An iterable object of
-recorded events is returned. This iterable object will stop when it has
-yielded the last recorded event.
-
-The method `read_stream_events()` supports six optional arguments,
-`commit_position`, `backwards`, `filter_exclude`, `filter_include`, `limit`,
-and `timeout`.
-
-The optional argument `position` is an optional integer that can be used to specify
-the commit position from which to start reading. This argument is `None` by
-default, meaning that all the events will be read either from the start, or
-from the end if `backwards` is `True` (see below). Please note, if specified,
-the specified position must be an actually existing commit position, because
-any other number will result in a server error (at least in EventStoreDB v21.10).
-
-Please also note, when reading forwards from a specific commit position, the event
-at the specified position WILL be included. However, when reading backwards, the
-event at the specified position will NOT be included. (This non-inclusive behaviour
-of excluding the specified commit position when reading all streams differs from the
-behaviour when reading a named stream backwards from a specific stream position, I'm
-not sure why.)
-
-The optional argument `backwards` is a boolean which is by default `False` meaning the
-events will be read forwards by default, so that events are returned in the
-order they were committed, If `backwards` is `True`, the events will be read
-backwards, so that events are returned in reverse order.
-
-The optional argument `filter_exclude` is a sequence of regular expressions that
-match the type strings of recorded events that should not be included. By default,
-this argument will match "system events", so that they will not be included.
-This argument is ignored if `filter_include` is set to a non-empty sequence.
-
-The optional argument `filter_include` is a sequence of regular expressions
-that match the type strings of recorded events that should be included. By
-default, this argument is an empty tuple. If this argument is set to a
-non-empty sequence, the `filter_exclude` argument is ignored.
-
-Please note, the filtering happens on the EventStoreDB server, and the
-`limit` argument is applied on the server after filtering. See below for
-more information about filter regular expressions.
-
-The optional argument `limit` is an integer which limits the number of events that will
-be returned. The default value is `sys.maxint`.
-
-The optional argument `timeout` is a float which sets a deadline for the completion of
-the gRPC operation.
-
-The example below shows how to read all events in the database in the
-order they were recorded.
-
-```python
-events = list(client.read_all_events())
-
-assert len(events) >= 3
-```
-
-The example below shows how to read all recorded events from a particular commit position.
-
-```python
-events = list(
-    client.read_all_events(
-        commit_position=commit_position1
-    )
-)
-
-assert len(events) == 3
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 0
-assert events[0].type == event1.type
-assert events[0].data == event1.data
-
-assert events[1].stream_name == stream_name1
-assert events[1].stream_position == 1
-assert events[1].type == event2.type
-assert events[1].data == event2.data
-
-assert events[2].stream_name == stream_name1
-assert events[2].stream_position == 2
-assert events[2].type == event3.type
-assert events[2].data == event3.data
-```
-
-The example below shows how to read all recorded events in reverse order.
-
-```python
-events = list(
-    client.read_all_events(
-        backwards=True
-    )
-)
-
-assert len(events) >= 3
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 2
-assert events[0].type == event3.type
-assert events[0].data == event3.data
-
-assert events[1].stream_name == stream_name1
-assert events[1].stream_position == 1
-assert events[1].type == event2.type
-assert events[1].data == event2.data
-
-assert events[2].stream_name == stream_name1
-assert events[2].stream_position == 0
-assert events[2].type == event1.type
-assert events[2].data == event1.data
-```
-
-The example below shows how to read a limited number (one) of the recorded events
-in the database forwards from a specific commit position. Please note, when reading
-all events forwards from a specific commit position, the event at the specified
-position WILL be included.
-
-
-```python
-events = list(
-    client.read_all_events(
-        commit_position=commit_position1,
-        limit=1,
-    )
-)
-
-assert len(events) == 1
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 0
-assert events[0].type == event1.type
-assert events[0].data == event1.data
-
-assert events[0].commit_position == commit_position1
-```
-
-The example below shows how to read a limited number (one) of the recorded events
-in the database backwards from the end. This gives the last recorded event.
-
-```python
-events = list(
-    client.read_all_events(
-        backwards=True,
-        limit=1,
-    )
-)
-
-assert len(events) == 1
-
-assert events[0].stream_name == stream_name1
-assert events[0].stream_position == 2
-assert events[0].type == event3.type
-assert events[0].data == event3.data
-```
-
-The example below shows how to read a limited number (one) of the recorded events
-in the database backwards from a specific commit position. Please note, when reading
-all events backwards from a specific commit position, the event at the specified
-position WILL NOT be included.
-
-```python
-events = list(
-    client.read_all_events(
-        commit_position=commit_position2,
-        backwards=True,
-        limit=1,
-    )
-)
-
-assert len(events) == 1
-
-assert events[0].commit_position < commit_position2
-```
-
-### Get current commit position
-
-The method `get_commit_position()` can be used to get the current
-commit position of the database.
-
-```python
-commit_position = client.get_commit_position()
-```
-
-This method takes an optional argument `timeout` which is a float that sets
-a deadline for the completion of the gRPC operation.
-
-This method can be useful to measure progress of a downstream component
-that is processing all recorded events, by comparing the current commit
-position with the recorded commit position of the last successfully processed
-event in a downstream component.
-
-The value of the `commit_position` argument when reading events either by using
-the `read_all_events()` method or by using a catch-up subscription would usually
-be determined by the recorded commit position of the last successfully processed
-event in a downstream component.
-
-## Subscriptions
-
-### Catch-up subscriptions
-
-The client has a `subscribe_all_events()` method, which can be used
-to start a "catch-up" subscription.
-
-Many catch-up subscriptions can be created, concurrently or
-successively, and all will receive all the events they are
-subscribed to receive.
-
-This method returns an iterator object which yields recorded events,
-including events that are recorded after the subscription was created.
-This iterator object will therefore not stop, unless the connection
-to the database is lost. The connection will be closed when the
-iterator object is deleted from memory, which will happen when the
-iterator object goes out of scope is explicitly deleted (see below),
-and the connection may be closed by the server.
-
-This method takes an optional `commit_position` argument, which can be
-used to specify a commit position from which to subscribe for
-recorded events. The default value is `None`, which means
-the subscription will operate from the first recorded event
-in the database. If a commit position is given, it must match
-an actually existing commit position in the database. The events
-that are obtained will not include the event recorded at that commit
-position.
-
-This method also takes three other optional arguments, `filter_exclude`,
-`filter_include`, and `timeout`.
-
-The argument `filter_exclude` is a sequence of regular expressions matching
-the type strings of recorded events that should be excluded. By default,
-this argument will match "system events", so that they will not be included.
-This argument is ignored if `filter_include` is set to a non-empty sequence.
-
-The argument `filter_include` is a sequence of regular expressions
-matching the type strings of recorded events that should be included. By
-default, this argument is an empty tuple. If this argument is set to a
-non-empty sequence, the `filter_exclude` argument is ignored.
-
-Please note, the filtering happens on the EventStoreDB server, and the
-`limit` argument is applied on the server after filtering. See below for
-more information about filter regular expressions.
-
-The argument `timeout` is a float which sets a deadline for the completion of
-the gRPC operation. This probably isn't very useful, but is included for
-completeness and consistency with the other methods.
-
-The example below shows how to subscribe to receive all recorded
-events from a specific commit position. Three already-recorded
-events are received, and then three new events are recorded, which
-are then received via the subscription.
-
-```python
-
-# Get the commit position (usually from database of materialised views).
-commit_position = client.get_commit_position()
-
-# Append three events to another stream.
-stream_name2 = str(uuid4())
-event4 = NewEvent(
-    type='OrderCreated',
-    data=b'data4',
-    metadata=b'{}',
-)
-event5 = NewEvent(
-    type='OrderUpdated',
-    data=b'data5',
-    metadata=b'{}',
-)
-event6 = NewEvent(
-    type='OrderDeleted',
-    data=b'data6',
-    metadata=b'{}',
-)
-client.append_events(
-    stream_name=stream_name2,
-    expected_position=None,
-    events=[event4, event5, event6],
-)
-
-# Subscribe from the commit position.
-subscription = client.subscribe_all_events(
-    commit_position=commit_position
-)
-
-# Catch up by receiving the three events from the subscription.
-events = []
-for event in subscription:
-    events.append(event)
-    if event.data == event6.data and event.stream_name:
-        break
-
-assert events[0].data == event4.data
-assert events[1].data == event5.data
-assert events[2].data == event6.data
-
-
-# Append three more events.
-stream_name3 = str(uuid4())
-event7 = NewEvent(
-    type='OrderCreated',
-    data=b'data7',
-    metadata=b'{}',
-)
-event8 = NewEvent(
-    type='OrderUpdated',
-    data=b'data8',
-    metadata=b'{}',
-)
-event9 = NewEvent(
-    type='OrderDeleted',
-    data=b'data9',
-    metadata=b'{}',
-)
-
-client.append_events(
-    stream_name=stream_name3,
-    expected_position=None,
-    events=[event7, event8, event9],
-)
-
-# Receive the three new events from the same subscription.
-for event in subscription:
-    # Check the stream name.
-    events.append(event)
-    if event.stream_name == stream_name3:
-        if event.data == event9.data:
-            break
-
-assert events[3].data == event7.data
-assert events[4].data == event8.data
-assert events[5].data == event9.data
-```
-
-Catch-up subscriptions are not registered in EventStoreDB (they are not
-"persistent" subscriptions). It is simply a streaming gRPC call which is
-kept open by the server, with newly recorded events sent to the client
-as the client iterates over the subscription. This kind of subscription
-is closed as soon as the subscription object goes out of memory.
-
-```python
-# End the subscription.
-del subscription
-```
-
-Please note, when processing events in a downstream component, the commit position of
-the last successfully processed event is usefully recorded by the downstream component
-so that the commit position can be determined by the downstream component from its own
-recorded when it is restarted. This commit position can be used to specify the commit
-position from which to subscribe. Since this commit position represents the position of
-the last successfully processed event in a downstream component, so it will be usual to
-want the next event after this position, because that is the next event that needs to
-be processed. When subscribing for events using a catchup-subscription
-in EventStoreDB, the event at the specified commit position will NOT be included in
-the sequence of recorded events.
-
-To accomplish "exactly once" processing of the events, the commit position
-of a recorded event should be recorded atomically and uniquely along with
-the result of processing recorded events, for example in the same database
-as materialised views when implementing eventually-consistent CQRS, or in
-the same database as a downstream analytics or reporting or archiving
-application. This avoids "dual writing" in the processing of events.
-
-Recorded events received from a catch-up subscription cannot be acknowledged back
-to the EventStoreDB server (there is no need to do this). Acknowledging events is
-an aspect of "persistent subscriptions" (see below).
-
-The subscription object might be used directly when processing events. It might
-also be used within a thread dedicated to receiving events, with recorded events
-put on a queue for processing in a different thread. This package doesn't provide
-such thread or queue objects, you would need to do that yourself. Just make sure
-to reconstruct the subscription (and the queue) using your last recorded commit
-position when resuming the subscription after an error, to be sure all events
-are processed once.
-
-### Persistent subscriptions
-
-The method `create_subscription()` can be used to create a
-"persistent subscription" to EventStoreDB.
-
-This method takes a required `group_name` argument, which is the
-name of a "group" of consumers of the subscription.
-
-This method takes an optional `from_end` argument, which can be
-used to specify that the group of consumers of the subscription should
-only receive events that were recorded after the subscription was created.
-
-This method takes an optional `commit_position` argument, which can be
-used to specify a commit position from which the group of consumers of
-the subscription should receive events. Please note, the recorded event
-at the specified commit position MAY be included in the recorded events
-received by the group of consumers.
-
-If neither `from_end` or `position` are specified, the group of consumers
-of the subscription will receive all recorded events.
-
-The method `create_subscription()` does not return a value, because
-recorded events are obtained by the group of consumers of the subscription
-using the `read_subscription()` method.
-
-In the example below, a persistent subscription is created.
-
-```python
-# Create a persistent subscription.
-group_name = f"group-{uuid4()}"
-client.create_subscription(group_name=group_name)
-```
-
-The method `read_subscription()` can be used by a group of consumers to receive
-recorded events from a persistent subscription created using `create_subscription`.
-
-This method takes a required `group_name` argument, which is
-the name of a "group" of consumers of the subscription specified
-when `create_subscription()` was called.
-
-This method returns a 2-tuple: a "read request" object and a "read response" object.
-
-```python
-read_req, read_resp = client.read_subscription(group_name=group_name)
-```
-
-The "read response" object is an iterator that yields recorded events from
-the specified commit position.
-
-The "read request" object has an `ack()` method that can be used by a consumer
-in a group to acknowledge to the server that it has received and successfully
-processed a recorded event. This will prevent that recorded event being received
-by another consumer in the same group. The `ack()` method takes an `event_id`
-argument, which is the ID of the recorded event that has been received.
-
-The example below iterates over the "read response" object, and calls `ack()`
-on the "read response" object. The for loop breaks when we have received
-the last event, so that we can continue with the examples below.
-
-```python
-events = []
-for event in read_resp:
-    events.append(event)
-
-    # Acknowledge the received event.
-    read_req.ack(event_id=event.id)
-
-    # Break when the last event has been received.
-    if event.stream_name == stream_name3:
-        if event.data == event9.data:
-            break
-```
-
-The received events are the events we appended above.
-
-```python
-assert events[-9].data == event1.data
-assert events[-8].data == event2.data
-assert events[-7].data == event3.data
-assert events[-6].data == event4.data
-assert events[-5].data == event5.data
-assert events[-4].data == event6.data
-assert events[-3].data == event7.data
-assert events[-2].data == event8.data
-assert events[-1].data == event9.data
-```
-
-The "read request" object also has an `nack()` method that can be used by a consumer
-in a group to acknowledge to the server that it has failed successfully to
-process a recorded event. This will allow that recorded event to be received
-by this or another consumer in the same group.
-
-It might be more useful to encapsulate the request and response objects and to iterate
-over the "read response" in a separate thread, to call back to a handler function when
-a recorded event is received, and call `ack()` if the handler does not raise an
-exception, and to call `nack()` if an exception is raised. The example below shows how
-this might be done.
-
-```python
-from threading import Thread
-
-
-class SubscriptionReader:
-    def __init__(self, client, group_name, callback):
-        self.client = client
-        self.group_name = group_name
-        self.callback = callback
-        self.thread = Thread(target=self.read_subscription, daemon=True)
-        self.error = None
-
-    def start(self):
-        self.thread.start()
-
-    def join(self):
-        self.thread.join()
-
-    def read_subscription(self):
-        req, resp = self.client.read_subscription(group_name=self.group_name)
-        for event in resp:
-            try:
-                self.callback(event)
-            except Exception as e:
-                # req.nack(event.id)  # not yet implemented....
-                self.error = e
-                break
-            else:
-                req.ack(event.id)
-
-
-# Create another persistent subscription.
-group_name = f"group-{uuid4()}"
-client.create_subscription(group_name=group_name)
-
-events = []
-
-def handle_event(event):
-    events.append(event)
-    if event.stream_name == stream_name3:
-        if event.data == event9.data:
-            raise Exception()
-
-
-reader = SubscriptionReader(
-    client=client,
-    group_name=group_name,
-    callback=handle_event
-)
-
-reader.start()
-reader.join()
-
-assert events[-1].data == event9.data
-```
-
-Please note, when processing events in a downstream component, the commit position of
-the last successfully processed event is usefully recorded by the downstream component
-so that the commit position can be determined by the downstream component from its own
-recorded when it is restarted. This commit position can be used to specify the commit
-position from which to subscribe. Since this commit position represents the position of
-the last successfully processed event in a downstream component, so it will be usual to
-want to read from the next event after this position, because that is the next event
-that needs to be processed. However, when subscribing for events using a persistent
-subscription in EventStoreDB, the event at the specified commit position MAY be returned
-as the first event in the received sequence of recorded events, and so it may
-be necessary to check the commit position of the received events and to discard
-any  recorded event object that has a commit position equal to the commit position
-specified in the request.
-
-Whilst there are some advantages of persistent subscriptions, by tracking in the
-upstream server the position in the commit sequence of events that have been processed,
-there is a danger of "dual writing" in the consumption of events. The danger is that if
-an event is successfully processed but then the acknowledgment fails, the event may be
-received more than once. On the other hand, if the acknowledgment is successful but
-then the processing fails, the event may effectively not be been processed. By either
-processing an events more than once, or failing to process an event, the resulting state
-of the processing of the recorded events might be inaccurate, or possibly
-inconsistent, and perhaps catastrophically so. Any relatively minor consequences may or
-may not matter in your situation. But sometimes inconsistencies may halt processing
-until the issue is resolved. You can avoid "dual writing" in the consumption of events
-by atomically recording the commit position of an event that has been processed along
-with the results of processing that event (that is, with both things being recorded in
-the same transaction), and making these records unique so that transactions will be
-rolled back preventing the results of reprocessing the event being committed.
-
-## Notes
-
-### Regular expression filters
-
-The `filter_exclude` and `filter_include` arguments in `read_all_events()` and
-`subscribe_all_events()` are applied to the `type` attribute of recorded events.
-
-The default value of the `filter_exclude` arguments is designed to exclude
-EventStoreDB "system events", which otherwise would be included. System
-events, by convention in EventStoreDB, all have `type` strings that
-start with the `$` sign.
-
-Please note, characters that have a special meaning in regular expressions
-will need to be escaped (with double-backslash) when matching these characters
-in type strings.
-
-For example, to match EventStoreDB system events, use the sequence `['\\$.*']`.
-Please note, the constant `ESDB_EVENTS_REGEX` is set to `'\\$.*'`. You
-can import this value (`from esdbclient import ESDB_EVENTS_REGEX`) and use
-it when building longer sequences of regular expressions. For example,
-to exclude system events and snapshots, you might use the sequence
-`[ESDB_EVENTS_REGEX, '.*Snapshot']` as the value of the `filter_exclude`
-argument.
-
-
-### The NewEvent class
-
-The `NewEvent` class can be used to define new events.
-
-The attribute `type` is a unicode string, used to specify the type of the event
-to be recorded.
-
-The attribute `data` is a byte string, used to specify the data of the event
-to be recorded. Please note, in this version of this Python client,
-writing JSON event data to EventStoreDB isn't supported, but it might be in
-a future version.
-
-The attribute `metadata` is a byte string, used to specify metadata for the event
-to be recorded.
-
-```python
-new_event = NewEvent(
-    type='OrderCreated',
-    data=b'{}',
-    metadata=b'{}',
-)
-```
-
-### The RecordedEvent class
-
-The `RecordedEvent` class is used when reading recorded events.
-
-The attribute `type` is a unicode string, used to indicate the type of the event
-that was recorded.
-
-The attribute `data` is a byte string, used to indicate the data of the event
-that was recorded.
-
-The attribute `metadata` is a byte string, used to indicate metadata for the event
-that was recorded.
-
-The attribute `stream_name` is a unicode string, used to indicate the type of
-the name of the stream in which the event was recorded.
-
-The attribute `stream_position` is an integer, used to indicate
-the position in the stream at which the event was recorded.
-
-The attribute `commit_position` is an integer, used to indicate
-the position in total order of all recorded events at which the
-event was recorded.
-
-```python
-from esdbclient.events import RecordedEvent
-
-recorded_event = RecordedEvent(
-    id=uuid4(),
-    type='OrderCreated',
-    data=b'{}',
-    metadata=b'{}',
-    stream_name='stream1',
-    stream_position=0,
-    commit_position=512,
-)
-```
-
-## Contributors
-
-### Install Poetry
-
-The first thing is to check you have Poetry installed.
-
-    $ poetry --version
-
-If you don't, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).
-
-    $ curl -sSL https://install.python-poetry.org | python3 -
-
-It will help to make sure Poetry's bin directory is in your `PATH` environment variable.
-
-But in any case, make sure you know the path to the `poetry` executable. The Poetry
-installer tells you where it has been installed, and how to configure your shell.
-
-Please refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on
-using Poetry.
-
-### Setup for PyCharm users
-
-You can easily obtain the project files using PyCharm (menu "Git > Clone...").
-PyCharm will then usually prompt you to open the project.
-
-Open the project in a new window. PyCharm will then usually prompt you to create
-a new virtual environment.
-
-Create a new Poetry virtual environment for the project. If PyCharm doesn't already
-know where your `poetry` executable is, then set the path to your `poetry` executable
-in the "New Poetry Environment" form input field labelled "Poetry executable". In the
-"New Poetry Environment" form, you will also have the opportunity to select which
-Python executable will be used by the virtual environment.
-
-PyCharm will then create a new Poetry virtual environment for your project, using
-a particular version of Python, and also install into this virtual environment the
-project's package dependencies according to the `pyproject.toml` file, or the
-`poetry.lock` file if that exists in the project files.
-
-You can add different Poetry environments for different Python versions, and switch
-between them using the "Python Interpreter" settings of PyCharm. If you want to use
-a version of Python that isn't installed, either use your favourite package manager,
-or install Python by downloading an installer for recent versions of Python directly
-from the [Python website](https://www.python.org/downloads/).
-
-Once project dependencies have been installed, you should be able to run tests
-from within PyCharm (right-click on the `tests` folder and select the 'Run' option).
-
-Because of a conflict between pytest and PyCharm's debugger and the coverage tool,
-you may need to add ``--no-cov`` as an option to the test runner template. Alternatively,
-just use the Python Standard Library's ``unittest`` module.
-
-You should also be able to open a terminal window in PyCharm, and run the project's
-Makefile commands from the command line (see below).
-
-### Setup from command line
-
-Obtain the project files, using Git or suitable alternative.
-
-In a terminal application, change your current working directory
-to the root folder of the project files. There should be a Makefile
-in this folder.
-
-Use the Makefile to create a new Poetry virtual environment for the
-project and install the project's package dependencies into it,
-using the following command.
-
-    $ make install-packages
-
-It's also possible to also install the project in 'editable mode'.
-
-    $ make install
-
-Please note, if you create the virtual environment in this way, and then try to
-open the project in PyCharm and configure the project to use this virtual
-environment as an "Existing Poetry Environment", PyCharm sometimes has some
-issues (don't know why) which might be problematic. If you encounter such
-issues, you can resolve these issues by deleting the virtual environment
-and creating the Poetry virtual environment using PyCharm (see above).
-
-### Project Makefile commands
-
-You can start EventStoreDB using the following command.
-
-    $ make start-eventstoredb
-
-You can run tests using the following command (needs EventStoreDB to be running).
-
-    $ make test
-
-You can stop EventStoreDB using the following command.
-
-    $ make stop-eventstoredb
-
-You can check the formatting of the code using the following command.
-
-    $ make lint
-
-You can reformat the code using the following command.
-
-    $ make fmt
-
-Tests belong in `./tests`. Code-under-test belongs in `./esdbclient`.
-
-Edit package dependencies in `pyproject.toml`. Update installed packages (and the
-`poetry.lock` file) using the following command.
-
-    $ make update-packages
 
+setup(**setup_kwargs)
```

