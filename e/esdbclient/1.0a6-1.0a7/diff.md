# Comparing `tmp/esdbclient-1.0a6.tar.gz` & `tmp/esdbclient-1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdbclient-1.0a6.tar", max compression
+gzip compressed data, was "esdbclient-1.0a7.tar", max compression
```

## Comparing `esdbclient-1.0a6.tar` & `esdbclient-1.0a7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.0a6/LICENSE
--rw-r--r--   0        0        0   111383 2023-05-22 13:13:57.511132 esdbclient-1.0a6/README.md
--rw-r--r--   0        0        0      515 2023-05-10 19:02:05.845353 esdbclient-1.0a6/esdbclient/__init__.py
--rw-r--r--   0        0        0    14175 2023-05-20 01:30:08.950137 esdbclient-1.0a6/esdbclient/asyncio_client.py
--rw-r--r--   0        0        0    35531 2023-05-20 03:12:59.117064 esdbclient-1.0a6/esdbclient/client.py
--rw-r--r--   0        0        0    11560 2023-05-19 15:05:34.128220 esdbclient-1.0a6/esdbclient/connection.py
--rw-r--r--   0        0        0     2386 2023-05-19 15:05:37.413801 esdbclient-1.0a6/esdbclient/esdbapibase.py
--rw-r--r--   0        0        0      838 2023-05-11 20:15:54.815803 esdbclient-1.0a6/esdbclient/events.py
--rw-r--r--   0        0        0     3245 2023-05-20 01:32:12.161060 esdbclient-1.0a6/esdbclient/exceptions.py
--rw-r--r--   0        0        0     4928 2023-05-19 15:05:40.918186 esdbclient-1.0a6/esdbclient/gossip.py
--rw-r--r--   0        0        0    30889 2023-05-19 16:02:42.915580 esdbclient-1.0a6/esdbclient/persistent.py
--rw-r--r--   0        0        0    13401 2023-05-09 15:45:39.784205 esdbclient-1.0a6/esdbclient/protos/Grpc/cluster_pb2.py
--rw-r--r--   0        0        0    37958 2023-05-09 15:45:38.350807 esdbclient-1.0a6/esdbclient/protos/Grpc/cluster_pb2.pyi
--rw-r--r--   0        0        0    19336 2023-05-09 15:45:39.761236 esdbclient-1.0a6/esdbclient/protos/Grpc/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     1790 2023-05-09 15:45:39.793881 esdbclient-1.0a6/esdbclient/protos/Grpc/code_pb2.py
--rw-r--r--   0        0        0    13555 2023-05-09 15:45:37.813695 esdbclient-1.0a6/esdbclient/protos/Grpc/code_pb2.pyi
--rw-r--r--   0        0        0      158 2023-05-09 15:45:37.734763 esdbclient-1.0a6/esdbclient/protos/Grpc/code_pb2_grpc.py
--rw-r--r--   0        0        0     2817 2023-05-09 15:45:39.765118 esdbclient-1.0a6/esdbclient/protos/Grpc/gossip_pb2.py
--rw-r--r--   0        0        0     5524 2023-05-09 15:45:37.858863 esdbclient-1.0a6/esdbclient/protos/Grpc/gossip_pb2.pyi
--rw-r--r--   0        0        0     2752 2023-05-09 15:45:39.763073 esdbclient-1.0a6/esdbclient/protos/Grpc/gossip_pb2_grpc.py
--rw-r--r--   0        0        0    22467 2023-05-09 15:45:39.771649 esdbclient-1.0a6/esdbclient/protos/Grpc/persistent_pb2.py
--rw-r--r--   0        0        0    73220 2023-05-09 15:45:38.784305 esdbclient-1.0a6/esdbclient/protos/Grpc/persistent_pb2.pyi
--rw-r--r--   0        0        0    15771 2023-05-09 15:45:39.791304 esdbclient-1.0a6/esdbclient/protos/Grpc/persistent_pb2_grpc.py
--rw-r--r--   0        0        0     3782 2023-05-09 15:45:39.773845 esdbclient-1.0a6/esdbclient/protos/Grpc/shared_pb2.py
--rw-r--r--   0        0        0     9874 2023-05-09 15:45:37.963369 esdbclient-1.0a6/esdbclient/protos/Grpc/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2023-05-09 15:45:37.783977 esdbclient-1.0a6/esdbclient/protos/Grpc/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1686 2023-05-09 15:45:39.755017 esdbclient-1.0a6/esdbclient/protos/Grpc/status_pb2.py
--rw-r--r--   0        0        0     2838 2023-05-09 15:45:37.828819 esdbclient-1.0a6/esdbclient/protos/Grpc/status_pb2.pyi
--rw-r--r--   0        0        0      158 2023-05-09 15:45:37.797991 esdbclient-1.0a6/esdbclient/protos/Grpc/status_pb2_grpc.py
--rw-r--r--   0        0        0    19933 2023-05-09 15:45:39.801455 esdbclient-1.0a6/esdbclient/protos/Grpc/streams_pb2.py
--rw-r--r--   0        0        0    71744 2023-05-09 15:45:38.782146 esdbclient-1.0a6/esdbclient/protos/Grpc/streams_pb2.pyi
--rw-r--r--   0        0        0     9787 2023-05-09 15:45:37.926522 esdbclient-1.0a6/esdbclient/protos/Grpc/streams_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.0a6/esdbclient/py.typed
--rw-r--r--   0        0        0    44026 2023-05-22 13:07:29.542125 esdbclient-1.0a6/esdbclient/streams.py
--rw-r--r--   0        0        0     2670 2023-05-16 23:53:58.006272 esdbclient-1.0a6/pyproject.toml
--rw-r--r--   0        0        0   115310 1970-01-01 00:00:00.000000 esdbclient-1.0a6/setup.py
--rw-r--r--   0        0        0   112713 1970-01-01 00:00:00.000000 esdbclient-1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.0a7/LICENSE
+-rw-r--r--   0        0        0   112366 2023-06-01 12:36:25.987151 esdbclient-1.0a7/README.md
+-rw-r--r--   0        0        0      639 2023-05-26 19:08:34.577226 esdbclient-1.0a7/esdbclient/__init__.py
+-rw-r--r--   0        0        0    15403 2023-06-02 22:54:12.163873 esdbclient-1.0a7/esdbclient/asyncio_client.py
+-rw-r--r--   0        0        0    37563 2023-06-02 22:33:17.877074 esdbclient-1.0a7/esdbclient/client.py
+-rw-r--r--   0        0        0     2600 2023-06-02 22:33:14.719087 esdbclient-1.0a7/esdbclient/connection.py
+-rw-r--r--   0        0        0     9591 2023-06-02 22:33:39.164826 esdbclient-1.0a7/esdbclient/connection_spec.py
+-rw-r--r--   0        0        0     3131 2023-06-02 22:33:14.745159 esdbclient-1.0a7/esdbclient/esdbapibase.py
+-rw-r--r--   0        0        0     1258 2023-05-26 16:32:12.440216 esdbclient-1.0a7/esdbclient/events.py
+-rw-r--r--   0        0        0     3548 2023-05-24 15:39:06.891852 esdbclient-1.0a7/esdbclient/exceptions.py
+-rw-r--r--   0        0        0     5226 2023-06-02 22:33:14.763658 esdbclient-1.0a7/esdbclient/gossip.py
+-rw-r--r--   0        0        0    31527 2023-06-02 22:33:15.125378 esdbclient-1.0a7/esdbclient/persistent.py
+-rw-r--r--   0        0        0    13401 2023-05-09 15:45:39.784205 esdbclient-1.0a7/esdbclient/protos/Grpc/cluster_pb2.py
+-rw-r--r--   0        0        0    37958 2023-05-09 15:45:38.350807 esdbclient-1.0a7/esdbclient/protos/Grpc/cluster_pb2.pyi
+-rw-r--r--   0        0        0    19336 2023-05-09 15:45:39.761236 esdbclient-1.0a7/esdbclient/protos/Grpc/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1790 2023-05-09 15:45:39.793881 esdbclient-1.0a7/esdbclient/protos/Grpc/code_pb2.py
+-rw-r--r--   0        0        0    13555 2023-05-09 15:45:37.813695 esdbclient-1.0a7/esdbclient/protos/Grpc/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:37.734763 esdbclient-1.0a7/esdbclient/protos/Grpc/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2817 2023-05-09 15:45:39.765118 esdbclient-1.0a7/esdbclient/protos/Grpc/gossip_pb2.py
+-rw-r--r--   0        0        0     5524 2023-05-09 15:45:37.858863 esdbclient-1.0a7/esdbclient/protos/Grpc/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2752 2023-05-09 15:45:39.763073 esdbclient-1.0a7/esdbclient/protos/Grpc/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0    22467 2023-05-09 15:45:39.771649 esdbclient-1.0a7/esdbclient/protos/Grpc/persistent_pb2.py
+-rw-r--r--   0        0        0    73220 2023-05-09 15:45:38.784305 esdbclient-1.0a7/esdbclient/protos/Grpc/persistent_pb2.pyi
+-rw-r--r--   0        0        0    15771 2023-05-09 15:45:39.791304 esdbclient-1.0a7/esdbclient/protos/Grpc/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0     3782 2023-05-09 15:45:39.773845 esdbclient-1.0a7/esdbclient/protos/Grpc/shared_pb2.py
+-rw-r--r--   0        0        0     9874 2023-05-09 15:45:37.963369 esdbclient-1.0a7/esdbclient/protos/Grpc/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:37.783977 esdbclient-1.0a7/esdbclient/protos/Grpc/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1686 2023-05-09 15:45:39.755017 esdbclient-1.0a7/esdbclient/protos/Grpc/status_pb2.py
+-rw-r--r--   0        0        0     2838 2023-05-09 15:45:37.828819 esdbclient-1.0a7/esdbclient/protos/Grpc/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:37.797991 esdbclient-1.0a7/esdbclient/protos/Grpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0    19933 2023-05-09 15:45:39.801455 esdbclient-1.0a7/esdbclient/protos/Grpc/streams_pb2.py
+-rw-r--r--   0        0        0    71744 2023-05-09 15:45:38.782146 esdbclient-1.0a7/esdbclient/protos/Grpc/streams_pb2.pyi
+-rw-r--r--   0        0        0     9787 2023-05-09 15:45:37.926522 esdbclient-1.0a7/esdbclient/protos/Grpc/streams_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.0a7/esdbclient/py.typed
+-rw-r--r--   0        0        0    46742 2023-06-02 22:55:53.376506 esdbclient-1.0a7/esdbclient/streams.py
+-rw-r--r--   0        0        0     2670 2023-06-02 23:10:09.811605 esdbclient-1.0a7/pyproject.toml
+-rw-r--r--   0        0        0   116335 1970-01-01 00:00:00.000000 esdbclient-1.0a7/setup.py
+-rw-r--r--   0        0        0   113696 1970-01-01 00:00:00.000000 esdbclient-1.0a7/PKG-INFO
```

### Comparing `esdbclient-1.0a6/LICENSE` & `esdbclient-1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/README.md` & `esdbclient-1.0a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,43 @@
+Metadata-Version: 2.1
+Name: esdbclient
+Version: 1.0a7
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
+Requires-Dist: dnspython (>=2.3.0,<3.0.0)
+Requires-Dist: grpcio (>=1.51.0,!=1.52.*)
+Requires-Dist: protobuf (>=3.11.0)
+Requires-Dist: typing_extensions
+Project-URL: Repository, https://github.com/pyeventsourcing/esdbclient
+Description-Content-Type: text/markdown
+
 # Python gRPC Client for EventStoreDB
 
 This [Python package](https://pypi.org/project/esdbclient/) provides a Python
-gRPC client for [EventStoreDB](https://www.eventstore.com/).
+gRPC client for the [EventStoreDB](https://www.eventstore.com/) database.
 
 This client has been developed in collaboration with the EventStoreDB
 team. Although not all the features of EventStoreDB are supported
 by this client, many of the most useful features are presented
 in an easy-to-use interface.
 
 This client has been tested to work with EventStoreDB LTS versions 21.10,
@@ -13,42 +45,45 @@
 is 100% test coverage. The code has typing annotations, checked with mypy.
 The code is formatted with black and isort, and checked with flake8. Poetry
 is used for package management during development, and for building and
 publishing distributions to [PyPI](https://pypi.org/project/esdbclient/).
 
 ## Synopsis
 
-The `ESDBClient` class can be imported from the `esdbclient` package.
+You can connect to an EventStoreDB database using the `EventStoreDBClient` class.
+
+The `EventStoreDBClient` class can be imported from the `esdbclient` package.
 
-Probably the three most useful methods of `ESDBClient` are:
+Probably the three most useful methods of `EventStoreDBClient` are:
 
-* `append_events()` This method can be used to record events in a particular
-"stream". This is useful for example when executing a command in an application
+* `append_to_stream()` This method can be used to record new events in a particular
+"stream". This is useful, for example, when executing a command in an application
 that mutates an aggregate. This method is "atomic" in that either all or none of
 the events will be recorded.
 
-* `read_stream_events()` This method can be used to retrieve all the recorded
-events in a "stream". This is useful for example when reconstructing an aggregate
-before executing a command in an application.
-
-* `subscribe_all_events()` This method can be used to receive all recorded
-events across all "streams". This is useful in downstream event-processing
-components, and supports processing events with "exactly-once" semantics (see below).
+* `read_stream()` This method can be used to retrieve all the recorded
+events in a "stream". This is useful, for example, when reconstructing
+an aggregate from recorded events before executing a command in an
+application that creates new events.
+
+* `subscribe_to_all()` This method can be used to receive all recorded events in
+the database. This is useful, for example, in event-processing components because
+it supports processing events with "exactly-once" semantics.
 
 The example below uses an "insecure" EventStoreDB server running locally on port 2114.
 
 ```python
 import uuid
 
-from esdbclient import ESDBClient, NewEvent
+from esdbclient import EventStoreDBClient, NewEvent, StreamState
 
 
-# Construct ESDBClient with an EventStoreDB URI.
+# Construct EventStoreDBClient with an EventStoreDB URI.
 
-client = ESDBClient(
+client = EventStoreDBClient(
     uri="esdb://localhost:2114?Tls=false"
 )
 
 
 # Generate new events. Typically, domain events of different
 # types are generated in a domain model, and then serialized
 # into NewEvent objects. An aggregate ID may be used as the
@@ -59,110 +94,133 @@
     type='OrderCreated',
     data=b'{"order_number": "123456"}'
 )
 event2 = NewEvent(
     type='OrderSubmitted',
     data=b'{}'
 )
+event3 = NewEvent(
+    type='OrderCancelled',
+    data=b'{}'
+)
 
 
-# Append new events to a stream. The stream does not exist so
-# the "current version" is None. The value returned from the
-# append_events() method is the overall position in the database
-# of the last new event recorded by this operation. The returned
-# "commit position" value may be used in a user interface to poll
-# a downstream event-processing component before it presents an
-# up-to-date eventually consistent materialized view.
+# Append new events to a new stream. The value returned
+# from the append_to_stream() method is the overall
+# "commit position" in the database of the last new event
+# recorded by this operation. The returned "commit position"
+# may be used in a user interface to poll an eventually
+# consistent event-processing component until it can
+# present an up-to-date materialized view. New events are
+# each allocated a "stream position", which is the next
+# available position in the stream, starting from 0.
 
-commit_position1 = client.append_events(
+commit_position1 = client.append_to_stream(
     stream_name=stream_name1,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event1, event2],
 )
 
-# The "current version" is the "stream position" of the last
-# recorded event in a stream. Stream positions are zero-based.
-# We have recorded two new events, and so the "current version"
-# of this stream is 1. Concurrency is controlled in this way
-# to ensure the consistency of recorded events. An incorrect
-# value will cause a WrongCurrentVersion exception to be raised.
+# Append events to an existing stream. The "current version"
+# is the "stream position" of the last recorded event in a
+# stream. We have recorded two new events, so the "current
+# version" is 1. The exception 'WrongCurrentVersion' will be
+# raised if an incorrect value is given.
 
-event3 = NewEvent(
-    type='OrderCancelled',
-    data=b'{}'
-)
-
-commit_position2 = client.append_events(
+commit_position2 = client.append_to_stream(
     stream_name=stream_name1,
     current_version=1,
     events=[event3],
 )
 
+# - allocated commit positions increase monotonically
+assert commit_position2 > commit_position1
+
 
-# Read events from a stream. The recorded events may be
-# deserialized to domain events objects of different types,
-# then used to reconstruct an aggregate in a domain model.
+# Read events from a stream. This method returns a
+# "read response" iterator, which returns recorded
+# events. The iterator will stop when there are no
+# more events to be returned.
 
-recorded = client.read_stream_events(
+read_response = client.read_stream(
     stream_name=stream_name1
 )
 
-assert len(recorded) == 3
+# Iterate over "read response" to get recorded events.
+# The recorded events may be deserialized to domain event
+# objects of different types and used to reconstruct an
+# aggregate in a domain model.
+recorded_events = tuple(read_response)
+
+# - stream 'stream_name1' now has three events
+assert len(recorded_events) == 3
+
+# - allocated stream positions are zero-based and gapless
+assert recorded_events[0].stream_position == 0
+assert recorded_events[1].stream_position == 1
+assert recorded_events[2].stream_position == 2
+
+# - event attribute values are recorded faithfully
+assert recorded_events[0].type == "OrderCreated"
+assert recorded_events[0].data == b'{"order_number": "123456"}'
+assert recorded_events[0].id == event1.id
+
+assert recorded_events[1].type == "OrderSubmitted"
+assert recorded_events[1].data == b'{}'
+assert recorded_events[1].id == event2.id
+
+assert recorded_events[2].type == "OrderCancelled"
+assert recorded_events[2].data == b'{}'
+assert recorded_events[2].id == event3.id
+
+
+# Start a catch-up subscription from last recorded position.
+# This method returns a "catch-up subscription" iterator,
+# which returns recorded events. The iterator will not stop
+# when there are no more recorded events to be returned, but
+# will block, and continue when further events are recorded.
+
+catchup_subscription = client.subscribe_to_all()
+
+
+# Iterate over the catch-up subscription. Process each recorded
+# event in turn. Within an atomic database transaction, record
+# the event's "commit position" along with any new state generated
+# by processing the event. Use the component's last recorded commit
+# position when restarting the catch-up subscription.
 
-assert recorded[0].stream_name == stream_name1
-assert recorded[1].stream_name == stream_name1
-assert recorded[2].stream_name == stream_name1
-
-assert recorded[0].stream_position == 0
-assert recorded[1].stream_position == 1
-assert recorded[2].stream_position == 2
-
-assert recorded[0].type == "OrderCreated"
-assert recorded[1].type == "OrderSubmitted"
-assert recorded[2].type == "OrderCancelled"
-
-assert recorded[0].data == b'{"order_number": "123456"}'
-
-
-# Start a catch-up subscription to receive all recorded
-# events across all streams. A catch-up subscription may
-# be used in a downstream event-processing component to
-# receive recorded events from a particular commit position.
-# The first "commit position" in an EventStoreDB database is 0.
-
-last_saved_commit_position = 0
+received_events = []
+for event in catchup_subscription:
+    received_events.append(event)
 
-catch_subscription = client.subscribe_all_events(
-    commit_position=last_saved_commit_position
-)
+    if event.commit_position == commit_position2:
+        # Break so we can continue with the example.
+        break
 
 
-# Iterate over the catch-up subscription. Process each
-# recorded event in turn. In an atomic database transaction
-# save the event's "commit position" with any new state
-# generated by processing the event. Use the component's
-# last saved "commit position" when restarting the subscription.
+# - events are received in the order they were recorded
+assert received_events[-3].type == "OrderCreated"
+assert received_events[-3].data == b'{"order_number": "123456"}'
+assert received_events[-3].id == event1.id
 
+assert received_events[-2].type == "OrderSubmitted"
+assert received_events[-2].data == b'{}'
+assert received_events[-2].id == event2.id
 
-received = []
-for event in catch_subscription:
-    last_saved_commit_position = event.commit_position
-    received.append(event)
+assert received_events[-1].type == "OrderCancelled"
+assert received_events[-1].data == b'{}'
+assert received_events[-1].id == event3.id
 
-    if last_saved_commit_position == commit_position2:
-        # Stop so we can continue with the example.
-        catch_subscription.stop()
 
+# Stop the catch-up subscription iterator.
 
-assert received[-3].type == "OrderCreated"
-assert received[-2].type == "OrderSubmitted"
-assert received[-1].type == "OrderCancelled"
+catchup_subscription.stop()
 
 
-# Close the client after use.
+# Close the client's gRPC connection.
 
 client.close()
 ```
 
 See below for more details.
 
 For an example of usage, see the [eventsourcing-eventstoredb](
@@ -182,32 +240,32 @@
   * [Construct client](#construct-client)
 * [Connection strings](#connection-strings)
   * [Two schemes](#two-schemes)
   * [User info string](#user-info-string)
   * [Query string](#query-string)
   * [Examples](#examples)
 * [Event objects](#event-objects)
-  * [The NewEvent class](#the-newevent-class)
-  * [The RecordedEvent class](#the-recordedevent-class)
+  * [New events](#new-events)
+  * [Recorded events](#recorded-events)
 * [Streams](#streams)
   * [Append events](#append-events)
   * [Append event](#append-event)
   * [Idempotent append operations](#idempotent-append-operations)
   * [Read stream events](#read-stream-events)
   * [Get current version](#get-current-version)
   * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)
   * [Read all events](#read-all-events)
   * [Get commit position](#get-commit-position)
   * [Get stream metadata](#get-stream-metadata)
   * [Set stream metadata](#set-stream-metadata)
   * [Delete stream](#delete-stream)
   * [Tombstone stream](#tombstone-stream)
 * [Catch-up subscriptions](#catch-up-subscriptions)
-  * [Subscribe all events](#subscribe-all-events)
-  * [Subscribe stream events](#subscribe-stream-events)
+  * [Subscribe to all events](#subscribe-to-all-events)
+  * [Subscribe to stream events](#subscribe-to-stream-events)
   * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)
 * [Persistent subscriptions](#persistent-subscriptions)
   * [Create subscription](#create-subscription)
   * [Read subscription](#read-subscription)
   * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)
   * [Get subscription info](#get-subscription-info)
   * [List subscriptions](#list-subscriptions)
@@ -222,14 +280,15 @@
 * [Connection](#connection)
   * [Reconnect](#reconnect)
   * [Close](#close)
 * [Asyncio client](#asyncio-client)
   * [Synopsis](#synopsis-1)
 * [Notes](#notes)
   * [Regular expression filters](#regular-expression-filters)
+  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)
 * [Contributors](#contributors)
   * [Install Poetry](#install-poetry)
   * [Setup for PyCharm users](#setup-for-pycharm-users)
   * [Setup from command line](#setup-from-command-line)
   * [Project Makefile commands](#project-makefile-commands)
 <!-- TOC -->
 
@@ -312,27 +371,27 @@
     $ docker stop eventstoredb-insecure
 	$ docker rm eventstoredb-insecure
 
 
 ## EventStoreDB client
 
 This EventStoreDB client is implemented in the `esdbclient` package with
-the `ESDBClient` class.
+the `EventStoreDBClient` class.
 
 ### Import class
 
-The `ESDBClient` class can be imported from the `esdbclient` package.
+The `EventStoreDBClient` class can be imported from the `esdbclient` package.
 
 ```python
-from esdbclient import ESDBClient
+from esdbclient import EventStoreDBClient
 ```
 
 ### Construct client
 
-The `ESDBClient` class has one required constructor argument, `uri`, and one
+The `EventStoreDBClient` class has one required constructor argument, `uri`, and one
 optional constructor argument, `root_certificates`.
 
 The `uri` argument is expected to be an EventStoreDB connection string URI that
 conforms with the standard EventStoreDB "esdb" or "esdb+discover" URI schemes.
 
 For example, the following connection string specifies that the client should
 attempt to create a "secure" connection to port 2113 on "localhost", and use the
@@ -370,15 +429,15 @@
 system environment. This is a typical arrangement in a production environment. It is
 done this way here so that the code in this documentation can be tested with both
 a "secure" and an "insecure" server.
 
 ```python
 import os
 
-client = ESDBClient(
+client = EventStoreDBClient(
     uri=os.getenv("ESDB_URI"),
     root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),
 )
 ```
 
 ## Connection strings
 
@@ -464,15 +523,15 @@
 
 | Field               | Value                                                                 | Description                                                                                                                                                       |
 |---------------------|-----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Tls                 | "true", "false" (default: "true")                                     | If "true" the client will create a "secure" gRPC channel. If "false" the client will create an "insecure" gRPC channel. This must match the server configuration. |
 | TlsVerifyCert       | "true", "false" (default: "true")                                     | This value is currently ignored.                                                                                                                                  |
 | ConnectionName      | string (default: auto-generated version-4 UUID)                       | Sent in call metadata for every call, to identify the client to the cluster.                                                                                      |
 | NodePreference      | "leader", "follower", "readonlyreplica", "random" (default: "leader") | The node state preferred by the client. The client will select a node from the cluster info received from the Gossip API according to this preference.            |
-| DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_events()`.                                                     |
+| DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_to_stream()`.                                                  |
 | GossipTimeout       | integer (default: 5)                                                  | The default value (in seconds) of the `timeout` argument of gossip read methods, such as `read_gossip()`.                                                         |
 | MaxDiscoverAttempts | integer (default: 10)                                                 | The number of attempts to read gossip when connecting or reconnecting to a cluster member.                                                                        |
 | DiscoveryInterval   | integer (default: 100)                                                | How long to wait (in milliseconds) between gossip retries.                                                                                                        |
 | KeepAliveInterval   | integer (default: `None`)                                             | The value of the "grpc.keepalive_ms" gRPC channel option.                                                                                                         |
 | KeepAliveTimeout    | integer (default: `None`)                                             | The value of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                                                 |
 
 
@@ -547,18 +606,17 @@
 This package defines a `NewEvent` class and a `RecordedEvent` class. The
 `NewEvent` class should be used when writing events to the database. The
 `RecordedEvent` class is used when reading events from the database.
 
 ### New events
 
 The `NewEvent` class should be used when writing events to an EventStoreDB database.
-You will need to construct new event objects before calling the `append_events()`
-and `append_event()` methods.
+You will need to construct new event objects before calling `append_to_stream()`.
 
-The `NewEvent` class is a frozen Python database. It has two required constructor
+The `NewEvent` class is a frozen Python dataclass. It has two required constructor
 arguments (`type` and `data`) and three optional constructor arguments (`metadata`,
 `content_type` and `id`).
 
 The required `type` argument is a Python `str`, used to describe the type of
 domain event that is being recorded.
 
 The required `data` argument is a Python `bytes` object, used to state the
@@ -603,34 +661,34 @@
 assert new_event2.id == event_id
 ```
 
 ### Recorded events
 
 The `RecordedEvent` class is used when reading events from an EventStoreDB
 database. The client will return event objects of this type from all methods
-that return recorded events, such as `read_stream_events()`, `subscribe_all_events()`,
+that return recorded events, such as `get_stream()`, `subscribe_to_all()`,
 and `read_subscription()`. You do not need to construct recorded event objects.
 
-Like `NewEvent`, the `RecordedEvent` class is also a frozen Python database. It has
+Like `NewEvent`, the `RecordedEvent` class is also a frozen Python dataclass. It has
 all the attributes that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`)
 and some additional attributes that follow from the fact that an event was recorded
 (`stream_name`, `stream_position`, `commit_position`).
 
 The `type` attribute is a Python `str`, used to indicate the type of an event
 that was recorded.
 
 The `data` attribute is a Python `bytes` object, used to indicate the data of an
 event that was recorded.
 
 The `metadata` attribute is a Python `bytes` object, used to indicate the metadata of
 an event that was recorded.
 
 The `content_type` attribute is a Python `str`, used to indicate the type of
-data that was recorded for an event. It is usually `application/json`, indicating
-that the data can be parsed as JSON. Alternatively, it is `application/octet-stream`.
+data that was recorded for an event. It is usually `'application/json'`, indicating
+that the data can be parsed as JSON. Alternatively, it is `'application/octet-stream'`.
 
 The `id` attribute is a Python `UUID` object, used to indicate the unique ID of an
 event that was recorded.
 
 The `stream_name` attribute is a Python `str`, used to indicate the name of a
 stream in which an event was recorded.
 
@@ -648,14 +706,21 @@
 In EventStoreDB, a "commit position" is an integer representing the position of a
 recorded event in the database. Each recorded event is recorded at a position in the
 database. Each commit position is occupied by only one recorded event. Commit positions
 are zero-based and increase monotonically as new events are recorded. But, unlike stream
 positions, the sequence of successive commit positions is not gapless. Indeed, there are
 usually large differences between the commit positions of successively recorded events.
 
+Please note, in EventStoreDB 21.10, the `commit_position` of all `RecordedEvent` objects
+obtained from `read_stream()` is `None`, whereas those obtained from `read_all()` have
+the actual commit position of the recorded event. This was changed in version 22.10, so
+that event objects obtained from both `get_stream()` and `read_all()` have the actual
+commit position. The `commit_position` attribute of the `RecordedEvent` class is
+annotated with the type `Optional[int]` for this reason only.
+
 
 ```python
 from esdbclient.events import RecordedEvent
 
 recorded_event = RecordedEvent(
     type='OrderCreated',
     data=b'{}',
@@ -674,82 +739,83 @@
 In EventStoreDB, a "stream" is a sequence of recorded events that all have
 the same "stream name". There will normally be many streams in a database,
 each with many recorded events. Each recorded event has a position in its stream
 (the "stream position"), and a position in the database (the "commit position").
 Stream positions are zero-based and gapless. Commit positions are also zero-based,
 but are not gapless.
 
-The methods `append_events()`, `read_stream_events()` and `read_all_events()` can
+The methods `append_to_stream()`, `get_stream()` and `read_all()` can
 be used to read and record in the database.
 
 ### Append events
 
 *requires leader*
 
-The `append_events()` method can be used atomically to record a sequence of new events.
+The `append_to_stream()` method can be used atomically to record a sequence of new events.
 If the operation is successful, it returns the commit position of the last event in the
 sequence that has been recorded.
 
 This method has three required arguments, `stream_name`, `current_version`
 and `events`.
 
 The required `stream_name` argument is a Python `str` that uniquely identifies a
 stream to which a sequence of events will be appended.
 
 The required `current_version` argument is expected to be either a Python `int`
 that indicates the stream position of the last recorded event in the stream, or
-`None` if the stream does not yet exist or has been deleted. The stream positions
-are zero-based and gapless, so that if a stream has two events, the `current_version`
-should be 1. If an incorrect value is given, this method will raise a
+`StreamState.NO_STREAM` if the stream does not yet exist or has been deleted. The
+stream positions are zero-based and gapless, so that if a stream has two events, the
+`current_version` should be 1. If an incorrect value is given, this method will raise a
 `WrongCurrentVersion` exception. This behavior is designed to provide concurrency
 control when recording new events. The correct value of `current_version` for any stream
 can be obtained by calling `get_current_version()`. However, the typical approach is to
-use the stream position of the recorded events as the version number of a reconstructed
-aggregate, and to use the current version of the aggregate as the `current_version` when
-appending new aggregate events. This ensures the consistency of the recorded state of
-the aggregate, and forces operations that generate new aggregate events to be retried with a freshly
-reconstructed aggregate when a `WrongCurrentVersion` exception is encountered.
-This controlling behavior can be disabled by setting the value of the
-`current_version` argument to `-1`.
+reconstruct an aggregate from the recorded events, so that the version of the aggregate
+is the stream position of the last recorded event, then have the aggregate generate new
+events, and then use the current version of the aggregate as the value of the
+`current_version` argument when appending the new aggregate events. This ensures
+the consistency of the recorded aggregate events, because operations that generate
+new aggregate events can be retried with a freshly reconstructed aggregate if
+a `WrongCurrentVersion` exception is encountered when recording new events. This
+controlling behavior can be disabled by setting the value of the `current_version`
+argument to the constant `StreamState.ANY`.
 
 The required `events` argument is expected to be a sequence of new event objects. The
-`NewEvent` class should be used to construct new event objects. The `append_events()`
+`NewEvent` class should be used to construct new event objects. The `append_to_stream()`
 operation is atomic, so that either all or none of the new events will be recorded. It
 is not possible with EventStoreDB atomically to record new events in more than one stream.
 
 This method also has an optional `timeout` argument, which is a Python `float`
 that sets a deadline for the completion of the gRPC operation.
 
-In the example below, a new event, `event1`, is appended to a new stream. The
-stream does not yet exist, so `current_version` is `None`.
+In the example below, a new event, `event1`, is appended to a new stream. The stream
+does not yet exist, so `current_version` is `StreamState.NO_STREAM`.
 
 ```python
 # Construct a new event object.
 event1 = NewEvent(type='OrderCreated', data=b'data1')
 
 # Define a new stream name.
 stream_name1 = str(uuid.uuid4())
 
 # Append the new events to the new stream.
-commit_position1 = client.append_events(
+commit_position1 = client.append_to_stream(
     stream_name=stream_name1,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event1],
 )
 ```
 
 In the example below, two subsequent events are appended to an existing
-stream. The stream, `stream_name1`, so far has one recorded event, and so
-the correct value of `current_version` is `0`.
+stream. The stream has one recorded event, so `current_version` is `0`.
 
 ```python
 event2 = NewEvent(type='OrderUpdated', data=b'data2')
 event3 = NewEvent(type='OrderDeleted', data=b'data3')
 
-commit_position2 = client.append_events(
+commit_position2 = client.append_to_stream(
     stream_name=stream_name1,
     current_version=0,
     events=[event2, event3],
 )
 ```
 
 The returned values, `commit_position1` and `commit_position2`, are the
@@ -763,139 +829,126 @@
 eventually consistent materialized view in a downstream component that is updated from
 these events. If the new events have not yet been processed, the view might be stale,
 or out-of-date. Instead of displaying a stale view, the user interface can poll the
 downstream component until it has processed the newly recorded events, and then display
 an up-to-date view to the user.
 
 
-### Append event
-
-*requires leader*
-
-The `append_event()` method is like `append_events()` but can be used only to write a
-single new event to a stream. If the operation is successful, it returns the commit
-position of the newly recorded event.
-
-This method has three required arguments, `stream_name`, `current_version` and `event`.
-
-The required `stream_name` argument is a Python `str` that uniquely identifies a
-stream to which a sequence of events will be appended.
-
-The required `current_version` argument is expected to be either a Python `int`
-that indicates the stream position of the last recorded event in the stream.
-
-The required `event` argument is expected to be a single new event object. The event
-object is expected to be an instance of the `NewEvent` class.
-
-This method also has an optional `timeout` argument, which is a Python `float`
-that sets a deadline for the completion of the gRPC operation.
-
-
 ### Idempotent append operations
 
-The `append_event()` and `append_events()` and methods are "idempotent", in that
-if the methods are called with new events whose `id` attribute values equal those
-of recorded events in the named stream immediately after the stream position specified
-by the value of the `current_version` argument, then these methods will return the
-commit position of the last new event, without making any changes to the database.
-
-Sometimes it may happen, when calling `append_event()` or `append_events()`, that
-the new events are successfully recorded but somehow a connection issue occurs before
-the successful call can return successfully to the client. We cannot be sure if
-the events were recorded or not, and so we may wish to retry. If the events were in
-fact successfully recorded, it is convenient for the retried operation to return
-successfully without raising an exception. If those new events were in fact not recorded,
-and in the meantime no other new events were recorded in that stream, then it makes sense
-that the new events will be recorded when the append operation is retried. Of course,
-if a `WrongCurrentVersion` exception is raised when retrying the operation, then an
-application command which generated the new events in the context of already recorded
-events may need to be executed again. Alternatively, a suitable error might be displayed
-by the application, with an up-to-date view of the recorded data, giving a user of the
-application an opportunity to decide if they still wish to proceed with their original
-intention.
+The `append_to_stream()` method is "idempotent", in that if called with new events whose
+`id` attribute values equal those of recorded events in the named stream immediately
+after the stream position specified by the value of the `current_version` argument, then
+it will return the commit position of the last new event, without making any changes to
+the database.
+
+Sometimes it may happen, when calling `append_to_stream()`, that the new events are
+successfully recorded but somehow a connection issue occurs before the successful call
+can return successfully to the client. We cannot be sure if the events were recorded
+or not, and so we may wish to retry. If the events were in fact successfully recorded,
+it is convenient for the retried operation to return successfully without raising an
+exception. If those new events were in fact not recorded, and in the meantime no other
+new events were recorded in that stream, then it makes sense that the new events will
+be recorded when the append operation is retried. Of course, if a `WrongCurrentVersion`
+exception is raised when retrying the operation, then an application command which
+generated the new events in the context of already recorded events may need to be
+executed again. Alternatively, a suitable error might be displayed by the application,
+with an up-to-date view of the recorded data, giving a user of the application an
+opportunity to decide if they still wish to proceed with their original intention.
 
-The example below shows the `append_events()` method being called again with
+The example below shows the `append_to_stream()` method being called again with
 `event3` and `current_version=0`. We can see that repeating the call to
-`append_events()` returns successfully.
+`append_to_stream()` returns successfully.
 
 ```python
 # Retry appending event3.
-commit_position_retry = client.append_events(
+commit_position_retry = client.append_to_stream(
     stream_name=stream_name1,
     current_version=0,
     events=[event2, event3],
 )
 ```
 
 We can see that the same commit position is returned as above.
 
 ```python
 assert commit_position_retry == commit_position2
 ```
 
-By calling `read_stream_events()`, we can also see the stream has been unchanged
-despite the `append_events()` method having been called twice with the same arguments.
+By calling `get_stream()`, we can also see the stream has been unchanged
+despite the `append_to_stream()` method having been called twice with the same arguments.
 That is, there are still only three events in the stream.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1
 )
 
 assert len(events) == 3
 ```
 
 This idempotent behaviour depends on the `id` attribute of the `NewEvent` class.
 This attribute, by default, is assigned a new and unique version-4 UUID when an
 instance of `NewEvent` is constructed. The `id` argument can be used when
 constructing `NewEvent` objects to set the value of this attribute.
 
 
 ### Read stream events
 
-The `read_stream_events()` method can be used to get events that have been appended
-to a stream. This method returns a Python `tuple` of recorded event objects. The
-recorded event objects are instances of the `RecordedEvent` class.
+The `read_stream()` method can be used to get events that have been appended
+to a stream. This method returns a "read response" object.
 
-This method has one required argument, `stream_name`.
+A "read response" object is a Python iterator. Recorded events can be
+obtained by iterating over the "read response" object. Recorded events are
+streamed from the server to the client as the iteration proceeds. The iteration
+will automatically stop when there are no more recorded events to be returned.
+The streaming of events, and hence the iterator, can also be stopped by calling
+the `stop()` method on the "read response" object.
+
+The `get_stream()` method can be used to get events that have been appended
+to a stream. This method returns a Python `tuple` of recorded event objects.
+The recorded event objects are instances of the `RecordedEvent` class. It
+calls `read_stream()` and passes the "read response" iterator into a Python
+`tuple`, so that the streaming will complete before the method returns.
+
+The `read_stream()` and `get_stream()` methods have one required argument, `stream_name`.
 
 The required `stream_name` argument is a Python `str` that uniquely identifies a
 stream from which recorded events will be returned.
 
-The `read_stream_events()` method also has four optional arguments,
+The `read_stream()` and `get_stream()` methods also have four optional arguments,
 `stream_position`, `backwards`, `limit`, and `timeout`.
 
 The optional `stream_position` argument is a Python `int` that can be used to
 indicate the position in the stream from which to start reading. The default value
 of `stream_position` is `None`. When reading a stream from a specific position in the
 stream, the recorded event at that position will be included, both when reading
 forwards from that position, and when reading backwards.
 
 The optional `backwards` argument is a Python `bool`. The default value of `backwards`
 is `False`, which means the stream will be read forwards, so that events are returned
 in the order they were recorded. If `backwards` is `True`, the events are returned in
 reverse order.
 
 If `backwards` is `False` and `stream_position` is `None`, the stream's events will be
-returned in the order they were recorded, starting from the first recorded event. This
-is the default behavior of `read_stream_events()`. If `backwards` is `True` and
-`stream_position` is `None`, the stream's events will be returned in reverse order,
-starting from the last recorded event.
+returned in the order they were recorded, starting from the first recorded event. If
+`backwards` is `True` and `stream_position` is `None`, the stream's events will be
+returned in reverse order, starting from the last recorded event.
 
 The optional `limit` argument is a Python `int` which restricts the number of events
 that will be returned. The default value of `limit` is `sys.maxint`.
 
 The optional `timeout` argument is a Python `float` which sets a deadline for
 the completion of the gRPC operation.
 
-The example below shows the default behavior of this method, which is to return all
-the recorded events of a stream forwards from the first recorded events to the last.
+The example below shows the default behavior, which is to return all the recorded
+events of a stream forwards from the first recorded events to the last.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1
 )
 
 assert len(events) == 3
 assert events[0].id == event1.id
 assert events[1].id == event2.id
 assert events[2].id == event3.id
@@ -903,105 +956,91 @@
 
 The example below shows how to use the `stream_position` argument to read a stream
 from a specific stream position to the end of the stream. Stream positions are
 zero-based, and so `stream_position=1` corresponds to the second event that was
 recorded in the stream, in this case `event2`.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1,
     stream_position=1,
 )
 
 assert len(events) == 2
 assert events[0].id == event2.id
 assert events[1].id == event3.id
 ```
 
 The example below shows how to use the `backwards` argument to read a stream backwards.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1,
     backwards=True,
 )
 
 assert len(events) == 3
 assert events[0].id == event3.id
 assert events[1].id == event2.id
 assert events[2].id == event1.id
 ```
 
 The example below shows how to use the `limit` argument to read a limited number of
 events.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1,
     limit=2,
 )
 
 assert len(events) == 2
 assert events[0].id == event1.id
 assert events[1].id == event2.id
 ```
 
-The `read_stream_events()` method will raise a `NotFound` exception if the named stream
-has never existed or has been deleted.
+The `read_stream()` and `get_stream()` methods will raise a `NotFound` exception if the
+named stream has never existed or has been deleted.
 
 ```python
 from esdbclient.exceptions import NotFound
 
 
 try:
-    client.read_stream_events('does-not-exist')
+    client.get_stream('does-not-exist')
 except NotFound:
     pass  # The stream does not exist.
 else:
     raise Exception("Shouldn't get here")
 ```
 
-Please note, this method streams recorded events from the server and then
-constructs and returns a Python `tuple`. In case you don't want the client to
-finish streaming events from the database before it returns, you can instead
-use the `iter_stream_events()` method, which returns an iterable "read response"
-object. A "read response" is an iterator, and not a sequence. Recorded events can
-be obtained by iterating over the "read response" object. It streams recorded events
-from the server as the iteration proceeds. The iteration will automatically stop
-when there are no more recorded events to be returned. The streaming of events,
-and hence the iterator, can also be stopped prematurely by calling the `stop()`
-method on the "read response" object.
-
-In fact, the `read_stream_events()` method calls `iter_stream_events()` and passes
-the "read response" iterator into the Python `tuple` constructor. However, the
-`read_stream_events()` method is decorated with retry and reconnect decorators,
-whilst the `iter_stream_events()` method is not. This means that all errors due to
-connection issues will be caught by the retry and reconnect decorators when calling
-the `read_stream_events()` method, but not when calling `iter_stream_events()`. The
-`iter_stream_events()` method has no such decorators because the streaming only starts
+Please note, the `get_stream()` method is decorated with the `@autoreconnect` and
+`@retrygrpc` decorators, whilst the `read_stream()` method is not. This means that
+all errors due to connection issues will be caught by the retry and reconnect decorators
+when calling the `get_stream()` method, but not when calling `read_stream()`. The
+`read_stream()` method has no such decorators because the streaming only starts
 when iterating over the "read response" starts, which means that the method returns
 before the streaming starts, and so there is no chance for any decorators to catch
 any connection issues.
 
-Nevertheless, if you are reading a very large stream, then you might prefer to call
-`iter_stream_events()`, and to begin iterating through the recorded events whilst
-they are being streamed from the server, rather than both waiting and having them
-all accumulate in memory. Because of the risk of connection issues arising during
-the streaming of recorded events from the server, you will need to care about
-connection issues when iterating over the "read response" object returned from
-`iter_stream_events()`.
+For the same reason, `read_stream()` will not raise a `NotFound` exception when
+the stream does not exist, until iterating over the "read response" object begins.
+
+If you are reading a very large stream, then you might prefer to call `read_stream()`,
+and begin iterating through the recorded events whilst they are being streamed from
+the server, rather than both waiting and having them all accumulate in memory.
 
 ### Get current version
 
 The `get_current_version()` method is a convenience method that essentially calls
-`read_stream_events()` with `backwards=True` and `limit=1`. This method returns
+`get_stream()` with `backwards=True` and `limit=1`. This method returns
 the value of the `stream_position` attribute of the last recorded event in a
-stream. If a stream does not exist, the returned value is `None`. The returned
-value is the correct value of `current_version` when appending new events to
-a stream.
+stream. If a stream does not exist, the returned value is `StreamState.NO_STREAM`.
+The returned value is the correct value of `current_version` when appending events
+to a stream, and when deleting or tombstoning a stream.
 
 This method has one required argument, `stream_name`.
 
 The required `stream_name` argument is a Python `str` that uniquely identifies a
 stream from which a stream position will be returned.
 
 This method also has an optional `timeout` argument, that
@@ -1016,25 +1055,25 @@
 current_version = client.get_current_version(
     stream_name=stream_name1
 )
 
 assert current_version == 2
 ```
 
-If a stream has never existed or has been deleted, the returned value is `None`,
-which matches the required value of the `current_version` argument both when
-appending the first event of a new stream, and also when appending events to
-a stream that has been deleted.
+If a stream has never existed or has been deleted, the returned value is
+`StreamState.NO_STREAM`, which is the correct value of the `current_version`
+argument both when appending the first event of a new stream, and also when
+appending events to a stream that has been deleted.
 
 ```python
 current_version = client.get_current_version(
     stream_name='does-not-exist'
 )
 
-assert current_version is None
+assert current_version is StreamState.NO_STREAM
 ```
 
 ### How to implement snapshotting with EventStoreDB
 
 Snapshots can improve the performance of aggregates that would otherwise be
 reconstructed from very long streams. However, it is generally recommended to design
 aggregates to have a finite lifecycle, and so to have relatively short streams,
@@ -1054,15 +1093,15 @@
 
 
 def get_aggregate(aggregate_id, mutator_func):
     stream_name = aggregate_id
 
     # Get recorded events.
     try:
-        events = client.read_stream_events(
+        events = client.get_stream(
             stream_name=stream_name,
             stream_position=None
         )
     except NotFound as e:
         raise AggregateNotFound(aggregate_id) from e
     else:
         # Reconstruct aggregate from recorded events.
@@ -1113,30 +1152,30 @@
 
 def get_aggregate(aggregate_id, mutator_func):
     stream_name = aggregate_id
     recorded_events = []
 
     # Look for a snapshot.
     try:
-        snapshots = client.read_stream_events(
+        snapshots = client.get_stream(
             stream_name=make_snapshot_stream_name(stream_name),
             backwards=True,
             limit=1
         )
     except NotFound:
         stream_position = None
     else:
         assert len(snapshots) == 1
         snapshot = snapshots[0]
         stream_position = deserialize(snapshot.metadata)['version'] + 1
         recorded_events.append(snapshot)
 
     # Get subsequent events.
     try:
-        events = client.read_stream_events(
+        events = client.get_stream(
             stream_name=stream_name,
             stream_position=stream_position
         )
     except NotFound as e:
         raise AggregateNotFound(aggregate_id) from e
     else:
         recorded_events += events
@@ -1176,15 +1215,15 @@
 
 @dataclass(frozen=True)
 class Dog(Aggregate):
     name: str
     tricks: list
 ```
 
-Let's also define a mutator function `mutate_dog()` that can evolve the state of a
+Let's also define a mutator function `mutate_dog()` that evolves the state of a
 `Dog` aggregate given various different types of events, `'DogRegistered'`,
 `'DogLearnedTrick'`, and `'Snapshot'`.
 
 ```python
 def mutate_dog(dog, event):
     data = deserialize(event.data)
     if event.type == 'DogRegistered':
@@ -1241,46 +1280,46 @@
 ```python
 def register_dog(name):
     dog_id = str(uuid.uuid4())
     event = NewEvent(
         type='DogRegistered',
         data=serialize({'name': name}),
     )
-    client.append_event(
+    client.append_to_stream(
         stream_name=dog_id,
-        current_version=None,
-        event=event,
+        current_version=StreamState.NO_STREAM,
+        events=event,
     )
     return dog_id
 
 
 def record_trick_learned(dog_id, trick):
     dog = get_dog(dog_id)
     event = NewEvent(
         type='DogLearnedTrick',
         data=serialize({'trick': trick}),
     )
-    client.append_event(
+    client.append_to_stream(
         stream_name=dog_id,
         current_version=dog.version,
-        event=event,
+        events=event,
     )
 
 
 def snapshot_dog(dog_id):
     dog = get_dog(dog_id)
     event = NewEvent(
         type='Snapshot',
         data=serialize({'name': dog.name, 'tricks': dog.tricks}),
         metadata=serialize({'version': dog.version}),
     )
-    client.append_event(
+    client.append_to_stream(
         stream_name=make_snapshot_stream_name(dog_id),
-        current_version=-1,
-        event=event,
+        current_version=StreamState.ANY,
+        events=event,
     )
 ```
 
 We can call `register_dog()` to register a new dog.
 
 ```python
 # Register a new dog.
@@ -1353,43 +1392,44 @@
 Snapshots can be created at fixed version number intervals, fixed time
 periods, after a particular type of event, immediately after events are
 appended, or as a background process.
 
 
 ### Read all events
 
-The `read_all_events()` method can be used to get all recorded events
-in the database in the order they were recorded. This method will return
-a "read response" object, just like `iter_stream_events()`.
+The `read_all()` method can be used to get all recorded events
+in the database in the order they were recorded. This method returns
+a "read response" object, just like `read_stream()`.
 
 A "read response" is an iterator, and not a sequence. Recorded events can be
-obtained by iterating over the "read response" object. It streams recorded
-events from the server as the iteration proceeds. The iteration will automatically
-stop when there are no more recorded events to be returned. The streaming of events,
-and hence the iterator, can also be stopped by calling the `stop()` method on the
-"read response" object.
-
-Just like `read_stream_events()` and `iter_stream_events()`, the received event objects
+obtained by iterating over the "read response" object. Recorded events are
+streamed from the server to the client as the iteration proceeds. The iteration
+will automatically stop when there are no more recorded events to be returned.
+The streaming of events, and hence the iterator, can also be stopped by calling
+the `stop()` method on the "read response" object. The recorded event objects
 are instances of the `RecordedEvent` class.
 
 This method has seven optional arguments, `commit_position`, `backwards`,
 `filter_exclude`, `filter_include`, `filter_by_stream_name`, `limit`, and `timeout`.
 
 The optional `commit_position` argument is a Python `int` that can be used to
 specify a commit position from which to start reading. The default value of
 `commit_position` is `None`. Please note, if a commit position is specified,
-it must be an actually existing commit position in the database.
+it must be an actually existing commit position in the database. When reading
+forwards, the event at the commit position may be included, depending upon the
+filter. When reading backwards, the event at the commit position will not be
+included.
 
 The optional `backwards` argument is a Python `bool`. The default of `backwards` is
 `False`, which means events are returned in the order they were recorded, If
 `backwards` is `True`, then events are returned in reverse order.
 
 If `backwards` is `False` and `commit_position` is `None`, the database's events will
 be returned in the order they were recorded, starting from the first recorded event.
-This is the default behavior of `read_all_events()`. If `backwards` is `True` and
+This is the default behavior of `read_all()`. If `backwards` is `True` and
 `commit_position` is `None`, the database's events will be returned in reverse order,
 starting from the last recorded event.
 
 The optional `filter_exclude` argument is a sequence of regular expressions that
 specifies which recorded events should be returned. This argument is ignored
 if `filter_include` is set to a non-empty sequence. The default value of this
 argument matches the event types of EventStoreDB "system events", so that system
@@ -1417,15 +1457,15 @@
 
 The example below shows how to get all the events we have recorded in the database
 so far, in the order they were recorded. We can see the three events of `stream_name1`
 (`event1`, `event2` and `event3`) are included, along with others.
 
 ```python
 # Read all events (creates a streaming gRPC call).
-read_response = client.read_all_events()
+read_response = client.read_all()
 
 # Convert the iterator into a sequence of recorded events.
 events = tuple(read_response)
 assert len(events) > 3  # more than three
 
 # Convert the sequence of recorded events into a set of event IDs.
 event_ids = set(e.id for e in events)
@@ -1439,15 +1479,15 @@
 forwards from a specific commit position, the event at the specified position
 will be included. The value of `commit_position1` is the position we obtained
 when appending `event1`. And so `event1` is the first recorded event we shall
 receive, `event2` is the second, and `event3` is the third.
 
 ```python
 # Read all events forwards from a commit position.
-read_response = client.read_all_events(
+read_response = client.read_all(
     commit_position=commit_position1
 )
 
 # Step through the "read response" iterator.
 assert next(read_response).id == event1.id
 assert next(read_response).id == event2.id
 assert next(read_response).id == event3.id
@@ -1459,15 +1499,15 @@
 The example below shows how to read all events recorded in the database in reverse
 order. We can see that the first events we receive are the last events that were
 recorded: the events of the `Dog` aggregate from the section about snapshotting
 and the snapshot.
 
 ```python
 # Read all events backwards from the end.
-read_response = client.read_all_events(
+read_response = client.read_all(
     backwards=True
 )
 
 # Step through the "read response" iterator.
 assert next(read_response).type == "DogLearnedTrick"
 assert next(read_response).type == "Snapshot"
 assert next(read_response).type == "DogLearnedTrick"
@@ -1479,15 +1519,15 @@
 ```
 
 The example below shows how to read a limited number of events
 forwards from a specific commit position.
 
 ```python
 events = tuple(
-    client.read_all_events(
+    client.read_all(
         commit_position=commit_position1,
         limit=1,
     )
 )
 
 assert len(events) == 1
 assert events[0].id == event1.id
@@ -1495,48 +1535,48 @@
 
 The example below shows how to read a limited number of the recorded events
 in the database backwards from the end. In this case, the limit is 1, and
 so we receive the last recorded event.
 
 ```python
 events = tuple(
-    client.read_all_events(
+    client.read_all(
         backwards=True,
         limit=1,
     )
 )
 
 assert len(events) == 1
 
 assert events[0].type == 'DogLearnedTrick'
 assert deserialize(events[0].data)['trick'] == 'sit'
 ```
 
-Please note, like the `iter_stream_events()` method, the `read_all_events()` method
+Please note, like the `read_stream()` method, the `read_all()` method
 is not decorated with retry and reconnect decorators, because the streaming of recorded
 events from the server only starts when iterating over the "read response" starts, which
 means that the method returns before the streaming starts, and so there is no chance for
 any decorators to catch any connection issues.
 
 ### Get commit position
 
 The `get_commit_position()` method can be used to get the commit position of the
-last recorded event in the database. It simply calls `read_all_events()` with
+last recorded event in the database. It simply calls `read_all()` with
 `backwards=True` and `limit=1`, and returns the value of the `commit_position`
 attribute of the last recorded event.
 
 ```python
 commit_position = client.get_commit_position()
 ```
 
 This method has four optional arguments, `filter_exclude`, `filter_include`,
-`filter_by_stream_name` and `timeout`. These values are passed to `read_all_events()`.
+`filter_by_stream_name` and `timeout`. These values are passed to `read_all()`.
 
 The optional `filter_exclude`, `filter_include` and `filter_by_stream_name` arguments
-work in the same way as they do in the `read_all_events()` method.
+work in the same way as they do in the `read_all()` method.
 
 This optional `timeout` argument is a Python `float` that sets
 a deadline for the completion of the gRPC operation.
 
 This method might be used to measure progress of a downstream component
 that is processing all recorded events, by comparing the current commit
 position with the recorded commit position of the last successfully processed
@@ -1608,58 +1648,59 @@
 
 After tombstoning a stream, it's not possible to append new events.
 
 
 ## Catch-up subscriptions
 
 A "catch-up" subscription can be used to receive events that have already been
-recorded in the database, and also events that are recorded subsequently.
+recorded in the database, and events that are recorded subsequently. A catch-up
+subscription can be used by an event-processing component that processes recorded
+events with "exactly-once" semantics.
+
+The `subscribe_to_all()` method starts a catch-up subscription that can receive
+all events in the database. The `subscribe_to_stream()` method starts a catch-up
+subscription that can receive events from a specific stream. Both methods return a
+"catch-up subscription" object, which is a Python iterator. Recorded events can be
+obtained by iteration. Recorded event objects obtained in this way are instances
+of the `RecordedEvent` class. Please note, the `subscribe_to_all()` method will
+occasionally return `Checkpoint` objects. These are a special type of `RecordedEvent`
+that have a `commit_position`, so that downstream event-processing components can
+record progress across a large number of events that have been filtered out.
+
+Before the "catch-up subscription" object is returned to the caller, the client will
+firstly obtain a "confirmation" response from the server, which allows the client to
+detect that both the gRPC connection and the streaming gRPC call is operational. For
+this reason, the `subscribe_to_all()` and `subscribe_to_stream()` methods are both
+usefully decorated with the reconnect and retry decorators. However, once the method
+has returned, the decorators will have exited, and any exceptions that are raised
+due to connection issues whilst iterating over the subscription object will have to
+be handled by your code.
+
+A "catch-up subscription" iterator will not automatically stop when there are no more
+events to be returned, but instead the iteration will block until new events are
+subsequently recorded in the database. Any subsequently recorded events will then be
+immediately streamed to the client, and the iteration will then continue. The streaming
+of events, and hence the iteration, can be stopped by calling the `stop()` method on the
+"catch-up subscription" object.
+
+### Subscribe to all events
+
+The`subscribe_to_all()` method can be used to start a catch-up subscription
+from which all events recorded in the database can be obtained in the order
+they were recorded. This method returns a "catch-up subscription" iterator.
 
-The `subscribe_all_events()` method starts a catch-up subscription that can receive
-all events in the database. The `subscribe_stream_events()` method starts a catch-up
-subscription that can receive events from a specific stream.
-
-The `subscribe_all_events()` and `subscribe_stream_events()` methods both return a
-"read response" iterator, much like `iter_stream_events()` and `read_all_events()`.
-The difference is the "read response" iterator returned for a catch-up subscription
-does not automatically stop when there are no more recorded events to be returned, but
-instead blocks on getting the next event until further events are recorded in the
-database. These subsequently recorded events will then be streamed to the iterator,
-which will then continue. Like `read_all_events()`, the returned "read response" has
-a `stop()` method which will cancel the streaming gRPC operation and cause the
-"read response" iterator to stop.
-
-Like with `read_stream_events()` and `read_all_events()`, the recorded event objects
-received from a catch-up subscription are instances of the `RecordedEvent` class.
-
-### Subscribe all events
-
-The`subscribe_all_events()` method can be used to start a catch-up subscription
-from which all events recorded in the database can be received.
-
-This method can be used by a downstream component that processes recorded events with
-exactly-once semantics.
-
-This method returns a "read response", from which recorded events can be
-obtained by iteration, including events that are recorded after all the
-recorded events have been received. Iterating over this "read response"
-object will therefore not stop, unless the `stop()` method of the
-"read response" object is called, or a connection issue occurs, or
-the returned object iterator object is deleted from memory.
-
-This method has an optional `commit_position` argument, which can be
-used to specify a commit position from which to subscribe. The default
-value is `None`, which means the subscription will operate from the first
-recorded event in the database. If a commit position is given, it must match
-an actually existing commit position in the database. The recoded events that
-are obtained will not include the event recorded at that commit position.
-
-This method also has four other optional arguments, `filter_exclude`,
+This method also has five optional arguments, `commit_position()`, `filter_exclude`,
 `filter_include`, `filter_by_stream_name`, and `timeout`.
 
+The optional `commit_position` argument specifies a commit position. The default
+value of `commit_position` is `None`, which means the catch-up subscription will
+start from the first recorded event in the database. If a commit position is given,
+it must match an actually existing commit position in the database. Only events
+recorded after that position will be obtained.
+
 The optional `filter_exclude` argument is a sequence of regular expressions that
 specifies which recorded events should be returned. This argument is ignored
 if `filter_include` is set to a non-empty sequence. The default value of this
 argument matches the event types of EventStoreDB "system events", so that system
 events will not normally be included. See the Notes section below for more
 information about filter expressions.
 
@@ -1672,124 +1713,124 @@
 whether the filtering will apply to event types or stream names. By default, this
 value is `False` and so the filtering will apply to the event type strings of
 recorded events.
 
 The optional `timeout` argument is a Python `float` which sets a
 deadline for the completion of the gRPC operation.
 
-The example below shows how to start a catch-up subscription to receive
+The example below shows how to start a catch-up subscription that starts
 from the first recorded event in the database.
 
 ```python
 # Subscribe from the first recorded event in the database.
-subscription = client.subscribe_all_events()
+catchup_subscription = client.subscribe_to_all()
 ```
 
-The example below is longer, and shows that the catch-up subscription
-does not stop automatically, but blocks when the last recorded event is
-received, and then continues when subsequent events are recorded.
+The example below shows that catch-up subscriptions do not stop
+automatically, but block when the last recorded event is received,
+and then continue when subsequent events are recorded.
 
 ```python
+from datetime import datetime
+from threading import Thread
+
+from esdbclient import Checkpoint
+
 # Append a new event to a new stream.
 stream_name2 = str(uuid.uuid4())
 event4 = NewEvent(type='OrderCreated', data=b'data4')
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name2,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event4],
 )
 
-# Subscribe from the first recorded event in the database.
-subscription = client.subscribe_all_events()
-received_events = []
-
 
 # Receive events from the catch-up subscription in a different thread.
-from datetime import datetime
-from threading import Thread
-
+received_events = []
 mark = datetime.now()
 
 def receive_events():
-    for event in subscription:
-        received_events.append(event)
+    for event in catchup_subscription:
         global mark
         mark = datetime.now()
+        received_events.append(event)
 
 
 def wait_for_subscription_to_block():
     while True:
          if (datetime.now() - mark).total_seconds() > 1:
              break
 
 
-thread = Thread(target=receive_events)
+thread = Thread(target=receive_events, daemon=True)
 thread.start()
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 # Check the last received event is 'event4'.
-assert received_events[-1].id == event4.id
+assert received_events[-1].id == event4.id, received_events[-1].id
 
 # Check we also received the other events we have recorded.
 assert received_events[-9].id == event1.id
 assert received_events[-8].id == event2.id
 assert received_events[-7].id == event3.id
 assert received_events[-6].type == "DogRegistered"
 assert received_events[-5].type == "DogLearnedTrick"
 assert received_events[-4].type == "DogLearnedTrick"
 assert received_events[-3].type == "Snapshot"
 assert received_events[-2].type == "DogLearnedTrick"
 
 # Append another event whilst the subscription is running.
 mark = datetime.now()
 event5 = NewEvent(type='OrderUpdated', data=b'data5')
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name2,
     current_version=0,
     events=[event5],
 )
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 # Check the last received event is 'event5'.
 assert received_events[-2].id == event4.id
 assert received_events[-1].id == event5.id
 
 # Stop the subscription.
-subscription.stop()
+catchup_subscription.stop()
 thread.join()
 ```
 
-The example below shows how to start a catch-up subscription to
-receive from a particular commit position, in this case from the
-commit position of the last recorded event that was received above.
-Another event is recorded before the subscription is restarted.
-Further events are recorded whilst the subscription is running.
-All the recorded events are received exactly once.
+The example below shows how to subscribe to events recorded after a
+particular commit position, in this case from the commit position of
+the last recorded event that was received above. Another event is
+recorded before the subscription is restarted. Further events are
+recorded whilst the subscription is running. All the recorded events
+are received exactly once.
 
 ```python
 
 # Append another event.
 event6 = NewEvent(type='OrderDeleted', data=b'data6')
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name2,
     current_version=1,
     events=[event6],
 )
 
-# Resume subscribing from the commit position of the last received event.
-subscription = client.subscribe_all_events(
+# Restart subscribing to all events after the
+# commit position of the last received event.
+catchup_subscription = client.subscribe_to_all(
     commit_position=received_events[-1].commit_position
 )
 
 mark = datetime.now()
-thread = Thread(target=receive_events)
+thread = Thread(target=receive_events, daemon=True)
 thread.start()
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 # Check the last received event was 'event6'.
 assert received_events[-3].id == event4.id
@@ -1799,17 +1840,17 @@
 # Append three more events to a new stream.
 mark = datetime.now()
 stream_name3 = str(uuid.uuid4())
 event7 = NewEvent(type='OrderCreated', data=b'data7')
 event8 = NewEvent(type='OrderUpdated', data=b'data8')
 event9 = NewEvent(type='OrderDeleted', data=b'data9')
 
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name3,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event7, event8, event9],
 )
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 
@@ -1818,54 +1859,56 @@
 assert received_events[-5].id == event5.id
 assert received_events[-4].id == event6.id
 assert received_events[-3].id == event7.id
 assert received_events[-2].id == event8.id
 assert received_events[-1].id == event9.id
 
 # Stop the subscription.
-subscription.stop()
+catchup_subscription.stop()
 thread.join()
 ```
 
 The catch-up subscription call is ended as soon as the subscription object's
 `stop()` method is called. This happens automatically when it goes out of scope,
 or when it is explicitly deleted from memory using the Python `del` keyword.
 
-### Subscribe stream events
+### Subscribe to stream events
 
-The `subscribe_stream_events()` method can be used to start a catch-up subscription
-that can return events that are recorded in a single stream.
+The `subscribe_to_stream()` method can be used to start a catch-up subscription
+from which events recorded in a single stream can be obtained. This method
+returns a "catch-up subscription" iterator.
 
 This method has a required `stream_name` argument, which specifies the name of the
 stream from which recorded events will be received.
 
 This method also has two optional arguments, `stream_position`, and `timeout`.
 
-The optional `stream_position` argument specifies a position in the stream from which
-recorded events will be received. The event at the specified stream position will not
-be included. The default value of `stream_position` is `None`, which means the
-subscription will start from the first recorded event in the stream.
+The optional `stream_position` argument specifies a position in the stream. The
+default value of `stream_position` is `None`, which means that all events
+recorded in the stream will be obtained in the order they were recorded.
+If a stream position is given, then only events recorded after that position
+will be obtained.
 
 The optional `timeout` argument is a Python `float` that sets
 a deadline for the completion of the gRPC operation.
 
 The example below shows how to start a catch-up subscription from
 the first recorded event in a stream.
 
 ```python
 # Subscribe from the start of 'stream2'.
-subscription = client.subscribe_stream_events(stream_name=stream_name2)
+subscription = client.subscribe_to_stream(stream_name=stream_name2)
 ```
 
 The example below shows how to start a catch-up subscription from
 a particular stream position.
 
 ```python
 # Subscribe to stream2, from the second recorded event.
-subscription = client.subscribe_stream_events(
+subscription = client.subscribe_to_stream(
     stream_name=stream_name2,
     stream_position=1,
 )
 ```
 
 ### How to implement exactly-once event processing
 
@@ -2536,136 +2579,96 @@
 
 An example of when it might be desirable to reconnect manually is when (for performance
 reasons) the client's node preference is to be connected to a follower node in the
 cluster, and, after a cluster leader election, the follower becomes the leader.
 Reconnecting to a follower node in this case is currently beyond the capabilities of
 this client, but this behavior might be implemented in a future release.
 
-Please note, nearly all the client methods are decorated with `@autoreconnect` (which
-calls the `reconnect()` method when the client detects that reconnecting is required)
-and a `@retry` decorator that more generally will retry operations that fail due to
-connection issues.
-
-The `@autoreconnect` decorator will reconnect to a suitable node in the cluster when
-the server to which the client has been connected has become unavailable, or when the
-client's gRPC channel happens to have been closed. The client will also reconnect when
-a method is called that requires a leader, and the client's node preference is to be
-connected to a leader, but the node that the client has been connected to stops being
-the leader. In this case, the client will reconnect to the current leader. After
-reconnecting, the failed operation will be retried.
-
-The `@retry` decorator retries operations that have failed due to more general
-connection issues, such as a deadline being reached (so that the operation times
-out), or in case the server throws an exception when handling a client request.
-
-Please also note, the aspects not covered by the reconnect and retry decorator
-behaviours have to do with methods that return iterators. For example, consider
-the "read response" iterator returned from the `read_all_events()` method. The
-`read_all_events()` method will have returned, and the method decorators will therefore
-have exited, before iterating over the "read response" begins. Therefore, if a
-connection issues occurs whilst iterating over the "read response", it isn't possible
-for any decorator on the `read_all_events()` method to trigger a reconnection.
-
-Another example is iterating over the "read response" from a catch-up subscription.
-Although, with these methods there is an initial "confirmation" response from the server
-which is received and checked by the client before the method returns the
-"read response" iterator. And so, when the call is made, if the server is unavailable,
-or if the channel has somehow been closed, then the client will reconnect and retry.
-However, if an event-processing component that is iterating over a successfully returned
-catch-up subscription "read response" somehow fails, the catch-up subscription will
-need to be restarted, using the event-processing component's "last saved commit position".
-This is completely safe, so long as the event-processing component has been recording
-the commit position of each recorded event atomically and uniquely along with any new
-state that results from processing the recorded events and the commit positions are
-recorded with a uniqueness constraint. In this case, the client will automatically
-reconnect to a node in the cluster when the subsequent call to a catch-up subscription
-method is made. Similarly, when reading persistent subscriptions, if there are
-connectivity issues after you have started iterating over a successfully received
-response, then the consumer will need to be restarted.
-
+Reconnection will happen automatically in many cases, due to the `@autoreconnect`
+decorator.
 
 ### Close
 
 The `close()` method can be used to cleanly close the client's gRPC connection.
 
 ```python
 client.close()
 ```
 
 
 ## Asyncio client
 
 The `esdbclient` package also includes an early version of an asynchronous I/O
 gRPC Python client. It follows exactly the same behaviors as the multithreaded
-`ESDBClient`, but uses the `grpc.aio` package and the `asyncio` module, instead of
+`EventStoreDBClient`, but uses the `grpc.aio` package and the `asyncio` module, instead of
 `grpc` and `threading`.
 
-The async function `AsyncioESDBClient` constructs the client, and connects to
+The async function `AsyncioEventStoreDBClient` constructs the client, and connects to
 a server. It can be imported from `esdbclient`, and can be called with the same
-arguments as `ESDBClient`. It supports both the "esdb" and the "esdb+discover"
+arguments as `EventStoreDBClient`. It supports both the "esdb" and the "esdb+discover"
 connection string URI schemes, and can connect to both "secure" and "insecure"
 EventStoreDB servers. It reconnects or retries when connection issues or server
 errors are encountered.
 
 ```python
-from esdbclient import AsyncioESDBClient
+from esdbclient import AsyncioEventStoreDBClient
 ```
 
-The asynchronous I/O client has the following methods: `append_events()`,
-`read_stream_events()`, `read_all_events()`, `subscribe_all_events()`,
+The asynchronous I/O client has the following methods: `append_to_stream()`,
+`get_stream()`, `read_all()`, `subscribe_to_all()`,
 `delete_stream()`, `tombstone_stream()`, and `reconnect()`.
 
-These methods are equivalent to the methods on `ESDBClient`. They have the same
+These methods are equivalent to the methods on `EventStoreDBClient`. They have the same
 method signatures, and can be called with the same arguments, to the same effect.
-The methods which appear on `ESDBClient` but not on `AsyncioESDBClient` will be
+The methods which appear on `EventStoreDBClient` but not on `AsyncioEventStoreDBClient` will be
 added soon.
 
 ### Synopsis
 
-The example below demonstrates the `append_events()`, `read_stream_events()` and
-`subscribe_all_events()` methods. These are the most useful methods for writing
+The example below demonstrates the `append_to_stream()`, `get_stream()` and
+`subscribe_to_all()` methods. These are the most useful methods for writing
 an event-sourced application, allowing new aggregate events to be recorded, the
 recorded events of an aggregate to be obtained so aggregates can be reconstructed,
 and the state of an application to propagated and processed with "exactly-once"
 semantics.
 
 ```python
 import asyncio
 
 async def demonstrate_asyncio_client():
 
     # Construct client.
-    client = await AsyncioESDBClient(
+    client = await AsyncioEventStoreDBClient(
         uri=os.getenv("ESDB_URI"),
         root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),
     )
 
     # Append events.
     stream_name = str(uuid.uuid4())
     event1 = NewEvent("OrderCreated", data=b'{}')
     event2 = NewEvent("OrderUpdated", data=b'{}')
     event3 = NewEvent("OrderDeleted", data=b'{}')
 
-    commit_position = await client.append_events(
+    commit_position = await client.append_to_stream(
         stream_name=stream_name,
-        current_version=None,
+        current_version=StreamState.NO_STREAM,
         events=[event1, event2, event3]
     )
 
     # Read stream events.
-    recorded = await client.read_stream_events(stream_name)
+    recorded = await client.get_stream(stream_name)
     assert len(recorded) == 3
     assert recorded[0].id == event1.id
     assert recorded[1].id == event2.id
     assert recorded[2].id == event3.id
 
 
     # Subscribe all events.
     received = []
-    async for event in await client.subscribe_all_events():
+    async for event in await client.subscribe_to_all():
         received.append(event)
         if event.commit_position == commit_position:
             break
     assert received[-3].id == event1.id
     assert received[-2].id == event2.id
     assert received[-1].id == event3.id
 
@@ -2680,22 +2683,30 @@
 )
 ```
 
 ## Notes
 
 ### Regular expression filters
 
-The `read_all_events()`, `subscribe_all_events()`, `create_subscription()`
+The `read_all()`, `subscribe_to_all()`, `create_subscription()`
 and `get_commit_position()` methods have `filter_exclude` and `filter_include`
 arguments. This section provides some more details about the values of these
 arguments.
 
-The default value of the `filter_exclude` arguments is designed to exclude
-EventStoreDB "system" and "persistence subscription config" events, which
-otherwise would be included.
+The first thing to note is that these arguments are sequences of regular expressions.
+They are concatenated together by the client as bracketed alternatives in a larger
+regular expression that is anchored to the start and end of the strings being
+matched. So you shouldn't include the `'^'` and `'$'` anchor characters, unless
+these characters are escaped as literal characters to be matched. But you should
+use wildcards if you want to match substrings, for example `'.*Snapshot'` to match
+all strings that end with `'Snapshot`'.
+
+In all methods, the default value of the `filter_exclude` argument is the constant
+`DEFAULT_EXCLUDE_FILTER`, which is designed to exclude EventStoreDB "system" and
+"persistence subscription config" event types, which otherwise would be included.
 
 System events generated by EventStoreDB have `type` strings that start with
 the `$` sign. Persistence subscription events generated when manipulating
 persistence subscriptions have `type` strings that start with `PersistentConfig`.
 
 For example, to match the type of EventStoreDB system events, use the regular
 expression string `r'\$.+'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is
@@ -2706,20 +2717,55 @@
 regular expression `r'PersistentConfig\d+'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`
 is set to this value. You can import this constant from `esdbclient`  and use it when
 building longer sequences of regular expressions.
 
 The constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that includes
 both `ESDB_SYSTEM_EVENTS_REGEX` and `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`. It is used
 as the default value of `filter_exclude` so that the events that EventStoreDB generates
-internally are excluded by default, events other than to those which you record using
-the `append_events()` method.
+internally are excluded by default.
+
+For example, if you want to exclude snapshots and system events and persistent subscription
+events, then you may wish to use a appropriately extended copy of `DEFAULT_EXCLUDE_FILTER`
+as the value of the `filter_exclude` arguments, such as `DEFAULT_EXCLUDE_FILTER + ['.*Snapshot']`.
+
+
+### Reconnect and retry method decorators
+
+Please note, nearly all the client methods are decorated with the `@autoreconnect` and
+the `@retrygrpc` decorators.
+
+The `@autoreconnect` decorator will reconnect to a suitable node in the cluster when
+the server to which the client has been connected has become unavailable, or when the
+client's gRPC channel happens to have been closed. The client will also reconnect when
+a method is called that requires a leader, and the client's node preference is to be
+connected to a leader, but the node that the client has been connected to stops being
+the leader. In this case, the client will reconnect to the current leader. After
+reconnecting, the failed operation will be retried.
 
-If you want to exclude, for example, snapshots from the recorded events returned when
-reading events from the database, then you may wish to use a appropriately extended
-copy of `DEFAULT_EXCLUDE_FILTER` as the value of the `filter_exclude` arguments.
+The `@retrygrpc` decorator retries operations that have failed due to a deadline being
+reached (so that the operation times out), and in case the server throws an exception
+when handling a client request.
+
+Please also note, the aspects not covered by the reconnect and retry decorator
+behaviours have to do with methods that return iterators. For example, consider
+the "read response" iterator returned from the `read_all()` method. The
+`read_all()` method will have returned, and the method decorators will therefore
+have exited, before iterating over the "read response" begins. Therefore, if a
+connection issues occurs whilst iterating over the "read response", it isn't possible
+for any decorator on the `read_all()` method to trigger a reconnection.
+
+With the "catch-up subscription" objects, there is an initial "confirmation" response
+from the server which is received and checked by the client. And so, when a call is
+made to `subscribe_to_all()` or `subscribe_to_stream()`, if the server is unavailable,
+or if the channel has somehow been closed, or if the request fails for some other reason,
+then the client will reconnect and retry. However, if an exception is raised when iterating over a
+successfully returned "catch-up subscription" object, the catch-up subscription will
+need to be restarted. Similarly, when reading persistent subscriptions, if there are
+connection issues whilst iterating over a successfully received response, the consumer
+will need to be restarted.
 
 
 ## Contributors
 
 ### Install Poetry
 
 The first thing is to check you have Poetry installed.
@@ -2821,7 +2867,8 @@
 
 Tests belong in `./tests`. Code-under-test belongs in `./esdbclient`.
 
 Edit package dependencies in `pyproject.toml`. Update installed packages (and the
 `poetry.lock` file) using the following command.
 
     $ make update-packages
+
```

### Comparing `esdbclient-1.0a6/esdbclient/asyncio_client.py` & `esdbclient-1.0a7/esdbclient/asyncio_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 import asyncio
 import random
 import sys
 from asyncio import Event, Lock
 from functools import wraps
 from typing import (
     Any,
-    AsyncIterable,
     Callable,
     Iterable,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
+    Union,
     cast,
 )
 
 import dns
 import dns.asyncresolver
 import grpc.aio
 
-from esdbclient.client import DEFAULT_EXCLUDE_FILTER, BaseESDBClient
-from esdbclient.connection import (
+from esdbclient.client import DEFAULT_EXCLUDE_FILTER, BaseEventStoreDBClient
+from esdbclient.connection import AsyncioESDBConnection
+from esdbclient.connection_spec import (
     NODE_PREFERENCE_FOLLOWER,
     NODE_PREFERENCE_LEADER,
     NODE_PREFERENCE_RANDOM,
     NODE_PREFERENCE_REPLICA,
     URI_SCHEME_ESDB,
     URI_SCHEME_ESDB_DISCOVER,
-    AsyncioESDBConnection,
+)
+from esdbclient.esdbapibase import (
+    DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
+    DEFAULT_WINDOW_SIZE,
 )
 from esdbclient.events import NewEvent, RecordedEvent
 from esdbclient.exceptions import (
     DiscoveryFailed,
     DNSError,
     FollowerNotFound,
     GossipSeedError,
@@ -44,22 +48,27 @@
 )
 from esdbclient.gossip import (
     NODE_STATE_FOLLOWER,
     NODE_STATE_LEADER,
     NODE_STATE_REPLICA,
     ClusterMember,
 )
+from esdbclient.streams import (
+    AsyncioCatchupSubscription,
+    AsyncioReadResponse,
+    StreamState,
+)
 
 _TCallable = TypeVar("_TCallable", bound=Callable[..., Any])
 
 
 def autoreconnect(f: _TCallable) -> _TCallable:
     @wraps(f)
     async def autoreconnect_decorator(
-        client: "_AsyncioESDBClient", *args: Any, **kwargs: Any
+        client: "_AsyncioEventStoreDBClient", *args: Any, **kwargs: Any
     ) -> Any:
         try:
             return await f(client, *args, **kwargs)
 
         except NodeIsNotLeader:
             if client.connection_spec.options.NodePreference == NODE_PREFERENCE_LEADER:
                 await client.reconnect()
@@ -92,23 +101,23 @@
         except GrpcError:
             await asyncio.sleep(0.1)
             return await f(*args, **kwargs)
 
     return cast(_TCallable, retrygrpc_decorator)
 
 
-async def AsyncioESDBClient(
+async def AsyncioEventStoreDBClient(
     uri: str, root_certificates: Optional[str] = None
-) -> "_AsyncioESDBClient":
-    client = _AsyncioESDBClient(uri=uri, root_certificates=root_certificates)
+) -> "_AsyncioEventStoreDBClient":
+    client = _AsyncioEventStoreDBClient(uri=uri, root_certificates=root_certificates)
     await client.connect()
     return client
 
 
-class _AsyncioESDBClient(BaseESDBClient):
+class _AsyncioEventStoreDBClient(BaseEventStoreDBClient):
     def __init__(self, uri: str, root_certificates: Optional[str] = None):
         super().__init__(uri=uri, root_certificates=root_certificates)
         self._is_reconnection_required = Event()
         self._reconnection_lock = Lock()
 
     async def connect(self) -> None:
         self._connection = await self._connect_to_preferred_node()
@@ -240,48 +249,68 @@
                 options=grpc_options,
             )
         else:
             grpc_channel = grpc.aio.insecure_channel(
                 target=grpc_target, options=grpc_options
             )
 
-        return AsyncioESDBConnection(grpc_channel=grpc_channel, grpc_target=grpc_target)
+        return AsyncioESDBConnection(
+            grpc_channel=grpc_channel,
+            grpc_target=grpc_target,
+            connection_spec=self.connection_spec,
+        )
 
     @retrygrpc
     @autoreconnect
     async def append_events(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         events: Iterable[NewEvent],
         timeout: Optional[float] = None,
     ) -> int:
         timeout = timeout if timeout is not None else self._default_deadline
         result = await self._connection.streams.batch_append(
             stream_name=stream_name,
             current_version=current_version,
             events=events,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
         return result.commit_position
 
+    async def append_to_stream(
+        self,
+        stream_name: str,
+        current_version: Union[int, StreamState],
+        events: Union[NewEvent, Iterable[NewEvent]],
+        timeout: Optional[float] = None,
+    ) -> int:
+        if isinstance(events, NewEvent):
+            events = [events]
+        return await self.append_events(
+            stream_name=stream_name,
+            current_version=current_version,
+            events=events,
+            timeout=timeout,
+        )
+
     @retrygrpc
     @autoreconnect
-    async def read_all_events(
+    async def read_all(
         self,
         commit_position: Optional[int] = None,
         backwards: bool = False,
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioReadResponse:
         """
         Reads recorded events in "all streams" in the database.
         """
         return await self._connection.streams.read(
             commit_position=commit_position,
             backwards=backwards,
             filter_exclude=filter_exclude,
@@ -291,84 +320,92 @@
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
-    async def read_stream_events(
+    async def get_stream(
         self,
         stream_name: str,
         stream_position: Optional[int] = None,
         backwards: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
     ) -> Sequence[RecordedEvent]:
         """
         Lists recorded events from the named stream.
         """
-        events = await self.iter_stream_events(
+        events = await self.read_stream(
             stream_name=stream_name,
             stream_position=stream_position,
             backwards=backwards,
             limit=limit,
             timeout=timeout,
         )
         return tuple([e async for e in events])
 
-    async def iter_stream_events(
+    async def read_stream(
         self,
         stream_name: str,
         stream_position: Optional[int] = None,
         backwards: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioReadResponse:
         """
         Reads recorded events from the named stream.
         """
         return await self._connection.streams.read(
             stream_name=stream_name,
             stream_position=stream_position,
             backwards=backwards,
             limit=limit,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
-    async def subscribe_all_events(
+    @retrygrpc
+    @autoreconnect
+    async def subscribe_to_all(
         self,
         commit_position: Optional[int] = None,
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        include_checkpoints: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioCatchupSubscription:
         """
         Starts a catch-up subscription, from which all
         recorded events in the database can be received.
         """
         return await self._connection.streams.read(
             commit_position=commit_position,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
             subscribe=True,
+            include_checkpoints=include_checkpoints,
+            window_size=window_size,
+            checkpoint_interval_multiplier=checkpoint_interval_multiplier,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     async def delete_stream(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
     ) -> None:
         # Todo: Reconsider using current_version=None to indicate "stream exists"?
         timeout = timeout if timeout is not None else self._default_deadline
         await self._connection.streams.delete(
             stream_name=stream_name,
             current_version=current_version,
@@ -378,15 +415,15 @@
         )
 
     @retrygrpc
     @autoreconnect
     async def tombstone_stream(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
     ) -> None:
         timeout = timeout if timeout is not None else self._default_deadline
         await self._connection.streams.tombstone(
             stream_name=stream_name,
             current_version=current_version,
             timeout=timeout,
```

### Comparing `esdbclient-1.0a6/esdbclient/client.py` & `esdbclient-1.0a7/esdbclient/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,39 @@
     Callable,
     Dict,
     Iterable,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
+    Union,
     cast,
     overload,
 )
 
 import dns.exception
 import dns.resolver
 import grpc
+from typing_extensions import Literal
 
-from esdbclient.connection import (
+from esdbclient.connection import ESDBConnection
+from esdbclient.connection_spec import (
     NODE_PREFERENCE_FOLLOWER,
     NODE_PREFERENCE_LEADER,
     NODE_PREFERENCE_RANDOM,
     NODE_PREFERENCE_REPLICA,
     URI_SCHEME_ESDB,
     URI_SCHEME_ESDB_DISCOVER,
     ConnectionSpec,
-    ESDBConnection,
 )
-from esdbclient.esdbapibase import BasicAuthCallCredentials
+from esdbclient.esdbapibase import (
+    DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
+    DEFAULT_WINDOW_SIZE,
+    BasicAuthCallCredentials,
+)
 from esdbclient.events import NewEvent, RecordedEvent
 from esdbclient.exceptions import (
     DiscoveryFailed,
     DNSError,
     FollowerNotFound,
     GossipSeedError,
     GrpcError,
@@ -53,29 +59,31 @@
     ClusterMember,
 )
 from esdbclient.persistent import (
     ConsumerStrategy,
     PersistentSubscription,
     SubscriptionInfo,
 )
-from esdbclient.streams import CatchupSubscription, ReadResponse
+from esdbclient.streams import CatchupSubscription, ReadResponse, StreamState
 
 # Matches the 'type' of "system" events.
 ESDB_SYSTEM_EVENTS_REGEX = r"\$.+"
 # Matches the 'type' of "PersistentConfig" events.
 ESDB_PERSISTENT_CONFIG_EVENTS_REGEX = r"PersistentConfig\d+"
 
 DEFAULT_EXCLUDE_FILTER = (ESDB_SYSTEM_EVENTS_REGEX, ESDB_PERSISTENT_CONFIG_EVENTS_REGEX)
 
 _TCallable = TypeVar("_TCallable", bound=Callable[..., Any])
 
 
 def autoreconnect(f: _TCallable) -> _TCallable:
     @wraps(f)
-    def autoreconnect_decorator(client: "ESDBClient", *args: Any, **kwargs: Any) -> Any:
+    def autoreconnect_decorator(
+        client: "EventStoreDBClient", *args: Any, **kwargs: Any
+    ) -> Any:
         try:
             return f(client, *args, **kwargs)
 
         except NodeIsNotLeader:
             if client.connection_spec.options.NodePreference == NODE_PREFERENCE_LEADER:
                 client.reconnect()
                 sleep(0.1)
@@ -107,15 +115,15 @@
         except GrpcError:
             sleep(0.1)
             return f(*args, **kwargs)
 
     return cast(_TCallable, retrygrpc_decorator)
 
 
-class BaseESDBClient:
+class BaseEventStoreDBClient:
     def __init__(
         self,
         uri: Optional[str] = None,
         *,
         root_certificates: Optional[str] = None,
     ) -> None:
         self.root_certificates = root_certificates
@@ -153,15 +161,15 @@
             return grpc.metadata_call_credentials(
                 BasicAuthCallCredentials(username, password)
             )
         else:
             return None
 
 
-class ESDBClient(BaseESDBClient):
+class EventStoreDBClient(BaseEventStoreDBClient):
     """
     Encapsulates the EventStoreDB gRPC API.
     """
 
     def __init__(
         self,
         uri: Optional[str] = None,
@@ -305,34 +313,38 @@
                 options=grpc_options,
             )
         else:
             grpc_channel = grpc.insecure_channel(
                 target=grpc_target, options=grpc_options
             )
 
-        return ESDBConnection(grpc_channel=grpc_channel, grpc_target=grpc_target)
+        return ESDBConnection(
+            grpc_channel=grpc_channel,
+            grpc_target=grpc_target,
+            connection_spec=self.connection_spec,
+        )
 
     # def _batch_append_future_result_loop(self) -> None:
     #     # while self._channel_connectivity_state is not ChannelConnectivity.SHUTDOWN:
     #     try:
     #         self._connection.streams.batch_append_multiplexed(
     #             futures_queue=self._batch_append_futures_queue,
     #             timeout=None,
     #             metadata=self._call_metadata,
     #             credentials=self._call_credentials,
     #         )
-    #     except ESDBClientException as e:
+    #     except EventStoreDBClientException as e:
     #         self._clear_batch_append_futures_queue(e)
     #     else:
     #         self._clear_batch_append_futures_queue(  # pragma: no cover
-    #             ESDBClientException("Request not sent")
+    #             EventStoreDBClientException("Request not sent")
     #         )
     #     # print("Looping on call to batch_append_multiplexed()....")
     #
-    # def _clear_batch_append_futures_queue(self, error: ESDBClientException) -> None:
+    # def _clear_batch_append_futures_queue(self, error: EventStoreDBClientException) -> None:
     #     with self._batch_append_futures_lock:
     #         try:
     #             while True:
     #                 future = self._batch_append_futures_queue.get(block=False)
     #                 future.set_exception(error)  # pragma: no cover
     #         except Empty:
     #             pass
@@ -356,15 +368,15 @@
     #     return response.commit_position
 
     @retrygrpc
     @autoreconnect
     def append_events(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         events: Iterable[NewEvent],
         timeout: Optional[float] = None,
     ) -> int:
         timeout = timeout if timeout is not None else self._default_deadline
         return self._connection.streams.batch_append(
             stream_name=stream_name,
             current_version=current_version,
@@ -375,15 +387,15 @@
         ).commit_position
 
     @retrygrpc
     @autoreconnect
     def append_event(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         event: NewEvent,
         timeout: Optional[float] = None,
     ) -> int:
         """
         Appends a new event to the named stream.
         """
         timeout = timeout if timeout is not None else self._default_deadline
@@ -392,20 +404,45 @@
             current_version=current_version,
             events=[event],
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
+    def append_to_stream(
+        self,
+        stream_name: str,
+        current_version: Union[int, StreamState],
+        events: Union[NewEvent, Sequence[NewEvent]],
+        timeout: Optional[float] = None,
+    ) -> int:
+        """
+        Appends a new event or a sequence of new events to the named stream.
+        """
+        if isinstance(events, NewEvent):
+            return self.append_event(
+                stream_name=stream_name,
+                current_version=current_version,
+                event=events,
+                timeout=timeout,
+            )
+        else:
+            return self.append_events(
+                stream_name=stream_name,
+                current_version=current_version,
+                events=events,
+                timeout=timeout,
+            )
+
     @retrygrpc
     @autoreconnect
     def delete_stream(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
     ) -> None:
         # Todo: Reconsider using current_version=None to indicate "stream exists"?
         timeout = timeout if timeout is not None else self._default_deadline
         self._connection.streams.delete(
             stream_name=stream_name,
             current_version=current_version,
@@ -415,50 +452,50 @@
         )
 
     @retrygrpc
     @autoreconnect
     def tombstone_stream(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
     ) -> None:
         timeout = timeout if timeout is not None else self._default_deadline
         self._connection.streams.tombstone(
             stream_name=stream_name,
             current_version=current_version,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
-    def read_stream_events(
+    def get_stream(
         self,
         stream_name: str,
         stream_position: Optional[int] = None,
         backwards: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
     ) -> Sequence[RecordedEvent]:
         """
-        Lists recorded events from the named stream.
+        Returns a sequence of recorded events from the named stream.
         """
         return tuple(
-            self.iter_stream_events(
+            self.read_stream(
                 stream_name=stream_name,
                 stream_position=stream_position,
                 backwards=backwards,
                 limit=limit,
                 timeout=timeout,
             )
         )
 
-    def iter_stream_events(
+    def read_stream(
         self,
         stream_name: str,
         stream_position: Optional[int] = None,
         backwards: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
     ) -> ReadResponse:
@@ -471,15 +508,15 @@
             backwards=backwards,
             limit=limit,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
-    def read_all_events(
+    def read_all(
         self,
         commit_position: Optional[int] = None,
         backwards: bool = False,
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         limit: int = sys.maxsize,
@@ -502,15 +539,15 @@
 
     @retrygrpc
     @autoreconnect
     def get_current_version(
         self,
         stream_name: str,
         timeout: Optional[float] = None,
-    ) -> Optional[int]:
+    ) -> Union[int, Literal[StreamState.NO_STREAM]]:
         """
         Returns the current position of the end of a stream.
         """
         try:
             last_event = list(
                 self._connection.streams.read(
                     stream_name=stream_name,
@@ -518,18 +555,19 @@
                     limit=1,
                     timeout=timeout,
                     metadata=self._call_metadata,
                     credentials=self._call_credentials,
                 )
             )[0]
         except NotFound:
-            # None is the correct expected position when appending both to a stream that
-            # never existed, and for appending to a stream that has been deleted (in
-            # this case the old "stream position" int is also correct, but None works).
-            return None
+            # StreamState.NO_STREAM is the correct "current version" both when appending
+            # to a stream that never existed and when appending to a stream that has
+            # been deleted (in this case of a deleted stream, the "current version"
+            # before deletion is also correct).
+            return StreamState.NO_STREAM
         else:
             return last_event.stream_position
 
     @retrygrpc
     @autoreconnect
     def get_commit_position(
         self,
@@ -537,15 +575,15 @@
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
     ) -> int:
         """
         Returns the current commit position of the database.
         """
-        recorded_events = self.read_all_events(
+        recorded_events = self.read_all(
             backwards=True,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
             limit=1,
             timeout=timeout,
         )
@@ -555,39 +593,39 @@
             commit_position = ev.commit_position
         return commit_position
 
     @retrygrpc
     @autoreconnect
     def get_stream_metadata(
         self, stream_name: str, timeout: Optional[float] = None
-    ) -> Tuple[Dict[str, Any], Optional[int]]:
+    ) -> Tuple[Dict[str, Any], Union[int, Literal[StreamState.NO_STREAM]]]:
         """
         Gets the stream metadata.
         """
         metadata_stream_name = f"$${stream_name}"
         try:
             metadata_events = list(
-                self.read_stream_events(
+                self.get_stream(
                     stream_name=metadata_stream_name,
                     backwards=True,
                     limit=1,
                     timeout=timeout,
                 )
             )
         except NotFound:
-            return {}, None
+            return {}, StreamState.NO_STREAM
         else:
             metadata_event = metadata_events[0]
             return json.loads(metadata_event.data), metadata_event.stream_position
 
     def set_stream_metadata(
         self,
         stream_name: str,
         metadata: Dict[str, Any],
-        current_version: Optional[int] = -1,
+        current_version: Union[int, StreamState] = StreamState.ANY,
         timeout: Optional[float] = None,
     ) -> None:
         """
         Sets the stream metadata.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
@@ -601,40 +639,46 @@
             current_version=current_version,
             event=metadata_event,
             timeout=timeout,
         )
 
     @retrygrpc
     @autoreconnect
-    def subscribe_all_events(
+    def subscribe_to_all(
         self,
         commit_position: Optional[int] = None,
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        include_checkpoints: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
     ) -> CatchupSubscription:
         """
         Starts a catch-up subscription, from which all
         recorded events in the database can be received.
         """
         return self._connection.streams.read(
             commit_position=commit_position,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
             subscribe=True,
+            include_checkpoints=include_checkpoints,
+            window_size=window_size,
+            checkpoint_interval_multiplier=checkpoint_interval_multiplier,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
-    def subscribe_stream_events(
+    def subscribe_to_stream(
         self,
         stream_name: str,
         stream_position: Optional[int] = None,
         timeout: Optional[float] = None,
     ) -> CatchupSubscription:
         """
         Starts a catch-up subscription from which
@@ -685,14 +729,16 @@
         self,
         group_name: str,
         *,
         from_end: bool = True,
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         consumer_strategy: ConsumerStrategy = "DispatchToSingle",
         timeout: Optional[float] = None,
     ) -> None:
         """
         Signature for creating persistent subscription from end of database.
         """
 
@@ -702,14 +748,16 @@
         self,
         group_name: str,
         from_end: bool = False,
         commit_position: Optional[int] = None,
         filter_exclude: Sequence[str] = DEFAULT_EXCLUDE_FILTER,
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         consumer_strategy: ConsumerStrategy = "DispatchToSingle",
         timeout: Optional[float] = None,
     ) -> None:
         """
         Creates a persistent subscription on all streams.
         """
         timeout = timeout if timeout is not None else self._default_deadline
@@ -718,14 +766,16 @@
             group_name=group_name,
             from_end=from_end,
             commit_position=commit_position,
             consumer_strategy=consumer_strategy,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
+            window_size=window_size,
+            checkpoint_interval_multiplier=checkpoint_interval_multiplier,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
     @overload
     def create_stream_subscription(
@@ -794,15 +844,18 @@
             metadata=self._call_metadata,
             credentials=self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     def read_subscription(
-        self, group_name: str, buffer_size: int = 100, timeout: Optional[float] = None
+        self,
+        group_name: str,
+        buffer_size: int = 100,
+        timeout: Optional[float] = None,
     ) -> PersistentSubscription:
         """
         Reads a persistent subscription on all streams.
         """
         return self._connection.persistent_subscriptions.read(
             group_name=group_name,
             buffer_size=buffer_size,
```

### Comparing `esdbclient-1.0a6/esdbclient/connection.py` & `esdbclient-1.0a7/esdbclient/connection_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,12 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Dict, Optional, Sequence
 from urllib.parse import ParseResult, parse_qs, urlparse
 from uuid import uuid4
 
-import grpc
-import grpc.aio
-
-from esdbclient.gossip import (
-    AsyncioClusterGossipService,
-    AsyncioGossipService,
-    ClusterGossipService,
-    GossipService,
-)
-from esdbclient.persistent import (
-    AsyncioPersistentSubscriptionsService,
-    PersistentSubscriptionsService,
-)
-from esdbclient.streams import AsyncioStreamsService, StreamsService
-
 URI_SCHEME_ESDB = "esdb"
 URI_SCHEME_ESDB_DISCOVER = "esdb+discover"
 VALID_URI_SCHEMES = [
     URI_SCHEME_ESDB,
     URI_SCHEME_ESDB_DISCOVER,
 ]
 NODE_PREFERENCE_LEADER = "leader"
@@ -305,45 +290,7 @@
     @property
     def targets(self) -> Sequence[str]:
         return self._targets
 
     @property
     def options(self) -> ConnectionOptions:
         return self._options
-
-
-class ESDBConnection:
-    def __init__(self, grpc_channel: grpc.Channel, grpc_target: str) -> None:
-        self.grpc_channel = grpc_channel
-        self.grpc_target = grpc_target
-        self.streams = StreamsService(grpc_channel)
-        self.persistent_subscriptions = PersistentSubscriptionsService(grpc_channel)
-        self.gossip = GossipService(grpc_channel)
-        self.cluster_gossip = ClusterGossipService(grpc_channel)
-        # self._channel_connectivity_state: Optional[ChannelConnectivity] = None
-        # self.grpc_channel.subscribe(self._receive_channel_connectivity_state)
-
-    # def _receive_channel_connectivity_state(
-    #     self, connectivity: ChannelConnectivity
-    # ) -> None:
-    #     self._channel_connectivity_state = connectivity
-    #     # print("Channel connectivity state:", connectivity)
-
-    def close(self) -> None:
-        # self.grpc_channel.unsubscribe(self._receive_channel_connectivity_state)
-        # sleep(0.1)  # Allow connectivity polling to stop.
-        self.grpc_channel.close()
-
-
-class AsyncioESDBConnection:
-    def __init__(self, grpc_channel: grpc.aio.Channel, grpc_target: str) -> None:
-        self.grpc_channel = grpc_channel
-        self.grpc_target = grpc_target
-        self.streams = AsyncioStreamsService(grpc_channel)
-        self.persistent_subscriptions = AsyncioPersistentSubscriptionsService(
-            grpc_channel
-        )
-        self.gossip = AsyncioGossipService(grpc_channel)
-        self.cluster_gossip = AsyncioClusterGossipService(grpc_channel)
-
-    async def close(self) -> None:
-        await self.grpc_channel.close(grace=5)
```

### Comparing `esdbclient-1.0a6/esdbclient/esdbapibase.py` & `esdbclient-1.0a7/esdbclient/esdbapibase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # -*- coding: utf-8 -*-
 from base64 import b64encode
 from typing import TYPE_CHECKING, Optional, Tuple
 
 import grpc
 import grpc.aio
 
+from esdbclient.connection_spec import ConnectionSpec
 from esdbclient.exceptions import (
+    AbortedByServer,
     CancelledByClient,
+    ConsumerTooSlow,
     DeadlineExceeded,
-    ESDBClientException,
+    EventStoreDBClientException,
     ExceptionThrownByHandler,
     GrpcError,
     NodeIsNotLeader,
     NotFound,
     ServiceUnavailable,
 )
 
@@ -21,37 +24,48 @@
 
 else:
     Metadata = Tuple[Tuple[str, str], ...]
 
 __all__ = ["handle_rpc_error", "BasicAuthCallCredentials", "ESDBService", "Metadata"]
 
 
+DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER = 5
+DEFAULT_BATCH_APPEND_REQUEST_DEADLINE = 315576000000
+DEFAULT_WINDOW_SIZE = 30
+
+
 class BasicAuthCallCredentials(grpc.AuthMetadataPlugin):
     def __init__(self, username: str, password: str):
         credentials = b64encode(f"{username}:{password}".encode())
         self._metadata = (("authorization", (b"Basic " + credentials)),)
 
     def __call__(
         self,
         context: grpc.AuthMetadataContext,
         callback: grpc.AuthMetadataPluginCallback,
     ) -> None:
         callback(self._metadata, None)
 
 
-def handle_rpc_error(e: grpc.RpcError) -> ESDBClientException:
+def handle_rpc_error(e: grpc.RpcError) -> EventStoreDBClientException:
     """
     Converts gRPC errors to client exceptions.
     """
     if isinstance(e, (grpc.Call, grpc.aio.AioRpcError)):
         if (
             e.code() == grpc.StatusCode.UNKNOWN
             and "Exception was thrown by handler" in str(e.details())
         ):
             return ExceptionThrownByHandler(e)
+        elif e.code() == grpc.StatusCode.ABORTED:
+            details = e.details()
+            if isinstance(details, str) and "Consumer too slow" in details:
+                return ConsumerTooSlow()
+            else:
+                return AbortedByServer()
         elif (
             e.code() == grpc.StatusCode.CANCELLED
             and e.details() == "Locally cancelled by application!"
         ):
             return CancelledByClient(e)
         elif e.code() == grpc.StatusCode.DEADLINE_EXCEEDED:
             return DeadlineExceeded(e)
@@ -64,15 +78,23 @@
             return NodeIsNotLeader(e)
         elif e.code() == grpc.StatusCode.NOT_FOUND:
             return NotFound()
     return GrpcError(e)
 
 
 class ESDBService:
+    def __init__(self, connection_spec: ConnectionSpec):
+        self.connection_spec = connection_spec
+
     def _metadata(
         self, metadata: Optional[Metadata], requires_leader: bool = False
     ) -> Metadata:
+        default = (
+            "true"
+            if self.connection_spec.options.NodePreference == "leader"
+            else "false"
+        )
         requires_leader_metadata: Metadata = (
-            ("requires-leader", "true" if requires_leader else "false"),
+            ("requires-leader", "true" if requires_leader else default),
         )
         metadata = tuple() if metadata is None else metadata
         return metadata + requires_leader_metadata
```

### Comparing `esdbclient-1.0a6/esdbclient/exceptions.py` & `esdbclient-1.0a7/esdbclient/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
-class ESDBClientException(Exception):
+class EventStoreDBClientException(Exception):
     """
     Base class for exceptions raised by the client.
     """
 
 
-class GrpcError(ESDBClientException):
+class GrpcError(EventStoreDBClientException):
     """
     Base class for exceptions raised by gRPC.
     """
 
 
 class ExceptionThrownByHandler(GrpcError):
     """
@@ -32,87 +32,99 @@
 
 class CancelledByClient(GrpcError):
     """
     Raised when gRPC operation is cancelled.
     """
 
 
-class NodeIsNotLeader(ESDBClientException):
+class AbortedByServer(GrpcError):
+    """
+    Raised when gRPC operation is aborted.
+    """
+
+
+class ConsumerTooSlow(AbortedByServer):
+    """
+    Raised when buffer is overloaded.
+    """
+
+
+class NodeIsNotLeader(EventStoreDBClientException):
     """
     Raised when client attempts to write to a node that is not a leader.
     """
 
 
-class NotFound(ESDBClientException):
+class NotFound(EventStoreDBClientException):
     """
     Raised when stream or subscription is not found.
     """
 
 
-class SubscriptionConfirmationError(ESDBClientException):
+class SubscriptionConfirmationError(EventStoreDBClientException):
     """
     Raised when subscription confirmation fails.
     """
 
 
-class WrongCurrentVersion(ESDBClientException):
+class WrongCurrentVersion(EventStoreDBClientException):
     """
     Raised when expected position does not match the
     actual position of the last event in a stream.
     """
 
 
-class AccessDeniedError(ESDBClientException):
+class AccessDeniedError(EventStoreDBClientException):
     """
     Raised when access is denied by the server.
     """
 
 
-class StreamIsDeleted(ESDBClientException):
+class StreamIsDeleted(EventStoreDBClientException):
     """
     Raised when reading from or appending to a stream that has been
     tombstoned, and when deleting a stream that has been deleted
     whilst expecting the stream exists, and when getting or setting
     metadata for a stream that has been tombstoned, and when deleting
     a stream that has been tombstoned, and when tombstoning a stream
     that has been tombstoned.
     """
 
 
-class TimeoutError(ESDBClientException):
+class TimeoutError(EventStoreDBClientException):
     """
     Raised when append operation is timed out by the server.
     """
 
 
-class UnknownError(ESDBClientException):
+class UnknownError(EventStoreDBClientException):
     """
     Raised when append operation fails with an "unknown" error.
     """
 
 
-class InvalidTransactionError(ESDBClientException):
+class InvalidTransactionError(EventStoreDBClientException):
     """
     Raised when append operation fails with an "invalid transaction" error.
     """
 
 
-class MaximumAppendSizeExceededError(ESDBClientException):
+class MaximumAppendSizeExceededError(EventStoreDBClientException):
     """
     Raised when append operation fails with a "maximum append size exceeded" error.
     """
 
 
-class BadRequestError(ESDBClientException):
+class BadRequestError(EventStoreDBClientException):
     """
     Raised when append operation fails with a "bad request" error.
     """
 
 
-class DiscoveryFailed(ESDBClientException):
+class DiscoveryFailed(EventStoreDBClientException):
     """
     Raised when client fails to satisfy node preference using gossip cluster info.
     """
 
 
 class GossipSeedError(DiscoveryFailed):
     """
```

### Comparing `esdbclient-1.0a6/esdbclient/gossip.py` & `esdbclient-1.0a7/esdbclient/gossip.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from dataclasses import dataclass
 from typing import Optional, Sequence, Union
 
 import grpc
 import grpc.aio
 
+from esdbclient.connection_spec import ConnectionSpec
 from esdbclient.esdbapibase import ESDBService, Metadata, handle_rpc_error
 from esdbclient.protos.Grpc import (
     cluster_pb2,
     cluster_pb2_grpc,
     gossip_pb2,
     gossip_pb2_grpc,
     shared_pb2,
@@ -30,15 +31,20 @@
     gossip_pb2.MemberInfo.VNodeState.Follower: NODE_STATE_FOLLOWER,
     gossip_pb2.MemberInfo.VNodeState.Leader: NODE_STATE_LEADER,
     gossip_pb2.MemberInfo.VNodeState.ReadOnlyReplica: NODE_STATE_REPLICA,
 }
 
 
 class BaseGossipService(ESDBService):
-    def __init__(self, channel: Union[grpc.Channel, grpc.aio.Channel]):
+    def __init__(
+        self,
+        channel: Union[grpc.Channel, grpc.aio.Channel],
+        connection_spec: ConnectionSpec,
+    ):
+        super().__init__(connection_spec=connection_spec)
         self._stub = gossip_pb2_grpc.GossipStub(channel)
 
     @staticmethod
     def _construct_cluster_members(
         cluster_info: gossip_pb2.ClusterInfo,
     ) -> Sequence[ClusterMember]:
         members = []
@@ -100,15 +106,20 @@
     cluster_pb2.MemberInfo.VNodeState.Follower: NODE_STATE_FOLLOWER,
     cluster_pb2.MemberInfo.VNodeState.Leader: NODE_STATE_LEADER,
     cluster_pb2.MemberInfo.VNodeState.ReadOnlyReplica: NODE_STATE_REPLICA,
 }
 
 
 class BaseClusterGossipService(ESDBService):
-    def __init__(self, channel: Union[grpc.Channel, grpc.aio.Channel]):
+    def __init__(
+        self,
+        channel: Union[grpc.Channel, grpc.aio.Channel],
+        connection_spec: ConnectionSpec,
+    ):
+        super().__init__(connection_spec=connection_spec)
         self._stub = cluster_pb2_grpc.GossipStub(channel)
 
 
 class AsyncioClusterGossipService(BaseClusterGossipService):
     pass
```

### Comparing `esdbclient-1.0a6/esdbclient/persistent.py` & `esdbclient-1.0a7/esdbclient/persistent.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,26 @@
 from dataclasses import dataclass
 from typing import Iterator, List, Optional, Sequence, Tuple, Union, overload
 from uuid import UUID
 
 import grpc
 from typing_extensions import Literal, Protocol, runtime_checkable
 
-from esdbclient.esdbapibase import ESDBService, Metadata, handle_rpc_error
+from esdbclient.connection_spec import ConnectionSpec
+from esdbclient.esdbapibase import (
+    DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
+    DEFAULT_WINDOW_SIZE,
+    ESDBService,
+    Metadata,
+    handle_rpc_error,
+)
 from esdbclient.events import RecordedEvent
 from esdbclient.exceptions import (
     CancelledByClient,
-    ESDBClientException,
+    EventStoreDBClientException,
     NodeIsNotLeader,
     SubscriptionConfirmationError,
 )
 from esdbclient.protos.Grpc import persistent_pb2, persistent_pb2_grpc, shared_pb2
 
 
 @runtime_checkable
@@ -135,27 +142,34 @@
     outstanding_messages_count: int
     named_consumer_strategy: str
     max_subscriber_count: int
     parked_message_count: int
 
 
 class BasePersistentSubscriptionsService(ESDBService):
-    def __init__(self, channel: Union[grpc.Channel, grpc.aio.Channel]):
+    def __init__(
+        self,
+        channel: Union[grpc.Channel, grpc.aio.Channel],
+        connection_spec: ConnectionSpec,
+    ):
+        super().__init__(connection_spec=connection_spec)
         self._stub = persistent_pb2_grpc.PersistentSubscriptionsStub(channel)
 
     def _construct_create_req(
         self,
         group_name: str,
         stream_name: Optional[str] = None,
         from_end: bool = False,
         commit_position: Optional[int] = None,
         stream_position: Optional[int] = None,
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         consumer_strategy: ConsumerStrategy = "DispatchToSingle",
     ) -> persistent_pb2.CreateReq:
         # Construct 'settings'.
         settings = persistent_pb2.CreateReq.Settings(
             resolve_links=False,
             extra_statistics=False,
             max_retry_count=5,
@@ -235,19 +249,16 @@
                 else:
                     stream_identifier_filter = None
                     event_type_filter = filter_expression
 
                 filter = persistent_pb2.CreateReq.AllOptions.FilterOptions(
                     stream_identifier=stream_identifier_filter,
                     event_type=event_type_filter,
-                    # Todo: What does 'window' mean?
-                    # max=shared_pb2.Empty(),
-                    count=shared_pb2.Empty(),
-                    # Todo: What does 'checkpointIntervalMultiplier' mean?
-                    checkpointIntervalMultiplier=5,
+                    max=window_size,
+                    checkpointIntervalMultiplier=checkpoint_interval_multiplier,
                 )
                 all_options.filter.CopyFrom(filter)
             else:
                 no_filter = shared_pb2.Empty()
                 all_options.no_filter.CopyFrom(no_filter)
 
             options.all.CopyFrom(all_options)
@@ -514,15 +525,15 @@
             )
             if (
                 confirmed_group_name != expected_group_name
                 or confirmed_stream_name != expected_stream_name
             ):  # pragma: no cover
                 raise SubscriptionConfirmationError()
         else:  # pragma: no cover
-            raise ESDBClientException(
+            raise EventStoreDBClientException(
                 f"Expected subscription confirmation, got: {first_read_resp}"
             )
 
     def __iter__(self) -> Iterator[RecordedEvent]:
         return self
 
     def __next__(self) -> RecordedEvent:
@@ -575,14 +586,16 @@
         *,
         from_end: bool = False,
         commit_position: Optional[int] = None,
         consumer_strategy: ConsumerStrategy = "DispatchToSingle",
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Signature for creating a persistent "all streams" subscription.
         """
@@ -610,28 +623,32 @@
         stream_name: Optional[str] = None,
         from_end: bool = False,
         commit_position: Optional[int] = None,
         stream_position: Optional[int] = None,
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         consumer_strategy: ConsumerStrategy = "DispatchToSingle",
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         request = self._construct_create_req(
             group_name=group_name,
             stream_name=stream_name,
             from_end=from_end,
             commit_position=commit_position,
             stream_position=stream_position,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
+            window_size=window_size,
+            checkpoint_interval_multiplier=checkpoint_interval_multiplier,
             consumer_strategy=consumer_strategy,
         )
         # Call 'Create' RPC.
         try:
             response = self._stub.Create(
                 request,
                 timeout=timeout,
```

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/cluster_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/cluster_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/cluster_pb2_grpc.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/code_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/code_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/gossip_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/gossip_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/gossip_pb2_grpc.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/persistent_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/persistent_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/persistent_pb2_grpc.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/shared_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/shared_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/status_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/status_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/streams_pb2.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/streams_pb2.pyi` & `esdbclient-1.0a7/esdbclient/protos/Grpc/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/protos/Grpc/streams_pb2_grpc.py` & `esdbclient-1.0a7/esdbclient/protos/Grpc/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.0a6/esdbclient/streams.py` & `esdbclient-1.0a7/esdbclient/streams.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 # -*- coding: utf-8 -*-
 import sys
 from abc import abstractmethod
+from asyncio import CancelledError
 from dataclasses import dataclass
+from enum import Enum
 from typing import (
-    AsyncIterable,
+    AsyncIterator,
     Iterable,
     Iterator,
     Optional,
     Sequence,
     Union,
     overload,
 )
 from uuid import UUID, uuid4
 
 import grpc
 import grpc.aio
 from google.protobuf import duration_pb2, empty_pb2
 from typing_extensions import Literal, Protocol, runtime_checkable
 
-from esdbclient.esdbapibase import ESDBService, Metadata, handle_rpc_error
-from esdbclient.events import NewEvent, RecordedEvent
+from esdbclient.connection_spec import ConnectionSpec
+from esdbclient.esdbapibase import (
+    DEFAULT_BATCH_APPEND_REQUEST_DEADLINE,
+    DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
+    DEFAULT_WINDOW_SIZE,
+    ESDBService,
+    Metadata,
+    handle_rpc_error,
+)
+from esdbclient.events import Checkpoint, NewEvent, RecordedEvent
 from esdbclient.exceptions import (
     AccessDeniedError,
     BadRequestError,
     CancelledByClient,
-    ESDBClientException,
+    EventStoreDBClientException,
     InvalidTransactionError,
     MaximumAppendSizeExceededError,
     NotFound,
     StreamIsDeleted,
     SubscriptionConfirmationError,
     TimeoutError,
     UnknownError,
@@ -40,200 +50,228 @@
 @runtime_checkable
 class _ReadResps(Iterator[streams_pb2.ReadResp], Protocol):
     @abstractmethod
     def cancel(self) -> None:
         ...  # pragma: no cover
 
 
-class AsyncioReadResponse:
+class StreamState(Enum):
+    ANY = "ANY"
+    NO_STREAM = "NO_STREAM"
+    EXISTS = "EXISTS"
+
+
+class BaseReadResponse:
     def __init__(
         self,
-        read_resp_iter: AsyncIterable[streams_pb2.ReadResp],
         stream_name: Optional[str],
-        is_subscription: bool,
     ):
-        self.read_resp_iter = read_resp_iter.__aiter__()
         self.stream_name = stream_name
-        self.subscription_id: Optional[UUID] = None
-        self.is_subscription = is_subscription
+
+    def handle_stream_read_rpc_error(
+        self, e: grpc.RpcError
+    ) -> EventStoreDBClientException:
+        if e.code() == grpc.StatusCode.FAILED_PRECONDITION:
+            details = e.details() or ""
+            if self.stream_name and details and "is deleted" in details:
+                return StreamIsDeleted()
+            else:  # pragma: no cover
+                return handle_rpc_error(e)
+        else:
+            return handle_rpc_error(e)
+
+    def _convert_read_resp(
+        self, read_resp: streams_pb2.ReadResp
+    ) -> Optional[RecordedEvent]:
+        content_oneof = read_resp.WhichOneof("content")
+        if content_oneof == "stream_not_found":
+            raise NotFound(f"Stream {self.stream_name!r} not found")
+        elif content_oneof == "event":
+            read_event = read_resp.event
+            assert isinstance(read_event, streams_pb2.ReadResp.ReadEvent)
+            recorded_event = read_event.event
+            assert isinstance(
+                recorded_event, streams_pb2.ReadResp.ReadEvent.RecordedEvent
+            )
+            # There's also read_event.link...
+            position_oneof = read_event.WhichOneof("position")
+            if position_oneof == "commit_position":
+                commit_position = read_event.commit_position
+            else:  # pragma: no cover
+                # We only get here with EventStoreDB < 22.10.
+                assert position_oneof == "no_position", position_oneof
+                commit_position = None
+
+            # print("Recorded event commit position:", commit_position)
+            return RecordedEvent(
+                id=UUID(read_event.event.id.string),
+                type=recorded_event.metadata["type"],
+                data=recorded_event.data,
+                content_type=recorded_event.metadata["content-type"],
+                metadata=recorded_event.custom_metadata,
+                stream_name=recorded_event.stream_identifier.stream_name.decode("utf8"),
+                stream_position=recorded_event.stream_revision,
+                commit_position=commit_position,
+            )
+        elif content_oneof == "checkpoint":
+            checkpoint = read_resp.checkpoint
+            # print("Checkpoint commit position:", checkpoint.commit_position)
+            return Checkpoint(
+                commit_position=checkpoint.commit_position,
+            )
+        else:  # pragma: no cover
+            return None
+            # Todo: Maybe support other content_oneof values:
+            # 		uint64 first_stream_position = 5;
+            # 		uint64 last_stream_position = 6;
+            # 		AllStreamPosition last_all_stream_position = 7;
+            #
+            # Todo: Not sure how to request to get first_stream_position,
+            #   last_stream_position, first_all_stream_position.
+
+
+class AsyncioReadResponse(AsyncIterator[RecordedEvent], BaseReadResponse):
+    def __init__(
+        self,
+        aio_call: grpc.aio.UnaryStreamCall[streams_pb2.ReadReq, streams_pb2.ReadResp],
+        stream_name: Optional[str],
+    ):
+        super().__init__(stream_name=stream_name)
+        self.aio_call = aio_call
+        self.read_resp_iter = aio_call.__aiter__()
+
+    def __aiter__(self) -> AsyncIterator[RecordedEvent]:
+        return self
+
+    async def __anext__(self) -> RecordedEvent:
+        while True:
+            try:
+                read_resp = await self._get_next_read_resp()
+            except CancelledByClient as e:
+                raise StopAsyncIteration() from e
+            else:
+                recorded_event = self._convert_read_resp(read_resp)
+                if recorded_event is not None:
+                    return recorded_event
+                else:  # pragma: no cover
+                    pass
 
     async def _get_next_read_resp(self) -> streams_pb2.ReadResp:
         try:
             read_resp = await self.read_resp_iter.__anext__()
         except grpc.RpcError as e:
-            if e.code() == grpc.StatusCode.FAILED_PRECONDITION:
-                details = e.details() or ""
-                if self.stream_name and details and "is deleted" in details:
-                    raise StreamIsDeleted() from e
-                else:  # pragma: no cover
-                    raise handle_rpc_error(e) from e
-            else:
-                raise handle_rpc_error(e) from e
-        assert isinstance(read_resp, streams_pb2.ReadResp)
-        return read_resp
+            raise self.handle_stream_read_rpc_error(e) from e
+        except CancelledError as e:
+            raise CancelledByClient() from e
+        else:
+            assert isinstance(read_resp, streams_pb2.ReadResp)
+            return read_resp
 
-    async def check_confirmation(self) -> None:
-        if self.is_subscription:
-            read_resp = await self._get_next_read_resp()
-            content_oneof = read_resp.WhichOneof("content")
-            if content_oneof != "confirmation":  # pragma: no cover
-                raise SubscriptionConfirmationError(
-                    f"Expected subscription confirmation, got: {read_resp}"
-                )
+    def stop(self) -> None:
+        self.aio_call.cancel()
 
-    def __aiter__(self) -> "AsyncioReadResponse":
-        return self
+
+class AsyncioCatchupSubscription(AsyncioReadResponse):
+    def __init__(
+        self,
+        aio_call: grpc.aio.UnaryStreamCall[streams_pb2.ReadReq, streams_pb2.ReadResp],
+        stream_name: Optional[str],
+        include_checkpoints: bool = False,
+    ):
+        super().__init__(aio_call=aio_call, stream_name=stream_name)
+        self.include_checkpoints = include_checkpoints
+
+    async def check_confirmation(self) -> None:
+        read_resp = await self._get_next_read_resp()
+        content_oneof = read_resp.WhichOneof("content")
+        if content_oneof != "confirmation":  # pragma: no cover
+            raise SubscriptionConfirmationError(
+                f"Expected subscription confirmation, got: {read_resp}"
+            )
 
     async def __anext__(self) -> RecordedEvent:
         while True:
-            read_resp = await self._get_next_read_resp()
-            content_oneof = read_resp.WhichOneof("content")
-            if content_oneof == "event":
-                event = read_resp.event.event
-                position_oneof = read_resp.event.WhichOneof("position")
-                if position_oneof == "commit_position":
-                    commit_position = read_resp.event.commit_position
-                else:  # pragma: no cover
-                    # We only get here with EventStoreDB < 22.10.
-                    assert position_oneof == "no_position", position_oneof
-                    commit_position = None
-
-                return RecordedEvent(
-                    id=UUID(event.id.string),
-                    type=event.metadata["type"],
-                    data=event.data,
-                    content_type=event.metadata["content-type"],
-                    metadata=event.custom_metadata,
-                    stream_name=event.stream_identifier.stream_name.decode("utf8"),
-                    stream_position=event.stream_revision,
-                    commit_position=commit_position,
-                )
-            elif content_oneof == "stream_not_found":
-                raise NotFound(f"Stream {self.stream_name!r} not found")
-            else:
-                pass  # pragma: no cover
-                # Todo: Maybe support other content_oneof values:
-                #   oneof content {
-                # 		ReadEvent event = 1;
-                # 		SubscriptionConfirmation confirmation = 2;
-                # 		Checkpoint checkpoint = 3;
-                # 		StreamNotFound stream_not_found = 4;
-                # 		uint64 first_stream_position = 5;
-                # 		uint64 last_stream_position = 6;
-                # 		AllStreamPosition last_all_stream_position = 7;
-                # 	}
-                #
-                # Todo: Not sure how to request to get first_stream_position,
-                #   last_stream_position, first_all_stream_position.
+            recorded_event = await super().__anext__()
+            if self.include_checkpoints or not isinstance(recorded_event, Checkpoint):
+                return recorded_event
 
 
-class ReadResponse(Iterator[RecordedEvent]):
+class ReadResponse(Iterator[RecordedEvent], BaseReadResponse):
     def __init__(
         self,
         read_resps: _ReadResps,
         stream_name: Optional[str],
     ):
+        super().__init__(stream_name=stream_name)
         self.read_resps = read_resps
-        self.stream_name = stream_name
 
     def __iter__(self) -> "ReadResponse":
         return self
 
     def __next__(self) -> RecordedEvent:
         while True:
             try:
                 read_resp = self._get_next_read_resp()
             except CancelledByClient as e:
                 raise StopIteration() from e
-            content_oneof = read_resp.WhichOneof("content")
-            if content_oneof == "event":
-                event = read_resp.event.event
-                position_oneof = read_resp.event.WhichOneof("position")
-                if position_oneof == "commit_position":
-                    commit_position = read_resp.event.commit_position
-                else:  # pragma: no cover
-                    # We only get here with EventStoreDB < 22.10.
-                    assert position_oneof == "no_position", position_oneof
-                    commit_position = None
-
-                return RecordedEvent(
-                    id=UUID(event.id.string),
-                    type=event.metadata["type"],
-                    data=event.data,
-                    content_type=event.metadata["content-type"],
-                    metadata=event.custom_metadata,
-                    stream_name=event.stream_identifier.stream_name.decode("utf8"),
-                    stream_position=event.stream_revision,
-                    commit_position=commit_position,
-                )
-            elif content_oneof == "stream_not_found":
-                raise NotFound(f"Stream {self.stream_name!r} not found")
             else:
-                pass  # pragma: no cover
-                # Todo: Maybe support other content_oneof values:
-                #   oneof content {
-                # 		ReadEvent event = 1;
-                # 		SubscriptionConfirmation confirmation = 2;
-                # 		Checkpoint checkpoint = 3;
-                # 		StreamNotFound stream_not_found = 4;
-                # 		uint64 first_stream_position = 5;
-                # 		uint64 last_stream_position = 6;
-                # 		AllStreamPosition last_all_stream_position = 7;
-                # 	}
-                #
-                # Todo: Not sure how to request to get first_stream_position,
-                #   last_stream_position, first_all_stream_position.
+                recorded_event = self._convert_read_resp(read_resp)
+                if recorded_event is not None:
+                    return recorded_event
+                else:  # pragma: no cover
+                    pass
 
     def _get_next_read_resp(self) -> streams_pb2.ReadResp:
         try:
             read_resp = next(self.read_resps)
         except grpc.RpcError as e:
-            if e.code() == grpc.StatusCode.FAILED_PRECONDITION:
-                details = e.details() or ""
-                if self.stream_name and details and "is deleted" in details:
-                    raise StreamIsDeleted() from e
-                else:  # pragma: no cover
-                    raise handle_rpc_error(e) from e
-            else:
-                raise handle_rpc_error(e) from e
-        assert isinstance(read_resp, streams_pb2.ReadResp)
-        return read_resp
+            raise self.handle_stream_read_rpc_error(e) from e
+        else:
+            assert isinstance(read_resp, streams_pb2.ReadResp)
+            return read_resp
 
     def stop(self) -> None:
         self.read_resps.cancel()
 
     def __del__(self) -> None:
         self.stop()
+        del self
 
 
 class CatchupSubscription(ReadResponse):
     def __init__(
         self,
         read_resps: _ReadResps,
         stream_name: Optional[str],
+        include_checkpoints: bool = False,
     ):
         super().__init__(read_resps=read_resps, stream_name=stream_name)
         self.subscription_id: Optional[UUID] = None
+        self.include_checkpoints = include_checkpoints
         first_read_resp = self._get_next_read_resp()
         content_oneof = first_read_resp.WhichOneof("content")
         if content_oneof == "confirmation":
             pass
             # Todo: What is '.confirmation.subscription_id' for?
         else:  # pragma: no cover
             raise SubscriptionConfirmationError(
                 f"Expected subscription confirmation, got: {first_read_resp}"
             )
 
+    def __next__(self) -> RecordedEvent:
+        while True:
+            recorded_event = super().__next__()
+            if self.include_checkpoints or not isinstance(recorded_event, Checkpoint):
+                return recorded_event
 
-DEFAULT_BATCH_APPEND_REQUEST_DEADLINE = 315576000000
 
 # @dataclass
 # class BatchAppendRequest:
 #     stream_name: str
-#     current_version: Optional[int]
+#     current_version: Union[int, StreamState]
 #     events: Iterable[NewEvent]
 #     correlation_id: UUID = field(default_factory=uuid4)
 #     deadline: int = DEFAULT_BATCH_APPEND_REQUEST_DEADLINE
 
 
 # if TYPE_CHECKING:  # pragma: no cover
 #
@@ -275,138 +313,64 @@
 #         return _construct_batch_append_req(batch)
 #
 #     def pop_future(self, correlation_id: UUID) -> BatchAppendFuture:
 #         return self.futures_by_correlation_id.pop(correlation_id)
 
 
 class BaseStreamsService(ESDBService):
-    def __init__(self, channel: Union[grpc.Channel, grpc.aio.Channel]):
+    def __init__(
+        self,
+        channel: Union[grpc.Channel, grpc.aio.Channel],
+        connection_spec: ConnectionSpec,
+    ):
+        super().__init__(connection_spec=connection_spec)
         self._stub = streams_pb2_grpc.StreamsStub(channel)
 
     @staticmethod
-    def _construct_read_request(
-        stream_name: Optional[str] = None,
-        stream_position: Optional[int] = None,
-        commit_position: Optional[int] = None,
-        backwards: bool = False,
-        filter_exclude: Sequence[str] = (),
-        filter_include: Sequence[str] = (),
-        filter_by_stream_name: bool = False,
-        limit: int = sys.maxsize,
-        subscribe: bool = False,
-    ) -> streams_pb2.ReadReq:
-        # Construct ReadReq.Options.
-        options = streams_pb2.ReadReq.Options()
-
-        # Decide 'stream_option'.
-        if isinstance(stream_name, str):
-            assert isinstance(stream_name, str)
-            assert commit_position is None
-            stream_options = streams_pb2.ReadReq.Options.StreamOptions(
-                stream_identifier=shared_pb2.StreamIdentifier(
-                    stream_name=stream_name.encode("utf8")
-                ),
-                revision=stream_position or 0,
+    def _generate_append_reqs(
+        stream_name: str,
+        current_version: Union[int, StreamState],
+        events: Iterable[NewEvent],
+    ) -> Iterator[streams_pb2.AppendReq]:
+        # First, define append request that has 'content' as 'options'.
+        options = streams_pb2.AppendReq.Options(
+            stream_identifier=shared_pb2.StreamIdentifier(
+                stream_name=stream_name.encode("utf8")
             )
-
-            # Decide 'revision_option'.
-            if stream_position is not None:
-                stream_options.revision = stream_position
-            elif backwards is False:
-                stream_options.start.CopyFrom(shared_pb2.Empty())
-            else:
-                stream_options.end.CopyFrom(shared_pb2.Empty())
-            options.stream.CopyFrom(stream_options)
-        else:
-            assert stream_position is None
-            if commit_position is not None:
-                all_options = streams_pb2.ReadReq.Options.AllOptions(
-                    position=streams_pb2.ReadReq.Options.Position(
-                        commit_position=commit_position,
-                        prepare_position=commit_position,
-                    )
-                )
-            elif backwards:
-                all_options = streams_pb2.ReadReq.Options.AllOptions(
-                    end=shared_pb2.Empty()
-                )
-            else:
-                all_options = streams_pb2.ReadReq.Options.AllOptions(
-                    start=shared_pb2.Empty()
-                )
-            options.all.CopyFrom(all_options)
-
-        # Decide 'read_direction'.
-        if backwards is False:
-            options.read_direction = streams_pb2.ReadReq.Options.Forwards
-        else:
-            options.read_direction = streams_pb2.ReadReq.Options.Backwards
-
-        # Decide 'resolve_links'.
-        options.resolve_links = False
-
-        # Decide 'count_option'.
-        if subscribe:
-            subscription = streams_pb2.ReadReq.Options.SubscriptionOptions()
-            options.subscription.CopyFrom(subscription)
-
+        )
+        # Decide 'expected_stream_revision'.
+        if isinstance(current_version, int):
+            assert current_version >= 0
+            options.revision = current_version
         else:
-            options.count = limit
-
-        # Decide 'filter_option'.
-        if filter_exclude or filter_include:
-            if filter_include:
-                filter_include = (
-                    [filter_include]
-                    if isinstance(filter_include, str)
-                    else filter_include
-                )
-                filter_regex = "^" + "|".join(filter_include) + "$"
+            assert isinstance(current_version, StreamState)
+            if current_version is StreamState.EXISTS:
+                options.stream_exists.CopyFrom(shared_pb2.Empty())
+            elif current_version is StreamState.ANY:
+                options.any.CopyFrom(shared_pb2.Empty())
             else:
-                filter_exclude = (
-                    [filter_exclude]
-                    if isinstance(filter_exclude, str)
-                    else filter_exclude
-                )
-                filter_regex = "^(?!(" + "|".join(filter_exclude) + ")).*$"
+                assert current_version is StreamState.NO_STREAM
+                options.no_stream.CopyFrom(shared_pb2.Empty())
 
-            filter_expression = streams_pb2.ReadReq.Options.FilterOptions.Expression(
-                regex=filter_regex
-            )
-            if filter_by_stream_name:
-                stream_identifier_filter = filter_expression
-                event_type_filter = None
-            else:
-                stream_identifier_filter = None
-                event_type_filter = filter_expression
+        yield streams_pb2.AppendReq(options=options)
 
-            filter_options = streams_pb2.ReadReq.Options.FilterOptions(
-                stream_identifier=stream_identifier_filter,
-                event_type=event_type_filter,
-                # Todo: What does 'window' mean?
-                # max=shared_pb2.Empty(),
-                count=shared_pb2.Empty(),
-                # Todo: What does 'checkpointIntervalMultiplier' mean?
-                checkpointIntervalMultiplier=5,
+        # Secondly, define append requests that has 'content' as 'proposed_message'.
+        for event in events:
+            proposed_message = streams_pb2.AppendReq.ProposedMessage(
+                id=shared_pb2.UUID(string=str(event.id)),
+                metadata={"type": event.type, "content-type": event.content_type},
+                custom_metadata=event.metadata,
+                data=event.data,
             )
-            options.filter.CopyFrom(filter_options)
-        else:
-            options.no_filter.CopyFrom(shared_pb2.Empty())
-
-        # Decide 'uuid_option'.
-        options.uuid_option.CopyFrom(
-            streams_pb2.ReadReq.Options.UUIDOption(string=shared_pb2.Empty())
-        )
-
-        return streams_pb2.ReadReq(options=options)
+            yield streams_pb2.AppendReq(proposed_message=proposed_message)
 
     @staticmethod
     def _construct_batch_append_req(
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         events: Iterable[NewEvent],
         deadline: int,
         correlation_id: UUID,
     ) -> streams_pb2.BatchAppendReq:
         # Construct batch request 'options'.
         options = streams_pb2.BatchAppendReq.Options(
             stream_identifier=shared_pb2.StreamIdentifier(
@@ -415,23 +379,26 @@
             deadline=duration_pb2.Duration(
                 seconds=deadline,
                 nanos=0,
             ),
         )
         # Decide options 'expected_stream_revision'.
         if isinstance(current_version, int):
-            if current_version >= 0:
-                # Stream is expected to exist.
-                options.stream_position = current_version
-            else:
-                # Disable optimistic concurrency control.
-                options.any.CopyFrom(empty_pb2.Empty())
+            assert current_version >= 0
+            options.stream_position = current_version
         else:
-            # Stream is expected not to exist.
-            options.no_stream.CopyFrom(empty_pb2.Empty())
+            assert isinstance(current_version, StreamState)
+            if current_version is StreamState.EXISTS:
+                options.stream_exists.CopyFrom(empty_pb2.Empty())
+            elif current_version is StreamState.ANY:
+                options.any.CopyFrom(empty_pb2.Empty())
+            else:
+                assert current_version is StreamState.NO_STREAM
+                options.no_stream.CopyFrom(empty_pb2.Empty())
+
         # Construct batch request 'proposed_messages'.
         # Todo: Split batch.events into chunks of 20?
         proposed_messages = []
         for event in events:
             proposed_message = streams_pb2.BatchAppendReq.ProposedMessage(
                 id=shared_pb2.UUID(string=str(event.id)),
                 metadata={"type": event.type, "content-type": event.content_type},
@@ -445,16 +412,16 @@
             proposed_messages=proposed_messages,
             is_final=True,  # This specifies the end of an atomic transaction.
         )
 
     @staticmethod
     def _convert_batch_append_resp(
         response: streams_pb2.BatchAppendResp, stream_name: str
-    ) -> Union[BatchAppendResponse, ESDBClientException]:
-        result: Union[BatchAppendResponse, ESDBClientException]
+    ) -> Union[BatchAppendResponse, EventStoreDBClientException]:
+        result: Union[BatchAppendResponse, EventStoreDBClientException]
         # Response 'result' is either 'success' or 'error'.
         result_oneof = response.WhichOneof("result")
         if result_oneof == "success":
             # Construct response object.
             result = BatchAppendResponse(
                 commit_position=response.success.position.commit_position,
             )
@@ -504,67 +471,191 @@
                 result = MaximumAppendSizeExceededError(f"Max size is {size}")
             elif error_details.Is(shared_pb2.BadRequest.DESCRIPTOR):  # pragma: no cover
                 bad_request = shared_pb2.BadRequest()
                 error_details.Unpack(bad_request)
                 result = BadRequestError(f"Bad request: {bad_request.message}")
             else:
                 # Unexpected error details type.
-                result = ESDBClientException(error_details)  # pragma: no cover
+                result = EventStoreDBClientException(error_details)  # pragma: no cover
         return result
 
     @staticmethod
+    def _construct_read_request(
+        stream_name: Optional[str] = None,
+        stream_position: Optional[int] = None,
+        commit_position: Optional[int] = None,
+        backwards: bool = False,
+        filter_exclude: Sequence[str] = (),
+        filter_include: Sequence[str] = (),
+        filter_by_stream_name: bool = False,
+        limit: int = sys.maxsize,
+        subscribe: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
+    ) -> streams_pb2.ReadReq:
+        # Construct ReadReq.Options.
+        options = streams_pb2.ReadReq.Options()
+
+        # Decide 'stream_option'.
+        if isinstance(stream_name, str):
+            assert isinstance(stream_name, str)
+            assert commit_position is None
+            stream_options = streams_pb2.ReadReq.Options.StreamOptions(
+                stream_identifier=shared_pb2.StreamIdentifier(
+                    stream_name=stream_name.encode("utf8")
+                ),
+                revision=stream_position or 0,
+            )
+
+            # Decide 'revision_option'.
+            if stream_position is not None:
+                stream_options.revision = stream_position
+            elif backwards is False:
+                stream_options.start.CopyFrom(shared_pb2.Empty())
+            else:
+                stream_options.end.CopyFrom(shared_pb2.Empty())
+            options.stream.CopyFrom(stream_options)
+        else:
+            assert stream_position is None
+            if commit_position is not None:
+                all_options = streams_pb2.ReadReq.Options.AllOptions(
+                    position=streams_pb2.ReadReq.Options.Position(
+                        commit_position=commit_position,
+                        prepare_position=commit_position,
+                    )
+                )
+            elif backwards:
+                all_options = streams_pb2.ReadReq.Options.AllOptions(
+                    end=shared_pb2.Empty()
+                )
+            else:
+                all_options = streams_pb2.ReadReq.Options.AllOptions(
+                    start=shared_pb2.Empty()
+                )
+            options.all.CopyFrom(all_options)
+
+        # Decide 'read_direction'.
+        if backwards is False:
+            options.read_direction = streams_pb2.ReadReq.Options.Forwards
+        else:
+            options.read_direction = streams_pb2.ReadReq.Options.Backwards
+
+        # Decide 'resolve_links'.
+        options.resolve_links = False
+
+        # Decide 'count_option'.
+        if subscribe:
+            subscription = streams_pb2.ReadReq.Options.SubscriptionOptions()
+            options.subscription.CopyFrom(subscription)
+
+        else:
+            options.count = limit
+
+        # Decide 'filter_option'.
+        if filter_exclude or filter_include:
+            filter_options = streams_pb2.ReadReq.Options.FilterOptions(
+                max=window_size,
+                checkpointIntervalMultiplier=checkpoint_interval_multiplier,
+            )
+
+            # Decide 'filter'
+            if filter_include:
+                filter_include = (
+                    [filter_include]
+                    if isinstance(filter_include, str)
+                    else filter_include
+                )
+                filter_regex = "^" + "|".join(filter_include) + "$"
+            else:
+                filter_exclude = (
+                    [filter_exclude]
+                    if isinstance(filter_exclude, str)
+                    else filter_exclude
+                )
+                filter_regex = "^(?!(" + "|".join(filter_exclude) + ")).*$"
+
+            filter_expression = streams_pb2.ReadReq.Options.FilterOptions.Expression(
+                regex=filter_regex
+            )
+
+            if filter_by_stream_name:
+                filter_options.stream_identifier.CopyFrom(filter_expression)
+            else:
+                filter_options.event_type.CopyFrom(filter_expression)
+
+            options.filter.CopyFrom(filter_options)
+        else:
+            options.no_filter.CopyFrom(shared_pb2.Empty())
+
+        # Decide 'uuid_option'.
+        options.uuid_option.CopyFrom(
+            streams_pb2.ReadReq.Options.UUIDOption(string=shared_pb2.Empty())
+        )
+
+        # Decide 'control_option'.
+        # Todo: What does this do, and what value should it have?
+
+        return streams_pb2.ReadReq(options=options)
+
+    @staticmethod
     def _construct_delete_req(
-        stream_name: str, current_version: Optional[int]
+        stream_name: str, current_version: Union[int, StreamState]
     ) -> streams_pb2.DeleteReq:
         options = streams_pb2.DeleteReq.Options(
             stream_identifier=shared_pb2.StreamIdentifier(
                 stream_name=stream_name.encode("utf8")
             )
         )
         # Decide 'expected_stream_revision'.
         if isinstance(current_version, int):
-            if current_version >= 0:
-                # Stream position is expected to be a certain value.
-                options.revision = current_version
-            else:
-                # Disable optimistic concurrency control.
-                options.any.CopyFrom(shared_pb2.Empty())
+            assert current_version >= 0
+            options.revision = current_version
         else:
-            # Stream is expected to exist.
-            options.stream_exists.CopyFrom(shared_pb2.Empty())
+            assert isinstance(current_version, StreamState)
+            if current_version is StreamState.EXISTS:
+                options.stream_exists.CopyFrom(shared_pb2.Empty())
+            elif current_version is StreamState.ANY:
+                options.any.CopyFrom(shared_pb2.Empty())
+            else:
+                assert current_version is StreamState.NO_STREAM
+                options.no_stream.CopyFrom(shared_pb2.Empty())
+
         return streams_pb2.DeleteReq(options=options)
 
     @staticmethod
     def _construct_tombstone_req(
-        stream_name: str, current_version: Optional[int]
+        stream_name: str, current_version: Union[int, StreamState]
     ) -> streams_pb2.TombstoneReq:
         options = streams_pb2.TombstoneReq.Options(
             stream_identifier=shared_pb2.StreamIdentifier(
                 stream_name=stream_name.encode("utf8")
             )
         )
         # Decide 'expected_stream_revision'.
         if isinstance(current_version, int):
-            if current_version >= 0:
-                # Stream position is expected to be a certain value.
-                options.revision = current_version
-            else:
-                # Disable optimistic concurrency control.
-                options.any.CopyFrom(shared_pb2.Empty())
+            assert current_version >= 0
+            # Stream position is expected to be a certain value.
+            options.revision = current_version
         else:
-            # Stream is expected to exist.
-            options.stream_exists.CopyFrom(shared_pb2.Empty())
+            assert isinstance(current_version, StreamState)
+            if current_version is StreamState.EXISTS:
+                options.stream_exists.CopyFrom(shared_pb2.Empty())
+            elif current_version is StreamState.ANY:
+                options.any.CopyFrom(shared_pb2.Empty())
+            else:
+                assert current_version is StreamState.NO_STREAM
+                options.no_stream.CopyFrom(shared_pb2.Empty())
         return streams_pb2.TombstoneReq(options=options)
 
 
 class AsyncioStreamsService(BaseStreamsService):
     async def batch_append(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         events: Iterable[NewEvent],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> BatchAppendResponse:
         # Call the gRPC method.
         try:
@@ -582,18 +673,18 @@
                 credentials=credentials,
             ):
                 assert isinstance(response, streams_pb2.BatchAppendResp)
                 result = self._convert_batch_append_resp(response, stream_name)
                 if isinstance(result, BatchAppendResponse):
                     return result
                 else:
-                    assert isinstance(result, ESDBClientException)
+                    assert isinstance(result, EventStoreDBClientException)
                     raise result
             else:  # pragma: no cover
-                raise ESDBClientException("Batch append response not received")
+                raise EventStoreDBClientException("Batch append response not received")
 
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from e
 
     @overload
     async def read(
         self,
@@ -601,30 +692,30 @@
         stream_name: Optional[str] = None,
         stream_position: Optional[int] = None,
         backwards: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioReadResponse:
         """
         Signature for reading events from a stream.
         """
 
     @overload
     async def read(
         self,
         *,
         stream_name: Optional[str] = None,
         stream_position: Optional[int] = None,
         subscribe: Literal[True],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioCatchupSubscription:
         """
         Signature for reading events from a stream with a catch-up subscription.
         """
 
     @overload
     async def read(
         self,
@@ -634,32 +725,35 @@
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         limit: int = sys.maxsize,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioReadResponse:
         """
         Signature for reading all events.
         """
 
     @overload
     async def read(
         self,
         *,
         commit_position: Optional[int] = None,
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         subscribe: Literal[True],
+        include_checkpoints: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> AsyncioCatchupSubscription:
         """
         Signature for reading all events with a catch-up subscription.
         """
 
     async def read(
         self,
         *,
@@ -668,18 +762,21 @@
         commit_position: Optional[int] = None,
         backwards: bool = False,
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         limit: int = sys.maxsize,
         subscribe: bool = False,
+        include_checkpoints: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> AsyncIterable[RecordedEvent]:
+    ) -> Union[AsyncioReadResponse, AsyncioCatchupSubscription]:
         """
         Constructs and sends a gRPC 'ReadReq' to the 'Read' rpc.
 
         Returns a generator which yields RecordedEvent objects.
         """
 
         # Construct read request.
@@ -689,34 +786,46 @@
             commit_position=commit_position,
             backwards=backwards,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
             limit=limit,
             subscribe=subscribe,
+            window_size=window_size,
+            checkpoint_interval_multiplier=checkpoint_interval_multiplier,
         )
 
         # Send the read request, and iterate over the response.
-        unary_stream_call: AsyncIterable[streams_pb2.ReadResp] = self._stub.Read(
+        unary_stream_call: grpc.aio.UnaryStreamCall[
+            streams_pb2.ReadReq, streams_pb2.ReadResp
+        ] = self._stub.Read(
             read_req,
             timeout=timeout,
             metadata=self._metadata(metadata),
             credentials=credentials,
         )
 
-        response = AsyncioReadResponse(
-            unary_stream_call, stream_name=stream_name, is_subscription=subscribe
-        )
-        await response.check_confirmation()
+        if not subscribe:
+            response = AsyncioReadResponse(
+                aio_call=unary_stream_call,
+                stream_name=stream_name,
+            )
+        else:
+            response = AsyncioCatchupSubscription(
+                aio_call=unary_stream_call,
+                stream_name=stream_name,
+                include_checkpoints=include_checkpoints,
+            )
+            await response.check_confirmation()
         return response
 
     async def delete(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         delete_req = self._construct_delete_req(stream_name, current_version)
 
         try:
@@ -742,15 +851,15 @@
                 raise handle_rpc_error(e) from e
         else:
             assert isinstance(delete_resp, streams_pb2.DeleteResp), delete_resp
 
     async def tombstone(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         tombstone_req = self._construct_tombstone_req(stream_name, current_version)
 
         try:
@@ -837,14 +946,17 @@
         self,
         *,
         commit_position: Optional[int] = None,
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         subscribe: Literal[True],
+        include_checkpoints: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> CatchupSubscription:
         """
         Signature for reading all events with a catch-up subscription.
         """
@@ -857,14 +969,17 @@
         commit_position: Optional[int] = None,
         backwards: bool = False,
         filter_exclude: Sequence[str] = (),
         filter_include: Sequence[str] = (),
         filter_by_stream_name: bool = False,
         limit: int = sys.maxsize,
         subscribe: bool = False,
+        include_checkpoints: bool = False,
+        window_size: int = DEFAULT_WINDOW_SIZE,
+        checkpoint_interval_multiplier: int = DEFAULT_CHECKPOINT_INTERVAL_MULTIPLIER,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> Union[ReadResponse, CatchupSubscription]:
         """
         Constructs and sends a gRPC 'ReadReq' to the 'Read' rpc.
 
@@ -878,111 +993,82 @@
             commit_position=commit_position,
             backwards=backwards,
             filter_exclude=filter_exclude,
             filter_include=filter_include,
             filter_by_stream_name=filter_by_stream_name,
             limit=limit,
             subscribe=subscribe,
+            window_size=window_size,
+            checkpoint_interval_multiplier=checkpoint_interval_multiplier,
         )
 
         # Send the read request, and iterate over the response.
         read_resps = self._stub.Read(
             read_req,
             timeout=timeout,
             metadata=self._metadata(metadata),
             credentials=credentials,
         )
         assert isinstance(read_resps, _ReadResps)  # a _MultiThreadedRendezvous
 
         if subscribe is False:
             return ReadResponse(read_resps, stream_name=stream_name)
         else:
-            return CatchupSubscription(read_resps, stream_name=stream_name)
+            return CatchupSubscription(
+                read_resps,
+                stream_name=stream_name,
+                include_checkpoints=include_checkpoints,
+            )
 
     def append(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         events: Iterable[NewEvent],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> int:
         """
         Constructs and sends a stream of gRPC 'AppendReq' to the 'Append' rpc.
 
         Returns the commit position of the last appended event.
         """
         try:
-            response = self._stub.Append(
-                self._generate_append_requests(
-                    stream_name=stream_name,
-                    current_version=current_version,
-                    events=events,
-                ),
+            append_reqs = self._generate_append_reqs(
+                stream_name=stream_name,
+                current_version=current_version,
+                events=events,
+            )
+            append_resp = self._stub.Append(
+                append_reqs,
                 timeout=timeout,
                 metadata=self._metadata(metadata, requires_leader=True),
                 credentials=credentials,
             )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from e
         else:
-            assert isinstance(response, streams_pb2.AppendResp)
+            assert isinstance(append_resp, streams_pb2.AppendResp)
             # Response 'result' is either 'success' or 'wrong_expected_version'.
-            result_oneof = response.WhichOneof("result")
+            result_oneof = append_resp.WhichOneof("result")
             if result_oneof == "success":
-                return response.success.position.commit_position
+                return append_resp.success.position.commit_position
             else:
                 assert result_oneof == "wrong_expected_version", result_oneof
-                wev = response.wrong_expected_version
+                wev = append_resp.wrong_expected_version
                 cro_oneof = wev.WhichOneof("current_revision_option")
                 if cro_oneof == "current_revision":
                     raise WrongCurrentVersion(
-                        f"Current position is {wev.current_revision}"
+                        f"Current version is {wev.current_revision}"
                     )
                 else:
                     assert cro_oneof == "current_no_stream", cro_oneof
                     raise WrongCurrentVersion(f"Stream {stream_name!r} does not exist")
 
-    @staticmethod
-    def _generate_append_requests(
-        stream_name: str,
-        current_version: Optional[int],
-        events: Iterable[NewEvent],
-    ) -> Iterator[streams_pb2.AppendReq]:
-        # First, define append request that has 'content' as 'options'.
-        options = streams_pb2.AppendReq.Options(
-            stream_identifier=shared_pb2.StreamIdentifier(
-                stream_name=stream_name.encode("utf8")
-            )
-        )
-        # Decide 'expected_stream_revision'.
-        if isinstance(current_version, int):
-            if current_version >= 0:
-                # Stream is expected to exist.
-                options.revision = current_version
-            else:
-                # Disable optimistic concurrency control.
-                options.any.CopyFrom(shared_pb2.Empty())
-        else:
-            # Stream is expected not to exist.
-            options.no_stream.CopyFrom(shared_pb2.Empty())
-
-        yield streams_pb2.AppendReq(options=options)
-
-        # Secondly, define append requests that has 'content' as 'proposed_message'.
-        for event in events:
-            proposed_message = streams_pb2.AppendReq.ProposedMessage(
-                id=shared_pb2.UUID(string=str(event.id)),
-                metadata={"type": event.type, "content-type": event.content_type},
-                custom_metadata=event.metadata,
-                data=event.data,
-            )
-            yield streams_pb2.AppendReq(proposed_message=proposed_message)
-
     # def batch_append_multiplexed(
     #     self,
     #     futures_queue: BatchAppendFutureQueue,
     #     timeout: Optional[float] = None,
     #     metadata: Optional[Metadata] = None,
     #     credentials: Optional[grpc.CallCredentials] = None,
     # ) -> None:
@@ -1006,25 +1092,25 @@
     #             stream_name = future.batch_append_request.stream_name
     #             result = self._convert_batch_append_result(response, stream_name)
     #
     #             # Finish the future.
     #             if isinstance(result, BatchAppendResponse):
     #                 future.set_result(result)
     #             else:
-    #                 assert isinstance(result, ESDBClientException)
+    #                 assert isinstance(result, EventStoreDBClientException)
     #                 future.set_exception(result)
     #
     #         else:
     #             # The response stream ended without an RPC error.
     #             for (
     #                 correlation_id
     #             ) in requests.futures_by_correlation_id:  # pragma: no cover
     #                 future = requests.pop_future(correlation_id)
     #                 future.set_exception(
-    #                     ESDBClientException("Batch append response not received")
+    #                     EventStoreDBClientException("Batch append response not received")
     #                 )
     #
     #     except grpc.RpcError as rpc_error:
     #         # The response stream ended with an RPC error.
     #         try:
     #             raise handle_rpc_error(rpc_error) from rpc_error
     #         except GrpcError as grpc_error:
@@ -1034,15 +1120,15 @@
     #                 future = requests.pop_future(correlation_id)
     #                 future.set_exception(grpc_error)
     #             raise
 
     def batch_append(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         events: Iterable[NewEvent],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> BatchAppendResponse:
         # Call the gRPC method.
         try:
@@ -1060,26 +1146,26 @@
                 credentials=credentials,
             ):
                 assert isinstance(response, streams_pb2.BatchAppendResp)
                 result = self._convert_batch_append_resp(response, stream_name)
                 if isinstance(result, BatchAppendResponse):
                     return result
                 else:
-                    assert isinstance(result, ESDBClientException)
+                    assert isinstance(result, EventStoreDBClientException)
                     raise result
             else:  # pragma: no cover
-                raise ESDBClientException("Batch append response not received")
+                raise EventStoreDBClientException("Batch append response not received")
 
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from e
 
     def delete(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         delete_req = self._construct_delete_req(stream_name, current_version)
 
         try:
@@ -1110,15 +1196,15 @@
             #     return delete_resp.position
             # else:
             #     return delete_resp.no_position
 
     def tombstone(
         self,
         stream_name: str,
-        current_version: Optional[int],
+        current_version: Union[int, StreamState],
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         tombstone_req = self._construct_tombstone_req(stream_name, current_version)
 
         try:
```

### Comparing `esdbclient-1.0a6/pyproject.toml` & `esdbclient-1.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdbclient"
-version = "1.0a6"
+version = "1.0a7"
 description = "Python gRPC Client for EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `esdbclient-1.0a6/setup.py` & `esdbclient-1.0a7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['dnspython>=2.3.0,<3.0.0',
  'grpcio>=1.51.0,!=1.52.*',
  'protobuf>=3.11.0',
  'typing_extensions']
 
 setup_kwargs = {
     'name': 'esdbclient',
-    'version': '1.0a6',
+    'version': '1.0a7',
     'description': 'Python gRPC Client for EventStoreDB',
-    'long_description': '# Python gRPC Client for EventStoreDB\n\nThis [Python package](https://pypi.org/project/esdbclient/) provides a Python\ngRPC client for [EventStoreDB](https://www.eventstore.com/).\n\nThis client has been developed in collaboration with the EventStoreDB\nteam. Although not all the features of EventStoreDB are supported\nby this client, many of the most useful features are presented\nin an easy-to-use interface.\n\nThis client has been tested to work with EventStoreDB LTS versions 21.10,\nwithout and without SSL/TLS, and with Python versions 3.7 to 3.11. There\nis 100% test coverage. The code has typing annotations, checked with mypy.\nThe code is formatted with black and isort, and checked with flake8. Poetry\nis used for package management during development, and for building and\npublishing distributions to [PyPI](https://pypi.org/project/esdbclient/).\n\n## Synopsis\n\nThe `ESDBClient` class can be imported from the `esdbclient` package.\n\nProbably the three most useful methods of `ESDBClient` are:\n\n* `append_events()` This method can be used to record events in a particular\n"stream". This is useful for example when executing a command in an application\nthat mutates an aggregate. This method is "atomic" in that either all or none of\nthe events will be recorded.\n\n* `read_stream_events()` This method can be used to retrieve all the recorded\nevents in a "stream". This is useful for example when reconstructing an aggregate\nbefore executing a command in an application.\n\n* `subscribe_all_events()` This method can be used to receive all recorded\nevents across all "streams". This is useful in downstream event-processing\ncomponents, and supports processing events with "exactly-once" semantics (see below).\n\nThe example below uses an "insecure" EventStoreDB server running locally on port 2114.\n\n```python\nimport uuid\n\nfrom esdbclient import ESDBClient, NewEvent\n\n\n# Construct ESDBClient with an EventStoreDB URI.\n\nclient = ESDBClient(\n    uri="esdb://localhost:2114?Tls=false"\n)\n\n\n# Generate new events. Typically, domain events of different\n# types are generated in a domain model, and then serialized\n# into NewEvent objects. An aggregate ID may be used as the\n# name of a stream in EventStoreDB.\n\nstream_name1 = str(uuid.uuid4())\nevent1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'{"order_number": "123456"}\'\n)\nevent2 = NewEvent(\n    type=\'OrderSubmitted\',\n    data=b\'{}\'\n)\n\n\n# Append new events to a stream. The stream does not exist so\n# the "current version" is None. The value returned from the\n# append_events() method is the overall position in the database\n# of the last new event recorded by this operation. The returned\n# "commit position" value may be used in a user interface to poll\n# a downstream event-processing component before it presents an\n# up-to-date eventually consistent materialized view.\n\ncommit_position1 = client.append_events(\n    stream_name=stream_name1,\n    current_version=None,\n    events=[event1, event2],\n)\n\n# The "current version" is the "stream position" of the last\n# recorded event in a stream. Stream positions are zero-based.\n# We have recorded two new events, and so the "current version"\n# of this stream is 1. Concurrency is controlled in this way\n# to ensure the consistency of recorded events. An incorrect\n# value will cause a WrongCurrentVersion exception to be raised.\n\nevent3 = NewEvent(\n    type=\'OrderCancelled\',\n    data=b\'{}\'\n)\n\ncommit_position2 = client.append_events(\n    stream_name=stream_name1,\n    current_version=1,\n    events=[event3],\n)\n\n\n# Read events from a stream. The recorded events may be\n# deserialized to domain events objects of different types,\n# then used to reconstruct an aggregate in a domain model.\n\nrecorded = client.read_stream_events(\n    stream_name=stream_name1\n)\n\nassert len(recorded) == 3\n\nassert recorded[0].stream_name == stream_name1\nassert recorded[1].stream_name == stream_name1\nassert recorded[2].stream_name == stream_name1\n\nassert recorded[0].stream_position == 0\nassert recorded[1].stream_position == 1\nassert recorded[2].stream_position == 2\n\nassert recorded[0].type == "OrderCreated"\nassert recorded[1].type == "OrderSubmitted"\nassert recorded[2].type == "OrderCancelled"\n\nassert recorded[0].data == b\'{"order_number": "123456"}\'\n\n\n# Start a catch-up subscription to receive all recorded\n# events across all streams. A catch-up subscription may\n# be used in a downstream event-processing component to\n# receive recorded events from a particular commit position.\n# The first "commit position" in an EventStoreDB database is 0.\n\nlast_saved_commit_position = 0\n\ncatch_subscription = client.subscribe_all_events(\n    commit_position=last_saved_commit_position\n)\n\n\n# Iterate over the catch-up subscription. Process each\n# recorded event in turn. In an atomic database transaction\n# save the event\'s "commit position" with any new state\n# generated by processing the event. Use the component\'s\n# last saved "commit position" when restarting the subscription.\n\n\nreceived = []\nfor event in catch_subscription:\n    last_saved_commit_position = event.commit_position\n    received.append(event)\n\n    if last_saved_commit_position == commit_position2:\n        # Stop so we can continue with the example.\n        catch_subscription.stop()\n\n\nassert received[-3].type == "OrderCreated"\nassert received[-2].type == "OrderSubmitted"\nassert received[-1].type == "OrderCancelled"\n\n\n# Close the client after use.\n\nclient.close()\n```\n\nSee below for more details.\n\nFor an example of usage, see the [eventsourcing-eventstoredb](\nhttps://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.\n\n## Table of contents\n\n<!-- TOC -->\n* [Install package](#install-package)\n  * [From PyPI](#from-pypi)\n  * [With Poetry](#with-poetry)\n* [EventStoreDB server](#eventstoredb-server)\n  * [Run container](#run-container)\n  * [Stop container](#stop-container)\n* [EventStoreDB client](#eventstoredb-client)\n  * [Import class](#import-class)\n  * [Construct client](#construct-client)\n* [Connection strings](#connection-strings)\n  * [Two schemes](#two-schemes)\n  * [User info string](#user-info-string)\n  * [Query string](#query-string)\n  * [Examples](#examples)\n* [Event objects](#event-objects)\n  * [The NewEvent class](#the-newevent-class)\n  * [The RecordedEvent class](#the-recordedevent-class)\n* [Streams](#streams)\n  * [Append events](#append-events)\n  * [Append event](#append-event)\n  * [Idempotent append operations](#idempotent-append-operations)\n  * [Read stream events](#read-stream-events)\n  * [Get current version](#get-current-version)\n  * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)\n  * [Read all events](#read-all-events)\n  * [Get commit position](#get-commit-position)\n  * [Get stream metadata](#get-stream-metadata)\n  * [Set stream metadata](#set-stream-metadata)\n  * [Delete stream](#delete-stream)\n  * [Tombstone stream](#tombstone-stream)\n* [Catch-up subscriptions](#catch-up-subscriptions)\n  * [Subscribe all events](#subscribe-all-events)\n  * [Subscribe stream events](#subscribe-stream-events)\n  * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)\n* [Persistent subscriptions](#persistent-subscriptions)\n  * [Create subscription](#create-subscription)\n  * [Read subscription](#read-subscription)\n  * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)\n  * [Get subscription info](#get-subscription-info)\n  * [List subscriptions](#list-subscriptions)\n  * [Update subscription](#update-subscription)\n  * [Create stream subscription](#create-stream-subscription)\n  * [Read stream subscription](#read-stream-subscription)\n  * [Get stream subscription info](#get-stream-subscription-info)\n  * [List stream subscriptions](#list-stream-subscriptions)\n  * [Update stream subscription](#update-stream-subscription)\n  * [Replay parked events](#replay-parked-events)\n  * [Delete persistent subscription](#delete-persistent-subscription)\n* [Connection](#connection)\n  * [Reconnect](#reconnect)\n  * [Close](#close)\n* [Asyncio client](#asyncio-client)\n  * [Synopsis](#synopsis-1)\n* [Notes](#notes)\n  * [Regular expression filters](#regular-expression-filters)\n* [Contributors](#contributors)\n  * [Install Poetry](#install-poetry)\n  * [Setup for PyCharm users](#setup-for-pycharm-users)\n  * [Setup from command line](#setup-from-command-line)\n  * [Project Makefile commands](#project-makefile-commands)\n<!-- TOC -->\n\n## Install package\n\nIt is recommended to install Python packages into a Python virtual environment.\n\n### From PyPI\n\nYou can use pip to install this package directly from\n[the Python Package Index](https://pypi.org/project/esdbclient/).\n\n    $ pip install esdbclient\n\n### With Poetry\n\nYou can use Poetry to add this package to your pyproject.toml and install it.\n\n    $ poetry add esdbclient\n\n## EventStoreDB server\n\nThe EventStoreDB server can be run locally using the official Docker container image.\n\n### Run container\n\nFor development, you can run a "secure" EventStoreDB server using the following command.\n\n    $ docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:21.10.9-buster-slim --dev\n\nAs we will see, your client will need an EventStoreDB connection string URI as the value\nof its `uri` constructor argument. The connection string for this "secure" EventStoreDB\nserver would be:\n\n    esdb://admin:changeit@localhost:2113\n\nTo connect to a "secure" server, you will usually need to include a "username"\nand a "password" in the connection string, so that the server can authenticate the\nclient. With EventStoreDB, the default username is "admin" and the default password\nis "changeit".\n\nWhen connecting to a "secure" server, your client will also need an SSL/TLS certificate\nas the value of its `root_certificates` constructor argument. The client uses the\nSSL/TLS certificate to authenticate the server. For development, you can either use the\nSSL/TLS certificate of the certificate authority used to create the server\'s certificate,\nor when using a single-node cluster, you can use the server certificate itself. You can\nget the server certificate with the following Python code.\n\n\n```python\nimport ssl\n\nserver_certificate = ssl.get_server_certificate(addr=(\'localhost\', 2113))\n```\n\nYou can also start an "insecure" server using the following command.\n\n    $ docker run -d --name eventstoredb-insecure -it -p 2114:2113 eventstore/eventstore:21.10.9-buster-slim --insecure\n\nThe connection string URI for this "insecure" server would be:\n\n    esdb://localhost:2114?Tls=false\n\nAs we will see, when connecting to an "insecure" server, there is no need to include\na "username" and a "password" in the connection string. If you do, these values will\nbe ignored by the client, so that they are not sent over an insecure channel.\n\nPlease note, the "insecure" connection string uses a query string with the field-value\n`Tls=false`. The value of this field is by default `true`.\n\n### Stop container\n\nTo stop and remove the "secure" container, use the following Docker commands.\n\n    $ docker stop eventstoredb-secure\n\t$ docker rm eventstoredb-secure\n\nTo stop and remove the "insecure" container, use the following Docker commands.\n\n    $ docker stop eventstoredb-insecure\n\t$ docker rm eventstoredb-insecure\n\n\n## EventStoreDB client\n\nThis EventStoreDB client is implemented in the `esdbclient` package with\nthe `ESDBClient` class.\n\n### Import class\n\nThe `ESDBClient` class can be imported from the `esdbclient` package.\n\n```python\nfrom esdbclient import ESDBClient\n```\n\n### Construct client\n\nThe `ESDBClient` class has one required constructor argument, `uri`, and one\noptional constructor argument, `root_certificates`.\n\nThe `uri` argument is expected to be an EventStoreDB connection string URI that\nconforms with the standard EventStoreDB "esdb" or "esdb+discover" URI schemes.\n\nFor example, the following connection string specifies that the client should\nattempt to create a "secure" connection to port 2113 on "localhost", and use the\nclient credentials "username" and "password" when making calls to the server.\n\n    esdb://username:password@localhost:2113?Tls=true\n\nThe client must be configured to create a "secure" connection to a "secure" server,\nor alternatively an "insecure" connection to an "insecure" server. By default, the\nclient will attempt to create a "secure" connection. And so, when connecting to an\n"insecure" server, the connection string must specify that the client should attempt\nto make an "insecure" connection.\n\nThe following connection string specifies that the client should\nattempt to create an "insecure" connection to port 2114 on "localhost".\nWhen connecting to an "insecure" server, the client will ignore any\nusername and password information included in the connection string,\nso that usernames and passwords are not sent over an "insecure" connection.\n\n    esdb://localhost:2114?Tls=false\n\nPlease note, the "insecure" connection string uses a query string with the field-value\n`Tls=false`. The value of this field is by default `true`. Unless the connection string\nURI includes the field-value `Tls=false` in the query string, the `root_certificates`\nconstructor argument is also required.\n\nWhen connecting to a "secure" server, the `root_certificates` argument is expected to\nbe a Python `str` containing PEM encoded SSL/TLS root certificates. This value is\npassed directly to `grpc.ssl_channel_credentials()`. It is used for authenticating the\nserver to the client. It is commonly the certificate of the certificate authority that\nwas responsible for generating the SSL/TLS certificate used by the EventStoreDB server.\nBut, alternatively for development, you can use the server\'s certificate itself.\n\nIn the example below, the constructor argument values are taken from the operating\nsystem environment. This is a typical arrangement in a production environment. It is\ndone this way here so that the code in this documentation can be tested with both\na "secure" and an "insecure" server.\n\n```python\nimport os\n\nclient = ESDBClient(\n    uri=os.getenv("ESDB_URI"),\n    root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),\n)\n```\n\n## Connection strings\n\nAn EventStoreDB connection string is a URI that conforms with one of two possible\nschemes: either the "esdb" scheme, or the "esdb+discover" scheme.\n\nThe syntax and semantics of the EventStoreDB URI schemes are described below. The\nsyntax is defined using [EBNF](https://en.wikipedia.org/wiki/Extended_Backus–Naur_form).\n\n### Two schemes\n\nThe "esdb" URI scheme can be defined in the following way.\n\n    esdb-uri = "esdb://" , [ user-info , "@" ] , grpc-target, { "," , grpc-target } , [ "?" , query-string ] ;\n\nIn the "esdb" URI scheme, after the optional user info string, there must be at least\none gRPC target. If there are several gRPC targets, they must be separated from each\nother with the "," character. Each gRPC target should indicate an EventStoreDB gRPC\nserver socket, by specifying a host and a port number separated with the ":" character.\nThe host may be a hostname that can be resolved to an IP address, or an IP address.\n\n    grpc-target = ( hostname | ip-address ) , ":" , port-number ;\n\n\nThe "esdb+discover" URI scheme can be defined in the following way.\n\n    esdb-discover-uri = "esdb+discover://" , [ user-info, "@" ] , cluster-domainname , [ "?" , query-string ] ;\n\nIn the "esdb+discover" URI scheme, after the optional user info string, there must be a\ndomain name which should identify a cluster of EventStoreDB servers. The client will use\na DNS server to resolve the domain name to a list of addresses of EventStoreDB servers,\nby querying for \'A\' records. In this case, the port number "2113" will be used to\nconstruct gRPC targets from the addresses obtained from \'A\' records provided by the\nDNS server. Therefore, if you want to use the "esdb+discover" URI scheme, you will\nneed to configure DNS when setting up your EventStoreDB cluster.\n\nWith both the "esdb" and "esdb+discover" URI schemes, the client firstly obtains\na list of gRPC targets: either directly from "esdb" connection strings; or indirectly\nfrom "esdb+discover" connection strings via DNS. This list of targets is known as the\n"gossip seed". The client will then attempt to connect to each gRPC target in turn,\nattempting to call the EventStoreDB Gossip API to obtain information about the\nEventStoreDB cluster. A member of the cluster is selected by the client, according\nto the "node preference" option. The client may then need to close its\nconnection and reconnect to the selected server.\n\n### User info string\n\nIn both the "esdb" and "esdb+discover" schemes, the URI may include a user info string.\nIf it exists in the URI, the user info string must be separated from the rest of the URI\nwith the "@" character. The user info string must include a username and a password,\nseparated with the ":" character.\n\n    user-info = username , ":" , password ;\n\nThe user info is sent by the client as "call credentials" in each call to a "secure"\nserver, in a "basic auth" authorization header. This authorization header is used by\nthe server to authenticate the client. The authorization header is not sent to\n"insecure" servers.\n\n### Query string\n\nIn both the "esdb" and "esdb+discover" schemes, the optional query string must be one\nor many field-value arguments, separated from each other with the "&" character.\n\n    query-string = field-value, { "&", field-value } ;\n\nEach field-value argument must be one of the supported fields, and an\nappropriate value, separated with the "=" character.\n\n    field-value = ( "Tls", "=" , "true" | "false" )\n                | ( "TlsVerifyCert", "=" , "true" | "false" )\n                | ( "ConnectionName", "=" , string )\n                | ( "NodePreference", "=" , "leader" | "follower" | "readonlyreplica" | "random" )\n                | ( "DefaultDeadline", "=" , integer )\n                | ( "GossipTimeout", "=" , integer )\n                | ( "MaxDiscoverAttempts", "=" , integer )\n                | ( "DiscoveryInterval", "=" , integer )\n                | ( "MaxDiscoverAttempts", "=" , integer )\n                | ( "KeepAliveInterval", "=" , integer )\n                | ( "KeepAliveInterval", "=" , integer ) ;\n\nThe table below describes the query field-values supported by this client.\n\n| Field               | Value                                                                 | Description                                                                                                                                                       |\n|---------------------|-----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| Tls                 | "true", "false" (default: "true")                                     | If "true" the client will create a "secure" gRPC channel. If "false" the client will create an "insecure" gRPC channel. This must match the server configuration. |\n| TlsVerifyCert       | "true", "false" (default: "true")                                     | This value is currently ignored.                                                                                                                                  |\n| ConnectionName      | string (default: auto-generated version-4 UUID)                       | Sent in call metadata for every call, to identify the client to the cluster.                                                                                      |\n| NodePreference      | "leader", "follower", "readonlyreplica", "random" (default: "leader") | The node state preferred by the client. The client will select a node from the cluster info received from the Gossip API according to this preference.            |\n| DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_events()`.                                                     |\n| GossipTimeout       | integer (default: 5)                                                  | The default value (in seconds) of the `timeout` argument of gossip read methods, such as `read_gossip()`.                                                         |\n| MaxDiscoverAttempts | integer (default: 10)                                                 | The number of attempts to read gossip when connecting or reconnecting to a cluster member.                                                                        |\n| DiscoveryInterval   | integer (default: 100)                                                | How long to wait (in milliseconds) between gossip retries.                                                                                                        |\n| KeepAliveInterval   | integer (default: `None`)                                             | The value of the "grpc.keepalive_ms" gRPC channel option.                                                                                                         |\n| KeepAliveTimeout    | integer (default: `None`)                                             | The value of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                                                 |\n\n\n### Examples\n\nHere are some examples of EventStoreDB connection string URIs.\n\nThe following URI will cause the client to connect to, and get\ncluster info, from "secure" server socket `localhost:2113`. And\nthen to connect to a "leader" node. And also to use "admin" and\n"changeit" as the username and password when making calls to\nEventStoreDB API methods.\n\n    esdb://admin:changeit@localhost:2113\n\n\nThe following URI will cause the client to get cluster info from\n"insecure" server socket 127.0.0.1:2114.  And then to connect to\na "leader" node.\n\n    esdb://127.0.0.1:2114?Tls=false\n\n\nThe following URI will cause the client to get cluster info from\naddresses in DNS \'A\' records for cluster1.example.com. And then\nto connect to a "leader" node. And use a default deadline of 5\nseconds when making calls to EventStore API "write" methods.\n\n    esdb+discover://admin:changeit@cluster1.example.com?DefaultDeadline=5\n\n\nThe following URI will cause the client to get cluster info from either\nlocalhost:2111, or localhost:2112, or localhost:2113. And then to connect\nto a "follower" node.\n\n    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower\n\n\nThe following URI will cause the client to get cluster info from addresses in\nDNS \'A\' records for cluster1.example.com. And to configure "keep alive" timeout\nand interval in the gRPC channel.\n\n    esdb+discover://admin:changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000\n\n\nPlease note, the client is insensitive to the case of fields and values. If fields are\nrepeated in the query string, the query string will be parsed without error. However,\nthe connection options used by the client will use the value of the first field. All\nthe other field-values in the query string with the same field name will be ignored.\nFields without values will also be ignored.\n\nIf the client\'s node preference is "leader" and the node becomes a\n"follower", the client will attempt to reconnect to the current leader when a method\nis called that expects to call a leader. Methods which mutate the state of the database\nexpect to call a leader. For such methods, the HTTP header "requires-leader" is set to\n"true", and this header is observed by the server, and so a node which is not a leader\nthat receives such a request will return an error. This error is detected by the client,\nwhich will then close the current gRPC connection and create a new connection to the\nleader. The request will then be retried with the leader.\n\nIf the client\'s node preference is "follower" and there are no follower\nnodes in the cluster, then the client will raise an exception. Similarly, if the\nclient\'s node preference is "readonlyreplica" and there are no read-only replica\nnodes in the cluster, then the client will also raise an exception.\n\nThe gRPC channel option "grpc.max_receive_message_length" is automatically\nconfigured to the value `17 * 1024 * 1024`. This value cannot be changed.\n\n\n## Event objects\n\nThis package defines a `NewEvent` class and a `RecordedEvent` class. The\n`NewEvent` class should be used when writing events to the database. The\n`RecordedEvent` class is used when reading events from the database.\n\n### New events\n\nThe `NewEvent` class should be used when writing events to an EventStoreDB database.\nYou will need to construct new event objects before calling the `append_events()`\nand `append_event()` methods.\n\nThe `NewEvent` class is a frozen Python database. It has two required constructor\narguments (`type` and `data`) and three optional constructor arguments (`metadata`,\n`content_type` and `id`).\n\nThe required `type` argument is a Python `str`, used to describe the type of\ndomain event that is being recorded.\n\nThe required `data` argument is a Python `bytes` object, used to state the\nserialized data of the domain event that is being recorded.\n\nThe optional `metadata` argument is a Python `bytes` object, used to indicate any\nmetadata of the event that will be recorded. The default value is an empty `bytes`\nobject.\n\nThe optional `content_type` argument is a Python `str`, used to indicate the\nkind of data that is being recorded. The default value is `\'application/json\'`,\nwhich indicates that the `data` was serialised using JSON. An alternative value\nfor this argument is the more general indication `\'application/octet-stream\'`.\n\nThe optional `id` argument is a Python `UUID` object, used to specify the unique ID\nof the event that will be recorded. If no value is provided, a new version-4 UUID\nwill be generated.\n\n```python\nnew_event1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'{"name": "Greg"}\',\n)\nassert new_event1.type == \'OrderCreated\'\nassert new_event1.data == b\'{"name": "Greg"}\'\nassert new_event1.metadata == b\'\'\nassert new_event1.content_type == \'application/json\'\nassert isinstance(new_event1.id, uuid.UUID)\n\nevent_id = uuid.uuid4()\nnew_event2 = NewEvent(\n    type=\'ImageCreated\',\n    data=b\'01010101010101\',\n    metadata=b\'{"a": 1}\',\n    content_type=\'application/octet-stream\',\n    id=event_id,\n)\nassert new_event2.type == \'ImageCreated\'\nassert new_event2.data == b\'01010101010101\'\nassert new_event2.metadata == b\'{"a": 1}\'\nassert new_event2.content_type == \'application/octet-stream\'\nassert new_event2.id == event_id\n```\n\n### Recorded events\n\nThe `RecordedEvent` class is used when reading events from an EventStoreDB\ndatabase. The client will return event objects of this type from all methods\nthat return recorded events, such as `read_stream_events()`, `subscribe_all_events()`,\nand `read_subscription()`. You do not need to construct recorded event objects.\n\nLike `NewEvent`, the `RecordedEvent` class is also a frozen Python database. It has\nall the attributes that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`)\nand some additional attributes that follow from the fact that an event was recorded\n(`stream_name`, `stream_position`, `commit_position`).\n\nThe `type` attribute is a Python `str`, used to indicate the type of an event\nthat was recorded.\n\nThe `data` attribute is a Python `bytes` object, used to indicate the data of an\nevent that was recorded.\n\nThe `metadata` attribute is a Python `bytes` object, used to indicate the metadata of\nan event that was recorded.\n\nThe `content_type` attribute is a Python `str`, used to indicate the type of\ndata that was recorded for an event. It is usually `application/json`, indicating\nthat the data can be parsed as JSON. Alternatively, it is `application/octet-stream`.\n\nThe `id` attribute is a Python `UUID` object, used to indicate the unique ID of an\nevent that was recorded.\n\nThe `stream_name` attribute is a Python `str`, used to indicate the name of a\nstream in which an event was recorded.\n\nThe `stream_position` attribute is a Python `int`, used to indicate the position in a\nstream at which an event was recorded.\n\nIn EventStoreDB, a "stream position" is an integer representing the position of a\nrecorded event in a stream. Each recorded event is recorded at a position in a stream.\nEach stream position is occupied by only one recorded event. New events are recorded at the\nnext unoccupied position. All sequences of stream positions are zero-based and gapless.\n\nThe `commit_position` attribute is a Python `int`, used to indicate the position in the\ndatabase at which an event was recorded.\n\nIn EventStoreDB, a "commit position" is an integer representing the position of a\nrecorded event in the database. Each recorded event is recorded at a position in the\ndatabase. Each commit position is occupied by only one recorded event. Commit positions\nare zero-based and increase monotonically as new events are recorded. But, unlike stream\npositions, the sequence of successive commit positions is not gapless. Indeed, there are\nusually large differences between the commit positions of successively recorded events.\n\n\n```python\nfrom esdbclient.events import RecordedEvent\n\nrecorded_event = RecordedEvent(\n    type=\'OrderCreated\',\n    data=b\'{}\',\n    metadata=b\'\',\n    content_type=\'application/json\',\n    id=uuid.uuid4(),\n    stream_name=\'stream1\',\n    stream_position=0,\n    commit_position=512,\n)\n```\n\n\n## Streams\n\nIn EventStoreDB, a "stream" is a sequence of recorded events that all have\nthe same "stream name". There will normally be many streams in a database,\neach with many recorded events. Each recorded event has a position in its stream\n(the "stream position"), and a position in the database (the "commit position").\nStream positions are zero-based and gapless. Commit positions are also zero-based,\nbut are not gapless.\n\nThe methods `append_events()`, `read_stream_events()` and `read_all_events()` can\nbe used to read and record in the database.\n\n### Append events\n\n*requires leader*\n\nThe `append_events()` method can be used atomically to record a sequence of new events.\nIf the operation is successful, it returns the commit position of the last event in the\nsequence that has been recorded.\n\nThis method has three required arguments, `stream_name`, `current_version`\nand `events`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream to which a sequence of events will be appended.\n\nThe required `current_version` argument is expected to be either a Python `int`\nthat indicates the stream position of the last recorded event in the stream, or\n`None` if the stream does not yet exist or has been deleted. The stream positions\nare zero-based and gapless, so that if a stream has two events, the `current_version`\nshould be 1. If an incorrect value is given, this method will raise a\n`WrongCurrentVersion` exception. This behavior is designed to provide concurrency\ncontrol when recording new events. The correct value of `current_version` for any stream\ncan be obtained by calling `get_current_version()`. However, the typical approach is to\nuse the stream position of the recorded events as the version number of a reconstructed\naggregate, and to use the current version of the aggregate as the `current_version` when\nappending new aggregate events. This ensures the consistency of the recorded state of\nthe aggregate, and forces operations that generate new aggregate events to be retried with a freshly\nreconstructed aggregate when a `WrongCurrentVersion` exception is encountered.\nThis controlling behavior can be disabled by setting the value of the\n`current_version` argument to `-1`.\n\nThe required `events` argument is expected to be a sequence of new event objects. The\n`NewEvent` class should be used to construct new event objects. The `append_events()`\noperation is atomic, so that either all or none of the new events will be recorded. It\nis not possible with EventStoreDB atomically to record new events in more than one stream.\n\nThis method also has an optional `timeout` argument, which is a Python `float`\nthat sets a deadline for the completion of the gRPC operation.\n\nIn the example below, a new event, `event1`, is appended to a new stream. The\nstream does not yet exist, so `current_version` is `None`.\n\n```python\n# Construct a new event object.\nevent1 = NewEvent(type=\'OrderCreated\', data=b\'data1\')\n\n# Define a new stream name.\nstream_name1 = str(uuid.uuid4())\n\n# Append the new events to the new stream.\ncommit_position1 = client.append_events(\n    stream_name=stream_name1,\n    current_version=None,\n    events=[event1],\n)\n```\n\nIn the example below, two subsequent events are appended to an existing\nstream. The stream, `stream_name1`, so far has one recorded event, and so\nthe correct value of `current_version` is `0`.\n\n```python\nevent2 = NewEvent(type=\'OrderUpdated\', data=b\'data2\')\nevent3 = NewEvent(type=\'OrderDeleted\', data=b\'data3\')\n\ncommit_position2 = client.append_events(\n    stream_name=stream_name1,\n    current_version=0,\n    events=[event2, event3],\n)\n```\n\nThe returned values, `commit_position1` and `commit_position2`, are the\ncommit positions in the database of the last events in the recorded sequences.\nThat is, `commit_position1` is the commit position of `event1` and\n`commit_position2` is the commit position of `event3`.\n\nCommit positions that are returned in this way can be used by a user interface to poll\na downstream component until it has processed all the newly recorded events. For example,\nconsider a user interface command that results in the recording of new events, and an\neventually consistent materialized view in a downstream component that is updated from\nthese events. If the new events have not yet been processed, the view might be stale,\nor out-of-date. Instead of displaying a stale view, the user interface can poll the\ndownstream component until it has processed the newly recorded events, and then display\nan up-to-date view to the user.\n\n\n### Append event\n\n*requires leader*\n\nThe `append_event()` method is like `append_events()` but can be used only to write a\nsingle new event to a stream. If the operation is successful, it returns the commit\nposition of the newly recorded event.\n\nThis method has three required arguments, `stream_name`, `current_version` and `event`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream to which a sequence of events will be appended.\n\nThe required `current_version` argument is expected to be either a Python `int`\nthat indicates the stream position of the last recorded event in the stream.\n\nThe required `event` argument is expected to be a single new event object. The event\nobject is expected to be an instance of the `NewEvent` class.\n\nThis method also has an optional `timeout` argument, which is a Python `float`\nthat sets a deadline for the completion of the gRPC operation.\n\n\n### Idempotent append operations\n\nThe `append_event()` and `append_events()` and methods are "idempotent", in that\nif the methods are called with new events whose `id` attribute values equal those\nof recorded events in the named stream immediately after the stream position specified\nby the value of the `current_version` argument, then these methods will return the\ncommit position of the last new event, without making any changes to the database.\n\nSometimes it may happen, when calling `append_event()` or `append_events()`, that\nthe new events are successfully recorded but somehow a connection issue occurs before\nthe successful call can return successfully to the client. We cannot be sure if\nthe events were recorded or not, and so we may wish to retry. If the events were in\nfact successfully recorded, it is convenient for the retried operation to return\nsuccessfully without raising an exception. If those new events were in fact not recorded,\nand in the meantime no other new events were recorded in that stream, then it makes sense\nthat the new events will be recorded when the append operation is retried. Of course,\nif a `WrongCurrentVersion` exception is raised when retrying the operation, then an\napplication command which generated the new events in the context of already recorded\nevents may need to be executed again. Alternatively, a suitable error might be displayed\nby the application, with an up-to-date view of the recorded data, giving a user of the\napplication an opportunity to decide if they still wish to proceed with their original\nintention.\n\nThe example below shows the `append_events()` method being called again with\n`event3` and `current_version=0`. We can see that repeating the call to\n`append_events()` returns successfully.\n\n```python\n# Retry appending event3.\ncommit_position_retry = client.append_events(\n    stream_name=stream_name1,\n    current_version=0,\n    events=[event2, event3],\n)\n```\n\nWe can see that the same commit position is returned as above.\n\n```python\nassert commit_position_retry == commit_position2\n```\n\nBy calling `read_stream_events()`, we can also see the stream has been unchanged\ndespite the `append_events()` method having been called twice with the same arguments.\nThat is, there are still only three events in the stream.\n\n```python\nevents = client.read_stream_events(\n    stream_name=stream_name1\n)\n\nassert len(events) == 3\n```\n\nThis idempotent behaviour depends on the `id` attribute of the `NewEvent` class.\nThis attribute, by default, is assigned a new and unique version-4 UUID when an\ninstance of `NewEvent` is constructed. The `id` argument can be used when\nconstructing `NewEvent` objects to set the value of this attribute.\n\n\n### Read stream events\n\nThe `read_stream_events()` method can be used to get events that have been appended\nto a stream. This method returns a Python `tuple` of recorded event objects. The\nrecorded event objects are instances of the `RecordedEvent` class.\n\nThis method has one required argument, `stream_name`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream from which recorded events will be returned.\n\nThe `read_stream_events()` method also has four optional arguments,\n`stream_position`, `backwards`, `limit`, and `timeout`.\n\nThe optional `stream_position` argument is a Python `int` that can be used to\nindicate the position in the stream from which to start reading. The default value\nof `stream_position` is `None`. When reading a stream from a specific position in the\nstream, the recorded event at that position will be included, both when reading\nforwards from that position, and when reading backwards.\n\nThe optional `backwards` argument is a Python `bool`. The default value of `backwards`\nis `False`, which means the stream will be read forwards, so that events are returned\nin the order they were recorded. If `backwards` is `True`, the events are returned in\nreverse order.\n\nIf `backwards` is `False` and `stream_position` is `None`, the stream\'s events will be\nreturned in the order they were recorded, starting from the first recorded event. This\nis the default behavior of `read_stream_events()`. If `backwards` is `True` and\n`stream_position` is `None`, the stream\'s events will be returned in reverse order,\nstarting from the last recorded event.\n\nThe optional `limit` argument is a Python `int` which restricts the number of events\nthat will be returned. The default value of `limit` is `sys.maxint`.\n\nThe optional `timeout` argument is a Python `float` which sets a deadline for\nthe completion of the gRPC operation.\n\nThe example below shows the default behavior of this method, which is to return all\nthe recorded events of a stream forwards from the first recorded events to the last.\n\n```python\nevents = client.read_stream_events(\n    stream_name=stream_name1\n)\n\nassert len(events) == 3\nassert events[0].id == event1.id\nassert events[1].id == event2.id\nassert events[2].id == event3.id\n```\n\nThe example below shows how to use the `stream_position` argument to read a stream\nfrom a specific stream position to the end of the stream. Stream positions are\nzero-based, and so `stream_position=1` corresponds to the second event that was\nrecorded in the stream, in this case `event2`.\n\n```python\nevents = client.read_stream_events(\n    stream_name=stream_name1,\n    stream_position=1,\n)\n\nassert len(events) == 2\nassert events[0].id == event2.id\nassert events[1].id == event3.id\n```\n\nThe example below shows how to use the `backwards` argument to read a stream backwards.\n\n```python\nevents = client.read_stream_events(\n    stream_name=stream_name1,\n    backwards=True,\n)\n\nassert len(events) == 3\nassert events[0].id == event3.id\nassert events[1].id == event2.id\nassert events[2].id == event1.id\n```\n\nThe example below shows how to use the `limit` argument to read a limited number of\nevents.\n\n```python\nevents = client.read_stream_events(\n    stream_name=stream_name1,\n    limit=2,\n)\n\nassert len(events) == 2\nassert events[0].id == event1.id\nassert events[1].id == event2.id\n```\n\nThe `read_stream_events()` method will raise a `NotFound` exception if the named stream\nhas never existed or has been deleted.\n\n```python\nfrom esdbclient.exceptions import NotFound\n\n\ntry:\n    client.read_stream_events(\'does-not-exist\')\nexcept NotFound:\n    pass  # The stream does not exist.\nelse:\n    raise Exception("Shouldn\'t get here")\n```\n\nPlease note, this method streams recorded events from the server and then\nconstructs and returns a Python `tuple`. In case you don\'t want the client to\nfinish streaming events from the database before it returns, you can instead\nuse the `iter_stream_events()` method, which returns an iterable "read response"\nobject. A "read response" is an iterator, and not a sequence. Recorded events can\nbe obtained by iterating over the "read response" object. It streams recorded events\nfrom the server as the iteration proceeds. The iteration will automatically stop\nwhen there are no more recorded events to be returned. The streaming of events,\nand hence the iterator, can also be stopped prematurely by calling the `stop()`\nmethod on the "read response" object.\n\nIn fact, the `read_stream_events()` method calls `iter_stream_events()` and passes\nthe "read response" iterator into the Python `tuple` constructor. However, the\n`read_stream_events()` method is decorated with retry and reconnect decorators,\nwhilst the `iter_stream_events()` method is not. This means that all errors due to\nconnection issues will be caught by the retry and reconnect decorators when calling\nthe `read_stream_events()` method, but not when calling `iter_stream_events()`. The\n`iter_stream_events()` method has no such decorators because the streaming only starts\nwhen iterating over the "read response" starts, which means that the method returns\nbefore the streaming starts, and so there is no chance for any decorators to catch\nany connection issues.\n\nNevertheless, if you are reading a very large stream, then you might prefer to call\n`iter_stream_events()`, and to begin iterating through the recorded events whilst\nthey are being streamed from the server, rather than both waiting and having them\nall accumulate in memory. Because of the risk of connection issues arising during\nthe streaming of recorded events from the server, you will need to care about\nconnection issues when iterating over the "read response" object returned from\n`iter_stream_events()`.\n\n### Get current version\n\nThe `get_current_version()` method is a convenience method that essentially calls\n`read_stream_events()` with `backwards=True` and `limit=1`. This method returns\nthe value of the `stream_position` attribute of the last recorded event in a\nstream. If a stream does not exist, the returned value is `None`. The returned\nvalue is the correct value of `current_version` when appending new events to\na stream.\n\nThis method has one required argument, `stream_name`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream from which a stream position will be returned.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nIn the example below, the last stream position of `stream_name1` is obtained.\nSince three events have been appended to `stream_name1`, and because positions\nin a stream are zero-based and gapless, so the current version is `2`.\n\n```python\ncurrent_version = client.get_current_version(\n    stream_name=stream_name1\n)\n\nassert current_version == 2\n```\n\nIf a stream has never existed or has been deleted, the returned value is `None`,\nwhich matches the required value of the `current_version` argument both when\nappending the first event of a new stream, and also when appending events to\na stream that has been deleted.\n\n```python\ncurrent_version = client.get_current_version(\n    stream_name=\'does-not-exist\'\n)\n\nassert current_version is None\n```\n\n### How to implement snapshotting with EventStoreDB\n\nSnapshots can improve the performance of aggregates that would otherwise be\nreconstructed from very long streams. However, it is generally recommended to design\naggregates to have a finite lifecycle, and so to have relatively short streams,\nthereby avoiding the need for snapshotting. This "how to" section is intended merely\nto show how snapshotting of aggregates can be implemented with EventStoreDB using\nthis Python client.\n\nEvent-sourced aggregates are typically reconstructed from recorded events by calling\na mutator function for each recorded event, evolving from an initial state\n`None` to the current state of the aggregate. The function `get_aggregate()` shows\nhow this can be done. The aggregate ID is used as a stream name. The exception\n`AggregateNotFound` is raised if the aggregate stream is not found.\n\n```python\nclass AggregateNotFound(Exception):\n    """Raised when an aggregate is not found."""\n\n\ndef get_aggregate(aggregate_id, mutator_func):\n    stream_name = aggregate_id\n\n    # Get recorded events.\n    try:\n        events = client.read_stream_events(\n            stream_name=stream_name,\n            stream_position=None\n        )\n    except NotFound as e:\n        raise AggregateNotFound(aggregate_id) from e\n    else:\n        # Reconstruct aggregate from recorded events.\n        aggregate = None\n        for event in events:\n            aggregate = mutator_func(aggregate, event)\n        return aggregate\n```\n\nSnapshotting of aggregates can be implemented by recording the current state of\nan aggregate as a new event.\n\nIf an aggregate object has a version number that corresponds to the stream position of\nthe last event that was used to reconstruct the aggregate, and this version number\nis recorded in the snapshot metadata, then any events that are recorded after the\nsnapshot can be selected using this version number. The aggregate can then be\nreconstructed from the last snapshot and any subsequent events, without having\nto replay the entire history.\n\nWe will use a separate stream for an aggregate\'s snapshots that is named after the\nstream used for recording its events. The name of the snapshot stream will be\nconstructed by prefixing the aggregate\'s stream name with `\'snapshot-$\'`.\n\n```python\nSNAPSHOT_STREAM_NAME_PREFIX = \'snapshot-$\'\n\ndef make_snapshot_stream_name(stream_name):\n    return f\'{SNAPSHOT_STREAM_NAME_PREFIX}{stream_name}\'\n\n\ndef remove_snapshot_stream_prefix(snapshot_stream_name):\n    assert snapshot_stream_name.startswith(SNAPSHOT_STREAM_NAME_PREFIX)\n    return snapshot_stream_name[len(SNAPSHOT_STREAM_NAME_PREFIX):]\n```\n\nNow, let\'s redefine the `get_aggregate()` function, so that it looks for a snapshot event,\nthen selects subsequent aggregate events, and then calls a mutator function for each\nrecorded event.\n\nNotice that the aggregate events are read from a stream for serialized aggregate\nevents, whilst the snapshot is read from a separate stream for serialized aggregate\nsnapshots. We will use JSON to serialize and deserialize event data.\n\n\n```python\nimport json\n\n\ndef get_aggregate(aggregate_id, mutator_func):\n    stream_name = aggregate_id\n    recorded_events = []\n\n    # Look for a snapshot.\n    try:\n        snapshots = client.read_stream_events(\n            stream_name=make_snapshot_stream_name(stream_name),\n            backwards=True,\n            limit=1\n        )\n    except NotFound:\n        stream_position = None\n    else:\n        assert len(snapshots) == 1\n        snapshot = snapshots[0]\n        stream_position = deserialize(snapshot.metadata)[\'version\'] + 1\n        recorded_events.append(snapshot)\n\n    # Get subsequent events.\n    try:\n        events = client.read_stream_events(\n            stream_name=stream_name,\n            stream_position=stream_position\n        )\n    except NotFound as e:\n        raise AggregateNotFound(aggregate_id) from e\n    else:\n        recorded_events += events\n\n    # Reconstruct aggregate from recorded events.\n    aggregate = None\n    for event in recorded_events:\n        aggregate = mutator_func(aggregate, event)\n\n    return aggregate\n\n\ndef serialize(d):\n    return json.dumps(d).encode(\'utf8\')\n\n\ndef deserialize(s):\n    return json.loads(s.decode(\'utf8\'))\n```\n\nTo show how `get_aggregate()` can be used, let\'s define a `Dog` aggregate class, with\nattributes `name` and `tricks`. The attributes `id` and `version` will indicate an\naggregate object\'s ID and version number. The attribute `is_from_snapshot` is added\nhere merely to demonstrate below when an aggregate object has been reconstructed using\na snapshot.\n\n```python\nfrom dataclasses import dataclass\n\n\n@dataclass(frozen=True)\nclass Aggregate:\n    id: str\n    version: int\n    is_from_snapshot: bool\n\n\n@dataclass(frozen=True)\nclass Dog(Aggregate):\n    name: str\n    tricks: list\n```\n\nLet\'s also define a mutator function `mutate_dog()` that can evolve the state of a\n`Dog` aggregate given various different types of events, `\'DogRegistered\'`,\n`\'DogLearnedTrick\'`, and `\'Snapshot\'`.\n\n```python\ndef mutate_dog(dog, event):\n    data = deserialize(event.data)\n    if event.type == \'DogRegistered\':\n        return Dog(\n            id=event.stream_name,\n            version=event.stream_position,\n            is_from_snapshot=False,\n            name=data[\'name\'],\n            tricks=[],\n        )\n    elif event.type == \'DogLearnedTrick\':\n        assert event.stream_position == dog.version + 1\n        assert event.stream_name == dog.id, (event.stream_name, dog.id)\n        return Dog(\n            id=dog.id,\n            version=event.stream_position,\n            is_from_snapshot=dog.is_from_snapshot,\n            name=dog.name,\n            tricks=dog.tricks + [data[\'trick\']],\n        )\n    elif event.type == \'Snapshot\':\n        return Dog(\n            id=remove_snapshot_stream_prefix(event.stream_name),\n            version=deserialize(event.metadata)[\'version\'],\n            is_from_snapshot=True,\n            name=data[\'name\'],\n            tricks=data[\'tricks\'],\n        )\n    else:\n        raise Exception(f"Unknown event type: {event.type}")\n```\n\nFor convenience, let\'s also define a `get_dog()` function that calls `get_aggregate()`\nwith the `mutate_dog()` function as the value of its `mutator_func` argument.\n\n```python\ndef get_dog(dog_id):\n    return get_aggregate(\n        aggregate_id=dog_id,\n        mutator_func=mutate_dog,\n    )\n```\n\nWe can also define some "command" functions that append new events to the\ndatabase. The `register_dog()` function appends a `DogRegistered` event. The\n`record_trick_learned()` appends a `DogLearnedTrick` event. The function\n`snapshot_dog()` appends a `Snapshot` event. Notice that the\n`record_trick_learned()` and `snapshot_dog()` functions use `get_dog()`.\n\nNotice also that the `DogRegistered` and `DogLearnedTrick` events are appended to a\nstream for aggregate events, whilst the `Snapshot` event is appended to a separate\nstream for aggregate snapshots.\n\n```python\ndef register_dog(name):\n    dog_id = str(uuid.uuid4())\n    event = NewEvent(\n        type=\'DogRegistered\',\n        data=serialize({\'name\': name}),\n    )\n    client.append_event(\n        stream_name=dog_id,\n        current_version=None,\n        event=event,\n    )\n    return dog_id\n\n\ndef record_trick_learned(dog_id, trick):\n    dog = get_dog(dog_id)\n    event = NewEvent(\n        type=\'DogLearnedTrick\',\n        data=serialize({\'trick\': trick}),\n    )\n    client.append_event(\n        stream_name=dog_id,\n        current_version=dog.version,\n        event=event,\n    )\n\n\ndef snapshot_dog(dog_id):\n    dog = get_dog(dog_id)\n    event = NewEvent(\n        type=\'Snapshot\',\n        data=serialize({\'name\': dog.name, \'tricks\': dog.tricks}),\n        metadata=serialize({\'version\': dog.version}),\n    )\n    client.append_event(\n        stream_name=make_snapshot_stream_name(dog_id),\n        current_version=-1,\n        event=event,\n    )\n```\n\nWe can call `register_dog()` to register a new dog.\n\n```python\n# Register a new dog.\ndog_id = register_dog(\'Fido\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == []\nassert dog.version == 0\nassert dog.is_from_snapshot is False\n\n```\n\nWe can call `record_trick_learned()` to record that some tricks have been learned.\n\n```python\n\n# Record that \'Fido\' learned a new trick.\nrecord_trick_learned(dog_id, trick=\'roll over\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\']\nassert dog.version == 1\nassert dog.is_from_snapshot is False\n\n\n# Record that \'Fido\' learned another new trick.\nrecord_trick_learned(dog_id, trick=\'fetch ball\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\', \'fetch ball\']\nassert dog.version == 2\nassert dog.is_from_snapshot is False\n```\n\nWe can call `snapshot_dog()` to record a snapshot of the current state of the `Dog`\naggregate. After we call `snapshot_dog()`, the `get_dog()` function will return a `Dog`\nobject that has been constructed using the `Snapshot` event.\n\n```python\n# Snapshot \'Fido\'.\nsnapshot_dog(dog_id)\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\', \'fetch ball\']\nassert dog.version == 2\nassert dog.is_from_snapshot is True\n```\n\nWe can continue to evolve the state of the `Dog` aggregate, using\nthe snapshot both during the call to `record_trick_learned()` and\nwhen calling `get_dog()` directly.\n\n```python\nrecord_trick_learned(dog_id, trick=\'sit\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\', \'fetch ball\', \'sit\']\nassert dog.version == 3\nassert dog.is_from_snapshot is True\n```\n\nWe can see from the `is_from_snapshot` attribute that the `Dog` object was indeed\nreconstructed from the snapshot.\n\nSnapshots can be created at fixed version number intervals, fixed time\nperiods, after a particular type of event, immediately after events are\nappended, or as a background process.\n\n\n### Read all events\n\nThe `read_all_events()` method can be used to get all recorded events\nin the database in the order they were recorded. This method will return\na "read response" object, just like `iter_stream_events()`.\n\nA "read response" is an iterator, and not a sequence. Recorded events can be\nobtained by iterating over the "read response" object. It streams recorded\nevents from the server as the iteration proceeds. The iteration will automatically\nstop when there are no more recorded events to be returned. The streaming of events,\nand hence the iterator, can also be stopped by calling the `stop()` method on the\n"read response" object.\n\nJust like `read_stream_events()` and `iter_stream_events()`, the received event objects\nare instances of the `RecordedEvent` class.\n\nThis method has seven optional arguments, `commit_position`, `backwards`,\n`filter_exclude`, `filter_include`, `filter_by_stream_name`, `limit`, and `timeout`.\n\nThe optional `commit_position` argument is a Python `int` that can be used to\nspecify a commit position from which to start reading. The default value of\n`commit_position` is `None`. Please note, if a commit position is specified,\nit must be an actually existing commit position in the database.\n\nThe optional `backwards` argument is a Python `bool`. The default of `backwards` is\n`False`, which means events are returned in the order they were recorded, If\n`backwards` is `True`, then events are returned in reverse order.\n\nIf `backwards` is `False` and `commit_position` is `None`, the database\'s events will\nbe returned in the order they were recorded, starting from the first recorded event.\nThis is the default behavior of `read_all_events()`. If `backwards` is `True` and\n`commit_position` is `None`, the database\'s events will be returned in reverse order,\nstarting from the last recorded event.\n\nThe optional `filter_exclude` argument is a sequence of regular expressions that\nspecifies which recorded events should be returned. This argument is ignored\nif `filter_include` is set to a non-empty sequence. The default value of this\nargument matches the event types of EventStoreDB "system events", so that system\nevents will not normally be included. See the Notes section below for more\ninformation about filter expressions.\n\nThe optional `filter_include` argument is a sequence of regular expressions\nthat specifies which recorded events should be returned. By default, this\nargument is an empty tuple. If this argument is set to a non-empty sequence,\nthe `filter_exclude` argument is ignored.\n\nThe optional `filter_by_stream_name` argument is a Python `bool` that indicates\nwhether the filtering will apply to event types or stream names. By default, this\nvalue is `False` and so the filtering will apply to the event type strings of\nrecorded events.\n\nThe optional `limit` argument is an integer which restricts the number of events that\nwill be returned. The default value is `sys.maxint`.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe filtering of events is done on the EventStoreDB server. The\n`limit` argument is applied on the server after filtering.\n\nThe example below shows how to get all the events we have recorded in the database\nso far, in the order they were recorded. We can see the three events of `stream_name1`\n(`event1`, `event2` and `event3`) are included, along with others.\n\n```python\n# Read all events (creates a streaming gRPC call).\nread_response = client.read_all_events()\n\n# Convert the iterator into a sequence of recorded events.\nevents = tuple(read_response)\nassert len(events) > 3  # more than three\n\n# Convert the sequence of recorded events into a set of event IDs.\nevent_ids = set(e.id for e in events)\nassert event1.id in event_ids\nassert event2.id in event_ids\nassert event3.id in event_ids\n```\n\nThe example below shows how to read all recorded events in the database from\na particular commit position, in this case `commit_position1`. When reading\nforwards from a specific commit position, the event at the specified position\nwill be included. The value of `commit_position1` is the position we obtained\nwhen appending `event1`. And so `event1` is the first recorded event we shall\nreceive, `event2` is the second, and `event3` is the third.\n\n```python\n# Read all events forwards from a commit position.\nread_response = client.read_all_events(\n    commit_position=commit_position1\n)\n\n# Step through the "read response" iterator.\nassert next(read_response).id == event1.id\nassert next(read_response).id == event2.id\nassert next(read_response).id == event3.id\n\n# Stop the iterator.\nread_response.stop()\n```\n\nThe example below shows how to read all events recorded in the database in reverse\norder. We can see that the first events we receive are the last events that were\nrecorded: the events of the `Dog` aggregate from the section about snapshotting\nand the snapshot.\n\n```python\n# Read all events backwards from the end.\nread_response = client.read_all_events(\n    backwards=True\n)\n\n# Step through the "read response" iterator.\nassert next(read_response).type == "DogLearnedTrick"\nassert next(read_response).type == "Snapshot"\nassert next(read_response).type == "DogLearnedTrick"\nassert next(read_response).type == "DogLearnedTrick"\nassert next(read_response).type == "DogRegistered"\n\n# Stop the iterator.\nread_response.stop()\n```\n\nThe example below shows how to read a limited number of events\nforwards from a specific commit position.\n\n```python\nevents = tuple(\n    client.read_all_events(\n        commit_position=commit_position1,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\nassert events[0].id == event1.id\n```\n\nThe example below shows how to read a limited number of the recorded events\nin the database backwards from the end. In this case, the limit is 1, and\nso we receive the last recorded event.\n\n```python\nevents = tuple(\n    client.read_all_events(\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].type == \'DogLearnedTrick\'\nassert deserialize(events[0].data)[\'trick\'] == \'sit\'\n```\n\nPlease note, like the `iter_stream_events()` method, the `read_all_events()` method\nis not decorated with retry and reconnect decorators, because the streaming of recorded\nevents from the server only starts when iterating over the "read response" starts, which\nmeans that the method returns before the streaming starts, and so there is no chance for\nany decorators to catch any connection issues.\n\n### Get commit position\n\nThe `get_commit_position()` method can be used to get the commit position of the\nlast recorded event in the database. It simply calls `read_all_events()` with\n`backwards=True` and `limit=1`, and returns the value of the `commit_position`\nattribute of the last recorded event.\n\n```python\ncommit_position = client.get_commit_position()\n```\n\nThis method has four optional arguments, `filter_exclude`, `filter_include`,\n`filter_by_stream_name` and `timeout`. These values are passed to `read_all_events()`.\n\nThe optional `filter_exclude`, `filter_include` and `filter_by_stream_name` arguments\nwork in the same way as they do in the `read_all_events()` method.\n\nThis optional `timeout` argument is a Python `float` that sets\na deadline for the completion of the gRPC operation.\n\nThis method might be used to measure progress of a downstream component\nthat is processing all recorded events, by comparing the current commit\nposition with the recorded commit position of the last successfully processed\nevent in a downstream component. In this case, the value of the `filter_exclude`,\n`filter_include` and `filter_by_stream_name` arguments should equal those used\nby the downstream component to obtain recorded events.\n\n\n### Get stream metadata\n\nThe `get_stream_metadata()` method returns the metadata for a stream, along\nwith the version of the stream metadata.\n\n```python\nmetadata, metadata_version = client.get_stream_metadata(stream_name=stream_name1)\n```\n\nThe returned `metadata` value is a Python `dict`. The returned `metadata_version`\nvalue is either an `int` if the stream exists, or `None` if the stream does not exist\nand no metadata has been set. These values can be passed into `set_stream_metadata()`.\n\n\n### Set stream metadata\n\n*requires leader*\n\nThe method `set_stream_metadata()` sets the metadata for a stream. Stream metadata\ncan be set before appending events to a stream.\n\n```python\nmetadata["foo"] = "bar"\n\nclient.set_stream_metadata(\n    stream_name=stream_name1,\n    metadata=metadata,\n    current_version=metadata_version,\n)\n```\n\nThe `current_version` argument should be the current version of the stream metadata\nobtained from `get_stream_metadata()`.\n\nPlease refer to the EventStoreDB documentation for more information about stream\nmetadata.\n\n### Delete stream\n\n*requires leader*\n\nThe method `delete_stream()` can be used to "delete" a stream.\n\n```python\ncommit_position = client.delete_stream(stream_name=stream_name1, current_version=2)\n```\n\nAfter deleting a stream, it\'s still possible to append new events. Reading from a\ndeleted stream will return only events that have been appended after it was\ndeleted.\n\n### Tombstone stream\n\n*requires leader*\n\nThe method `tombstone_stream()` can be used to "tombstone" a stream.\n\n```python\ncommit_position = client.tombstone_stream(stream_name=stream_name1, current_version=2)\n```\n\nAfter tombstoning a stream, it\'s not possible to append new events.\n\n\n## Catch-up subscriptions\n\nA "catch-up" subscription can be used to receive events that have already been\nrecorded in the database, and also events that are recorded subsequently.\n\nThe `subscribe_all_events()` method starts a catch-up subscription that can receive\nall events in the database. The `subscribe_stream_events()` method starts a catch-up\nsubscription that can receive events from a specific stream.\n\nThe `subscribe_all_events()` and `subscribe_stream_events()` methods both return a\n"read response" iterator, much like `iter_stream_events()` and `read_all_events()`.\nThe difference is the "read response" iterator returned for a catch-up subscription\ndoes not automatically stop when there are no more recorded events to be returned, but\ninstead blocks on getting the next event until further events are recorded in the\ndatabase. These subsequently recorded events will then be streamed to the iterator,\nwhich will then continue. Like `read_all_events()`, the returned "read response" has\na `stop()` method which will cancel the streaming gRPC operation and cause the\n"read response" iterator to stop.\n\nLike with `read_stream_events()` and `read_all_events()`, the recorded event objects\nreceived from a catch-up subscription are instances of the `RecordedEvent` class.\n\n### Subscribe all events\n\nThe`subscribe_all_events()` method can be used to start a catch-up subscription\nfrom which all events recorded in the database can be received.\n\nThis method can be used by a downstream component that processes recorded events with\nexactly-once semantics.\n\nThis method returns a "read response", from which recorded events can be\nobtained by iteration, including events that are recorded after all the\nrecorded events have been received. Iterating over this "read response"\nobject will therefore not stop, unless the `stop()` method of the\n"read response" object is called, or a connection issue occurs, or\nthe returned object iterator object is deleted from memory.\n\nThis method has an optional `commit_position` argument, which can be\nused to specify a commit position from which to subscribe. The default\nvalue is `None`, which means the subscription will operate from the first\nrecorded event in the database. If a commit position is given, it must match\nan actually existing commit position in the database. The recoded events that\nare obtained will not include the event recorded at that commit position.\n\nThis method also has four other optional arguments, `filter_exclude`,\n`filter_include`, `filter_by_stream_name`, and `timeout`.\n\nThe optional `filter_exclude` argument is a sequence of regular expressions that\nspecifies which recorded events should be returned. This argument is ignored\nif `filter_include` is set to a non-empty sequence. The default value of this\nargument matches the event types of EventStoreDB "system events", so that system\nevents will not normally be included. See the Notes section below for more\ninformation about filter expressions.\n\nThe optional `filter_include` argument is a sequence of regular expressions\nthat specifies which recorded events should be returned. By default, this\nargument is an empty tuple. If this argument is set to a non-empty sequence,\nthe `filter_exclude` argument is ignored.\n\nThe optional `filter_by_stream_name` argument is a Python `bool` that indicates\nwhether the filtering will apply to event types or stream names. By default, this\nvalue is `False` and so the filtering will apply to the event type strings of\nrecorded events.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe example below shows how to start a catch-up subscription to receive\nfrom the first recorded event in the database.\n\n```python\n# Subscribe from the first recorded event in the database.\nsubscription = client.subscribe_all_events()\n```\n\nThe example below is longer, and shows that the catch-up subscription\ndoes not stop automatically, but blocks when the last recorded event is\nreceived, and then continues when subsequent events are recorded.\n\n```python\n# Append a new event to a new stream.\nstream_name2 = str(uuid.uuid4())\nevent4 = NewEvent(type=\'OrderCreated\', data=b\'data4\')\nclient.append_events(\n    stream_name=stream_name2,\n    current_version=None,\n    events=[event4],\n)\n\n# Subscribe from the first recorded event in the database.\nsubscription = client.subscribe_all_events()\nreceived_events = []\n\n\n# Receive events from the catch-up subscription in a different thread.\nfrom datetime import datetime\nfrom threading import Thread\n\nmark = datetime.now()\n\ndef receive_events():\n    for event in subscription:\n        received_events.append(event)\n        global mark\n        mark = datetime.now()\n\n\ndef wait_for_subscription_to_block():\n    while True:\n         if (datetime.now() - mark).total_seconds() > 1:\n             break\n\n\nthread = Thread(target=receive_events)\nthread.start()\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n# Check the last received event is \'event4\'.\nassert received_events[-1].id == event4.id\n\n# Check we also received the other events we have recorded.\nassert received_events[-9].id == event1.id\nassert received_events[-8].id == event2.id\nassert received_events[-7].id == event3.id\nassert received_events[-6].type == "DogRegistered"\nassert received_events[-5].type == "DogLearnedTrick"\nassert received_events[-4].type == "DogLearnedTrick"\nassert received_events[-3].type == "Snapshot"\nassert received_events[-2].type == "DogLearnedTrick"\n\n# Append another event whilst the subscription is running.\nmark = datetime.now()\nevent5 = NewEvent(type=\'OrderUpdated\', data=b\'data5\')\nclient.append_events(\n    stream_name=stream_name2,\n    current_version=0,\n    events=[event5],\n)\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n# Check the last received event is \'event5\'.\nassert received_events[-2].id == event4.id\nassert received_events[-1].id == event5.id\n\n# Stop the subscription.\nsubscription.stop()\nthread.join()\n```\n\nThe example below shows how to start a catch-up subscription to\nreceive from a particular commit position, in this case from the\ncommit position of the last recorded event that was received above.\nAnother event is recorded before the subscription is restarted.\nFurther events are recorded whilst the subscription is running.\nAll the recorded events are received exactly once.\n\n```python\n\n# Append another event.\nevent6 = NewEvent(type=\'OrderDeleted\', data=b\'data6\')\nclient.append_events(\n    stream_name=stream_name2,\n    current_version=1,\n    events=[event6],\n)\n\n# Resume subscribing from the commit position of the last received event.\nsubscription = client.subscribe_all_events(\n    commit_position=received_events[-1].commit_position\n)\n\nmark = datetime.now()\nthread = Thread(target=receive_events)\nthread.start()\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n# Check the last received event was \'event6\'.\nassert received_events[-3].id == event4.id\nassert received_events[-2].id == event5.id\nassert received_events[-1].id == event6.id\n\n# Append three more events to a new stream.\nmark = datetime.now()\nstream_name3 = str(uuid.uuid4())\nevent7 = NewEvent(type=\'OrderCreated\', data=b\'data7\')\nevent8 = NewEvent(type=\'OrderUpdated\', data=b\'data8\')\nevent9 = NewEvent(type=\'OrderDeleted\', data=b\'data9\')\n\nclient.append_events(\n    stream_name=stream_name3,\n    current_version=None,\n    events=[event7, event8, event9],\n)\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n\n# Check all the events have been received exactly once.\nassert received_events[-6].id == event4.id\nassert received_events[-5].id == event5.id\nassert received_events[-4].id == event6.id\nassert received_events[-3].id == event7.id\nassert received_events[-2].id == event8.id\nassert received_events[-1].id == event9.id\n\n# Stop the subscription.\nsubscription.stop()\nthread.join()\n```\n\nThe catch-up subscription call is ended as soon as the subscription object\'s\n`stop()` method is called. This happens automatically when it goes out of scope,\nor when it is explicitly deleted from memory using the Python `del` keyword.\n\n### Subscribe stream events\n\nThe `subscribe_stream_events()` method can be used to start a catch-up subscription\nthat can return events that are recorded in a single stream.\n\nThis method has a required `stream_name` argument, which specifies the name of the\nstream from which recorded events will be received.\n\nThis method also has two optional arguments, `stream_position`, and `timeout`.\n\nThe optional `stream_position` argument specifies a position in the stream from which\nrecorded events will be received. The event at the specified stream position will not\nbe included. The default value of `stream_position` is `None`, which means the\nsubscription will start from the first recorded event in the stream.\n\nThe optional `timeout` argument is a Python `float` that sets\na deadline for the completion of the gRPC operation.\n\nThe example below shows how to start a catch-up subscription from\nthe first recorded event in a stream.\n\n```python\n# Subscribe from the start of \'stream2\'.\nsubscription = client.subscribe_stream_events(stream_name=stream_name2)\n```\n\nThe example below shows how to start a catch-up subscription from\na particular stream position.\n\n```python\n# Subscribe to stream2, from the second recorded event.\nsubscription = client.subscribe_stream_events(\n    stream_name=stream_name2,\n    stream_position=1,\n)\n```\n\n### How to implement exactly-once event processing\n\nThe commit positions of recorded events that are received and processed by a\ndownstream component are usefully recorded by the downstream component, so that\nthe commit position of last processed event can be determined when processing is\nresumed.\n\nThe last recorded commit position can be used to specify the commit position from which\nto subscribe when processing is resumed. Since this commit position will represent the\nposition of the last successfully processed event in a downstream component, so it\nwill be usual to want the next event after this position, because that is the next\nevent that has not yet been processed. For this reason, when subscribing for events\nfrom a specific commit position using a catch-up subscription in EventStoreDB, the\nrecorded event at the specified commit position will NOT be included in the sequence\nof recorded events that are received.\n\nTo accomplish "exactly-once" processing of recorded events in a downstream\ncomponent when using a catch-up subscription, the commit position of a recorded\nevent should be recorded atomically and uniquely along with the result of processing\nrecorded events, for example in the same database as materialised views when\nimplementing eventually-consistent CQRS, or in the same database as a downstream\nanalytics or reporting or archiving application. By recording the commit position\nof recorded events atomically with the new state that results from processing\nrecorded events, "dual writing" in the consumption of recorded events can be\navoided. By also recording the commit position uniquely, the new state cannot be\nrecorded twice, and hence the recorded state of the downstream component will be\nupdated only once for any recorded event. By using the greatest recorded commit\nposition to resume a catch-up subscription, all recorded events will eventually\nbe processed. The combination of the "at-most-once" condition and the "at-least-once"\ncondition gives the "exactly-once" condition.\n\nThe danger with "dual writing" in the consumption of recorded events is that if a\nrecorded event is successfully processed and new state recorded atomically in one\ntransaction with the commit position recorded in a separate transaction, one may\nhappen and not the other. If the new state is recorded but the position is lost,\nand then the processing is stopped and resumed, the recorded event may be processed\ntwice. On the other hand, if the commit position is recorded but the new state is\nlost, the recorded event may effectively not be processed at all. By either\nprocessing an event more than once, or by failing to process an event, the recorded\nstate of the downstream component might be inaccurate, or possibly inconsistent, and\nperhaps catastrophically so. Such consequences may or may not matter in your situation.\nBut sometimes inconsistencies may halt processing until the issue is resolved. You can\navoid "dual writing" in the consumption of events by atomically recording the commit\nposition of a recorded event along with the new state that results from processing that\nevent in the same atomic transaction. By making the recording of the commit positions\nunique, so that transactions will be rolled back when there is a conflict, you will\nprevent the results of any duplicate processing of a recorded event being committed.\n\nRecorded events received from a catch-up subscription cannot be acknowledged back\nto the EventStoreDB server. Acknowledging events, however, is an aspect of "persistent\nsubscriptions". Hoping to rely on acknowledging events to an upstream\ncomponent is an example of dual writing.\n\n\n## Persistent subscriptions\n\nIn EventStoreDB, "persistent" subscriptions are similar to catch-up subscriptions,\nin that reading a persistent subscription will block when there are no more recorded\nevents to be received, and then continue when new events are subsequently recorded.\n\nPersistent subscriptions can\n\nPersistent subscriptions can be consumed by a group of consumers operating with one\nof the supported "consumer strategies".\n\nThe significant different with persistent subscriptions is the server will keep track\nof the progress of the consumers. The consumer of a persistent subscription will\ntherefore need to "acknowledge" when a recorded event has been processed successfully,\nand otherwise "negatively acknowledge" a recorded event that has been received but was\nnot successfully processed.\n\nAll of this means that for persistent subscriptions there are "create", "read", "update"\n"delete", "ack", and "nack" operations to consider.\n\nWhilst there are some advantages of persistent subscriptions, in particular the\nconcurrent processing of recorded events by a group of consumers, by tracking in\nthe server the position in the commit sequence of events that have been processed,\nthe issue of "dual writing" in the consumption of events arises. Reliability in the\nprocessing of recorded events by a group of persistent subscription consumers will\nrely on their idempotent handling of duplicate messages, and their resilience to\nout-of-order delivery.\n\n\n### Create subscription\n\n*requires leader*\n\nThe `create_subscription()` method can be used to create a "persistent subscription"\nto all the recorded events in the database across all streams.\n\nThis method has a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription.\n\nThis method also has seven optional arguments, `from_end`, `commit_position`,\n`filter_exclude`, `filter_include`, `filter_by_stream_name`, `consumer_strategy`,\nand `timeout`.\n\nThe optional `from_end` argument can be used to specify that the group of consumers\nof the subscription should only receive events that were recorded after the subscription\nwas created.\n\nAlternatively, the optional `commit_position` argument can be used to specify a commit\nposition from which commit position the group of consumers of the subscription should\nreceive events. Please note, the recorded event at the specified commit position might\nbe included in the recorded events received by the group of consumers.\n\nIf neither `from_end` or `commit_position` are specified, the group of consumers\nof the subscription will potentially receive all recorded events in the database.\n\nThe optional `filter_exclude` argument is a sequence of regular expressions that\nspecifies which recorded events should be returned. This argument is ignored\nif `filter_include` is set to a non-empty sequence. The default value of this\nargument matches the event types of EventStoreDB "system events", so that system\nevents will not normally be included. See the Notes section below for more\ninformation about filter expressions.\n\nThe optional `filter_include` argument is a sequence of regular expressions\nthat specifies which recorded events should be returned. By default, this\nargument is an empty tuple. If this argument is set to a non-empty sequence,\nthe `filter_exclude` argument is ignored.\n\nThe optional `filter_by_stream_name` argument is a Python `bool` that indicates\nwhether the filtering will apply to event types or stream names. By default, this\nvalue is `False` and so the filtering will apply to the event type strings of\nrecorded events.\n\nThe optional `consumer_strategy` argument is a Python `str` that defines\nthe consumer strategy for this persistent subscription. The value of this argument\ncan be `\'DispatchToSingle\'`, `\'RoundRobin\'`, `\'Pinned\'`, or `\'PinnedByCorrelation\'`. The\ndefault value is `\'DispatchToSingle\'`.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe method `create_subscription()` does not return a value. Recorded events are\nobtained by calling the `read_subscription()` method.\n\nIn the example below, a persistent subscription is created to operate from the\nfirst recorded non-system event in the database.\n\n```python\n# Create a persistent subscription.\ngroup_name1 = f"group-{uuid.uuid4()}"\nclient.create_subscription(group_name=group_name1)\n```\n\n### Read subscription\n\n*requires leader*\n\nThe `read_subscription()` method can be used by a group of consumers to receive\nrecorded events from a persistent subscription that has been created using\nthe `create_subscription()` method.\n\nThis method has a required `group_name` argument, which is\nthe name of a "group" of consumers of the subscription specified\nwhen `create_subscription()` was called.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method returns a `PersistentSubscription` object, which is an iterator\ngiving `RecordedEvent` objects. It also has `ack()`, `nack()` and `stop()`\nmethods.\n\n```python\nsubscription = client.read_subscription(group_name=group_name1)\n```\n\nThe `ack()` method should be used by a consumer to indicate to the server that it\nhas received and successfully processed a recorded event. This will prevent that\nrecorded event being received by another consumer in the same group. The `ack()`\nmethod takes an `event_id` argument, which is the ID of the recorded event that\nhas been received.\n\nThe example below iterates over the subscription object, and calls `ack()`. The\n`stop()` method is called when we have received the last event, so that we can\ncontinue with the examples below.\n\n```python\nevents = []\nfor event in subscription:\n    events.append(event)\n\n    # Acknowledge the received event.\n    subscription.ack(event_id=event.id)\n\n    # Stop when \'event9\' has been received.\n    if event.id == event9.id:\n        subscription.stop()\n```\n\nThe received events are the events we appended above.\n\n```python\nassert events[-14].id == event1.id\nassert events[-13].id == event2.id\nassert events[-12].id == event3.id\nassert events[-11].type == "DogRegistered"\nassert events[-10].type == "DogLearnedTrick"\nassert events[-9].type == "DogLearnedTrick"\nassert events[-8].type == "Snapshot"\nassert events[-7].type == "DogLearnedTrick"\nassert events[-6].id == event4.id\nassert events[-5].id == event5.id\nassert events[-4].id == event6.id\nassert events[-3].id == event7.id\nassert events[-2].id == event8.id\nassert events[-1].id == event9.id\n```\n\nThe `PersistentSubscription` object also has an `nack()` method that should be used\nby a consumer to negatively acknowledge to the server that it has received but not\nsuccessfully processed a recorded event. The `nack()` method takes an `event_id`\nargument, which is the ID of the recorded event that has been received, and an `action`\nargument, which should be a Python `str`, either `\'unknown\'`, `\'park\'`, `\'retry\'`,\n`\'skip\'` or `\'stop\'`.\n\n\n### How to write a persistent subscription consumer\n\nThe reading of a persistent subscription can be encapsulated in a "consumer" that calls\na "policy" function when a recorded event is received and then automatically calls\n`ack()` if the policy function returns normally, and `nack()` if it raises an exception,\nperhaps retrying the event for a certain number of times before parking the event.\n\nThe simple example below shows how this might be done. We can see that \'event9\' is\nacknowledged before \'event5\' is finally parked.\n\n\n```python\nacked_events = {}\nnacked_events = {}\n\n\nclass ExampleConsumer:\n    def __init__(self, subscription, max_retries, final_action):\n        self.subscription = subscription\n        self.max_retries = max_retries\n        self.final_action = final_action\n        self.error = None\n\n    def run(self):\n        try:\n            for event in self.subscription:\n                try:\n                    self.policy(event)\n                except Exception:\n                    if event.retry_count < self.max_retries:\n                        action = "retry"\n                    else:\n                        action = self.final_action\n                    self.subscription.nack(event.id, action=action)\n                    self.after_nack(event, action)\n                else:\n                    self.subscription.ack(event.id)\n                    self.after_ack(event)\n        except Exception:\n            self.subscription.stop()\n            raise\n\n    def stop(self):\n        self.subscription.stop()\n\n    def policy(self, event):\n        # Raise an exception when we see "event5".\n        if event.id == event5.id:\n            raise Exception()\n\n    def after_ack(self, event):\n        # Track retry count of acked events.\n        acked_events[event.id] = event.retry_count\n\n    def after_nack(self, event, action):\n        # Track retry count of nacked events.\n        nacked_events[event.id] = event.retry_count\n\n        if action == self.final_action:\n            # Stop the consumer, so we can continue with the examples.\n            self.stop()\n\n\n# Create subscription.\ngroup_name = f"group-{uuid.uuid4()}"\nclient.create_subscription(group_name, commit_position=commit_position1)\n\n# Read subscription.\nsubscription = client.read_subscription(group_name)\n\n# Construct consumer.\nconsumer = ExampleConsumer(\n    subscription=subscription,\n    max_retries=5,\n    final_action="park",\n)\n\n# Run consumer.\nconsumer.run()\n\n# Check \'event9\' was acked and never retried.\nassert acked_events[event9.id] == 0\nassert event9.id not in nacked_events\n\n# Check \'event5\' was retried five times and never acked.\nassert nacked_events[event5.id] == 5\nassert event5.id not in acked_events\n```\n\n### Get subscription info\n\n*requires leader*\n\nThe `get_subscription_info()` method can be used to get information for a\npersistent subscription.\n\nThis method has one required argument, `group_name`, which\nshould match the value of the argument used when calling `create_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscription_info = client.get_subscription_info(\n    group_name=group_name1,\n)\n```\n\nThe returned value is a `SubscriptionInfo` object.\n\n### List subscriptions\n\n*requires leader*\n\nThe `list_subscriptions()` method can be used to get information for all\nexisting persistent subscriptions.\n\nThis method has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscriptions = client.list_subscriptions()\n```\n\nThe returned value is a list of `SubscriptionInfo` objects.\n\n### Update subscription\n\n*requires leader*\n\nThe `update_subscription()` method can be used to update a\n"persistent subscription".\n\nThis method has a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription.\n\nThis method also has three optional arguments, `from_end`, `commit_position`,\nand `timeout`.\n\nThe optional `from_end` argument can be used to specify that the group of consumers\nof the subscription should only receive events that were recorded after the subscription\nwas updated.\n\nAlternatively, the optional `commit_position` argument can be used to specify a commit\nposition from which commit position the group of consumers of the subscription should\nreceive events. Please note, the recorded event at the specified commit position might\nbe included in the recorded events received by the group of consumers.\n\nIf neither `from_end` or `commit_position` are specified, the group of consumers\nof the subscription will potentially receive all recorded events in the database.\n\nPlease note, the filter options and consumer strategy cannot be adjusted.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe method `update_subscription()` does not return a value.\n\nIn the example below, a persistent subscription is updated to run from the end of the\ndatabase.\n\n```python\n# Create a persistent subscription.\nclient.update_subscription(group_name=group_name1, from_end=True)\n```\n\n### Create stream subscription\n\n*requires leader*\n\nThe `create_stream_subscription()` method can be used to create a persistent\nsubscription for a stream.\n\nThis method has two required arguments, `group_name` and `stream_name`. The\n`group_name` argument names the group of consumers that will receive events\nfrom this subscription. The `stream_name` argument specifies which stream\nthe subscription will follow. The values of both these arguments are expected\nto be Python `str` objects.\n\nThe method also has four optional arguments, `stream_position`, `from_end`,\n`consumer_strategy`, and `timeout`.\n\nThis optional `stream_position` argument specifies a stream position from\nwhich to subscribe. The recorded event at this stream\nposition will be received when reading the subscription.\n\nThis optional `from_end` argument is a Python `bool`.\nBy default, the value of this argument is `False`. If this argument is set\nto `True`, reading from the subscription will receive only events\nrecorded after the subscription was created. That is, it is not inclusive\nof the current stream position.\n\nThe optional `consumer_strategy` argument is a Python `str` that defines\nthe consumer strategy for this persistent subscription. The value of this argument\ncan be `\'DispatchToSingle\'`, `\'RoundRobin\'`, `\'Pinned\'`, or `\'PinnedByCorrelation\'`. The\ndefault value is `\'DispatchToSingle\'`.\n\nThis method also takes an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method does not return a value. Events can be received by calling\n`read_stream_subscription()`.\n\nThe example below creates a persistent stream subscription from the start of the stream.\n\n```python\n# Create a persistent stream subscription from start of the stream.\ngroup_name2 = f"group-{uuid.uuid4()}"\nclient.create_stream_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\n### Read stream subscription\n\n*requires leader*\n\nThe `read_stream_subscription()` method can be used to read a persistent\nstream subscription.\n\nThis method has two required arguments, `group_name` and `stream_name`, which\nshould match the values of arguments used when calling `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method returns a `PersistentSubscription` object, which is an iterator\ngiving `RecordedEvent` objects, that also has `ack()`, `nack()` and `stop()`\nmethods.\n\n```python\nsubscription = client.read_stream_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\nThe example below iterates over the subscription object, and calls `ack()`.\nThe for loop breaks when we have received the last event in the stream, so\nthat we can finish the examples in this documentation.\n\n```python\nevents = []\nfor event in subscription:\n    events.append(event)\n\n    # Acknowledge the received event.\n    subscription.ack(event_id=event.id)\n\n    # Stop when \'event6\' has been received.\n    if event.id == event6.id:\n        subscription.stop()\n```\n\nWe can check we received all the events that were appended to `stream_name2`\nin the examples above.\n\n```python\nassert len(events) == 3\nassert events[0].stream_name == stream_name2\nassert events[0].id == event4.id\nassert events[1].stream_name == stream_name2\nassert events[1].id == event5.id\nassert events[2].stream_name == stream_name2\nassert events[2].id == event6.id\n```\n\n### Get stream subscription info\n\n*requires leader*\n\nThe `get_stream_subscription_info()` method can be used to get information for a\npersistent subscription for a stream.\n\nThis method has two required arguments, `group_name` and `stream_name`, which\nshould match the values of arguments used when calling `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscription_info = client.get_stream_subscription_info(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\nThe returned value is a `SubscriptionInfo` object.\n\n\n### List stream subscriptions\n\n*requires leader*\n\nThe `list_stream_subscriptions()` method can be used to get information for all\nthe persistent subscriptions for a stream.\n\nThis method has one required argument, `stream_name`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscriptions = client.list_stream_subscriptions(\n    stream_name=stream_name2,\n)\n```\n\nThe returned value is a list of `SubscriptionInfo` objects.\n\n### Update stream subscription\n\n*requires leader*\n\nThe `update_stream_subscription()` method can be used to update a\npersistent subscription for a stream.\n\nThis method has a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription, and a required\n`stream_name` argument, which is the name of a stream.\n\nThis method also has three optional arguments, `from_end`, `stream_position`,\nand `timeout`.\n\nThe optional `from_end` argument can be used to specify that the group of consumers\nof the subscription should only receive events that were recorded after the subscription\nwas updated.\n\nAlternatively, the optional `stream_position` argument can be used to specify a stream\nposition from which commit position the group of consumers of the subscription should\nreceive events. Please note, the recorded event at the specified stream position might\nbe included in the recorded events received by the group of consumers.\n\nIf neither `from_end` or `commit_position` are specified, the group of consumers\nof the subscription will potentially receive all recorded events in the stream.\n\nPlease note, the consumer strategy cannot be adjusted.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe `update_stream_subscription()` method does not return a value.\n\nIn the example below, a persistent subscription for a stream is updated to run from the\nend of the stream.\n\n```python\n# Create a persistent subscription.\nclient.update_stream_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n    from_end=True,\n)\n```\n\n### Replay parked events\n\n*requires leader*\n\nThe `replay_parked_events()` method can be used to "replay" events that have\nbeen "parked" (negatively acknowledged with the action `\'park\'`) when reading\na persistent subscription. Parked events will then be received by the consumers\nreading from the persistent subscription.\n\nThis method has one required argument, `group_name`. It has one optional argument,\n`stream_name`. The values of these arguments should match those used when calling\n`create_subscription()` or `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe example below replays parked events for group `group_name1`.\n\n```python\nclient.replay_parked_events(\n    group_name=group_name1,\n)\n```\n\nThe example below replays parked events for group `group_name2`.\n\n```python\nclient.replay_parked_events(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\n### Delete persistent subscription\n\n*requires leader*\n\nThe `delete_persistent_subscription()` method can be used to delete a persistent\nsubscription.\n\nThis method has one required argument, `group_name`. It has one optional argument,\n`stream_name`. The values of these arguments should match those used when calling\n`create_subscription()` or `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe example below deletes the subscription for group `group_name1` which was created\nby calling `create_subscription()`.\n\n```python\nclient.delete_persistent_subscription(\n    group_name=group_name1,\n)\n```\n\nThe example below deletes the subscription for group `group_name2` which was created\nby calling `create_stream_subscription()`.\n\n```python\nclient.delete_persistent_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\n## Connection\n\n### Reconnect\n\nThe `reconnect()` method can be used to manually reconnect the client to a\nsuitable EventStoreDB node. This method uses the same routine for reading the\ncluster node states and then connecting to a suitable node according to the\nclient\'s node preference that is specified in the connection string URI when\nthe client is constructed. This method is thread-safe, in that when it is called\nby several threads at the same time, only one reconnection will occur. Concurrent\nattempts to reconnect will block until the client has reconnected successfully,\nand then they will all return normally.\n\n```python\nclient.reconnect()\n```\n\nAn example of when it might be desirable to reconnect manually is when (for performance\nreasons) the client\'s node preference is to be connected to a follower node in the\ncluster, and, after a cluster leader election, the follower becomes the leader.\nReconnecting to a follower node in this case is currently beyond the capabilities of\nthis client, but this behavior might be implemented in a future release.\n\nPlease note, nearly all the client methods are decorated with `@autoreconnect` (which\ncalls the `reconnect()` method when the client detects that reconnecting is required)\nand a `@retry` decorator that more generally will retry operations that fail due to\nconnection issues.\n\nThe `@autoreconnect` decorator will reconnect to a suitable node in the cluster when\nthe server to which the client has been connected has become unavailable, or when the\nclient\'s gRPC channel happens to have been closed. The client will also reconnect when\na method is called that requires a leader, and the client\'s node preference is to be\nconnected to a leader, but the node that the client has been connected to stops being\nthe leader. In this case, the client will reconnect to the current leader. After\nreconnecting, the failed operation will be retried.\n\nThe `@retry` decorator retries operations that have failed due to more general\nconnection issues, such as a deadline being reached (so that the operation times\nout), or in case the server throws an exception when handling a client request.\n\nPlease also note, the aspects not covered by the reconnect and retry decorator\nbehaviours have to do with methods that return iterators. For example, consider\nthe "read response" iterator returned from the `read_all_events()` method. The\n`read_all_events()` method will have returned, and the method decorators will therefore\nhave exited, before iterating over the "read response" begins. Therefore, if a\nconnection issues occurs whilst iterating over the "read response", it isn\'t possible\nfor any decorator on the `read_all_events()` method to trigger a reconnection.\n\nAnother example is iterating over the "read response" from a catch-up subscription.\nAlthough, with these methods there is an initial "confirmation" response from the server\nwhich is received and checked by the client before the method returns the\n"read response" iterator. And so, when the call is made, if the server is unavailable,\nor if the channel has somehow been closed, then the client will reconnect and retry.\nHowever, if an event-processing component that is iterating over a successfully returned\ncatch-up subscription "read response" somehow fails, the catch-up subscription will\nneed to be restarted, using the event-processing component\'s "last saved commit position".\nThis is completely safe, so long as the event-processing component has been recording\nthe commit position of each recorded event atomically and uniquely along with any new\nstate that results from processing the recorded events and the commit positions are\nrecorded with a uniqueness constraint. In this case, the client will automatically\nreconnect to a node in the cluster when the subsequent call to a catch-up subscription\nmethod is made. Similarly, when reading persistent subscriptions, if there are\nconnectivity issues after you have started iterating over a successfully received\nresponse, then the consumer will need to be restarted.\n\n\n### Close\n\nThe `close()` method can be used to cleanly close the client\'s gRPC connection.\n\n```python\nclient.close()\n```\n\n\n## Asyncio client\n\nThe `esdbclient` package also includes an early version of an asynchronous I/O\ngRPC Python client. It follows exactly the same behaviors as the multithreaded\n`ESDBClient`, but uses the `grpc.aio` package and the `asyncio` module, instead of\n`grpc` and `threading`.\n\nThe async function `AsyncioESDBClient` constructs the client, and connects to\na server. It can be imported from `esdbclient`, and can be called with the same\narguments as `ESDBClient`. It supports both the "esdb" and the "esdb+discover"\nconnection string URI schemes, and can connect to both "secure" and "insecure"\nEventStoreDB servers. It reconnects or retries when connection issues or server\nerrors are encountered.\n\n```python\nfrom esdbclient import AsyncioESDBClient\n```\n\nThe asynchronous I/O client has the following methods: `append_events()`,\n`read_stream_events()`, `read_all_events()`, `subscribe_all_events()`,\n`delete_stream()`, `tombstone_stream()`, and `reconnect()`.\n\nThese methods are equivalent to the methods on `ESDBClient`. They have the same\nmethod signatures, and can be called with the same arguments, to the same effect.\nThe methods which appear on `ESDBClient` but not on `AsyncioESDBClient` will be\nadded soon.\n\n### Synopsis\n\nThe example below demonstrates the `append_events()`, `read_stream_events()` and\n`subscribe_all_events()` methods. These are the most useful methods for writing\nan event-sourced application, allowing new aggregate events to be recorded, the\nrecorded events of an aggregate to be obtained so aggregates can be reconstructed,\nand the state of an application to propagated and processed with "exactly-once"\nsemantics.\n\n```python\nimport asyncio\n\nasync def demonstrate_asyncio_client():\n\n    # Construct client.\n    client = await AsyncioESDBClient(\n        uri=os.getenv("ESDB_URI"),\n        root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),\n    )\n\n    # Append events.\n    stream_name = str(uuid.uuid4())\n    event1 = NewEvent("OrderCreated", data=b\'{}\')\n    event2 = NewEvent("OrderUpdated", data=b\'{}\')\n    event3 = NewEvent("OrderDeleted", data=b\'{}\')\n\n    commit_position = await client.append_events(\n        stream_name=stream_name,\n        current_version=None,\n        events=[event1, event2, event3]\n    )\n\n    # Read stream events.\n    recorded = await client.read_stream_events(stream_name)\n    assert len(recorded) == 3\n    assert recorded[0].id == event1.id\n    assert recorded[1].id == event2.id\n    assert recorded[2].id == event3.id\n\n\n    # Subscribe all events.\n    received = []\n    async for event in await client.subscribe_all_events():\n        received.append(event)\n        if event.commit_position == commit_position:\n            break\n    assert received[-3].id == event1.id\n    assert received[-2].id == event2.id\n    assert received[-1].id == event3.id\n\n\n    # Close the client.\n    await client.close()\n\n\n# Run the demo.\nasyncio.get_event_loop().run_until_complete(\n    demonstrate_asyncio_client()\n)\n```\n\n## Notes\n\n### Regular expression filters\n\nThe `read_all_events()`, `subscribe_all_events()`, `create_subscription()`\nand `get_commit_position()` methods have `filter_exclude` and `filter_include`\narguments. This section provides some more details about the values of these\narguments.\n\nThe default value of the `filter_exclude` arguments is designed to exclude\nEventStoreDB "system" and "persistence subscription config" events, which\notherwise would be included.\n\nSystem events generated by EventStoreDB have `type` strings that start with\nthe `$` sign. Persistence subscription events generated when manipulating\npersistence subscriptions have `type` strings that start with `PersistentConfig`.\n\nFor example, to match the type of EventStoreDB system events, use the regular\nexpression string `r\'\\$.+\'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is\nset to this value. You can import this constant from `esdbclient` and use it when\nbuilding longer sequences of regular expressions.\n\nSimilarly, to match the type of EventStoreDB persistence subscription events, use the\nregular expression `r\'PersistentConfig\\d+\'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`\nis set to this value. You can import this constant from `esdbclient`  and use it when\nbuilding longer sequences of regular expressions.\n\nThe constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that includes\nboth `ESDB_SYSTEM_EVENTS_REGEX` and `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`. It is used\nas the default value of `filter_exclude` so that the events that EventStoreDB generates\ninternally are excluded by default, events other than to those which you record using\nthe `append_events()` method.\n\nIf you want to exclude, for example, snapshots from the recorded events returned when\nreading events from the database, then you may wish to use a appropriately extended\ncopy of `DEFAULT_EXCLUDE_FILTER` as the value of the `filter_exclude` arguments.\n\n\n## Contributors\n\n### Install Poetry\n\nThe first thing is to check you have Poetry installed.\n\n    $ poetry --version\n\nIf you don\'t, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\n    $ curl -sSL https://install.python-poetry.org | python3 -\n\nIt will help to make sure Poetry\'s bin directory is in your `PATH` environment variable.\n\nBut in any case, make sure you know the path to the `poetry` executable. The Poetry\ninstaller tells you where it has been installed, and how to configure your shell.\n\nPlease refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on\nusing Poetry.\n\n### Setup for PyCharm users\n\nYou can easily obtain the project files using PyCharm (menu "Git > Clone...").\nPyCharm will then usually prompt you to open the project.\n\nOpen the project in a new window. PyCharm will then usually prompt you to create\na new virtual environment.\n\nCreate a new Poetry virtual environment for the project. If PyCharm doesn\'t already\nknow where your `poetry` executable is, then set the path to your `poetry` executable\nin the "New Poetry Environment" form input field labelled "Poetry executable". In the\n"New Poetry Environment" form, you will also have the opportunity to select which\nPython executable will be used by the virtual environment.\n\nPyCharm will then create a new Poetry virtual environment for your project, using\na particular version of Python, and also install into this virtual environment the\nproject\'s package dependencies according to the project\'s `poetry.lock` file.\n\nYou can add different Poetry environments for different Python versions, and switch\nbetween them using the "Python Interpreter" settings of PyCharm. If you want to use\na version of Python that isn\'t installed, either use your favourite package manager,\nor install Python by downloading an installer for recent versions of Python directly\nfrom the [Python website](https://www.python.org/downloads/).\n\nOnce project dependencies have been installed, you should be able to run tests\nfrom within PyCharm (right-click on the `tests` folder and select the \'Run\' option).\n\nBecause of a conflict between pytest and PyCharm\'s debugger and the coverage tool,\nyou may need to add ``--no-cov`` as an option to the test runner template. Alternatively,\njust use the Python Standard Library\'s ``unittest`` module.\n\nYou should also be able to open a terminal window in PyCharm, and run the project\'s\nMakefile commands from the command line (see below).\n\n### Setup from command line\n\nObtain the project files, using Git or suitable alternative.\n\nIn a terminal application, change your current working directory\nto the root folder of the project files. There should be a Makefile\nin this folder.\n\nUse the Makefile to create a new Poetry virtual environment for the\nproject and install the project\'s package dependencies into it,\nusing the following command.\n\n    $ make install-packages\n\nIt\'s also possible to also install the project in \'editable mode\'.\n\n    $ make install\n\nPlease note, if you create the virtual environment in this way, and then try to\nopen the project in PyCharm and configure the project to use this virtual\nenvironment as an "Existing Poetry Environment", PyCharm sometimes has some\nissues (don\'t know why) which might be problematic. If you encounter such\nissues, you can resolve these issues by deleting the virtual environment\nand creating the Poetry virtual environment using PyCharm (see above).\n\n### Project Makefile commands\n\nYou can start EventStoreDB using the following command.\n\n    $ make start-eventstoredb\n\nYou can run tests using the following command (needs EventStoreDB to be running).\n\n    $ make test\n\nYou can stop EventStoreDB using the following command.\n\n    $ make stop-eventstoredb\n\nYou can check the formatting of the code using the following command.\n\n    $ make lint\n\nYou can reformat the code using the following command.\n\n    $ make fmt\n\nTests belong in `./tests`. Code-under-test belongs in `./esdbclient`.\n\nEdit package dependencies in `pyproject.toml`. Update installed packages (and the\n`poetry.lock` file) using the following command.\n\n    $ make update-packages\n',
+    'long_description': '# Python gRPC Client for EventStoreDB\n\nThis [Python package](https://pypi.org/project/esdbclient/) provides a Python\ngRPC client for the [EventStoreDB](https://www.eventstore.com/) database.\n\nThis client has been developed in collaboration with the EventStoreDB\nteam. Although not all the features of EventStoreDB are supported\nby this client, many of the most useful features are presented\nin an easy-to-use interface.\n\nThis client has been tested to work with EventStoreDB LTS versions 21.10,\nwithout and without SSL/TLS, and with Python versions 3.7 to 3.11. There\nis 100% test coverage. The code has typing annotations, checked with mypy.\nThe code is formatted with black and isort, and checked with flake8. Poetry\nis used for package management during development, and for building and\npublishing distributions to [PyPI](https://pypi.org/project/esdbclient/).\n\n## Synopsis\n\nYou can connect to an EventStoreDB database using the `EventStoreDBClient` class.\n\nThe `EventStoreDBClient` class can be imported from the `esdbclient` package.\n\nProbably the three most useful methods of `EventStoreDBClient` are:\n\n* `append_to_stream()` This method can be used to record new events in a particular\n"stream". This is useful, for example, when executing a command in an application\nthat mutates an aggregate. This method is "atomic" in that either all or none of\nthe events will be recorded.\n\n* `read_stream()` This method can be used to retrieve all the recorded\nevents in a "stream". This is useful, for example, when reconstructing\nan aggregate from recorded events before executing a command in an\napplication that creates new events.\n\n* `subscribe_to_all()` This method can be used to receive all recorded events in\nthe database. This is useful, for example, in event-processing components because\nit supports processing events with "exactly-once" semantics.\n\nThe example below uses an "insecure" EventStoreDB server running locally on port 2114.\n\n```python\nimport uuid\n\nfrom esdbclient import EventStoreDBClient, NewEvent, StreamState\n\n\n# Construct EventStoreDBClient with an EventStoreDB URI.\n\nclient = EventStoreDBClient(\n    uri="esdb://localhost:2114?Tls=false"\n)\n\n\n# Generate new events. Typically, domain events of different\n# types are generated in a domain model, and then serialized\n# into NewEvent objects. An aggregate ID may be used as the\n# name of a stream in EventStoreDB.\n\nstream_name1 = str(uuid.uuid4())\nevent1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'{"order_number": "123456"}\'\n)\nevent2 = NewEvent(\n    type=\'OrderSubmitted\',\n    data=b\'{}\'\n)\nevent3 = NewEvent(\n    type=\'OrderCancelled\',\n    data=b\'{}\'\n)\n\n\n# Append new events to a new stream. The value returned\n# from the append_to_stream() method is the overall\n# "commit position" in the database of the last new event\n# recorded by this operation. The returned "commit position"\n# may be used in a user interface to poll an eventually\n# consistent event-processing component until it can\n# present an up-to-date materialized view. New events are\n# each allocated a "stream position", which is the next\n# available position in the stream, starting from 0.\n\ncommit_position1 = client.append_to_stream(\n    stream_name=stream_name1,\n    current_version=StreamState.NO_STREAM,\n    events=[event1, event2],\n)\n\n# Append events to an existing stream. The "current version"\n# is the "stream position" of the last recorded event in a\n# stream. We have recorded two new events, so the "current\n# version" is 1. The exception \'WrongCurrentVersion\' will be\n# raised if an incorrect value is given.\n\ncommit_position2 = client.append_to_stream(\n    stream_name=stream_name1,\n    current_version=1,\n    events=[event3],\n)\n\n# - allocated commit positions increase monotonically\nassert commit_position2 > commit_position1\n\n\n# Read events from a stream. This method returns a\n# "read response" iterator, which returns recorded\n# events. The iterator will stop when there are no\n# more events to be returned.\n\nread_response = client.read_stream(\n    stream_name=stream_name1\n)\n\n# Iterate over "read response" to get recorded events.\n# The recorded events may be deserialized to domain event\n# objects of different types and used to reconstruct an\n# aggregate in a domain model.\nrecorded_events = tuple(read_response)\n\n# - stream \'stream_name1\' now has three events\nassert len(recorded_events) == 3\n\n# - allocated stream positions are zero-based and gapless\nassert recorded_events[0].stream_position == 0\nassert recorded_events[1].stream_position == 1\nassert recorded_events[2].stream_position == 2\n\n# - event attribute values are recorded faithfully\nassert recorded_events[0].type == "OrderCreated"\nassert recorded_events[0].data == b\'{"order_number": "123456"}\'\nassert recorded_events[0].id == event1.id\n\nassert recorded_events[1].type == "OrderSubmitted"\nassert recorded_events[1].data == b\'{}\'\nassert recorded_events[1].id == event2.id\n\nassert recorded_events[2].type == "OrderCancelled"\nassert recorded_events[2].data == b\'{}\'\nassert recorded_events[2].id == event3.id\n\n\n# Start a catch-up subscription from last recorded position.\n# This method returns a "catch-up subscription" iterator,\n# which returns recorded events. The iterator will not stop\n# when there are no more recorded events to be returned, but\n# will block, and continue when further events are recorded.\n\ncatchup_subscription = client.subscribe_to_all()\n\n\n# Iterate over the catch-up subscription. Process each recorded\n# event in turn. Within an atomic database transaction, record\n# the event\'s "commit position" along with any new state generated\n# by processing the event. Use the component\'s last recorded commit\n# position when restarting the catch-up subscription.\n\nreceived_events = []\nfor event in catchup_subscription:\n    received_events.append(event)\n\n    if event.commit_position == commit_position2:\n        # Break so we can continue with the example.\n        break\n\n\n# - events are received in the order they were recorded\nassert received_events[-3].type == "OrderCreated"\nassert received_events[-3].data == b\'{"order_number": "123456"}\'\nassert received_events[-3].id == event1.id\n\nassert received_events[-2].type == "OrderSubmitted"\nassert received_events[-2].data == b\'{}\'\nassert received_events[-2].id == event2.id\n\nassert received_events[-1].type == "OrderCancelled"\nassert received_events[-1].data == b\'{}\'\nassert received_events[-1].id == event3.id\n\n\n# Stop the catch-up subscription iterator.\n\ncatchup_subscription.stop()\n\n\n# Close the client\'s gRPC connection.\n\nclient.close()\n```\n\nSee below for more details.\n\nFor an example of usage, see the [eventsourcing-eventstoredb](\nhttps://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.\n\n## Table of contents\n\n<!-- TOC -->\n* [Install package](#install-package)\n  * [From PyPI](#from-pypi)\n  * [With Poetry](#with-poetry)\n* [EventStoreDB server](#eventstoredb-server)\n  * [Run container](#run-container)\n  * [Stop container](#stop-container)\n* [EventStoreDB client](#eventstoredb-client)\n  * [Import class](#import-class)\n  * [Construct client](#construct-client)\n* [Connection strings](#connection-strings)\n  * [Two schemes](#two-schemes)\n  * [User info string](#user-info-string)\n  * [Query string](#query-string)\n  * [Examples](#examples)\n* [Event objects](#event-objects)\n  * [New events](#new-events)\n  * [Recorded events](#recorded-events)\n* [Streams](#streams)\n  * [Append events](#append-events)\n  * [Append event](#append-event)\n  * [Idempotent append operations](#idempotent-append-operations)\n  * [Read stream events](#read-stream-events)\n  * [Get current version](#get-current-version)\n  * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)\n  * [Read all events](#read-all-events)\n  * [Get commit position](#get-commit-position)\n  * [Get stream metadata](#get-stream-metadata)\n  * [Set stream metadata](#set-stream-metadata)\n  * [Delete stream](#delete-stream)\n  * [Tombstone stream](#tombstone-stream)\n* [Catch-up subscriptions](#catch-up-subscriptions)\n  * [Subscribe to all events](#subscribe-to-all-events)\n  * [Subscribe to stream events](#subscribe-to-stream-events)\n  * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)\n* [Persistent subscriptions](#persistent-subscriptions)\n  * [Create subscription](#create-subscription)\n  * [Read subscription](#read-subscription)\n  * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)\n  * [Get subscription info](#get-subscription-info)\n  * [List subscriptions](#list-subscriptions)\n  * [Update subscription](#update-subscription)\n  * [Create stream subscription](#create-stream-subscription)\n  * [Read stream subscription](#read-stream-subscription)\n  * [Get stream subscription info](#get-stream-subscription-info)\n  * [List stream subscriptions](#list-stream-subscriptions)\n  * [Update stream subscription](#update-stream-subscription)\n  * [Replay parked events](#replay-parked-events)\n  * [Delete persistent subscription](#delete-persistent-subscription)\n* [Connection](#connection)\n  * [Reconnect](#reconnect)\n  * [Close](#close)\n* [Asyncio client](#asyncio-client)\n  * [Synopsis](#synopsis-1)\n* [Notes](#notes)\n  * [Regular expression filters](#regular-expression-filters)\n  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)\n* [Contributors](#contributors)\n  * [Install Poetry](#install-poetry)\n  * [Setup for PyCharm users](#setup-for-pycharm-users)\n  * [Setup from command line](#setup-from-command-line)\n  * [Project Makefile commands](#project-makefile-commands)\n<!-- TOC -->\n\n## Install package\n\nIt is recommended to install Python packages into a Python virtual environment.\n\n### From PyPI\n\nYou can use pip to install this package directly from\n[the Python Package Index](https://pypi.org/project/esdbclient/).\n\n    $ pip install esdbclient\n\n### With Poetry\n\nYou can use Poetry to add this package to your pyproject.toml and install it.\n\n    $ poetry add esdbclient\n\n## EventStoreDB server\n\nThe EventStoreDB server can be run locally using the official Docker container image.\n\n### Run container\n\nFor development, you can run a "secure" EventStoreDB server using the following command.\n\n    $ docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:21.10.9-buster-slim --dev\n\nAs we will see, your client will need an EventStoreDB connection string URI as the value\nof its `uri` constructor argument. The connection string for this "secure" EventStoreDB\nserver would be:\n\n    esdb://admin:changeit@localhost:2113\n\nTo connect to a "secure" server, you will usually need to include a "username"\nand a "password" in the connection string, so that the server can authenticate the\nclient. With EventStoreDB, the default username is "admin" and the default password\nis "changeit".\n\nWhen connecting to a "secure" server, your client will also need an SSL/TLS certificate\nas the value of its `root_certificates` constructor argument. The client uses the\nSSL/TLS certificate to authenticate the server. For development, you can either use the\nSSL/TLS certificate of the certificate authority used to create the server\'s certificate,\nor when using a single-node cluster, you can use the server certificate itself. You can\nget the server certificate with the following Python code.\n\n\n```python\nimport ssl\n\nserver_certificate = ssl.get_server_certificate(addr=(\'localhost\', 2113))\n```\n\nYou can also start an "insecure" server using the following command.\n\n    $ docker run -d --name eventstoredb-insecure -it -p 2114:2113 eventstore/eventstore:21.10.9-buster-slim --insecure\n\nThe connection string URI for this "insecure" server would be:\n\n    esdb://localhost:2114?Tls=false\n\nAs we will see, when connecting to an "insecure" server, there is no need to include\na "username" and a "password" in the connection string. If you do, these values will\nbe ignored by the client, so that they are not sent over an insecure channel.\n\nPlease note, the "insecure" connection string uses a query string with the field-value\n`Tls=false`. The value of this field is by default `true`.\n\n### Stop container\n\nTo stop and remove the "secure" container, use the following Docker commands.\n\n    $ docker stop eventstoredb-secure\n\t$ docker rm eventstoredb-secure\n\nTo stop and remove the "insecure" container, use the following Docker commands.\n\n    $ docker stop eventstoredb-insecure\n\t$ docker rm eventstoredb-insecure\n\n\n## EventStoreDB client\n\nThis EventStoreDB client is implemented in the `esdbclient` package with\nthe `EventStoreDBClient` class.\n\n### Import class\n\nThe `EventStoreDBClient` class can be imported from the `esdbclient` package.\n\n```python\nfrom esdbclient import EventStoreDBClient\n```\n\n### Construct client\n\nThe `EventStoreDBClient` class has one required constructor argument, `uri`, and one\noptional constructor argument, `root_certificates`.\n\nThe `uri` argument is expected to be an EventStoreDB connection string URI that\nconforms with the standard EventStoreDB "esdb" or "esdb+discover" URI schemes.\n\nFor example, the following connection string specifies that the client should\nattempt to create a "secure" connection to port 2113 on "localhost", and use the\nclient credentials "username" and "password" when making calls to the server.\n\n    esdb://username:password@localhost:2113?Tls=true\n\nThe client must be configured to create a "secure" connection to a "secure" server,\nor alternatively an "insecure" connection to an "insecure" server. By default, the\nclient will attempt to create a "secure" connection. And so, when connecting to an\n"insecure" server, the connection string must specify that the client should attempt\nto make an "insecure" connection.\n\nThe following connection string specifies that the client should\nattempt to create an "insecure" connection to port 2114 on "localhost".\nWhen connecting to an "insecure" server, the client will ignore any\nusername and password information included in the connection string,\nso that usernames and passwords are not sent over an "insecure" connection.\n\n    esdb://localhost:2114?Tls=false\n\nPlease note, the "insecure" connection string uses a query string with the field-value\n`Tls=false`. The value of this field is by default `true`. Unless the connection string\nURI includes the field-value `Tls=false` in the query string, the `root_certificates`\nconstructor argument is also required.\n\nWhen connecting to a "secure" server, the `root_certificates` argument is expected to\nbe a Python `str` containing PEM encoded SSL/TLS root certificates. This value is\npassed directly to `grpc.ssl_channel_credentials()`. It is used for authenticating the\nserver to the client. It is commonly the certificate of the certificate authority that\nwas responsible for generating the SSL/TLS certificate used by the EventStoreDB server.\nBut, alternatively for development, you can use the server\'s certificate itself.\n\nIn the example below, the constructor argument values are taken from the operating\nsystem environment. This is a typical arrangement in a production environment. It is\ndone this way here so that the code in this documentation can be tested with both\na "secure" and an "insecure" server.\n\n```python\nimport os\n\nclient = EventStoreDBClient(\n    uri=os.getenv("ESDB_URI"),\n    root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),\n)\n```\n\n## Connection strings\n\nAn EventStoreDB connection string is a URI that conforms with one of two possible\nschemes: either the "esdb" scheme, or the "esdb+discover" scheme.\n\nThe syntax and semantics of the EventStoreDB URI schemes are described below. The\nsyntax is defined using [EBNF](https://en.wikipedia.org/wiki/Extended_Backus–Naur_form).\n\n### Two schemes\n\nThe "esdb" URI scheme can be defined in the following way.\n\n    esdb-uri = "esdb://" , [ user-info , "@" ] , grpc-target, { "," , grpc-target } , [ "?" , query-string ] ;\n\nIn the "esdb" URI scheme, after the optional user info string, there must be at least\none gRPC target. If there are several gRPC targets, they must be separated from each\nother with the "," character. Each gRPC target should indicate an EventStoreDB gRPC\nserver socket, by specifying a host and a port number separated with the ":" character.\nThe host may be a hostname that can be resolved to an IP address, or an IP address.\n\n    grpc-target = ( hostname | ip-address ) , ":" , port-number ;\n\n\nThe "esdb+discover" URI scheme can be defined in the following way.\n\n    esdb-discover-uri = "esdb+discover://" , [ user-info, "@" ] , cluster-domainname , [ "?" , query-string ] ;\n\nIn the "esdb+discover" URI scheme, after the optional user info string, there must be a\ndomain name which should identify a cluster of EventStoreDB servers. The client will use\na DNS server to resolve the domain name to a list of addresses of EventStoreDB servers,\nby querying for \'A\' records. In this case, the port number "2113" will be used to\nconstruct gRPC targets from the addresses obtained from \'A\' records provided by the\nDNS server. Therefore, if you want to use the "esdb+discover" URI scheme, you will\nneed to configure DNS when setting up your EventStoreDB cluster.\n\nWith both the "esdb" and "esdb+discover" URI schemes, the client firstly obtains\na list of gRPC targets: either directly from "esdb" connection strings; or indirectly\nfrom "esdb+discover" connection strings via DNS. This list of targets is known as the\n"gossip seed". The client will then attempt to connect to each gRPC target in turn,\nattempting to call the EventStoreDB Gossip API to obtain information about the\nEventStoreDB cluster. A member of the cluster is selected by the client, according\nto the "node preference" option. The client may then need to close its\nconnection and reconnect to the selected server.\n\n### User info string\n\nIn both the "esdb" and "esdb+discover" schemes, the URI may include a user info string.\nIf it exists in the URI, the user info string must be separated from the rest of the URI\nwith the "@" character. The user info string must include a username and a password,\nseparated with the ":" character.\n\n    user-info = username , ":" , password ;\n\nThe user info is sent by the client as "call credentials" in each call to a "secure"\nserver, in a "basic auth" authorization header. This authorization header is used by\nthe server to authenticate the client. The authorization header is not sent to\n"insecure" servers.\n\n### Query string\n\nIn both the "esdb" and "esdb+discover" schemes, the optional query string must be one\nor many field-value arguments, separated from each other with the "&" character.\n\n    query-string = field-value, { "&", field-value } ;\n\nEach field-value argument must be one of the supported fields, and an\nappropriate value, separated with the "=" character.\n\n    field-value = ( "Tls", "=" , "true" | "false" )\n                | ( "TlsVerifyCert", "=" , "true" | "false" )\n                | ( "ConnectionName", "=" , string )\n                | ( "NodePreference", "=" , "leader" | "follower" | "readonlyreplica" | "random" )\n                | ( "DefaultDeadline", "=" , integer )\n                | ( "GossipTimeout", "=" , integer )\n                | ( "MaxDiscoverAttempts", "=" , integer )\n                | ( "DiscoveryInterval", "=" , integer )\n                | ( "MaxDiscoverAttempts", "=" , integer )\n                | ( "KeepAliveInterval", "=" , integer )\n                | ( "KeepAliveInterval", "=" , integer ) ;\n\nThe table below describes the query field-values supported by this client.\n\n| Field               | Value                                                                 | Description                                                                                                                                                       |\n|---------------------|-----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| Tls                 | "true", "false" (default: "true")                                     | If "true" the client will create a "secure" gRPC channel. If "false" the client will create an "insecure" gRPC channel. This must match the server configuration. |\n| TlsVerifyCert       | "true", "false" (default: "true")                                     | This value is currently ignored.                                                                                                                                  |\n| ConnectionName      | string (default: auto-generated version-4 UUID)                       | Sent in call metadata for every call, to identify the client to the cluster.                                                                                      |\n| NodePreference      | "leader", "follower", "readonlyreplica", "random" (default: "leader") | The node state preferred by the client. The client will select a node from the cluster info received from the Gossip API according to this preference.            |\n| DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_to_stream()`.                                                  |\n| GossipTimeout       | integer (default: 5)                                                  | The default value (in seconds) of the `timeout` argument of gossip read methods, such as `read_gossip()`.                                                         |\n| MaxDiscoverAttempts | integer (default: 10)                                                 | The number of attempts to read gossip when connecting or reconnecting to a cluster member.                                                                        |\n| DiscoveryInterval   | integer (default: 100)                                                | How long to wait (in milliseconds) between gossip retries.                                                                                                        |\n| KeepAliveInterval   | integer (default: `None`)                                             | The value of the "grpc.keepalive_ms" gRPC channel option.                                                                                                         |\n| KeepAliveTimeout    | integer (default: `None`)                                             | The value of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                                                 |\n\n\n### Examples\n\nHere are some examples of EventStoreDB connection string URIs.\n\nThe following URI will cause the client to connect to, and get\ncluster info, from "secure" server socket `localhost:2113`. And\nthen to connect to a "leader" node. And also to use "admin" and\n"changeit" as the username and password when making calls to\nEventStoreDB API methods.\n\n    esdb://admin:changeit@localhost:2113\n\n\nThe following URI will cause the client to get cluster info from\n"insecure" server socket 127.0.0.1:2114.  And then to connect to\na "leader" node.\n\n    esdb://127.0.0.1:2114?Tls=false\n\n\nThe following URI will cause the client to get cluster info from\naddresses in DNS \'A\' records for cluster1.example.com. And then\nto connect to a "leader" node. And use a default deadline of 5\nseconds when making calls to EventStore API "write" methods.\n\n    esdb+discover://admin:changeit@cluster1.example.com?DefaultDeadline=5\n\n\nThe following URI will cause the client to get cluster info from either\nlocalhost:2111, or localhost:2112, or localhost:2113. And then to connect\nto a "follower" node.\n\n    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower\n\n\nThe following URI will cause the client to get cluster info from addresses in\nDNS \'A\' records for cluster1.example.com. And to configure "keep alive" timeout\nand interval in the gRPC channel.\n\n    esdb+discover://admin:changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000\n\n\nPlease note, the client is insensitive to the case of fields and values. If fields are\nrepeated in the query string, the query string will be parsed without error. However,\nthe connection options used by the client will use the value of the first field. All\nthe other field-values in the query string with the same field name will be ignored.\nFields without values will also be ignored.\n\nIf the client\'s node preference is "leader" and the node becomes a\n"follower", the client will attempt to reconnect to the current leader when a method\nis called that expects to call a leader. Methods which mutate the state of the database\nexpect to call a leader. For such methods, the HTTP header "requires-leader" is set to\n"true", and this header is observed by the server, and so a node which is not a leader\nthat receives such a request will return an error. This error is detected by the client,\nwhich will then close the current gRPC connection and create a new connection to the\nleader. The request will then be retried with the leader.\n\nIf the client\'s node preference is "follower" and there are no follower\nnodes in the cluster, then the client will raise an exception. Similarly, if the\nclient\'s node preference is "readonlyreplica" and there are no read-only replica\nnodes in the cluster, then the client will also raise an exception.\n\nThe gRPC channel option "grpc.max_receive_message_length" is automatically\nconfigured to the value `17 * 1024 * 1024`. This value cannot be changed.\n\n\n## Event objects\n\nThis package defines a `NewEvent` class and a `RecordedEvent` class. The\n`NewEvent` class should be used when writing events to the database. The\n`RecordedEvent` class is used when reading events from the database.\n\n### New events\n\nThe `NewEvent` class should be used when writing events to an EventStoreDB database.\nYou will need to construct new event objects before calling `append_to_stream()`.\n\nThe `NewEvent` class is a frozen Python dataclass. It has two required constructor\narguments (`type` and `data`) and three optional constructor arguments (`metadata`,\n`content_type` and `id`).\n\nThe required `type` argument is a Python `str`, used to describe the type of\ndomain event that is being recorded.\n\nThe required `data` argument is a Python `bytes` object, used to state the\nserialized data of the domain event that is being recorded.\n\nThe optional `metadata` argument is a Python `bytes` object, used to indicate any\nmetadata of the event that will be recorded. The default value is an empty `bytes`\nobject.\n\nThe optional `content_type` argument is a Python `str`, used to indicate the\nkind of data that is being recorded. The default value is `\'application/json\'`,\nwhich indicates that the `data` was serialised using JSON. An alternative value\nfor this argument is the more general indication `\'application/octet-stream\'`.\n\nThe optional `id` argument is a Python `UUID` object, used to specify the unique ID\nof the event that will be recorded. If no value is provided, a new version-4 UUID\nwill be generated.\n\n```python\nnew_event1 = NewEvent(\n    type=\'OrderCreated\',\n    data=b\'{"name": "Greg"}\',\n)\nassert new_event1.type == \'OrderCreated\'\nassert new_event1.data == b\'{"name": "Greg"}\'\nassert new_event1.metadata == b\'\'\nassert new_event1.content_type == \'application/json\'\nassert isinstance(new_event1.id, uuid.UUID)\n\nevent_id = uuid.uuid4()\nnew_event2 = NewEvent(\n    type=\'ImageCreated\',\n    data=b\'01010101010101\',\n    metadata=b\'{"a": 1}\',\n    content_type=\'application/octet-stream\',\n    id=event_id,\n)\nassert new_event2.type == \'ImageCreated\'\nassert new_event2.data == b\'01010101010101\'\nassert new_event2.metadata == b\'{"a": 1}\'\nassert new_event2.content_type == \'application/octet-stream\'\nassert new_event2.id == event_id\n```\n\n### Recorded events\n\nThe `RecordedEvent` class is used when reading events from an EventStoreDB\ndatabase. The client will return event objects of this type from all methods\nthat return recorded events, such as `get_stream()`, `subscribe_to_all()`,\nand `read_subscription()`. You do not need to construct recorded event objects.\n\nLike `NewEvent`, the `RecordedEvent` class is also a frozen Python dataclass. It has\nall the attributes that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`)\nand some additional attributes that follow from the fact that an event was recorded\n(`stream_name`, `stream_position`, `commit_position`).\n\nThe `type` attribute is a Python `str`, used to indicate the type of an event\nthat was recorded.\n\nThe `data` attribute is a Python `bytes` object, used to indicate the data of an\nevent that was recorded.\n\nThe `metadata` attribute is a Python `bytes` object, used to indicate the metadata of\nan event that was recorded.\n\nThe `content_type` attribute is a Python `str`, used to indicate the type of\ndata that was recorded for an event. It is usually `\'application/json\'`, indicating\nthat the data can be parsed as JSON. Alternatively, it is `\'application/octet-stream\'`.\n\nThe `id` attribute is a Python `UUID` object, used to indicate the unique ID of an\nevent that was recorded.\n\nThe `stream_name` attribute is a Python `str`, used to indicate the name of a\nstream in which an event was recorded.\n\nThe `stream_position` attribute is a Python `int`, used to indicate the position in a\nstream at which an event was recorded.\n\nIn EventStoreDB, a "stream position" is an integer representing the position of a\nrecorded event in a stream. Each recorded event is recorded at a position in a stream.\nEach stream position is occupied by only one recorded event. New events are recorded at the\nnext unoccupied position. All sequences of stream positions are zero-based and gapless.\n\nThe `commit_position` attribute is a Python `int`, used to indicate the position in the\ndatabase at which an event was recorded.\n\nIn EventStoreDB, a "commit position" is an integer representing the position of a\nrecorded event in the database. Each recorded event is recorded at a position in the\ndatabase. Each commit position is occupied by only one recorded event. Commit positions\nare zero-based and increase monotonically as new events are recorded. But, unlike stream\npositions, the sequence of successive commit positions is not gapless. Indeed, there are\nusually large differences between the commit positions of successively recorded events.\n\nPlease note, in EventStoreDB 21.10, the `commit_position` of all `RecordedEvent` objects\nobtained from `read_stream()` is `None`, whereas those obtained from `read_all()` have\nthe actual commit position of the recorded event. This was changed in version 22.10, so\nthat event objects obtained from both `get_stream()` and `read_all()` have the actual\ncommit position. The `commit_position` attribute of the `RecordedEvent` class is\nannotated with the type `Optional[int]` for this reason only.\n\n\n```python\nfrom esdbclient.events import RecordedEvent\n\nrecorded_event = RecordedEvent(\n    type=\'OrderCreated\',\n    data=b\'{}\',\n    metadata=b\'\',\n    content_type=\'application/json\',\n    id=uuid.uuid4(),\n    stream_name=\'stream1\',\n    stream_position=0,\n    commit_position=512,\n)\n```\n\n\n## Streams\n\nIn EventStoreDB, a "stream" is a sequence of recorded events that all have\nthe same "stream name". There will normally be many streams in a database,\neach with many recorded events. Each recorded event has a position in its stream\n(the "stream position"), and a position in the database (the "commit position").\nStream positions are zero-based and gapless. Commit positions are also zero-based,\nbut are not gapless.\n\nThe methods `append_to_stream()`, `get_stream()` and `read_all()` can\nbe used to read and record in the database.\n\n### Append events\n\n*requires leader*\n\nThe `append_to_stream()` method can be used atomically to record a sequence of new events.\nIf the operation is successful, it returns the commit position of the last event in the\nsequence that has been recorded.\n\nThis method has three required arguments, `stream_name`, `current_version`\nand `events`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream to which a sequence of events will be appended.\n\nThe required `current_version` argument is expected to be either a Python `int`\nthat indicates the stream position of the last recorded event in the stream, or\n`StreamState.NO_STREAM` if the stream does not yet exist or has been deleted. The\nstream positions are zero-based and gapless, so that if a stream has two events, the\n`current_version` should be 1. If an incorrect value is given, this method will raise a\n`WrongCurrentVersion` exception. This behavior is designed to provide concurrency\ncontrol when recording new events. The correct value of `current_version` for any stream\ncan be obtained by calling `get_current_version()`. However, the typical approach is to\nreconstruct an aggregate from the recorded events, so that the version of the aggregate\nis the stream position of the last recorded event, then have the aggregate generate new\nevents, and then use the current version of the aggregate as the value of the\n`current_version` argument when appending the new aggregate events. This ensures\nthe consistency of the recorded aggregate events, because operations that generate\nnew aggregate events can be retried with a freshly reconstructed aggregate if\na `WrongCurrentVersion` exception is encountered when recording new events. This\ncontrolling behavior can be disabled by setting the value of the `current_version`\nargument to the constant `StreamState.ANY`.\n\nThe required `events` argument is expected to be a sequence of new event objects. The\n`NewEvent` class should be used to construct new event objects. The `append_to_stream()`\noperation is atomic, so that either all or none of the new events will be recorded. It\nis not possible with EventStoreDB atomically to record new events in more than one stream.\n\nThis method also has an optional `timeout` argument, which is a Python `float`\nthat sets a deadline for the completion of the gRPC operation.\n\nIn the example below, a new event, `event1`, is appended to a new stream. The stream\ndoes not yet exist, so `current_version` is `StreamState.NO_STREAM`.\n\n```python\n# Construct a new event object.\nevent1 = NewEvent(type=\'OrderCreated\', data=b\'data1\')\n\n# Define a new stream name.\nstream_name1 = str(uuid.uuid4())\n\n# Append the new events to the new stream.\ncommit_position1 = client.append_to_stream(\n    stream_name=stream_name1,\n    current_version=StreamState.NO_STREAM,\n    events=[event1],\n)\n```\n\nIn the example below, two subsequent events are appended to an existing\nstream. The stream has one recorded event, so `current_version` is `0`.\n\n```python\nevent2 = NewEvent(type=\'OrderUpdated\', data=b\'data2\')\nevent3 = NewEvent(type=\'OrderDeleted\', data=b\'data3\')\n\ncommit_position2 = client.append_to_stream(\n    stream_name=stream_name1,\n    current_version=0,\n    events=[event2, event3],\n)\n```\n\nThe returned values, `commit_position1` and `commit_position2`, are the\ncommit positions in the database of the last events in the recorded sequences.\nThat is, `commit_position1` is the commit position of `event1` and\n`commit_position2` is the commit position of `event3`.\n\nCommit positions that are returned in this way can be used by a user interface to poll\na downstream component until it has processed all the newly recorded events. For example,\nconsider a user interface command that results in the recording of new events, and an\neventually consistent materialized view in a downstream component that is updated from\nthese events. If the new events have not yet been processed, the view might be stale,\nor out-of-date. Instead of displaying a stale view, the user interface can poll the\ndownstream component until it has processed the newly recorded events, and then display\nan up-to-date view to the user.\n\n\n### Idempotent append operations\n\nThe `append_to_stream()` method is "idempotent", in that if called with new events whose\n`id` attribute values equal those of recorded events in the named stream immediately\nafter the stream position specified by the value of the `current_version` argument, then\nit will return the commit position of the last new event, without making any changes to\nthe database.\n\nSometimes it may happen, when calling `append_to_stream()`, that the new events are\nsuccessfully recorded but somehow a connection issue occurs before the successful call\ncan return successfully to the client. We cannot be sure if the events were recorded\nor not, and so we may wish to retry. If the events were in fact successfully recorded,\nit is convenient for the retried operation to return successfully without raising an\nexception. If those new events were in fact not recorded, and in the meantime no other\nnew events were recorded in that stream, then it makes sense that the new events will\nbe recorded when the append operation is retried. Of course, if a `WrongCurrentVersion`\nexception is raised when retrying the operation, then an application command which\ngenerated the new events in the context of already recorded events may need to be\nexecuted again. Alternatively, a suitable error might be displayed by the application,\nwith an up-to-date view of the recorded data, giving a user of the application an\nopportunity to decide if they still wish to proceed with their original intention.\n\nThe example below shows the `append_to_stream()` method being called again with\n`event3` and `current_version=0`. We can see that repeating the call to\n`append_to_stream()` returns successfully.\n\n```python\n# Retry appending event3.\ncommit_position_retry = client.append_to_stream(\n    stream_name=stream_name1,\n    current_version=0,\n    events=[event2, event3],\n)\n```\n\nWe can see that the same commit position is returned as above.\n\n```python\nassert commit_position_retry == commit_position2\n```\n\nBy calling `get_stream()`, we can also see the stream has been unchanged\ndespite the `append_to_stream()` method having been called twice with the same arguments.\nThat is, there are still only three events in the stream.\n\n```python\nevents = client.get_stream(\n    stream_name=stream_name1\n)\n\nassert len(events) == 3\n```\n\nThis idempotent behaviour depends on the `id` attribute of the `NewEvent` class.\nThis attribute, by default, is assigned a new and unique version-4 UUID when an\ninstance of `NewEvent` is constructed. The `id` argument can be used when\nconstructing `NewEvent` objects to set the value of this attribute.\n\n\n### Read stream events\n\nThe `read_stream()` method can be used to get events that have been appended\nto a stream. This method returns a "read response" object.\n\nA "read response" object is a Python iterator. Recorded events can be\nobtained by iterating over the "read response" object. Recorded events are\nstreamed from the server to the client as the iteration proceeds. The iteration\nwill automatically stop when there are no more recorded events to be returned.\nThe streaming of events, and hence the iterator, can also be stopped by calling\nthe `stop()` method on the "read response" object.\n\nThe `get_stream()` method can be used to get events that have been appended\nto a stream. This method returns a Python `tuple` of recorded event objects.\nThe recorded event objects are instances of the `RecordedEvent` class. It\ncalls `read_stream()` and passes the "read response" iterator into a Python\n`tuple`, so that the streaming will complete before the method returns.\n\nThe `read_stream()` and `get_stream()` methods have one required argument, `stream_name`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream from which recorded events will be returned.\n\nThe `read_stream()` and `get_stream()` methods also have four optional arguments,\n`stream_position`, `backwards`, `limit`, and `timeout`.\n\nThe optional `stream_position` argument is a Python `int` that can be used to\nindicate the position in the stream from which to start reading. The default value\nof `stream_position` is `None`. When reading a stream from a specific position in the\nstream, the recorded event at that position will be included, both when reading\nforwards from that position, and when reading backwards.\n\nThe optional `backwards` argument is a Python `bool`. The default value of `backwards`\nis `False`, which means the stream will be read forwards, so that events are returned\nin the order they were recorded. If `backwards` is `True`, the events are returned in\nreverse order.\n\nIf `backwards` is `False` and `stream_position` is `None`, the stream\'s events will be\nreturned in the order they were recorded, starting from the first recorded event. If\n`backwards` is `True` and `stream_position` is `None`, the stream\'s events will be\nreturned in reverse order, starting from the last recorded event.\n\nThe optional `limit` argument is a Python `int` which restricts the number of events\nthat will be returned. The default value of `limit` is `sys.maxint`.\n\nThe optional `timeout` argument is a Python `float` which sets a deadline for\nthe completion of the gRPC operation.\n\nThe example below shows the default behavior, which is to return all the recorded\nevents of a stream forwards from the first recorded events to the last.\n\n```python\nevents = client.get_stream(\n    stream_name=stream_name1\n)\n\nassert len(events) == 3\nassert events[0].id == event1.id\nassert events[1].id == event2.id\nassert events[2].id == event3.id\n```\n\nThe example below shows how to use the `stream_position` argument to read a stream\nfrom a specific stream position to the end of the stream. Stream positions are\nzero-based, and so `stream_position=1` corresponds to the second event that was\nrecorded in the stream, in this case `event2`.\n\n```python\nevents = client.get_stream(\n    stream_name=stream_name1,\n    stream_position=1,\n)\n\nassert len(events) == 2\nassert events[0].id == event2.id\nassert events[1].id == event3.id\n```\n\nThe example below shows how to use the `backwards` argument to read a stream backwards.\n\n```python\nevents = client.get_stream(\n    stream_name=stream_name1,\n    backwards=True,\n)\n\nassert len(events) == 3\nassert events[0].id == event3.id\nassert events[1].id == event2.id\nassert events[2].id == event1.id\n```\n\nThe example below shows how to use the `limit` argument to read a limited number of\nevents.\n\n```python\nevents = client.get_stream(\n    stream_name=stream_name1,\n    limit=2,\n)\n\nassert len(events) == 2\nassert events[0].id == event1.id\nassert events[1].id == event2.id\n```\n\nThe `read_stream()` and `get_stream()` methods will raise a `NotFound` exception if the\nnamed stream has never existed or has been deleted.\n\n```python\nfrom esdbclient.exceptions import NotFound\n\n\ntry:\n    client.get_stream(\'does-not-exist\')\nexcept NotFound:\n    pass  # The stream does not exist.\nelse:\n    raise Exception("Shouldn\'t get here")\n```\n\nPlease note, the `get_stream()` method is decorated with the `@autoreconnect` and\n`@retrygrpc` decorators, whilst the `read_stream()` method is not. This means that\nall errors due to connection issues will be caught by the retry and reconnect decorators\nwhen calling the `get_stream()` method, but not when calling `read_stream()`. The\n`read_stream()` method has no such decorators because the streaming only starts\nwhen iterating over the "read response" starts, which means that the method returns\nbefore the streaming starts, and so there is no chance for any decorators to catch\nany connection issues.\n\nFor the same reason, `read_stream()` will not raise a `NotFound` exception when\nthe stream does not exist, until iterating over the "read response" object begins.\n\nIf you are reading a very large stream, then you might prefer to call `read_stream()`,\nand begin iterating through the recorded events whilst they are being streamed from\nthe server, rather than both waiting and having them all accumulate in memory.\n\n### Get current version\n\nThe `get_current_version()` method is a convenience method that essentially calls\n`get_stream()` with `backwards=True` and `limit=1`. This method returns\nthe value of the `stream_position` attribute of the last recorded event in a\nstream. If a stream does not exist, the returned value is `StreamState.NO_STREAM`.\nThe returned value is the correct value of `current_version` when appending events\nto a stream, and when deleting or tombstoning a stream.\n\nThis method has one required argument, `stream_name`.\n\nThe required `stream_name` argument is a Python `str` that uniquely identifies a\nstream from which a stream position will be returned.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nIn the example below, the last stream position of `stream_name1` is obtained.\nSince three events have been appended to `stream_name1`, and because positions\nin a stream are zero-based and gapless, so the current version is `2`.\n\n```python\ncurrent_version = client.get_current_version(\n    stream_name=stream_name1\n)\n\nassert current_version == 2\n```\n\nIf a stream has never existed or has been deleted, the returned value is\n`StreamState.NO_STREAM`, which is the correct value of the `current_version`\nargument both when appending the first event of a new stream, and also when\nappending events to a stream that has been deleted.\n\n```python\ncurrent_version = client.get_current_version(\n    stream_name=\'does-not-exist\'\n)\n\nassert current_version is StreamState.NO_STREAM\n```\n\n### How to implement snapshotting with EventStoreDB\n\nSnapshots can improve the performance of aggregates that would otherwise be\nreconstructed from very long streams. However, it is generally recommended to design\naggregates to have a finite lifecycle, and so to have relatively short streams,\nthereby avoiding the need for snapshotting. This "how to" section is intended merely\nto show how snapshotting of aggregates can be implemented with EventStoreDB using\nthis Python client.\n\nEvent-sourced aggregates are typically reconstructed from recorded events by calling\na mutator function for each recorded event, evolving from an initial state\n`None` to the current state of the aggregate. The function `get_aggregate()` shows\nhow this can be done. The aggregate ID is used as a stream name. The exception\n`AggregateNotFound` is raised if the aggregate stream is not found.\n\n```python\nclass AggregateNotFound(Exception):\n    """Raised when an aggregate is not found."""\n\n\ndef get_aggregate(aggregate_id, mutator_func):\n    stream_name = aggregate_id\n\n    # Get recorded events.\n    try:\n        events = client.get_stream(\n            stream_name=stream_name,\n            stream_position=None\n        )\n    except NotFound as e:\n        raise AggregateNotFound(aggregate_id) from e\n    else:\n        # Reconstruct aggregate from recorded events.\n        aggregate = None\n        for event in events:\n            aggregate = mutator_func(aggregate, event)\n        return aggregate\n```\n\nSnapshotting of aggregates can be implemented by recording the current state of\nan aggregate as a new event.\n\nIf an aggregate object has a version number that corresponds to the stream position of\nthe last event that was used to reconstruct the aggregate, and this version number\nis recorded in the snapshot metadata, then any events that are recorded after the\nsnapshot can be selected using this version number. The aggregate can then be\nreconstructed from the last snapshot and any subsequent events, without having\nto replay the entire history.\n\nWe will use a separate stream for an aggregate\'s snapshots that is named after the\nstream used for recording its events. The name of the snapshot stream will be\nconstructed by prefixing the aggregate\'s stream name with `\'snapshot-$\'`.\n\n```python\nSNAPSHOT_STREAM_NAME_PREFIX = \'snapshot-$\'\n\ndef make_snapshot_stream_name(stream_name):\n    return f\'{SNAPSHOT_STREAM_NAME_PREFIX}{stream_name}\'\n\n\ndef remove_snapshot_stream_prefix(snapshot_stream_name):\n    assert snapshot_stream_name.startswith(SNAPSHOT_STREAM_NAME_PREFIX)\n    return snapshot_stream_name[len(SNAPSHOT_STREAM_NAME_PREFIX):]\n```\n\nNow, let\'s redefine the `get_aggregate()` function, so that it looks for a snapshot event,\nthen selects subsequent aggregate events, and then calls a mutator function for each\nrecorded event.\n\nNotice that the aggregate events are read from a stream for serialized aggregate\nevents, whilst the snapshot is read from a separate stream for serialized aggregate\nsnapshots. We will use JSON to serialize and deserialize event data.\n\n\n```python\nimport json\n\n\ndef get_aggregate(aggregate_id, mutator_func):\n    stream_name = aggregate_id\n    recorded_events = []\n\n    # Look for a snapshot.\n    try:\n        snapshots = client.get_stream(\n            stream_name=make_snapshot_stream_name(stream_name),\n            backwards=True,\n            limit=1\n        )\n    except NotFound:\n        stream_position = None\n    else:\n        assert len(snapshots) == 1\n        snapshot = snapshots[0]\n        stream_position = deserialize(snapshot.metadata)[\'version\'] + 1\n        recorded_events.append(snapshot)\n\n    # Get subsequent events.\n    try:\n        events = client.get_stream(\n            stream_name=stream_name,\n            stream_position=stream_position\n        )\n    except NotFound as e:\n        raise AggregateNotFound(aggregate_id) from e\n    else:\n        recorded_events += events\n\n    # Reconstruct aggregate from recorded events.\n    aggregate = None\n    for event in recorded_events:\n        aggregate = mutator_func(aggregate, event)\n\n    return aggregate\n\n\ndef serialize(d):\n    return json.dumps(d).encode(\'utf8\')\n\n\ndef deserialize(s):\n    return json.loads(s.decode(\'utf8\'))\n```\n\nTo show how `get_aggregate()` can be used, let\'s define a `Dog` aggregate class, with\nattributes `name` and `tricks`. The attributes `id` and `version` will indicate an\naggregate object\'s ID and version number. The attribute `is_from_snapshot` is added\nhere merely to demonstrate below when an aggregate object has been reconstructed using\na snapshot.\n\n```python\nfrom dataclasses import dataclass\n\n\n@dataclass(frozen=True)\nclass Aggregate:\n    id: str\n    version: int\n    is_from_snapshot: bool\n\n\n@dataclass(frozen=True)\nclass Dog(Aggregate):\n    name: str\n    tricks: list\n```\n\nLet\'s also define a mutator function `mutate_dog()` that evolves the state of a\n`Dog` aggregate given various different types of events, `\'DogRegistered\'`,\n`\'DogLearnedTrick\'`, and `\'Snapshot\'`.\n\n```python\ndef mutate_dog(dog, event):\n    data = deserialize(event.data)\n    if event.type == \'DogRegistered\':\n        return Dog(\n            id=event.stream_name,\n            version=event.stream_position,\n            is_from_snapshot=False,\n            name=data[\'name\'],\n            tricks=[],\n        )\n    elif event.type == \'DogLearnedTrick\':\n        assert event.stream_position == dog.version + 1\n        assert event.stream_name == dog.id, (event.stream_name, dog.id)\n        return Dog(\n            id=dog.id,\n            version=event.stream_position,\n            is_from_snapshot=dog.is_from_snapshot,\n            name=dog.name,\n            tricks=dog.tricks + [data[\'trick\']],\n        )\n    elif event.type == \'Snapshot\':\n        return Dog(\n            id=remove_snapshot_stream_prefix(event.stream_name),\n            version=deserialize(event.metadata)[\'version\'],\n            is_from_snapshot=True,\n            name=data[\'name\'],\n            tricks=data[\'tricks\'],\n        )\n    else:\n        raise Exception(f"Unknown event type: {event.type}")\n```\n\nFor convenience, let\'s also define a `get_dog()` function that calls `get_aggregate()`\nwith the `mutate_dog()` function as the value of its `mutator_func` argument.\n\n```python\ndef get_dog(dog_id):\n    return get_aggregate(\n        aggregate_id=dog_id,\n        mutator_func=mutate_dog,\n    )\n```\n\nWe can also define some "command" functions that append new events to the\ndatabase. The `register_dog()` function appends a `DogRegistered` event. The\n`record_trick_learned()` appends a `DogLearnedTrick` event. The function\n`snapshot_dog()` appends a `Snapshot` event. Notice that the\n`record_trick_learned()` and `snapshot_dog()` functions use `get_dog()`.\n\nNotice also that the `DogRegistered` and `DogLearnedTrick` events are appended to a\nstream for aggregate events, whilst the `Snapshot` event is appended to a separate\nstream for aggregate snapshots.\n\n```python\ndef register_dog(name):\n    dog_id = str(uuid.uuid4())\n    event = NewEvent(\n        type=\'DogRegistered\',\n        data=serialize({\'name\': name}),\n    )\n    client.append_to_stream(\n        stream_name=dog_id,\n        current_version=StreamState.NO_STREAM,\n        events=event,\n    )\n    return dog_id\n\n\ndef record_trick_learned(dog_id, trick):\n    dog = get_dog(dog_id)\n    event = NewEvent(\n        type=\'DogLearnedTrick\',\n        data=serialize({\'trick\': trick}),\n    )\n    client.append_to_stream(\n        stream_name=dog_id,\n        current_version=dog.version,\n        events=event,\n    )\n\n\ndef snapshot_dog(dog_id):\n    dog = get_dog(dog_id)\n    event = NewEvent(\n        type=\'Snapshot\',\n        data=serialize({\'name\': dog.name, \'tricks\': dog.tricks}),\n        metadata=serialize({\'version\': dog.version}),\n    )\n    client.append_to_stream(\n        stream_name=make_snapshot_stream_name(dog_id),\n        current_version=StreamState.ANY,\n        events=event,\n    )\n```\n\nWe can call `register_dog()` to register a new dog.\n\n```python\n# Register a new dog.\ndog_id = register_dog(\'Fido\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == []\nassert dog.version == 0\nassert dog.is_from_snapshot is False\n\n```\n\nWe can call `record_trick_learned()` to record that some tricks have been learned.\n\n```python\n\n# Record that \'Fido\' learned a new trick.\nrecord_trick_learned(dog_id, trick=\'roll over\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\']\nassert dog.version == 1\nassert dog.is_from_snapshot is False\n\n\n# Record that \'Fido\' learned another new trick.\nrecord_trick_learned(dog_id, trick=\'fetch ball\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\', \'fetch ball\']\nassert dog.version == 2\nassert dog.is_from_snapshot is False\n```\n\nWe can call `snapshot_dog()` to record a snapshot of the current state of the `Dog`\naggregate. After we call `snapshot_dog()`, the `get_dog()` function will return a `Dog`\nobject that has been constructed using the `Snapshot` event.\n\n```python\n# Snapshot \'Fido\'.\nsnapshot_dog(dog_id)\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\', \'fetch ball\']\nassert dog.version == 2\nassert dog.is_from_snapshot is True\n```\n\nWe can continue to evolve the state of the `Dog` aggregate, using\nthe snapshot both during the call to `record_trick_learned()` and\nwhen calling `get_dog()` directly.\n\n```python\nrecord_trick_learned(dog_id, trick=\'sit\')\n\ndog = get_dog(dog_id)\nassert dog.name == \'Fido\'\nassert dog.tricks == [\'roll over\', \'fetch ball\', \'sit\']\nassert dog.version == 3\nassert dog.is_from_snapshot is True\n```\n\nWe can see from the `is_from_snapshot` attribute that the `Dog` object was indeed\nreconstructed from the snapshot.\n\nSnapshots can be created at fixed version number intervals, fixed time\nperiods, after a particular type of event, immediately after events are\nappended, or as a background process.\n\n\n### Read all events\n\nThe `read_all()` method can be used to get all recorded events\nin the database in the order they were recorded. This method returns\na "read response" object, just like `read_stream()`.\n\nA "read response" is an iterator, and not a sequence. Recorded events can be\nobtained by iterating over the "read response" object. Recorded events are\nstreamed from the server to the client as the iteration proceeds. The iteration\nwill automatically stop when there are no more recorded events to be returned.\nThe streaming of events, and hence the iterator, can also be stopped by calling\nthe `stop()` method on the "read response" object. The recorded event objects\nare instances of the `RecordedEvent` class.\n\nThis method has seven optional arguments, `commit_position`, `backwards`,\n`filter_exclude`, `filter_include`, `filter_by_stream_name`, `limit`, and `timeout`.\n\nThe optional `commit_position` argument is a Python `int` that can be used to\nspecify a commit position from which to start reading. The default value of\n`commit_position` is `None`. Please note, if a commit position is specified,\nit must be an actually existing commit position in the database. When reading\nforwards, the event at the commit position may be included, depending upon the\nfilter. When reading backwards, the event at the commit position will not be\nincluded.\n\nThe optional `backwards` argument is a Python `bool`. The default of `backwards` is\n`False`, which means events are returned in the order they were recorded, If\n`backwards` is `True`, then events are returned in reverse order.\n\nIf `backwards` is `False` and `commit_position` is `None`, the database\'s events will\nbe returned in the order they were recorded, starting from the first recorded event.\nThis is the default behavior of `read_all()`. If `backwards` is `True` and\n`commit_position` is `None`, the database\'s events will be returned in reverse order,\nstarting from the last recorded event.\n\nThe optional `filter_exclude` argument is a sequence of regular expressions that\nspecifies which recorded events should be returned. This argument is ignored\nif `filter_include` is set to a non-empty sequence. The default value of this\nargument matches the event types of EventStoreDB "system events", so that system\nevents will not normally be included. See the Notes section below for more\ninformation about filter expressions.\n\nThe optional `filter_include` argument is a sequence of regular expressions\nthat specifies which recorded events should be returned. By default, this\nargument is an empty tuple. If this argument is set to a non-empty sequence,\nthe `filter_exclude` argument is ignored.\n\nThe optional `filter_by_stream_name` argument is a Python `bool` that indicates\nwhether the filtering will apply to event types or stream names. By default, this\nvalue is `False` and so the filtering will apply to the event type strings of\nrecorded events.\n\nThe optional `limit` argument is an integer which restricts the number of events that\nwill be returned. The default value is `sys.maxint`.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe filtering of events is done on the EventStoreDB server. The\n`limit` argument is applied on the server after filtering.\n\nThe example below shows how to get all the events we have recorded in the database\nso far, in the order they were recorded. We can see the three events of `stream_name1`\n(`event1`, `event2` and `event3`) are included, along with others.\n\n```python\n# Read all events (creates a streaming gRPC call).\nread_response = client.read_all()\n\n# Convert the iterator into a sequence of recorded events.\nevents = tuple(read_response)\nassert len(events) > 3  # more than three\n\n# Convert the sequence of recorded events into a set of event IDs.\nevent_ids = set(e.id for e in events)\nassert event1.id in event_ids\nassert event2.id in event_ids\nassert event3.id in event_ids\n```\n\nThe example below shows how to read all recorded events in the database from\na particular commit position, in this case `commit_position1`. When reading\nforwards from a specific commit position, the event at the specified position\nwill be included. The value of `commit_position1` is the position we obtained\nwhen appending `event1`. And so `event1` is the first recorded event we shall\nreceive, `event2` is the second, and `event3` is the third.\n\n```python\n# Read all events forwards from a commit position.\nread_response = client.read_all(\n    commit_position=commit_position1\n)\n\n# Step through the "read response" iterator.\nassert next(read_response).id == event1.id\nassert next(read_response).id == event2.id\nassert next(read_response).id == event3.id\n\n# Stop the iterator.\nread_response.stop()\n```\n\nThe example below shows how to read all events recorded in the database in reverse\norder. We can see that the first events we receive are the last events that were\nrecorded: the events of the `Dog` aggregate from the section about snapshotting\nand the snapshot.\n\n```python\n# Read all events backwards from the end.\nread_response = client.read_all(\n    backwards=True\n)\n\n# Step through the "read response" iterator.\nassert next(read_response).type == "DogLearnedTrick"\nassert next(read_response).type == "Snapshot"\nassert next(read_response).type == "DogLearnedTrick"\nassert next(read_response).type == "DogLearnedTrick"\nassert next(read_response).type == "DogRegistered"\n\n# Stop the iterator.\nread_response.stop()\n```\n\nThe example below shows how to read a limited number of events\nforwards from a specific commit position.\n\n```python\nevents = tuple(\n    client.read_all(\n        commit_position=commit_position1,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\nassert events[0].id == event1.id\n```\n\nThe example below shows how to read a limited number of the recorded events\nin the database backwards from the end. In this case, the limit is 1, and\nso we receive the last recorded event.\n\n```python\nevents = tuple(\n    client.read_all(\n        backwards=True,\n        limit=1,\n    )\n)\n\nassert len(events) == 1\n\nassert events[0].type == \'DogLearnedTrick\'\nassert deserialize(events[0].data)[\'trick\'] == \'sit\'\n```\n\nPlease note, like the `read_stream()` method, the `read_all()` method\nis not decorated with retry and reconnect decorators, because the streaming of recorded\nevents from the server only starts when iterating over the "read response" starts, which\nmeans that the method returns before the streaming starts, and so there is no chance for\nany decorators to catch any connection issues.\n\n### Get commit position\n\nThe `get_commit_position()` method can be used to get the commit position of the\nlast recorded event in the database. It simply calls `read_all()` with\n`backwards=True` and `limit=1`, and returns the value of the `commit_position`\nattribute of the last recorded event.\n\n```python\ncommit_position = client.get_commit_position()\n```\n\nThis method has four optional arguments, `filter_exclude`, `filter_include`,\n`filter_by_stream_name` and `timeout`. These values are passed to `read_all()`.\n\nThe optional `filter_exclude`, `filter_include` and `filter_by_stream_name` arguments\nwork in the same way as they do in the `read_all()` method.\n\nThis optional `timeout` argument is a Python `float` that sets\na deadline for the completion of the gRPC operation.\n\nThis method might be used to measure progress of a downstream component\nthat is processing all recorded events, by comparing the current commit\nposition with the recorded commit position of the last successfully processed\nevent in a downstream component. In this case, the value of the `filter_exclude`,\n`filter_include` and `filter_by_stream_name` arguments should equal those used\nby the downstream component to obtain recorded events.\n\n\n### Get stream metadata\n\nThe `get_stream_metadata()` method returns the metadata for a stream, along\nwith the version of the stream metadata.\n\n```python\nmetadata, metadata_version = client.get_stream_metadata(stream_name=stream_name1)\n```\n\nThe returned `metadata` value is a Python `dict`. The returned `metadata_version`\nvalue is either an `int` if the stream exists, or `None` if the stream does not exist\nand no metadata has been set. These values can be passed into `set_stream_metadata()`.\n\n\n### Set stream metadata\n\n*requires leader*\n\nThe method `set_stream_metadata()` sets the metadata for a stream. Stream metadata\ncan be set before appending events to a stream.\n\n```python\nmetadata["foo"] = "bar"\n\nclient.set_stream_metadata(\n    stream_name=stream_name1,\n    metadata=metadata,\n    current_version=metadata_version,\n)\n```\n\nThe `current_version` argument should be the current version of the stream metadata\nobtained from `get_stream_metadata()`.\n\nPlease refer to the EventStoreDB documentation for more information about stream\nmetadata.\n\n### Delete stream\n\n*requires leader*\n\nThe method `delete_stream()` can be used to "delete" a stream.\n\n```python\ncommit_position = client.delete_stream(stream_name=stream_name1, current_version=2)\n```\n\nAfter deleting a stream, it\'s still possible to append new events. Reading from a\ndeleted stream will return only events that have been appended after it was\ndeleted.\n\n### Tombstone stream\n\n*requires leader*\n\nThe method `tombstone_stream()` can be used to "tombstone" a stream.\n\n```python\ncommit_position = client.tombstone_stream(stream_name=stream_name1, current_version=2)\n```\n\nAfter tombstoning a stream, it\'s not possible to append new events.\n\n\n## Catch-up subscriptions\n\nA "catch-up" subscription can be used to receive events that have already been\nrecorded in the database, and events that are recorded subsequently. A catch-up\nsubscription can be used by an event-processing component that processes recorded\nevents with "exactly-once" semantics.\n\nThe `subscribe_to_all()` method starts a catch-up subscription that can receive\nall events in the database. The `subscribe_to_stream()` method starts a catch-up\nsubscription that can receive events from a specific stream. Both methods return a\n"catch-up subscription" object, which is a Python iterator. Recorded events can be\nobtained by iteration. Recorded event objects obtained in this way are instances\nof the `RecordedEvent` class. Please note, the `subscribe_to_all()` method will\noccasionally return `Checkpoint` objects. These are a special type of `RecordedEvent`\nthat have a `commit_position`, so that downstream event-processing components can\nrecord progress across a large number of events that have been filtered out.\n\nBefore the "catch-up subscription" object is returned to the caller, the client will\nfirstly obtain a "confirmation" response from the server, which allows the client to\ndetect that both the gRPC connection and the streaming gRPC call is operational. For\nthis reason, the `subscribe_to_all()` and `subscribe_to_stream()` methods are both\nusefully decorated with the reconnect and retry decorators. However, once the method\nhas returned, the decorators will have exited, and any exceptions that are raised\ndue to connection issues whilst iterating over the subscription object will have to\nbe handled by your code.\n\nA "catch-up subscription" iterator will not automatically stop when there are no more\nevents to be returned, but instead the iteration will block until new events are\nsubsequently recorded in the database. Any subsequently recorded events will then be\nimmediately streamed to the client, and the iteration will then continue. The streaming\nof events, and hence the iteration, can be stopped by calling the `stop()` method on the\n"catch-up subscription" object.\n\n### Subscribe to all events\n\nThe`subscribe_to_all()` method can be used to start a catch-up subscription\nfrom which all events recorded in the database can be obtained in the order\nthey were recorded. This method returns a "catch-up subscription" iterator.\n\nThis method also has five optional arguments, `commit_position()`, `filter_exclude`,\n`filter_include`, `filter_by_stream_name`, and `timeout`.\n\nThe optional `commit_position` argument specifies a commit position. The default\nvalue of `commit_position` is `None`, which means the catch-up subscription will\nstart from the first recorded event in the database. If a commit position is given,\nit must match an actually existing commit position in the database. Only events\nrecorded after that position will be obtained.\n\nThe optional `filter_exclude` argument is a sequence of regular expressions that\nspecifies which recorded events should be returned. This argument is ignored\nif `filter_include` is set to a non-empty sequence. The default value of this\nargument matches the event types of EventStoreDB "system events", so that system\nevents will not normally be included. See the Notes section below for more\ninformation about filter expressions.\n\nThe optional `filter_include` argument is a sequence of regular expressions\nthat specifies which recorded events should be returned. By default, this\nargument is an empty tuple. If this argument is set to a non-empty sequence,\nthe `filter_exclude` argument is ignored.\n\nThe optional `filter_by_stream_name` argument is a Python `bool` that indicates\nwhether the filtering will apply to event types or stream names. By default, this\nvalue is `False` and so the filtering will apply to the event type strings of\nrecorded events.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe example below shows how to start a catch-up subscription that starts\nfrom the first recorded event in the database.\n\n```python\n# Subscribe from the first recorded event in the database.\ncatchup_subscription = client.subscribe_to_all()\n```\n\nThe example below shows that catch-up subscriptions do not stop\nautomatically, but block when the last recorded event is received,\nand then continue when subsequent events are recorded.\n\n```python\nfrom datetime import datetime\nfrom threading import Thread\n\nfrom esdbclient import Checkpoint\n\n# Append a new event to a new stream.\nstream_name2 = str(uuid.uuid4())\nevent4 = NewEvent(type=\'OrderCreated\', data=b\'data4\')\nclient.append_to_stream(\n    stream_name=stream_name2,\n    current_version=StreamState.NO_STREAM,\n    events=[event4],\n)\n\n\n# Receive events from the catch-up subscription in a different thread.\nreceived_events = []\nmark = datetime.now()\n\ndef receive_events():\n    for event in catchup_subscription:\n        global mark\n        mark = datetime.now()\n        received_events.append(event)\n\n\ndef wait_for_subscription_to_block():\n    while True:\n         if (datetime.now() - mark).total_seconds() > 1:\n             break\n\n\nthread = Thread(target=receive_events, daemon=True)\nthread.start()\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n# Check the last received event is \'event4\'.\nassert received_events[-1].id == event4.id, received_events[-1].id\n\n# Check we also received the other events we have recorded.\nassert received_events[-9].id == event1.id\nassert received_events[-8].id == event2.id\nassert received_events[-7].id == event3.id\nassert received_events[-6].type == "DogRegistered"\nassert received_events[-5].type == "DogLearnedTrick"\nassert received_events[-4].type == "DogLearnedTrick"\nassert received_events[-3].type == "Snapshot"\nassert received_events[-2].type == "DogLearnedTrick"\n\n# Append another event whilst the subscription is running.\nmark = datetime.now()\nevent5 = NewEvent(type=\'OrderUpdated\', data=b\'data5\')\nclient.append_to_stream(\n    stream_name=stream_name2,\n    current_version=0,\n    events=[event5],\n)\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n# Check the last received event is \'event5\'.\nassert received_events[-2].id == event4.id\nassert received_events[-1].id == event5.id\n\n# Stop the subscription.\ncatchup_subscription.stop()\nthread.join()\n```\n\nThe example below shows how to subscribe to events recorded after a\nparticular commit position, in this case from the commit position of\nthe last recorded event that was received above. Another event is\nrecorded before the subscription is restarted. Further events are\nrecorded whilst the subscription is running. All the recorded events\nare received exactly once.\n\n```python\n\n# Append another event.\nevent6 = NewEvent(type=\'OrderDeleted\', data=b\'data6\')\nclient.append_to_stream(\n    stream_name=stream_name2,\n    current_version=1,\n    events=[event6],\n)\n\n# Restart subscribing to all events after the\n# commit position of the last received event.\ncatchup_subscription = client.subscribe_to_all(\n    commit_position=received_events[-1].commit_position\n)\n\nmark = datetime.now()\nthread = Thread(target=receive_events, daemon=True)\nthread.start()\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n# Check the last received event was \'event6\'.\nassert received_events[-3].id == event4.id\nassert received_events[-2].id == event5.id\nassert received_events[-1].id == event6.id\n\n# Append three more events to a new stream.\nmark = datetime.now()\nstream_name3 = str(uuid.uuid4())\nevent7 = NewEvent(type=\'OrderCreated\', data=b\'data7\')\nevent8 = NewEvent(type=\'OrderUpdated\', data=b\'data8\')\nevent9 = NewEvent(type=\'OrderDeleted\', data=b\'data9\')\n\nclient.append_to_stream(\n    stream_name=stream_name3,\n    current_version=StreamState.NO_STREAM,\n    events=[event7, event8, event9],\n)\n\n# Wait for the subscription to block.\nwait_for_subscription_to_block()\n\n\n# Check all the events have been received exactly once.\nassert received_events[-6].id == event4.id\nassert received_events[-5].id == event5.id\nassert received_events[-4].id == event6.id\nassert received_events[-3].id == event7.id\nassert received_events[-2].id == event8.id\nassert received_events[-1].id == event9.id\n\n# Stop the subscription.\ncatchup_subscription.stop()\nthread.join()\n```\n\nThe catch-up subscription call is ended as soon as the subscription object\'s\n`stop()` method is called. This happens automatically when it goes out of scope,\nor when it is explicitly deleted from memory using the Python `del` keyword.\n\n### Subscribe to stream events\n\nThe `subscribe_to_stream()` method can be used to start a catch-up subscription\nfrom which events recorded in a single stream can be obtained. This method\nreturns a "catch-up subscription" iterator.\n\nThis method has a required `stream_name` argument, which specifies the name of the\nstream from which recorded events will be received.\n\nThis method also has two optional arguments, `stream_position`, and `timeout`.\n\nThe optional `stream_position` argument specifies a position in the stream. The\ndefault value of `stream_position` is `None`, which means that all events\nrecorded in the stream will be obtained in the order they were recorded.\nIf a stream position is given, then only events recorded after that position\nwill be obtained.\n\nThe optional `timeout` argument is a Python `float` that sets\na deadline for the completion of the gRPC operation.\n\nThe example below shows how to start a catch-up subscription from\nthe first recorded event in a stream.\n\n```python\n# Subscribe from the start of \'stream2\'.\nsubscription = client.subscribe_to_stream(stream_name=stream_name2)\n```\n\nThe example below shows how to start a catch-up subscription from\na particular stream position.\n\n```python\n# Subscribe to stream2, from the second recorded event.\nsubscription = client.subscribe_to_stream(\n    stream_name=stream_name2,\n    stream_position=1,\n)\n```\n\n### How to implement exactly-once event processing\n\nThe commit positions of recorded events that are received and processed by a\ndownstream component are usefully recorded by the downstream component, so that\nthe commit position of last processed event can be determined when processing is\nresumed.\n\nThe last recorded commit position can be used to specify the commit position from which\nto subscribe when processing is resumed. Since this commit position will represent the\nposition of the last successfully processed event in a downstream component, so it\nwill be usual to want the next event after this position, because that is the next\nevent that has not yet been processed. For this reason, when subscribing for events\nfrom a specific commit position using a catch-up subscription in EventStoreDB, the\nrecorded event at the specified commit position will NOT be included in the sequence\nof recorded events that are received.\n\nTo accomplish "exactly-once" processing of recorded events in a downstream\ncomponent when using a catch-up subscription, the commit position of a recorded\nevent should be recorded atomically and uniquely along with the result of processing\nrecorded events, for example in the same database as materialised views when\nimplementing eventually-consistent CQRS, or in the same database as a downstream\nanalytics or reporting or archiving application. By recording the commit position\nof recorded events atomically with the new state that results from processing\nrecorded events, "dual writing" in the consumption of recorded events can be\navoided. By also recording the commit position uniquely, the new state cannot be\nrecorded twice, and hence the recorded state of the downstream component will be\nupdated only once for any recorded event. By using the greatest recorded commit\nposition to resume a catch-up subscription, all recorded events will eventually\nbe processed. The combination of the "at-most-once" condition and the "at-least-once"\ncondition gives the "exactly-once" condition.\n\nThe danger with "dual writing" in the consumption of recorded events is that if a\nrecorded event is successfully processed and new state recorded atomically in one\ntransaction with the commit position recorded in a separate transaction, one may\nhappen and not the other. If the new state is recorded but the position is lost,\nand then the processing is stopped and resumed, the recorded event may be processed\ntwice. On the other hand, if the commit position is recorded but the new state is\nlost, the recorded event may effectively not be processed at all. By either\nprocessing an event more than once, or by failing to process an event, the recorded\nstate of the downstream component might be inaccurate, or possibly inconsistent, and\nperhaps catastrophically so. Such consequences may or may not matter in your situation.\nBut sometimes inconsistencies may halt processing until the issue is resolved. You can\navoid "dual writing" in the consumption of events by atomically recording the commit\nposition of a recorded event along with the new state that results from processing that\nevent in the same atomic transaction. By making the recording of the commit positions\nunique, so that transactions will be rolled back when there is a conflict, you will\nprevent the results of any duplicate processing of a recorded event being committed.\n\nRecorded events received from a catch-up subscription cannot be acknowledged back\nto the EventStoreDB server. Acknowledging events, however, is an aspect of "persistent\nsubscriptions". Hoping to rely on acknowledging events to an upstream\ncomponent is an example of dual writing.\n\n\n## Persistent subscriptions\n\nIn EventStoreDB, "persistent" subscriptions are similar to catch-up subscriptions,\nin that reading a persistent subscription will block when there are no more recorded\nevents to be received, and then continue when new events are subsequently recorded.\n\nPersistent subscriptions can\n\nPersistent subscriptions can be consumed by a group of consumers operating with one\nof the supported "consumer strategies".\n\nThe significant different with persistent subscriptions is the server will keep track\nof the progress of the consumers. The consumer of a persistent subscription will\ntherefore need to "acknowledge" when a recorded event has been processed successfully,\nand otherwise "negatively acknowledge" a recorded event that has been received but was\nnot successfully processed.\n\nAll of this means that for persistent subscriptions there are "create", "read", "update"\n"delete", "ack", and "nack" operations to consider.\n\nWhilst there are some advantages of persistent subscriptions, in particular the\nconcurrent processing of recorded events by a group of consumers, by tracking in\nthe server the position in the commit sequence of events that have been processed,\nthe issue of "dual writing" in the consumption of events arises. Reliability in the\nprocessing of recorded events by a group of persistent subscription consumers will\nrely on their idempotent handling of duplicate messages, and their resilience to\nout-of-order delivery.\n\n\n### Create subscription\n\n*requires leader*\n\nThe `create_subscription()` method can be used to create a "persistent subscription"\nto all the recorded events in the database across all streams.\n\nThis method has a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription.\n\nThis method also has seven optional arguments, `from_end`, `commit_position`,\n`filter_exclude`, `filter_include`, `filter_by_stream_name`, `consumer_strategy`,\nand `timeout`.\n\nThe optional `from_end` argument can be used to specify that the group of consumers\nof the subscription should only receive events that were recorded after the subscription\nwas created.\n\nAlternatively, the optional `commit_position` argument can be used to specify a commit\nposition from which commit position the group of consumers of the subscription should\nreceive events. Please note, the recorded event at the specified commit position might\nbe included in the recorded events received by the group of consumers.\n\nIf neither `from_end` or `commit_position` are specified, the group of consumers\nof the subscription will potentially receive all recorded events in the database.\n\nThe optional `filter_exclude` argument is a sequence of regular expressions that\nspecifies which recorded events should be returned. This argument is ignored\nif `filter_include` is set to a non-empty sequence. The default value of this\nargument matches the event types of EventStoreDB "system events", so that system\nevents will not normally be included. See the Notes section below for more\ninformation about filter expressions.\n\nThe optional `filter_include` argument is a sequence of regular expressions\nthat specifies which recorded events should be returned. By default, this\nargument is an empty tuple. If this argument is set to a non-empty sequence,\nthe `filter_exclude` argument is ignored.\n\nThe optional `filter_by_stream_name` argument is a Python `bool` that indicates\nwhether the filtering will apply to event types or stream names. By default, this\nvalue is `False` and so the filtering will apply to the event type strings of\nrecorded events.\n\nThe optional `consumer_strategy` argument is a Python `str` that defines\nthe consumer strategy for this persistent subscription. The value of this argument\ncan be `\'DispatchToSingle\'`, `\'RoundRobin\'`, `\'Pinned\'`, or `\'PinnedByCorrelation\'`. The\ndefault value is `\'DispatchToSingle\'`.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe method `create_subscription()` does not return a value. Recorded events are\nobtained by calling the `read_subscription()` method.\n\nIn the example below, a persistent subscription is created to operate from the\nfirst recorded non-system event in the database.\n\n```python\n# Create a persistent subscription.\ngroup_name1 = f"group-{uuid.uuid4()}"\nclient.create_subscription(group_name=group_name1)\n```\n\n### Read subscription\n\n*requires leader*\n\nThe `read_subscription()` method can be used by a group of consumers to receive\nrecorded events from a persistent subscription that has been created using\nthe `create_subscription()` method.\n\nThis method has a required `group_name` argument, which is\nthe name of a "group" of consumers of the subscription specified\nwhen `create_subscription()` was called.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method returns a `PersistentSubscription` object, which is an iterator\ngiving `RecordedEvent` objects. It also has `ack()`, `nack()` and `stop()`\nmethods.\n\n```python\nsubscription = client.read_subscription(group_name=group_name1)\n```\n\nThe `ack()` method should be used by a consumer to indicate to the server that it\nhas received and successfully processed a recorded event. This will prevent that\nrecorded event being received by another consumer in the same group. The `ack()`\nmethod takes an `event_id` argument, which is the ID of the recorded event that\nhas been received.\n\nThe example below iterates over the subscription object, and calls `ack()`. The\n`stop()` method is called when we have received the last event, so that we can\ncontinue with the examples below.\n\n```python\nevents = []\nfor event in subscription:\n    events.append(event)\n\n    # Acknowledge the received event.\n    subscription.ack(event_id=event.id)\n\n    # Stop when \'event9\' has been received.\n    if event.id == event9.id:\n        subscription.stop()\n```\n\nThe received events are the events we appended above.\n\n```python\nassert events[-14].id == event1.id\nassert events[-13].id == event2.id\nassert events[-12].id == event3.id\nassert events[-11].type == "DogRegistered"\nassert events[-10].type == "DogLearnedTrick"\nassert events[-9].type == "DogLearnedTrick"\nassert events[-8].type == "Snapshot"\nassert events[-7].type == "DogLearnedTrick"\nassert events[-6].id == event4.id\nassert events[-5].id == event5.id\nassert events[-4].id == event6.id\nassert events[-3].id == event7.id\nassert events[-2].id == event8.id\nassert events[-1].id == event9.id\n```\n\nThe `PersistentSubscription` object also has an `nack()` method that should be used\nby a consumer to negatively acknowledge to the server that it has received but not\nsuccessfully processed a recorded event. The `nack()` method takes an `event_id`\nargument, which is the ID of the recorded event that has been received, and an `action`\nargument, which should be a Python `str`, either `\'unknown\'`, `\'park\'`, `\'retry\'`,\n`\'skip\'` or `\'stop\'`.\n\n\n### How to write a persistent subscription consumer\n\nThe reading of a persistent subscription can be encapsulated in a "consumer" that calls\na "policy" function when a recorded event is received and then automatically calls\n`ack()` if the policy function returns normally, and `nack()` if it raises an exception,\nperhaps retrying the event for a certain number of times before parking the event.\n\nThe simple example below shows how this might be done. We can see that \'event9\' is\nacknowledged before \'event5\' is finally parked.\n\n\n```python\nacked_events = {}\nnacked_events = {}\n\n\nclass ExampleConsumer:\n    def __init__(self, subscription, max_retries, final_action):\n        self.subscription = subscription\n        self.max_retries = max_retries\n        self.final_action = final_action\n        self.error = None\n\n    def run(self):\n        try:\n            for event in self.subscription:\n                try:\n                    self.policy(event)\n                except Exception:\n                    if event.retry_count < self.max_retries:\n                        action = "retry"\n                    else:\n                        action = self.final_action\n                    self.subscription.nack(event.id, action=action)\n                    self.after_nack(event, action)\n                else:\n                    self.subscription.ack(event.id)\n                    self.after_ack(event)\n        except Exception:\n            self.subscription.stop()\n            raise\n\n    def stop(self):\n        self.subscription.stop()\n\n    def policy(self, event):\n        # Raise an exception when we see "event5".\n        if event.id == event5.id:\n            raise Exception()\n\n    def after_ack(self, event):\n        # Track retry count of acked events.\n        acked_events[event.id] = event.retry_count\n\n    def after_nack(self, event, action):\n        # Track retry count of nacked events.\n        nacked_events[event.id] = event.retry_count\n\n        if action == self.final_action:\n            # Stop the consumer, so we can continue with the examples.\n            self.stop()\n\n\n# Create subscription.\ngroup_name = f"group-{uuid.uuid4()}"\nclient.create_subscription(group_name, commit_position=commit_position1)\n\n# Read subscription.\nsubscription = client.read_subscription(group_name)\n\n# Construct consumer.\nconsumer = ExampleConsumer(\n    subscription=subscription,\n    max_retries=5,\n    final_action="park",\n)\n\n# Run consumer.\nconsumer.run()\n\n# Check \'event9\' was acked and never retried.\nassert acked_events[event9.id] == 0\nassert event9.id not in nacked_events\n\n# Check \'event5\' was retried five times and never acked.\nassert nacked_events[event5.id] == 5\nassert event5.id not in acked_events\n```\n\n### Get subscription info\n\n*requires leader*\n\nThe `get_subscription_info()` method can be used to get information for a\npersistent subscription.\n\nThis method has one required argument, `group_name`, which\nshould match the value of the argument used when calling `create_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscription_info = client.get_subscription_info(\n    group_name=group_name1,\n)\n```\n\nThe returned value is a `SubscriptionInfo` object.\n\n### List subscriptions\n\n*requires leader*\n\nThe `list_subscriptions()` method can be used to get information for all\nexisting persistent subscriptions.\n\nThis method has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscriptions = client.list_subscriptions()\n```\n\nThe returned value is a list of `SubscriptionInfo` objects.\n\n### Update subscription\n\n*requires leader*\n\nThe `update_subscription()` method can be used to update a\n"persistent subscription".\n\nThis method has a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription.\n\nThis method also has three optional arguments, `from_end`, `commit_position`,\nand `timeout`.\n\nThe optional `from_end` argument can be used to specify that the group of consumers\nof the subscription should only receive events that were recorded after the subscription\nwas updated.\n\nAlternatively, the optional `commit_position` argument can be used to specify a commit\nposition from which commit position the group of consumers of the subscription should\nreceive events. Please note, the recorded event at the specified commit position might\nbe included in the recorded events received by the group of consumers.\n\nIf neither `from_end` or `commit_position` are specified, the group of consumers\nof the subscription will potentially receive all recorded events in the database.\n\nPlease note, the filter options and consumer strategy cannot be adjusted.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe method `update_subscription()` does not return a value.\n\nIn the example below, a persistent subscription is updated to run from the end of the\ndatabase.\n\n```python\n# Create a persistent subscription.\nclient.update_subscription(group_name=group_name1, from_end=True)\n```\n\n### Create stream subscription\n\n*requires leader*\n\nThe `create_stream_subscription()` method can be used to create a persistent\nsubscription for a stream.\n\nThis method has two required arguments, `group_name` and `stream_name`. The\n`group_name` argument names the group of consumers that will receive events\nfrom this subscription. The `stream_name` argument specifies which stream\nthe subscription will follow. The values of both these arguments are expected\nto be Python `str` objects.\n\nThe method also has four optional arguments, `stream_position`, `from_end`,\n`consumer_strategy`, and `timeout`.\n\nThis optional `stream_position` argument specifies a stream position from\nwhich to subscribe. The recorded event at this stream\nposition will be received when reading the subscription.\n\nThis optional `from_end` argument is a Python `bool`.\nBy default, the value of this argument is `False`. If this argument is set\nto `True`, reading from the subscription will receive only events\nrecorded after the subscription was created. That is, it is not inclusive\nof the current stream position.\n\nThe optional `consumer_strategy` argument is a Python `str` that defines\nthe consumer strategy for this persistent subscription. The value of this argument\ncan be `\'DispatchToSingle\'`, `\'RoundRobin\'`, `\'Pinned\'`, or `\'PinnedByCorrelation\'`. The\ndefault value is `\'DispatchToSingle\'`.\n\nThis method also takes an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method does not return a value. Events can be received by calling\n`read_stream_subscription()`.\n\nThe example below creates a persistent stream subscription from the start of the stream.\n\n```python\n# Create a persistent stream subscription from start of the stream.\ngroup_name2 = f"group-{uuid.uuid4()}"\nclient.create_stream_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\n### Read stream subscription\n\n*requires leader*\n\nThe `read_stream_subscription()` method can be used to read a persistent\nstream subscription.\n\nThis method has two required arguments, `group_name` and `stream_name`, which\nshould match the values of arguments used when calling `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThis method returns a `PersistentSubscription` object, which is an iterator\ngiving `RecordedEvent` objects, that also has `ack()`, `nack()` and `stop()`\nmethods.\n\n```python\nsubscription = client.read_stream_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\nThe example below iterates over the subscription object, and calls `ack()`.\nThe for loop breaks when we have received the last event in the stream, so\nthat we can finish the examples in this documentation.\n\n```python\nevents = []\nfor event in subscription:\n    events.append(event)\n\n    # Acknowledge the received event.\n    subscription.ack(event_id=event.id)\n\n    # Stop when \'event6\' has been received.\n    if event.id == event6.id:\n        subscription.stop()\n```\n\nWe can check we received all the events that were appended to `stream_name2`\nin the examples above.\n\n```python\nassert len(events) == 3\nassert events[0].stream_name == stream_name2\nassert events[0].id == event4.id\nassert events[1].stream_name == stream_name2\nassert events[1].id == event5.id\nassert events[2].stream_name == stream_name2\nassert events[2].id == event6.id\n```\n\n### Get stream subscription info\n\n*requires leader*\n\nThe `get_stream_subscription_info()` method can be used to get information for a\npersistent subscription for a stream.\n\nThis method has two required arguments, `group_name` and `stream_name`, which\nshould match the values of arguments used when calling `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscription_info = client.get_stream_subscription_info(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\nThe returned value is a `SubscriptionInfo` object.\n\n\n### List stream subscriptions\n\n*requires leader*\n\nThe `list_stream_subscriptions()` method can be used to get information for all\nthe persistent subscriptions for a stream.\n\nThis method has one required argument, `stream_name`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\n```python\nsubscriptions = client.list_stream_subscriptions(\n    stream_name=stream_name2,\n)\n```\n\nThe returned value is a list of `SubscriptionInfo` objects.\n\n### Update stream subscription\n\n*requires leader*\n\nThe `update_stream_subscription()` method can be used to update a\npersistent subscription for a stream.\n\nThis method has a required `group_name` argument, which is the\nname of a "group" of consumers of the subscription, and a required\n`stream_name` argument, which is the name of a stream.\n\nThis method also has three optional arguments, `from_end`, `stream_position`,\nand `timeout`.\n\nThe optional `from_end` argument can be used to specify that the group of consumers\nof the subscription should only receive events that were recorded after the subscription\nwas updated.\n\nAlternatively, the optional `stream_position` argument can be used to specify a stream\nposition from which commit position the group of consumers of the subscription should\nreceive events. Please note, the recorded event at the specified stream position might\nbe included in the recorded events received by the group of consumers.\n\nIf neither `from_end` or `commit_position` are specified, the group of consumers\nof the subscription will potentially receive all recorded events in the stream.\n\nPlease note, the consumer strategy cannot be adjusted.\n\nThe optional `timeout` argument is a Python `float` which sets a\ndeadline for the completion of the gRPC operation.\n\nThe `update_stream_subscription()` method does not return a value.\n\nIn the example below, a persistent subscription for a stream is updated to run from the\nend of the stream.\n\n```python\n# Create a persistent subscription.\nclient.update_stream_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n    from_end=True,\n)\n```\n\n### Replay parked events\n\n*requires leader*\n\nThe `replay_parked_events()` method can be used to "replay" events that have\nbeen "parked" (negatively acknowledged with the action `\'park\'`) when reading\na persistent subscription. Parked events will then be received by the consumers\nreading from the persistent subscription.\n\nThis method has one required argument, `group_name`. It has one optional argument,\n`stream_name`. The values of these arguments should match those used when calling\n`create_subscription()` or `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe example below replays parked events for group `group_name1`.\n\n```python\nclient.replay_parked_events(\n    group_name=group_name1,\n)\n```\n\nThe example below replays parked events for group `group_name2`.\n\n```python\nclient.replay_parked_events(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\n### Delete persistent subscription\n\n*requires leader*\n\nThe `delete_persistent_subscription()` method can be used to delete a persistent\nsubscription.\n\nThis method has one required argument, `group_name`. It has one optional argument,\n`stream_name`. The values of these arguments should match those used when calling\n`create_subscription()` or `create_stream_subscription()`.\n\nThis method also has an optional `timeout` argument, that\nis expected to be a Python `float`, which sets a deadline\nfor the completion of the gRPC operation.\n\nThe example below deletes the subscription for group `group_name1` which was created\nby calling `create_subscription()`.\n\n```python\nclient.delete_persistent_subscription(\n    group_name=group_name1,\n)\n```\n\nThe example below deletes the subscription for group `group_name2` which was created\nby calling `create_stream_subscription()`.\n\n```python\nclient.delete_persistent_subscription(\n    group_name=group_name2,\n    stream_name=stream_name2,\n)\n```\n\n## Connection\n\n### Reconnect\n\nThe `reconnect()` method can be used to manually reconnect the client to a\nsuitable EventStoreDB node. This method uses the same routine for reading the\ncluster node states and then connecting to a suitable node according to the\nclient\'s node preference that is specified in the connection string URI when\nthe client is constructed. This method is thread-safe, in that when it is called\nby several threads at the same time, only one reconnection will occur. Concurrent\nattempts to reconnect will block until the client has reconnected successfully,\nand then they will all return normally.\n\n```python\nclient.reconnect()\n```\n\nAn example of when it might be desirable to reconnect manually is when (for performance\nreasons) the client\'s node preference is to be connected to a follower node in the\ncluster, and, after a cluster leader election, the follower becomes the leader.\nReconnecting to a follower node in this case is currently beyond the capabilities of\nthis client, but this behavior might be implemented in a future release.\n\nReconnection will happen automatically in many cases, due to the `@autoreconnect`\ndecorator.\n\n### Close\n\nThe `close()` method can be used to cleanly close the client\'s gRPC connection.\n\n```python\nclient.close()\n```\n\n\n## Asyncio client\n\nThe `esdbclient` package also includes an early version of an asynchronous I/O\ngRPC Python client. It follows exactly the same behaviors as the multithreaded\n`EventStoreDBClient`, but uses the `grpc.aio` package and the `asyncio` module, instead of\n`grpc` and `threading`.\n\nThe async function `AsyncioEventStoreDBClient` constructs the client, and connects to\na server. It can be imported from `esdbclient`, and can be called with the same\narguments as `EventStoreDBClient`. It supports both the "esdb" and the "esdb+discover"\nconnection string URI schemes, and can connect to both "secure" and "insecure"\nEventStoreDB servers. It reconnects or retries when connection issues or server\nerrors are encountered.\n\n```python\nfrom esdbclient import AsyncioEventStoreDBClient\n```\n\nThe asynchronous I/O client has the following methods: `append_to_stream()`,\n`get_stream()`, `read_all()`, `subscribe_to_all()`,\n`delete_stream()`, `tombstone_stream()`, and `reconnect()`.\n\nThese methods are equivalent to the methods on `EventStoreDBClient`. They have the same\nmethod signatures, and can be called with the same arguments, to the same effect.\nThe methods which appear on `EventStoreDBClient` but not on `AsyncioEventStoreDBClient` will be\nadded soon.\n\n### Synopsis\n\nThe example below demonstrates the `append_to_stream()`, `get_stream()` and\n`subscribe_to_all()` methods. These are the most useful methods for writing\nan event-sourced application, allowing new aggregate events to be recorded, the\nrecorded events of an aggregate to be obtained so aggregates can be reconstructed,\nand the state of an application to propagated and processed with "exactly-once"\nsemantics.\n\n```python\nimport asyncio\n\nasync def demonstrate_asyncio_client():\n\n    # Construct client.\n    client = await AsyncioEventStoreDBClient(\n        uri=os.getenv("ESDB_URI"),\n        root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),\n    )\n\n    # Append events.\n    stream_name = str(uuid.uuid4())\n    event1 = NewEvent("OrderCreated", data=b\'{}\')\n    event2 = NewEvent("OrderUpdated", data=b\'{}\')\n    event3 = NewEvent("OrderDeleted", data=b\'{}\')\n\n    commit_position = await client.append_to_stream(\n        stream_name=stream_name,\n        current_version=StreamState.NO_STREAM,\n        events=[event1, event2, event3]\n    )\n\n    # Read stream events.\n    recorded = await client.get_stream(stream_name)\n    assert len(recorded) == 3\n    assert recorded[0].id == event1.id\n    assert recorded[1].id == event2.id\n    assert recorded[2].id == event3.id\n\n\n    # Subscribe all events.\n    received = []\n    async for event in await client.subscribe_to_all():\n        received.append(event)\n        if event.commit_position == commit_position:\n            break\n    assert received[-3].id == event1.id\n    assert received[-2].id == event2.id\n    assert received[-1].id == event3.id\n\n\n    # Close the client.\n    await client.close()\n\n\n# Run the demo.\nasyncio.get_event_loop().run_until_complete(\n    demonstrate_asyncio_client()\n)\n```\n\n## Notes\n\n### Regular expression filters\n\nThe `read_all()`, `subscribe_to_all()`, `create_subscription()`\nand `get_commit_position()` methods have `filter_exclude` and `filter_include`\narguments. This section provides some more details about the values of these\narguments.\n\nThe first thing to note is that these arguments are sequences of regular expressions.\nThey are concatenated together by the client as bracketed alternatives in a larger\nregular expression that is anchored to the start and end of the strings being\nmatched. So you shouldn\'t include the `\'^\'` and `\'$\'` anchor characters, unless\nthese characters are escaped as literal characters to be matched. But you should\nuse wildcards if you want to match substrings, for example `\'.*Snapshot\'` to match\nall strings that end with `\'Snapshot`\'.\n\nIn all methods, the default value of the `filter_exclude` argument is the constant\n`DEFAULT_EXCLUDE_FILTER`, which is designed to exclude EventStoreDB "system" and\n"persistence subscription config" event types, which otherwise would be included.\n\nSystem events generated by EventStoreDB have `type` strings that start with\nthe `$` sign. Persistence subscription events generated when manipulating\npersistence subscriptions have `type` strings that start with `PersistentConfig`.\n\nFor example, to match the type of EventStoreDB system events, use the regular\nexpression string `r\'\\$.+\'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is\nset to this value. You can import this constant from `esdbclient` and use it when\nbuilding longer sequences of regular expressions.\n\nSimilarly, to match the type of EventStoreDB persistence subscription events, use the\nregular expression `r\'PersistentConfig\\d+\'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`\nis set to this value. You can import this constant from `esdbclient`  and use it when\nbuilding longer sequences of regular expressions.\n\nThe constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that includes\nboth `ESDB_SYSTEM_EVENTS_REGEX` and `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`. It is used\nas the default value of `filter_exclude` so that the events that EventStoreDB generates\ninternally are excluded by default.\n\nFor example, if you want to exclude snapshots and system events and persistent subscription\nevents, then you may wish to use a appropriately extended copy of `DEFAULT_EXCLUDE_FILTER`\nas the value of the `filter_exclude` arguments, such as `DEFAULT_EXCLUDE_FILTER + [\'.*Snapshot\']`.\n\n\n### Reconnect and retry method decorators\n\nPlease note, nearly all the client methods are decorated with the `@autoreconnect` and\nthe `@retrygrpc` decorators.\n\nThe `@autoreconnect` decorator will reconnect to a suitable node in the cluster when\nthe server to which the client has been connected has become unavailable, or when the\nclient\'s gRPC channel happens to have been closed. The client will also reconnect when\na method is called that requires a leader, and the client\'s node preference is to be\nconnected to a leader, but the node that the client has been connected to stops being\nthe leader. In this case, the client will reconnect to the current leader. After\nreconnecting, the failed operation will be retried.\n\nThe `@retrygrpc` decorator retries operations that have failed due to a deadline being\nreached (so that the operation times out), and in case the server throws an exception\nwhen handling a client request.\n\nPlease also note, the aspects not covered by the reconnect and retry decorator\nbehaviours have to do with methods that return iterators. For example, consider\nthe "read response" iterator returned from the `read_all()` method. The\n`read_all()` method will have returned, and the method decorators will therefore\nhave exited, before iterating over the "read response" begins. Therefore, if a\nconnection issues occurs whilst iterating over the "read response", it isn\'t possible\nfor any decorator on the `read_all()` method to trigger a reconnection.\n\nWith the "catch-up subscription" objects, there is an initial "confirmation" response\nfrom the server which is received and checked by the client. And so, when a call is\nmade to `subscribe_to_all()` or `subscribe_to_stream()`, if the server is unavailable,\nor if the channel has somehow been closed, or if the request fails for some other reason,\nthen the client will reconnect and retry. However, if an exception is raised when iterating over a\nsuccessfully returned "catch-up subscription" object, the catch-up subscription will\nneed to be restarted. Similarly, when reading persistent subscriptions, if there are\nconnection issues whilst iterating over a successfully received response, the consumer\nwill need to be restarted.\n\n\n## Contributors\n\n### Install Poetry\n\nThe first thing is to check you have Poetry installed.\n\n    $ poetry --version\n\nIf you don\'t, then please [install Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\n    $ curl -sSL https://install.python-poetry.org | python3 -\n\nIt will help to make sure Poetry\'s bin directory is in your `PATH` environment variable.\n\nBut in any case, make sure you know the path to the `poetry` executable. The Poetry\ninstaller tells you where it has been installed, and how to configure your shell.\n\nPlease refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on\nusing Poetry.\n\n### Setup for PyCharm users\n\nYou can easily obtain the project files using PyCharm (menu "Git > Clone...").\nPyCharm will then usually prompt you to open the project.\n\nOpen the project in a new window. PyCharm will then usually prompt you to create\na new virtual environment.\n\nCreate a new Poetry virtual environment for the project. If PyCharm doesn\'t already\nknow where your `poetry` executable is, then set the path to your `poetry` executable\nin the "New Poetry Environment" form input field labelled "Poetry executable". In the\n"New Poetry Environment" form, you will also have the opportunity to select which\nPython executable will be used by the virtual environment.\n\nPyCharm will then create a new Poetry virtual environment for your project, using\na particular version of Python, and also install into this virtual environment the\nproject\'s package dependencies according to the project\'s `poetry.lock` file.\n\nYou can add different Poetry environments for different Python versions, and switch\nbetween them using the "Python Interpreter" settings of PyCharm. If you want to use\na version of Python that isn\'t installed, either use your favourite package manager,\nor install Python by downloading an installer for recent versions of Python directly\nfrom the [Python website](https://www.python.org/downloads/).\n\nOnce project dependencies have been installed, you should be able to run tests\nfrom within PyCharm (right-click on the `tests` folder and select the \'Run\' option).\n\nBecause of a conflict between pytest and PyCharm\'s debugger and the coverage tool,\nyou may need to add ``--no-cov`` as an option to the test runner template. Alternatively,\njust use the Python Standard Library\'s ``unittest`` module.\n\nYou should also be able to open a terminal window in PyCharm, and run the project\'s\nMakefile commands from the command line (see below).\n\n### Setup from command line\n\nObtain the project files, using Git or suitable alternative.\n\nIn a terminal application, change your current working directory\nto the root folder of the project files. There should be a Makefile\nin this folder.\n\nUse the Makefile to create a new Poetry virtual environment for the\nproject and install the project\'s package dependencies into it,\nusing the following command.\n\n    $ make install-packages\n\nIt\'s also possible to also install the project in \'editable mode\'.\n\n    $ make install\n\nPlease note, if you create the virtual environment in this way, and then try to\nopen the project in PyCharm and configure the project to use this virtual\nenvironment as an "Existing Poetry Environment", PyCharm sometimes has some\nissues (don\'t know why) which might be problematic. If you encounter such\nissues, you can resolve these issues by deleting the virtual environment\nand creating the Poetry virtual environment using PyCharm (see above).\n\n### Project Makefile commands\n\nYou can start EventStoreDB using the following command.\n\n    $ make start-eventstoredb\n\nYou can run tests using the following command (needs EventStoreDB to be running).\n\n    $ make test\n\nYou can stop EventStoreDB using the following command.\n\n    $ make stop-eventstoredb\n\nYou can check the formatting of the code using the following command.\n\n    $ make lint\n\nYou can reformat the code using the following command.\n\n    $ make fmt\n\nTests belong in `./tests`. Code-under-test belongs in `./esdbclient`.\n\nEdit package dependencies in `pyproject.toml`. Update installed packages (and the\n`poetry.lock` file) using the following command.\n\n    $ make update-packages\n',
     'author': 'John Bywater',
     'author_email': 'john.bywater@appropriatesoftware.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pyeventsourcing/esdbclient',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `esdbclient-1.0a6/PKG-INFO` & `esdbclient-1.0a7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,11 @@
-Metadata-Version: 2.1
-Name: esdbclient
-Version: 1.0a6
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
-Requires-Dist: dnspython (>=2.3.0,<3.0.0)
-Requires-Dist: grpcio (>=1.51.0,!=1.52.*)
-Requires-Dist: protobuf (>=3.11.0)
-Requires-Dist: typing_extensions
-Project-URL: Repository, https://github.com/pyeventsourcing/esdbclient
-Description-Content-Type: text/markdown
-
 # Python gRPC Client for EventStoreDB
 
 This [Python package](https://pypi.org/project/esdbclient/) provides a Python
-gRPC client for [EventStoreDB](https://www.eventstore.com/).
+gRPC client for the [EventStoreDB](https://www.eventstore.com/) database.
 
 This client has been developed in collaboration with the EventStoreDB
 team. Although not all the features of EventStoreDB are supported
 by this client, many of the most useful features are presented
 in an easy-to-use interface.
 
 This client has been tested to work with EventStoreDB LTS versions 21.10,
@@ -45,42 +13,45 @@
 is 100% test coverage. The code has typing annotations, checked with mypy.
 The code is formatted with black and isort, and checked with flake8. Poetry
 is used for package management during development, and for building and
 publishing distributions to [PyPI](https://pypi.org/project/esdbclient/).
 
 ## Synopsis
 
-The `ESDBClient` class can be imported from the `esdbclient` package.
+You can connect to an EventStoreDB database using the `EventStoreDBClient` class.
+
+The `EventStoreDBClient` class can be imported from the `esdbclient` package.
 
-Probably the three most useful methods of `ESDBClient` are:
+Probably the three most useful methods of `EventStoreDBClient` are:
 
-* `append_events()` This method can be used to record events in a particular
-"stream". This is useful for example when executing a command in an application
+* `append_to_stream()` This method can be used to record new events in a particular
+"stream". This is useful, for example, when executing a command in an application
 that mutates an aggregate. This method is "atomic" in that either all or none of
 the events will be recorded.
 
-* `read_stream_events()` This method can be used to retrieve all the recorded
-events in a "stream". This is useful for example when reconstructing an aggregate
-before executing a command in an application.
-
-* `subscribe_all_events()` This method can be used to receive all recorded
-events across all "streams". This is useful in downstream event-processing
-components, and supports processing events with "exactly-once" semantics (see below).
+* `read_stream()` This method can be used to retrieve all the recorded
+events in a "stream". This is useful, for example, when reconstructing
+an aggregate from recorded events before executing a command in an
+application that creates new events.
+
+* `subscribe_to_all()` This method can be used to receive all recorded events in
+the database. This is useful, for example, in event-processing components because
+it supports processing events with "exactly-once" semantics.
 
 The example below uses an "insecure" EventStoreDB server running locally on port 2114.
 
 ```python
 import uuid
 
-from esdbclient import ESDBClient, NewEvent
+from esdbclient import EventStoreDBClient, NewEvent, StreamState
 
 
-# Construct ESDBClient with an EventStoreDB URI.
+# Construct EventStoreDBClient with an EventStoreDB URI.
 
-client = ESDBClient(
+client = EventStoreDBClient(
     uri="esdb://localhost:2114?Tls=false"
 )
 
 
 # Generate new events. Typically, domain events of different
 # types are generated in a domain model, and then serialized
 # into NewEvent objects. An aggregate ID may be used as the
@@ -91,110 +62,133 @@
     type='OrderCreated',
     data=b'{"order_number": "123456"}'
 )
 event2 = NewEvent(
     type='OrderSubmitted',
     data=b'{}'
 )
+event3 = NewEvent(
+    type='OrderCancelled',
+    data=b'{}'
+)
 
 
-# Append new events to a stream. The stream does not exist so
-# the "current version" is None. The value returned from the
-# append_events() method is the overall position in the database
-# of the last new event recorded by this operation. The returned
-# "commit position" value may be used in a user interface to poll
-# a downstream event-processing component before it presents an
-# up-to-date eventually consistent materialized view.
+# Append new events to a new stream. The value returned
+# from the append_to_stream() method is the overall
+# "commit position" in the database of the last new event
+# recorded by this operation. The returned "commit position"
+# may be used in a user interface to poll an eventually
+# consistent event-processing component until it can
+# present an up-to-date materialized view. New events are
+# each allocated a "stream position", which is the next
+# available position in the stream, starting from 0.
 
-commit_position1 = client.append_events(
+commit_position1 = client.append_to_stream(
     stream_name=stream_name1,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event1, event2],
 )
 
-# The "current version" is the "stream position" of the last
-# recorded event in a stream. Stream positions are zero-based.
-# We have recorded two new events, and so the "current version"
-# of this stream is 1. Concurrency is controlled in this way
-# to ensure the consistency of recorded events. An incorrect
-# value will cause a WrongCurrentVersion exception to be raised.
+# Append events to an existing stream. The "current version"
+# is the "stream position" of the last recorded event in a
+# stream. We have recorded two new events, so the "current
+# version" is 1. The exception 'WrongCurrentVersion' will be
+# raised if an incorrect value is given.
 
-event3 = NewEvent(
-    type='OrderCancelled',
-    data=b'{}'
-)
-
-commit_position2 = client.append_events(
+commit_position2 = client.append_to_stream(
     stream_name=stream_name1,
     current_version=1,
     events=[event3],
 )
 
+# - allocated commit positions increase monotonically
+assert commit_position2 > commit_position1
+
 
-# Read events from a stream. The recorded events may be
-# deserialized to domain events objects of different types,
-# then used to reconstruct an aggregate in a domain model.
+# Read events from a stream. This method returns a
+# "read response" iterator, which returns recorded
+# events. The iterator will stop when there are no
+# more events to be returned.
 
-recorded = client.read_stream_events(
+read_response = client.read_stream(
     stream_name=stream_name1
 )
 
-assert len(recorded) == 3
+# Iterate over "read response" to get recorded events.
+# The recorded events may be deserialized to domain event
+# objects of different types and used to reconstruct an
+# aggregate in a domain model.
+recorded_events = tuple(read_response)
+
+# - stream 'stream_name1' now has three events
+assert len(recorded_events) == 3
+
+# - allocated stream positions are zero-based and gapless
+assert recorded_events[0].stream_position == 0
+assert recorded_events[1].stream_position == 1
+assert recorded_events[2].stream_position == 2
+
+# - event attribute values are recorded faithfully
+assert recorded_events[0].type == "OrderCreated"
+assert recorded_events[0].data == b'{"order_number": "123456"}'
+assert recorded_events[0].id == event1.id
+
+assert recorded_events[1].type == "OrderSubmitted"
+assert recorded_events[1].data == b'{}'
+assert recorded_events[1].id == event2.id
+
+assert recorded_events[2].type == "OrderCancelled"
+assert recorded_events[2].data == b'{}'
+assert recorded_events[2].id == event3.id
+
+
+# Start a catch-up subscription from last recorded position.
+# This method returns a "catch-up subscription" iterator,
+# which returns recorded events. The iterator will not stop
+# when there are no more recorded events to be returned, but
+# will block, and continue when further events are recorded.
+
+catchup_subscription = client.subscribe_to_all()
+
+
+# Iterate over the catch-up subscription. Process each recorded
+# event in turn. Within an atomic database transaction, record
+# the event's "commit position" along with any new state generated
+# by processing the event. Use the component's last recorded commit
+# position when restarting the catch-up subscription.
 
-assert recorded[0].stream_name == stream_name1
-assert recorded[1].stream_name == stream_name1
-assert recorded[2].stream_name == stream_name1
-
-assert recorded[0].stream_position == 0
-assert recorded[1].stream_position == 1
-assert recorded[2].stream_position == 2
-
-assert recorded[0].type == "OrderCreated"
-assert recorded[1].type == "OrderSubmitted"
-assert recorded[2].type == "OrderCancelled"
-
-assert recorded[0].data == b'{"order_number": "123456"}'
-
-
-# Start a catch-up subscription to receive all recorded
-# events across all streams. A catch-up subscription may
-# be used in a downstream event-processing component to
-# receive recorded events from a particular commit position.
-# The first "commit position" in an EventStoreDB database is 0.
-
-last_saved_commit_position = 0
+received_events = []
+for event in catchup_subscription:
+    received_events.append(event)
 
-catch_subscription = client.subscribe_all_events(
-    commit_position=last_saved_commit_position
-)
+    if event.commit_position == commit_position2:
+        # Break so we can continue with the example.
+        break
 
 
-# Iterate over the catch-up subscription. Process each
-# recorded event in turn. In an atomic database transaction
-# save the event's "commit position" with any new state
-# generated by processing the event. Use the component's
-# last saved "commit position" when restarting the subscription.
+# - events are received in the order they were recorded
+assert received_events[-3].type == "OrderCreated"
+assert received_events[-3].data == b'{"order_number": "123456"}'
+assert received_events[-3].id == event1.id
 
+assert received_events[-2].type == "OrderSubmitted"
+assert received_events[-2].data == b'{}'
+assert received_events[-2].id == event2.id
 
-received = []
-for event in catch_subscription:
-    last_saved_commit_position = event.commit_position
-    received.append(event)
+assert received_events[-1].type == "OrderCancelled"
+assert received_events[-1].data == b'{}'
+assert received_events[-1].id == event3.id
 
-    if last_saved_commit_position == commit_position2:
-        # Stop so we can continue with the example.
-        catch_subscription.stop()
 
+# Stop the catch-up subscription iterator.
 
-assert received[-3].type == "OrderCreated"
-assert received[-2].type == "OrderSubmitted"
-assert received[-1].type == "OrderCancelled"
+catchup_subscription.stop()
 
 
-# Close the client after use.
+# Close the client's gRPC connection.
 
 client.close()
 ```
 
 See below for more details.
 
 For an example of usage, see the [eventsourcing-eventstoredb](
@@ -214,32 +208,32 @@
   * [Construct client](#construct-client)
 * [Connection strings](#connection-strings)
   * [Two schemes](#two-schemes)
   * [User info string](#user-info-string)
   * [Query string](#query-string)
   * [Examples](#examples)
 * [Event objects](#event-objects)
-  * [The NewEvent class](#the-newevent-class)
-  * [The RecordedEvent class](#the-recordedevent-class)
+  * [New events](#new-events)
+  * [Recorded events](#recorded-events)
 * [Streams](#streams)
   * [Append events](#append-events)
   * [Append event](#append-event)
   * [Idempotent append operations](#idempotent-append-operations)
   * [Read stream events](#read-stream-events)
   * [Get current version](#get-current-version)
   * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)
   * [Read all events](#read-all-events)
   * [Get commit position](#get-commit-position)
   * [Get stream metadata](#get-stream-metadata)
   * [Set stream metadata](#set-stream-metadata)
   * [Delete stream](#delete-stream)
   * [Tombstone stream](#tombstone-stream)
 * [Catch-up subscriptions](#catch-up-subscriptions)
-  * [Subscribe all events](#subscribe-all-events)
-  * [Subscribe stream events](#subscribe-stream-events)
+  * [Subscribe to all events](#subscribe-to-all-events)
+  * [Subscribe to stream events](#subscribe-to-stream-events)
   * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)
 * [Persistent subscriptions](#persistent-subscriptions)
   * [Create subscription](#create-subscription)
   * [Read subscription](#read-subscription)
   * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)
   * [Get subscription info](#get-subscription-info)
   * [List subscriptions](#list-subscriptions)
@@ -254,14 +248,15 @@
 * [Connection](#connection)
   * [Reconnect](#reconnect)
   * [Close](#close)
 * [Asyncio client](#asyncio-client)
   * [Synopsis](#synopsis-1)
 * [Notes](#notes)
   * [Regular expression filters](#regular-expression-filters)
+  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)
 * [Contributors](#contributors)
   * [Install Poetry](#install-poetry)
   * [Setup for PyCharm users](#setup-for-pycharm-users)
   * [Setup from command line](#setup-from-command-line)
   * [Project Makefile commands](#project-makefile-commands)
 <!-- TOC -->
 
@@ -344,27 +339,27 @@
     $ docker stop eventstoredb-insecure
 	$ docker rm eventstoredb-insecure
 
 
 ## EventStoreDB client
 
 This EventStoreDB client is implemented in the `esdbclient` package with
-the `ESDBClient` class.
+the `EventStoreDBClient` class.
 
 ### Import class
 
-The `ESDBClient` class can be imported from the `esdbclient` package.
+The `EventStoreDBClient` class can be imported from the `esdbclient` package.
 
 ```python
-from esdbclient import ESDBClient
+from esdbclient import EventStoreDBClient
 ```
 
 ### Construct client
 
-The `ESDBClient` class has one required constructor argument, `uri`, and one
+The `EventStoreDBClient` class has one required constructor argument, `uri`, and one
 optional constructor argument, `root_certificates`.
 
 The `uri` argument is expected to be an EventStoreDB connection string URI that
 conforms with the standard EventStoreDB "esdb" or "esdb+discover" URI schemes.
 
 For example, the following connection string specifies that the client should
 attempt to create a "secure" connection to port 2113 on "localhost", and use the
@@ -402,15 +397,15 @@
 system environment. This is a typical arrangement in a production environment. It is
 done this way here so that the code in this documentation can be tested with both
 a "secure" and an "insecure" server.
 
 ```python
 import os
 
-client = ESDBClient(
+client = EventStoreDBClient(
     uri=os.getenv("ESDB_URI"),
     root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),
 )
 ```
 
 ## Connection strings
 
@@ -496,15 +491,15 @@
 
 | Field               | Value                                                                 | Description                                                                                                                                                       |
 |---------------------|-----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Tls                 | "true", "false" (default: "true")                                     | If "true" the client will create a "secure" gRPC channel. If "false" the client will create an "insecure" gRPC channel. This must match the server configuration. |
 | TlsVerifyCert       | "true", "false" (default: "true")                                     | This value is currently ignored.                                                                                                                                  |
 | ConnectionName      | string (default: auto-generated version-4 UUID)                       | Sent in call metadata for every call, to identify the client to the cluster.                                                                                      |
 | NodePreference      | "leader", "follower", "readonlyreplica", "random" (default: "leader") | The node state preferred by the client. The client will select a node from the cluster info received from the Gossip API according to this preference.            |
-| DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_events()`.                                                     |
+| DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_to_stream()`.                                                  |
 | GossipTimeout       | integer (default: 5)                                                  | The default value (in seconds) of the `timeout` argument of gossip read methods, such as `read_gossip()`.                                                         |
 | MaxDiscoverAttempts | integer (default: 10)                                                 | The number of attempts to read gossip when connecting or reconnecting to a cluster member.                                                                        |
 | DiscoveryInterval   | integer (default: 100)                                                | How long to wait (in milliseconds) between gossip retries.                                                                                                        |
 | KeepAliveInterval   | integer (default: `None`)                                             | The value of the "grpc.keepalive_ms" gRPC channel option.                                                                                                         |
 | KeepAliveTimeout    | integer (default: `None`)                                             | The value of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                                                 |
 
 
@@ -579,18 +574,17 @@
 This package defines a `NewEvent` class and a `RecordedEvent` class. The
 `NewEvent` class should be used when writing events to the database. The
 `RecordedEvent` class is used when reading events from the database.
 
 ### New events
 
 The `NewEvent` class should be used when writing events to an EventStoreDB database.
-You will need to construct new event objects before calling the `append_events()`
-and `append_event()` methods.
+You will need to construct new event objects before calling `append_to_stream()`.
 
-The `NewEvent` class is a frozen Python database. It has two required constructor
+The `NewEvent` class is a frozen Python dataclass. It has two required constructor
 arguments (`type` and `data`) and three optional constructor arguments (`metadata`,
 `content_type` and `id`).
 
 The required `type` argument is a Python `str`, used to describe the type of
 domain event that is being recorded.
 
 The required `data` argument is a Python `bytes` object, used to state the
@@ -635,34 +629,34 @@
 assert new_event2.id == event_id
 ```
 
 ### Recorded events
 
 The `RecordedEvent` class is used when reading events from an EventStoreDB
 database. The client will return event objects of this type from all methods
-that return recorded events, such as `read_stream_events()`, `subscribe_all_events()`,
+that return recorded events, such as `get_stream()`, `subscribe_to_all()`,
 and `read_subscription()`. You do not need to construct recorded event objects.
 
-Like `NewEvent`, the `RecordedEvent` class is also a frozen Python database. It has
+Like `NewEvent`, the `RecordedEvent` class is also a frozen Python dataclass. It has
 all the attributes that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`)
 and some additional attributes that follow from the fact that an event was recorded
 (`stream_name`, `stream_position`, `commit_position`).
 
 The `type` attribute is a Python `str`, used to indicate the type of an event
 that was recorded.
 
 The `data` attribute is a Python `bytes` object, used to indicate the data of an
 event that was recorded.
 
 The `metadata` attribute is a Python `bytes` object, used to indicate the metadata of
 an event that was recorded.
 
 The `content_type` attribute is a Python `str`, used to indicate the type of
-data that was recorded for an event. It is usually `application/json`, indicating
-that the data can be parsed as JSON. Alternatively, it is `application/octet-stream`.
+data that was recorded for an event. It is usually `'application/json'`, indicating
+that the data can be parsed as JSON. Alternatively, it is `'application/octet-stream'`.
 
 The `id` attribute is a Python `UUID` object, used to indicate the unique ID of an
 event that was recorded.
 
 The `stream_name` attribute is a Python `str`, used to indicate the name of a
 stream in which an event was recorded.
 
@@ -680,14 +674,21 @@
 In EventStoreDB, a "commit position" is an integer representing the position of a
 recorded event in the database. Each recorded event is recorded at a position in the
 database. Each commit position is occupied by only one recorded event. Commit positions
 are zero-based and increase monotonically as new events are recorded. But, unlike stream
 positions, the sequence of successive commit positions is not gapless. Indeed, there are
 usually large differences between the commit positions of successively recorded events.
 
+Please note, in EventStoreDB 21.10, the `commit_position` of all `RecordedEvent` objects
+obtained from `read_stream()` is `None`, whereas those obtained from `read_all()` have
+the actual commit position of the recorded event. This was changed in version 22.10, so
+that event objects obtained from both `get_stream()` and `read_all()` have the actual
+commit position. The `commit_position` attribute of the `RecordedEvent` class is
+annotated with the type `Optional[int]` for this reason only.
+
 
 ```python
 from esdbclient.events import RecordedEvent
 
 recorded_event = RecordedEvent(
     type='OrderCreated',
     data=b'{}',
@@ -706,82 +707,83 @@
 In EventStoreDB, a "stream" is a sequence of recorded events that all have
 the same "stream name". There will normally be many streams in a database,
 each with many recorded events. Each recorded event has a position in its stream
 (the "stream position"), and a position in the database (the "commit position").
 Stream positions are zero-based and gapless. Commit positions are also zero-based,
 but are not gapless.
 
-The methods `append_events()`, `read_stream_events()` and `read_all_events()` can
+The methods `append_to_stream()`, `get_stream()` and `read_all()` can
 be used to read and record in the database.
 
 ### Append events
 
 *requires leader*
 
-The `append_events()` method can be used atomically to record a sequence of new events.
+The `append_to_stream()` method can be used atomically to record a sequence of new events.
 If the operation is successful, it returns the commit position of the last event in the
 sequence that has been recorded.
 
 This method has three required arguments, `stream_name`, `current_version`
 and `events`.
 
 The required `stream_name` argument is a Python `str` that uniquely identifies a
 stream to which a sequence of events will be appended.
 
 The required `current_version` argument is expected to be either a Python `int`
 that indicates the stream position of the last recorded event in the stream, or
-`None` if the stream does not yet exist or has been deleted. The stream positions
-are zero-based and gapless, so that if a stream has two events, the `current_version`
-should be 1. If an incorrect value is given, this method will raise a
+`StreamState.NO_STREAM` if the stream does not yet exist or has been deleted. The
+stream positions are zero-based and gapless, so that if a stream has two events, the
+`current_version` should be 1. If an incorrect value is given, this method will raise a
 `WrongCurrentVersion` exception. This behavior is designed to provide concurrency
 control when recording new events. The correct value of `current_version` for any stream
 can be obtained by calling `get_current_version()`. However, the typical approach is to
-use the stream position of the recorded events as the version number of a reconstructed
-aggregate, and to use the current version of the aggregate as the `current_version` when
-appending new aggregate events. This ensures the consistency of the recorded state of
-the aggregate, and forces operations that generate new aggregate events to be retried with a freshly
-reconstructed aggregate when a `WrongCurrentVersion` exception is encountered.
-This controlling behavior can be disabled by setting the value of the
-`current_version` argument to `-1`.
+reconstruct an aggregate from the recorded events, so that the version of the aggregate
+is the stream position of the last recorded event, then have the aggregate generate new
+events, and then use the current version of the aggregate as the value of the
+`current_version` argument when appending the new aggregate events. This ensures
+the consistency of the recorded aggregate events, because operations that generate
+new aggregate events can be retried with a freshly reconstructed aggregate if
+a `WrongCurrentVersion` exception is encountered when recording new events. This
+controlling behavior can be disabled by setting the value of the `current_version`
+argument to the constant `StreamState.ANY`.
 
 The required `events` argument is expected to be a sequence of new event objects. The
-`NewEvent` class should be used to construct new event objects. The `append_events()`
+`NewEvent` class should be used to construct new event objects. The `append_to_stream()`
 operation is atomic, so that either all or none of the new events will be recorded. It
 is not possible with EventStoreDB atomically to record new events in more than one stream.
 
 This method also has an optional `timeout` argument, which is a Python `float`
 that sets a deadline for the completion of the gRPC operation.
 
-In the example below, a new event, `event1`, is appended to a new stream. The
-stream does not yet exist, so `current_version` is `None`.
+In the example below, a new event, `event1`, is appended to a new stream. The stream
+does not yet exist, so `current_version` is `StreamState.NO_STREAM`.
 
 ```python
 # Construct a new event object.
 event1 = NewEvent(type='OrderCreated', data=b'data1')
 
 # Define a new stream name.
 stream_name1 = str(uuid.uuid4())
 
 # Append the new events to the new stream.
-commit_position1 = client.append_events(
+commit_position1 = client.append_to_stream(
     stream_name=stream_name1,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event1],
 )
 ```
 
 In the example below, two subsequent events are appended to an existing
-stream. The stream, `stream_name1`, so far has one recorded event, and so
-the correct value of `current_version` is `0`.
+stream. The stream has one recorded event, so `current_version` is `0`.
 
 ```python
 event2 = NewEvent(type='OrderUpdated', data=b'data2')
 event3 = NewEvent(type='OrderDeleted', data=b'data3')
 
-commit_position2 = client.append_events(
+commit_position2 = client.append_to_stream(
     stream_name=stream_name1,
     current_version=0,
     events=[event2, event3],
 )
 ```
 
 The returned values, `commit_position1` and `commit_position2`, are the
@@ -795,139 +797,126 @@
 eventually consistent materialized view in a downstream component that is updated from
 these events. If the new events have not yet been processed, the view might be stale,
 or out-of-date. Instead of displaying a stale view, the user interface can poll the
 downstream component until it has processed the newly recorded events, and then display
 an up-to-date view to the user.
 
 
-### Append event
-
-*requires leader*
-
-The `append_event()` method is like `append_events()` but can be used only to write a
-single new event to a stream. If the operation is successful, it returns the commit
-position of the newly recorded event.
-
-This method has three required arguments, `stream_name`, `current_version` and `event`.
-
-The required `stream_name` argument is a Python `str` that uniquely identifies a
-stream to which a sequence of events will be appended.
-
-The required `current_version` argument is expected to be either a Python `int`
-that indicates the stream position of the last recorded event in the stream.
-
-The required `event` argument is expected to be a single new event object. The event
-object is expected to be an instance of the `NewEvent` class.
-
-This method also has an optional `timeout` argument, which is a Python `float`
-that sets a deadline for the completion of the gRPC operation.
-
-
 ### Idempotent append operations
 
-The `append_event()` and `append_events()` and methods are "idempotent", in that
-if the methods are called with new events whose `id` attribute values equal those
-of recorded events in the named stream immediately after the stream position specified
-by the value of the `current_version` argument, then these methods will return the
-commit position of the last new event, without making any changes to the database.
-
-Sometimes it may happen, when calling `append_event()` or `append_events()`, that
-the new events are successfully recorded but somehow a connection issue occurs before
-the successful call can return successfully to the client. We cannot be sure if
-the events were recorded or not, and so we may wish to retry. If the events were in
-fact successfully recorded, it is convenient for the retried operation to return
-successfully without raising an exception. If those new events were in fact not recorded,
-and in the meantime no other new events were recorded in that stream, then it makes sense
-that the new events will be recorded when the append operation is retried. Of course,
-if a `WrongCurrentVersion` exception is raised when retrying the operation, then an
-application command which generated the new events in the context of already recorded
-events may need to be executed again. Alternatively, a suitable error might be displayed
-by the application, with an up-to-date view of the recorded data, giving a user of the
-application an opportunity to decide if they still wish to proceed with their original
-intention.
+The `append_to_stream()` method is "idempotent", in that if called with new events whose
+`id` attribute values equal those of recorded events in the named stream immediately
+after the stream position specified by the value of the `current_version` argument, then
+it will return the commit position of the last new event, without making any changes to
+the database.
+
+Sometimes it may happen, when calling `append_to_stream()`, that the new events are
+successfully recorded but somehow a connection issue occurs before the successful call
+can return successfully to the client. We cannot be sure if the events were recorded
+or not, and so we may wish to retry. If the events were in fact successfully recorded,
+it is convenient for the retried operation to return successfully without raising an
+exception. If those new events were in fact not recorded, and in the meantime no other
+new events were recorded in that stream, then it makes sense that the new events will
+be recorded when the append operation is retried. Of course, if a `WrongCurrentVersion`
+exception is raised when retrying the operation, then an application command which
+generated the new events in the context of already recorded events may need to be
+executed again. Alternatively, a suitable error might be displayed by the application,
+with an up-to-date view of the recorded data, giving a user of the application an
+opportunity to decide if they still wish to proceed with their original intention.
 
-The example below shows the `append_events()` method being called again with
+The example below shows the `append_to_stream()` method being called again with
 `event3` and `current_version=0`. We can see that repeating the call to
-`append_events()` returns successfully.
+`append_to_stream()` returns successfully.
 
 ```python
 # Retry appending event3.
-commit_position_retry = client.append_events(
+commit_position_retry = client.append_to_stream(
     stream_name=stream_name1,
     current_version=0,
     events=[event2, event3],
 )
 ```
 
 We can see that the same commit position is returned as above.
 
 ```python
 assert commit_position_retry == commit_position2
 ```
 
-By calling `read_stream_events()`, we can also see the stream has been unchanged
-despite the `append_events()` method having been called twice with the same arguments.
+By calling `get_stream()`, we can also see the stream has been unchanged
+despite the `append_to_stream()` method having been called twice with the same arguments.
 That is, there are still only three events in the stream.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1
 )
 
 assert len(events) == 3
 ```
 
 This idempotent behaviour depends on the `id` attribute of the `NewEvent` class.
 This attribute, by default, is assigned a new and unique version-4 UUID when an
 instance of `NewEvent` is constructed. The `id` argument can be used when
 constructing `NewEvent` objects to set the value of this attribute.
 
 
 ### Read stream events
 
-The `read_stream_events()` method can be used to get events that have been appended
-to a stream. This method returns a Python `tuple` of recorded event objects. The
-recorded event objects are instances of the `RecordedEvent` class.
+The `read_stream()` method can be used to get events that have been appended
+to a stream. This method returns a "read response" object.
 
-This method has one required argument, `stream_name`.
+A "read response" object is a Python iterator. Recorded events can be
+obtained by iterating over the "read response" object. Recorded events are
+streamed from the server to the client as the iteration proceeds. The iteration
+will automatically stop when there are no more recorded events to be returned.
+The streaming of events, and hence the iterator, can also be stopped by calling
+the `stop()` method on the "read response" object.
+
+The `get_stream()` method can be used to get events that have been appended
+to a stream. This method returns a Python `tuple` of recorded event objects.
+The recorded event objects are instances of the `RecordedEvent` class. It
+calls `read_stream()` and passes the "read response" iterator into a Python
+`tuple`, so that the streaming will complete before the method returns.
+
+The `read_stream()` and `get_stream()` methods have one required argument, `stream_name`.
 
 The required `stream_name` argument is a Python `str` that uniquely identifies a
 stream from which recorded events will be returned.
 
-The `read_stream_events()` method also has four optional arguments,
+The `read_stream()` and `get_stream()` methods also have four optional arguments,
 `stream_position`, `backwards`, `limit`, and `timeout`.
 
 The optional `stream_position` argument is a Python `int` that can be used to
 indicate the position in the stream from which to start reading. The default value
 of `stream_position` is `None`. When reading a stream from a specific position in the
 stream, the recorded event at that position will be included, both when reading
 forwards from that position, and when reading backwards.
 
 The optional `backwards` argument is a Python `bool`. The default value of `backwards`
 is `False`, which means the stream will be read forwards, so that events are returned
 in the order they were recorded. If `backwards` is `True`, the events are returned in
 reverse order.
 
 If `backwards` is `False` and `stream_position` is `None`, the stream's events will be
-returned in the order they were recorded, starting from the first recorded event. This
-is the default behavior of `read_stream_events()`. If `backwards` is `True` and
-`stream_position` is `None`, the stream's events will be returned in reverse order,
-starting from the last recorded event.
+returned in the order they were recorded, starting from the first recorded event. If
+`backwards` is `True` and `stream_position` is `None`, the stream's events will be
+returned in reverse order, starting from the last recorded event.
 
 The optional `limit` argument is a Python `int` which restricts the number of events
 that will be returned. The default value of `limit` is `sys.maxint`.
 
 The optional `timeout` argument is a Python `float` which sets a deadline for
 the completion of the gRPC operation.
 
-The example below shows the default behavior of this method, which is to return all
-the recorded events of a stream forwards from the first recorded events to the last.
+The example below shows the default behavior, which is to return all the recorded
+events of a stream forwards from the first recorded events to the last.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1
 )
 
 assert len(events) == 3
 assert events[0].id == event1.id
 assert events[1].id == event2.id
 assert events[2].id == event3.id
@@ -935,105 +924,91 @@
 
 The example below shows how to use the `stream_position` argument to read a stream
 from a specific stream position to the end of the stream. Stream positions are
 zero-based, and so `stream_position=1` corresponds to the second event that was
 recorded in the stream, in this case `event2`.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1,
     stream_position=1,
 )
 
 assert len(events) == 2
 assert events[0].id == event2.id
 assert events[1].id == event3.id
 ```
 
 The example below shows how to use the `backwards` argument to read a stream backwards.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1,
     backwards=True,
 )
 
 assert len(events) == 3
 assert events[0].id == event3.id
 assert events[1].id == event2.id
 assert events[2].id == event1.id
 ```
 
 The example below shows how to use the `limit` argument to read a limited number of
 events.
 
 ```python
-events = client.read_stream_events(
+events = client.get_stream(
     stream_name=stream_name1,
     limit=2,
 )
 
 assert len(events) == 2
 assert events[0].id == event1.id
 assert events[1].id == event2.id
 ```
 
-The `read_stream_events()` method will raise a `NotFound` exception if the named stream
-has never existed or has been deleted.
+The `read_stream()` and `get_stream()` methods will raise a `NotFound` exception if the
+named stream has never existed or has been deleted.
 
 ```python
 from esdbclient.exceptions import NotFound
 
 
 try:
-    client.read_stream_events('does-not-exist')
+    client.get_stream('does-not-exist')
 except NotFound:
     pass  # The stream does not exist.
 else:
     raise Exception("Shouldn't get here")
 ```
 
-Please note, this method streams recorded events from the server and then
-constructs and returns a Python `tuple`. In case you don't want the client to
-finish streaming events from the database before it returns, you can instead
-use the `iter_stream_events()` method, which returns an iterable "read response"
-object. A "read response" is an iterator, and not a sequence. Recorded events can
-be obtained by iterating over the "read response" object. It streams recorded events
-from the server as the iteration proceeds. The iteration will automatically stop
-when there are no more recorded events to be returned. The streaming of events,
-and hence the iterator, can also be stopped prematurely by calling the `stop()`
-method on the "read response" object.
-
-In fact, the `read_stream_events()` method calls `iter_stream_events()` and passes
-the "read response" iterator into the Python `tuple` constructor. However, the
-`read_stream_events()` method is decorated with retry and reconnect decorators,
-whilst the `iter_stream_events()` method is not. This means that all errors due to
-connection issues will be caught by the retry and reconnect decorators when calling
-the `read_stream_events()` method, but not when calling `iter_stream_events()`. The
-`iter_stream_events()` method has no such decorators because the streaming only starts
+Please note, the `get_stream()` method is decorated with the `@autoreconnect` and
+`@retrygrpc` decorators, whilst the `read_stream()` method is not. This means that
+all errors due to connection issues will be caught by the retry and reconnect decorators
+when calling the `get_stream()` method, but not when calling `read_stream()`. The
+`read_stream()` method has no such decorators because the streaming only starts
 when iterating over the "read response" starts, which means that the method returns
 before the streaming starts, and so there is no chance for any decorators to catch
 any connection issues.
 
-Nevertheless, if you are reading a very large stream, then you might prefer to call
-`iter_stream_events()`, and to begin iterating through the recorded events whilst
-they are being streamed from the server, rather than both waiting and having them
-all accumulate in memory. Because of the risk of connection issues arising during
-the streaming of recorded events from the server, you will need to care about
-connection issues when iterating over the "read response" object returned from
-`iter_stream_events()`.
+For the same reason, `read_stream()` will not raise a `NotFound` exception when
+the stream does not exist, until iterating over the "read response" object begins.
+
+If you are reading a very large stream, then you might prefer to call `read_stream()`,
+and begin iterating through the recorded events whilst they are being streamed from
+the server, rather than both waiting and having them all accumulate in memory.
 
 ### Get current version
 
 The `get_current_version()` method is a convenience method that essentially calls
-`read_stream_events()` with `backwards=True` and `limit=1`. This method returns
+`get_stream()` with `backwards=True` and `limit=1`. This method returns
 the value of the `stream_position` attribute of the last recorded event in a
-stream. If a stream does not exist, the returned value is `None`. The returned
-value is the correct value of `current_version` when appending new events to
-a stream.
+stream. If a stream does not exist, the returned value is `StreamState.NO_STREAM`.
+The returned value is the correct value of `current_version` when appending events
+to a stream, and when deleting or tombstoning a stream.
 
 This method has one required argument, `stream_name`.
 
 The required `stream_name` argument is a Python `str` that uniquely identifies a
 stream from which a stream position will be returned.
 
 This method also has an optional `timeout` argument, that
@@ -1048,25 +1023,25 @@
 current_version = client.get_current_version(
     stream_name=stream_name1
 )
 
 assert current_version == 2
 ```
 
-If a stream has never existed or has been deleted, the returned value is `None`,
-which matches the required value of the `current_version` argument both when
-appending the first event of a new stream, and also when appending events to
-a stream that has been deleted.
+If a stream has never existed or has been deleted, the returned value is
+`StreamState.NO_STREAM`, which is the correct value of the `current_version`
+argument both when appending the first event of a new stream, and also when
+appending events to a stream that has been deleted.
 
 ```python
 current_version = client.get_current_version(
     stream_name='does-not-exist'
 )
 
-assert current_version is None
+assert current_version is StreamState.NO_STREAM
 ```
 
 ### How to implement snapshotting with EventStoreDB
 
 Snapshots can improve the performance of aggregates that would otherwise be
 reconstructed from very long streams. However, it is generally recommended to design
 aggregates to have a finite lifecycle, and so to have relatively short streams,
@@ -1086,15 +1061,15 @@
 
 
 def get_aggregate(aggregate_id, mutator_func):
     stream_name = aggregate_id
 
     # Get recorded events.
     try:
-        events = client.read_stream_events(
+        events = client.get_stream(
             stream_name=stream_name,
             stream_position=None
         )
     except NotFound as e:
         raise AggregateNotFound(aggregate_id) from e
     else:
         # Reconstruct aggregate from recorded events.
@@ -1145,30 +1120,30 @@
 
 def get_aggregate(aggregate_id, mutator_func):
     stream_name = aggregate_id
     recorded_events = []
 
     # Look for a snapshot.
     try:
-        snapshots = client.read_stream_events(
+        snapshots = client.get_stream(
             stream_name=make_snapshot_stream_name(stream_name),
             backwards=True,
             limit=1
         )
     except NotFound:
         stream_position = None
     else:
         assert len(snapshots) == 1
         snapshot = snapshots[0]
         stream_position = deserialize(snapshot.metadata)['version'] + 1
         recorded_events.append(snapshot)
 
     # Get subsequent events.
     try:
-        events = client.read_stream_events(
+        events = client.get_stream(
             stream_name=stream_name,
             stream_position=stream_position
         )
     except NotFound as e:
         raise AggregateNotFound(aggregate_id) from e
     else:
         recorded_events += events
@@ -1208,15 +1183,15 @@
 
 @dataclass(frozen=True)
 class Dog(Aggregate):
     name: str
     tricks: list
 ```
 
-Let's also define a mutator function `mutate_dog()` that can evolve the state of a
+Let's also define a mutator function `mutate_dog()` that evolves the state of a
 `Dog` aggregate given various different types of events, `'DogRegistered'`,
 `'DogLearnedTrick'`, and `'Snapshot'`.
 
 ```python
 def mutate_dog(dog, event):
     data = deserialize(event.data)
     if event.type == 'DogRegistered':
@@ -1273,46 +1248,46 @@
 ```python
 def register_dog(name):
     dog_id = str(uuid.uuid4())
     event = NewEvent(
         type='DogRegistered',
         data=serialize({'name': name}),
     )
-    client.append_event(
+    client.append_to_stream(
         stream_name=dog_id,
-        current_version=None,
-        event=event,
+        current_version=StreamState.NO_STREAM,
+        events=event,
     )
     return dog_id
 
 
 def record_trick_learned(dog_id, trick):
     dog = get_dog(dog_id)
     event = NewEvent(
         type='DogLearnedTrick',
         data=serialize({'trick': trick}),
     )
-    client.append_event(
+    client.append_to_stream(
         stream_name=dog_id,
         current_version=dog.version,
-        event=event,
+        events=event,
     )
 
 
 def snapshot_dog(dog_id):
     dog = get_dog(dog_id)
     event = NewEvent(
         type='Snapshot',
         data=serialize({'name': dog.name, 'tricks': dog.tricks}),
         metadata=serialize({'version': dog.version}),
     )
-    client.append_event(
+    client.append_to_stream(
         stream_name=make_snapshot_stream_name(dog_id),
-        current_version=-1,
-        event=event,
+        current_version=StreamState.ANY,
+        events=event,
     )
 ```
 
 We can call `register_dog()` to register a new dog.
 
 ```python
 # Register a new dog.
@@ -1385,43 +1360,44 @@
 Snapshots can be created at fixed version number intervals, fixed time
 periods, after a particular type of event, immediately after events are
 appended, or as a background process.
 
 
 ### Read all events
 
-The `read_all_events()` method can be used to get all recorded events
-in the database in the order they were recorded. This method will return
-a "read response" object, just like `iter_stream_events()`.
+The `read_all()` method can be used to get all recorded events
+in the database in the order they were recorded. This method returns
+a "read response" object, just like `read_stream()`.
 
 A "read response" is an iterator, and not a sequence. Recorded events can be
-obtained by iterating over the "read response" object. It streams recorded
-events from the server as the iteration proceeds. The iteration will automatically
-stop when there are no more recorded events to be returned. The streaming of events,
-and hence the iterator, can also be stopped by calling the `stop()` method on the
-"read response" object.
-
-Just like `read_stream_events()` and `iter_stream_events()`, the received event objects
+obtained by iterating over the "read response" object. Recorded events are
+streamed from the server to the client as the iteration proceeds. The iteration
+will automatically stop when there are no more recorded events to be returned.
+The streaming of events, and hence the iterator, can also be stopped by calling
+the `stop()` method on the "read response" object. The recorded event objects
 are instances of the `RecordedEvent` class.
 
 This method has seven optional arguments, `commit_position`, `backwards`,
 `filter_exclude`, `filter_include`, `filter_by_stream_name`, `limit`, and `timeout`.
 
 The optional `commit_position` argument is a Python `int` that can be used to
 specify a commit position from which to start reading. The default value of
 `commit_position` is `None`. Please note, if a commit position is specified,
-it must be an actually existing commit position in the database.
+it must be an actually existing commit position in the database. When reading
+forwards, the event at the commit position may be included, depending upon the
+filter. When reading backwards, the event at the commit position will not be
+included.
 
 The optional `backwards` argument is a Python `bool`. The default of `backwards` is
 `False`, which means events are returned in the order they were recorded, If
 `backwards` is `True`, then events are returned in reverse order.
 
 If `backwards` is `False` and `commit_position` is `None`, the database's events will
 be returned in the order they were recorded, starting from the first recorded event.
-This is the default behavior of `read_all_events()`. If `backwards` is `True` and
+This is the default behavior of `read_all()`. If `backwards` is `True` and
 `commit_position` is `None`, the database's events will be returned in reverse order,
 starting from the last recorded event.
 
 The optional `filter_exclude` argument is a sequence of regular expressions that
 specifies which recorded events should be returned. This argument is ignored
 if `filter_include` is set to a non-empty sequence. The default value of this
 argument matches the event types of EventStoreDB "system events", so that system
@@ -1449,15 +1425,15 @@
 
 The example below shows how to get all the events we have recorded in the database
 so far, in the order they were recorded. We can see the three events of `stream_name1`
 (`event1`, `event2` and `event3`) are included, along with others.
 
 ```python
 # Read all events (creates a streaming gRPC call).
-read_response = client.read_all_events()
+read_response = client.read_all()
 
 # Convert the iterator into a sequence of recorded events.
 events = tuple(read_response)
 assert len(events) > 3  # more than three
 
 # Convert the sequence of recorded events into a set of event IDs.
 event_ids = set(e.id for e in events)
@@ -1471,15 +1447,15 @@
 forwards from a specific commit position, the event at the specified position
 will be included. The value of `commit_position1` is the position we obtained
 when appending `event1`. And so `event1` is the first recorded event we shall
 receive, `event2` is the second, and `event3` is the third.
 
 ```python
 # Read all events forwards from a commit position.
-read_response = client.read_all_events(
+read_response = client.read_all(
     commit_position=commit_position1
 )
 
 # Step through the "read response" iterator.
 assert next(read_response).id == event1.id
 assert next(read_response).id == event2.id
 assert next(read_response).id == event3.id
@@ -1491,15 +1467,15 @@
 The example below shows how to read all events recorded in the database in reverse
 order. We can see that the first events we receive are the last events that were
 recorded: the events of the `Dog` aggregate from the section about snapshotting
 and the snapshot.
 
 ```python
 # Read all events backwards from the end.
-read_response = client.read_all_events(
+read_response = client.read_all(
     backwards=True
 )
 
 # Step through the "read response" iterator.
 assert next(read_response).type == "DogLearnedTrick"
 assert next(read_response).type == "Snapshot"
 assert next(read_response).type == "DogLearnedTrick"
@@ -1511,15 +1487,15 @@
 ```
 
 The example below shows how to read a limited number of events
 forwards from a specific commit position.
 
 ```python
 events = tuple(
-    client.read_all_events(
+    client.read_all(
         commit_position=commit_position1,
         limit=1,
     )
 )
 
 assert len(events) == 1
 assert events[0].id == event1.id
@@ -1527,48 +1503,48 @@
 
 The example below shows how to read a limited number of the recorded events
 in the database backwards from the end. In this case, the limit is 1, and
 so we receive the last recorded event.
 
 ```python
 events = tuple(
-    client.read_all_events(
+    client.read_all(
         backwards=True,
         limit=1,
     )
 )
 
 assert len(events) == 1
 
 assert events[0].type == 'DogLearnedTrick'
 assert deserialize(events[0].data)['trick'] == 'sit'
 ```
 
-Please note, like the `iter_stream_events()` method, the `read_all_events()` method
+Please note, like the `read_stream()` method, the `read_all()` method
 is not decorated with retry and reconnect decorators, because the streaming of recorded
 events from the server only starts when iterating over the "read response" starts, which
 means that the method returns before the streaming starts, and so there is no chance for
 any decorators to catch any connection issues.
 
 ### Get commit position
 
 The `get_commit_position()` method can be used to get the commit position of the
-last recorded event in the database. It simply calls `read_all_events()` with
+last recorded event in the database. It simply calls `read_all()` with
 `backwards=True` and `limit=1`, and returns the value of the `commit_position`
 attribute of the last recorded event.
 
 ```python
 commit_position = client.get_commit_position()
 ```
 
 This method has four optional arguments, `filter_exclude`, `filter_include`,
-`filter_by_stream_name` and `timeout`. These values are passed to `read_all_events()`.
+`filter_by_stream_name` and `timeout`. These values are passed to `read_all()`.
 
 The optional `filter_exclude`, `filter_include` and `filter_by_stream_name` arguments
-work in the same way as they do in the `read_all_events()` method.
+work in the same way as they do in the `read_all()` method.
 
 This optional `timeout` argument is a Python `float` that sets
 a deadline for the completion of the gRPC operation.
 
 This method might be used to measure progress of a downstream component
 that is processing all recorded events, by comparing the current commit
 position with the recorded commit position of the last successfully processed
@@ -1640,58 +1616,59 @@
 
 After tombstoning a stream, it's not possible to append new events.
 
 
 ## Catch-up subscriptions
 
 A "catch-up" subscription can be used to receive events that have already been
-recorded in the database, and also events that are recorded subsequently.
+recorded in the database, and events that are recorded subsequently. A catch-up
+subscription can be used by an event-processing component that processes recorded
+events with "exactly-once" semantics.
+
+The `subscribe_to_all()` method starts a catch-up subscription that can receive
+all events in the database. The `subscribe_to_stream()` method starts a catch-up
+subscription that can receive events from a specific stream. Both methods return a
+"catch-up subscription" object, which is a Python iterator. Recorded events can be
+obtained by iteration. Recorded event objects obtained in this way are instances
+of the `RecordedEvent` class. Please note, the `subscribe_to_all()` method will
+occasionally return `Checkpoint` objects. These are a special type of `RecordedEvent`
+that have a `commit_position`, so that downstream event-processing components can
+record progress across a large number of events that have been filtered out.
+
+Before the "catch-up subscription" object is returned to the caller, the client will
+firstly obtain a "confirmation" response from the server, which allows the client to
+detect that both the gRPC connection and the streaming gRPC call is operational. For
+this reason, the `subscribe_to_all()` and `subscribe_to_stream()` methods are both
+usefully decorated with the reconnect and retry decorators. However, once the method
+has returned, the decorators will have exited, and any exceptions that are raised
+due to connection issues whilst iterating over the subscription object will have to
+be handled by your code.
+
+A "catch-up subscription" iterator will not automatically stop when there are no more
+events to be returned, but instead the iteration will block until new events are
+subsequently recorded in the database. Any subsequently recorded events will then be
+immediately streamed to the client, and the iteration will then continue. The streaming
+of events, and hence the iteration, can be stopped by calling the `stop()` method on the
+"catch-up subscription" object.
+
+### Subscribe to all events
+
+The`subscribe_to_all()` method can be used to start a catch-up subscription
+from which all events recorded in the database can be obtained in the order
+they were recorded. This method returns a "catch-up subscription" iterator.
 
-The `subscribe_all_events()` method starts a catch-up subscription that can receive
-all events in the database. The `subscribe_stream_events()` method starts a catch-up
-subscription that can receive events from a specific stream.
-
-The `subscribe_all_events()` and `subscribe_stream_events()` methods both return a
-"read response" iterator, much like `iter_stream_events()` and `read_all_events()`.
-The difference is the "read response" iterator returned for a catch-up subscription
-does not automatically stop when there are no more recorded events to be returned, but
-instead blocks on getting the next event until further events are recorded in the
-database. These subsequently recorded events will then be streamed to the iterator,
-which will then continue. Like `read_all_events()`, the returned "read response" has
-a `stop()` method which will cancel the streaming gRPC operation and cause the
-"read response" iterator to stop.
-
-Like with `read_stream_events()` and `read_all_events()`, the recorded event objects
-received from a catch-up subscription are instances of the `RecordedEvent` class.
-
-### Subscribe all events
-
-The`subscribe_all_events()` method can be used to start a catch-up subscription
-from which all events recorded in the database can be received.
-
-This method can be used by a downstream component that processes recorded events with
-exactly-once semantics.
-
-This method returns a "read response", from which recorded events can be
-obtained by iteration, including events that are recorded after all the
-recorded events have been received. Iterating over this "read response"
-object will therefore not stop, unless the `stop()` method of the
-"read response" object is called, or a connection issue occurs, or
-the returned object iterator object is deleted from memory.
-
-This method has an optional `commit_position` argument, which can be
-used to specify a commit position from which to subscribe. The default
-value is `None`, which means the subscription will operate from the first
-recorded event in the database. If a commit position is given, it must match
-an actually existing commit position in the database. The recoded events that
-are obtained will not include the event recorded at that commit position.
-
-This method also has four other optional arguments, `filter_exclude`,
+This method also has five optional arguments, `commit_position()`, `filter_exclude`,
 `filter_include`, `filter_by_stream_name`, and `timeout`.
 
+The optional `commit_position` argument specifies a commit position. The default
+value of `commit_position` is `None`, which means the catch-up subscription will
+start from the first recorded event in the database. If a commit position is given,
+it must match an actually existing commit position in the database. Only events
+recorded after that position will be obtained.
+
 The optional `filter_exclude` argument is a sequence of regular expressions that
 specifies which recorded events should be returned. This argument is ignored
 if `filter_include` is set to a non-empty sequence. The default value of this
 argument matches the event types of EventStoreDB "system events", so that system
 events will not normally be included. See the Notes section below for more
 information about filter expressions.
 
@@ -1704,124 +1681,124 @@
 whether the filtering will apply to event types or stream names. By default, this
 value is `False` and so the filtering will apply to the event type strings of
 recorded events.
 
 The optional `timeout` argument is a Python `float` which sets a
 deadline for the completion of the gRPC operation.
 
-The example below shows how to start a catch-up subscription to receive
+The example below shows how to start a catch-up subscription that starts
 from the first recorded event in the database.
 
 ```python
 # Subscribe from the first recorded event in the database.
-subscription = client.subscribe_all_events()
+catchup_subscription = client.subscribe_to_all()
 ```
 
-The example below is longer, and shows that the catch-up subscription
-does not stop automatically, but blocks when the last recorded event is
-received, and then continues when subsequent events are recorded.
+The example below shows that catch-up subscriptions do not stop
+automatically, but block when the last recorded event is received,
+and then continue when subsequent events are recorded.
 
 ```python
+from datetime import datetime
+from threading import Thread
+
+from esdbclient import Checkpoint
+
 # Append a new event to a new stream.
 stream_name2 = str(uuid.uuid4())
 event4 = NewEvent(type='OrderCreated', data=b'data4')
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name2,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event4],
 )
 
-# Subscribe from the first recorded event in the database.
-subscription = client.subscribe_all_events()
-received_events = []
-
 
 # Receive events from the catch-up subscription in a different thread.
-from datetime import datetime
-from threading import Thread
-
+received_events = []
 mark = datetime.now()
 
 def receive_events():
-    for event in subscription:
-        received_events.append(event)
+    for event in catchup_subscription:
         global mark
         mark = datetime.now()
+        received_events.append(event)
 
 
 def wait_for_subscription_to_block():
     while True:
          if (datetime.now() - mark).total_seconds() > 1:
              break
 
 
-thread = Thread(target=receive_events)
+thread = Thread(target=receive_events, daemon=True)
 thread.start()
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 # Check the last received event is 'event4'.
-assert received_events[-1].id == event4.id
+assert received_events[-1].id == event4.id, received_events[-1].id
 
 # Check we also received the other events we have recorded.
 assert received_events[-9].id == event1.id
 assert received_events[-8].id == event2.id
 assert received_events[-7].id == event3.id
 assert received_events[-6].type == "DogRegistered"
 assert received_events[-5].type == "DogLearnedTrick"
 assert received_events[-4].type == "DogLearnedTrick"
 assert received_events[-3].type == "Snapshot"
 assert received_events[-2].type == "DogLearnedTrick"
 
 # Append another event whilst the subscription is running.
 mark = datetime.now()
 event5 = NewEvent(type='OrderUpdated', data=b'data5')
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name2,
     current_version=0,
     events=[event5],
 )
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 # Check the last received event is 'event5'.
 assert received_events[-2].id == event4.id
 assert received_events[-1].id == event5.id
 
 # Stop the subscription.
-subscription.stop()
+catchup_subscription.stop()
 thread.join()
 ```
 
-The example below shows how to start a catch-up subscription to
-receive from a particular commit position, in this case from the
-commit position of the last recorded event that was received above.
-Another event is recorded before the subscription is restarted.
-Further events are recorded whilst the subscription is running.
-All the recorded events are received exactly once.
+The example below shows how to subscribe to events recorded after a
+particular commit position, in this case from the commit position of
+the last recorded event that was received above. Another event is
+recorded before the subscription is restarted. Further events are
+recorded whilst the subscription is running. All the recorded events
+are received exactly once.
 
 ```python
 
 # Append another event.
 event6 = NewEvent(type='OrderDeleted', data=b'data6')
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name2,
     current_version=1,
     events=[event6],
 )
 
-# Resume subscribing from the commit position of the last received event.
-subscription = client.subscribe_all_events(
+# Restart subscribing to all events after the
+# commit position of the last received event.
+catchup_subscription = client.subscribe_to_all(
     commit_position=received_events[-1].commit_position
 )
 
 mark = datetime.now()
-thread = Thread(target=receive_events)
+thread = Thread(target=receive_events, daemon=True)
 thread.start()
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 # Check the last received event was 'event6'.
 assert received_events[-3].id == event4.id
@@ -1831,17 +1808,17 @@
 # Append three more events to a new stream.
 mark = datetime.now()
 stream_name3 = str(uuid.uuid4())
 event7 = NewEvent(type='OrderCreated', data=b'data7')
 event8 = NewEvent(type='OrderUpdated', data=b'data8')
 event9 = NewEvent(type='OrderDeleted', data=b'data9')
 
-client.append_events(
+client.append_to_stream(
     stream_name=stream_name3,
-    current_version=None,
+    current_version=StreamState.NO_STREAM,
     events=[event7, event8, event9],
 )
 
 # Wait for the subscription to block.
 wait_for_subscription_to_block()
 
 
@@ -1850,54 +1827,56 @@
 assert received_events[-5].id == event5.id
 assert received_events[-4].id == event6.id
 assert received_events[-3].id == event7.id
 assert received_events[-2].id == event8.id
 assert received_events[-1].id == event9.id
 
 # Stop the subscription.
-subscription.stop()
+catchup_subscription.stop()
 thread.join()
 ```
 
 The catch-up subscription call is ended as soon as the subscription object's
 `stop()` method is called. This happens automatically when it goes out of scope,
 or when it is explicitly deleted from memory using the Python `del` keyword.
 
-### Subscribe stream events
+### Subscribe to stream events
 
-The `subscribe_stream_events()` method can be used to start a catch-up subscription
-that can return events that are recorded in a single stream.
+The `subscribe_to_stream()` method can be used to start a catch-up subscription
+from which events recorded in a single stream can be obtained. This method
+returns a "catch-up subscription" iterator.
 
 This method has a required `stream_name` argument, which specifies the name of the
 stream from which recorded events will be received.
 
 This method also has two optional arguments, `stream_position`, and `timeout`.
 
-The optional `stream_position` argument specifies a position in the stream from which
-recorded events will be received. The event at the specified stream position will not
-be included. The default value of `stream_position` is `None`, which means the
-subscription will start from the first recorded event in the stream.
+The optional `stream_position` argument specifies a position in the stream. The
+default value of `stream_position` is `None`, which means that all events
+recorded in the stream will be obtained in the order they were recorded.
+If a stream position is given, then only events recorded after that position
+will be obtained.
 
 The optional `timeout` argument is a Python `float` that sets
 a deadline for the completion of the gRPC operation.
 
 The example below shows how to start a catch-up subscription from
 the first recorded event in a stream.
 
 ```python
 # Subscribe from the start of 'stream2'.
-subscription = client.subscribe_stream_events(stream_name=stream_name2)
+subscription = client.subscribe_to_stream(stream_name=stream_name2)
 ```
 
 The example below shows how to start a catch-up subscription from
 a particular stream position.
 
 ```python
 # Subscribe to stream2, from the second recorded event.
-subscription = client.subscribe_stream_events(
+subscription = client.subscribe_to_stream(
     stream_name=stream_name2,
     stream_position=1,
 )
 ```
 
 ### How to implement exactly-once event processing
 
@@ -2568,136 +2547,96 @@
 
 An example of when it might be desirable to reconnect manually is when (for performance
 reasons) the client's node preference is to be connected to a follower node in the
 cluster, and, after a cluster leader election, the follower becomes the leader.
 Reconnecting to a follower node in this case is currently beyond the capabilities of
 this client, but this behavior might be implemented in a future release.
 
-Please note, nearly all the client methods are decorated with `@autoreconnect` (which
-calls the `reconnect()` method when the client detects that reconnecting is required)
-and a `@retry` decorator that more generally will retry operations that fail due to
-connection issues.
-
-The `@autoreconnect` decorator will reconnect to a suitable node in the cluster when
-the server to which the client has been connected has become unavailable, or when the
-client's gRPC channel happens to have been closed. The client will also reconnect when
-a method is called that requires a leader, and the client's node preference is to be
-connected to a leader, but the node that the client has been connected to stops being
-the leader. In this case, the client will reconnect to the current leader. After
-reconnecting, the failed operation will be retried.
-
-The `@retry` decorator retries operations that have failed due to more general
-connection issues, such as a deadline being reached (so that the operation times
-out), or in case the server throws an exception when handling a client request.
-
-Please also note, the aspects not covered by the reconnect and retry decorator
-behaviours have to do with methods that return iterators. For example, consider
-the "read response" iterator returned from the `read_all_events()` method. The
-`read_all_events()` method will have returned, and the method decorators will therefore
-have exited, before iterating over the "read response" begins. Therefore, if a
-connection issues occurs whilst iterating over the "read response", it isn't possible
-for any decorator on the `read_all_events()` method to trigger a reconnection.
-
-Another example is iterating over the "read response" from a catch-up subscription.
-Although, with these methods there is an initial "confirmation" response from the server
-which is received and checked by the client before the method returns the
-"read response" iterator. And so, when the call is made, if the server is unavailable,
-or if the channel has somehow been closed, then the client will reconnect and retry.
-However, if an event-processing component that is iterating over a successfully returned
-catch-up subscription "read response" somehow fails, the catch-up subscription will
-need to be restarted, using the event-processing component's "last saved commit position".
-This is completely safe, so long as the event-processing component has been recording
-the commit position of each recorded event atomically and uniquely along with any new
-state that results from processing the recorded events and the commit positions are
-recorded with a uniqueness constraint. In this case, the client will automatically
-reconnect to a node in the cluster when the subsequent call to a catch-up subscription
-method is made. Similarly, when reading persistent subscriptions, if there are
-connectivity issues after you have started iterating over a successfully received
-response, then the consumer will need to be restarted.
-
+Reconnection will happen automatically in many cases, due to the `@autoreconnect`
+decorator.
 
 ### Close
 
 The `close()` method can be used to cleanly close the client's gRPC connection.
 
 ```python
 client.close()
 ```
 
 
 ## Asyncio client
 
 The `esdbclient` package also includes an early version of an asynchronous I/O
 gRPC Python client. It follows exactly the same behaviors as the multithreaded
-`ESDBClient`, but uses the `grpc.aio` package and the `asyncio` module, instead of
+`EventStoreDBClient`, but uses the `grpc.aio` package and the `asyncio` module, instead of
 `grpc` and `threading`.
 
-The async function `AsyncioESDBClient` constructs the client, and connects to
+The async function `AsyncioEventStoreDBClient` constructs the client, and connects to
 a server. It can be imported from `esdbclient`, and can be called with the same
-arguments as `ESDBClient`. It supports both the "esdb" and the "esdb+discover"
+arguments as `EventStoreDBClient`. It supports both the "esdb" and the "esdb+discover"
 connection string URI schemes, and can connect to both "secure" and "insecure"
 EventStoreDB servers. It reconnects or retries when connection issues or server
 errors are encountered.
 
 ```python
-from esdbclient import AsyncioESDBClient
+from esdbclient import AsyncioEventStoreDBClient
 ```
 
-The asynchronous I/O client has the following methods: `append_events()`,
-`read_stream_events()`, `read_all_events()`, `subscribe_all_events()`,
+The asynchronous I/O client has the following methods: `append_to_stream()`,
+`get_stream()`, `read_all()`, `subscribe_to_all()`,
 `delete_stream()`, `tombstone_stream()`, and `reconnect()`.
 
-These methods are equivalent to the methods on `ESDBClient`. They have the same
+These methods are equivalent to the methods on `EventStoreDBClient`. They have the same
 method signatures, and can be called with the same arguments, to the same effect.
-The methods which appear on `ESDBClient` but not on `AsyncioESDBClient` will be
+The methods which appear on `EventStoreDBClient` but not on `AsyncioEventStoreDBClient` will be
 added soon.
 
 ### Synopsis
 
-The example below demonstrates the `append_events()`, `read_stream_events()` and
-`subscribe_all_events()` methods. These are the most useful methods for writing
+The example below demonstrates the `append_to_stream()`, `get_stream()` and
+`subscribe_to_all()` methods. These are the most useful methods for writing
 an event-sourced application, allowing new aggregate events to be recorded, the
 recorded events of an aggregate to be obtained so aggregates can be reconstructed,
 and the state of an application to propagated and processed with "exactly-once"
 semantics.
 
 ```python
 import asyncio
 
 async def demonstrate_asyncio_client():
 
     # Construct client.
-    client = await AsyncioESDBClient(
+    client = await AsyncioEventStoreDBClient(
         uri=os.getenv("ESDB_URI"),
         root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"),
     )
 
     # Append events.
     stream_name = str(uuid.uuid4())
     event1 = NewEvent("OrderCreated", data=b'{}')
     event2 = NewEvent("OrderUpdated", data=b'{}')
     event3 = NewEvent("OrderDeleted", data=b'{}')
 
-    commit_position = await client.append_events(
+    commit_position = await client.append_to_stream(
         stream_name=stream_name,
-        current_version=None,
+        current_version=StreamState.NO_STREAM,
         events=[event1, event2, event3]
     )
 
     # Read stream events.
-    recorded = await client.read_stream_events(stream_name)
+    recorded = await client.get_stream(stream_name)
     assert len(recorded) == 3
     assert recorded[0].id == event1.id
     assert recorded[1].id == event2.id
     assert recorded[2].id == event3.id
 
 
     # Subscribe all events.
     received = []
-    async for event in await client.subscribe_all_events():
+    async for event in await client.subscribe_to_all():
         received.append(event)
         if event.commit_position == commit_position:
             break
     assert received[-3].id == event1.id
     assert received[-2].id == event2.id
     assert received[-1].id == event3.id
 
@@ -2712,22 +2651,30 @@
 )
 ```
 
 ## Notes
 
 ### Regular expression filters
 
-The `read_all_events()`, `subscribe_all_events()`, `create_subscription()`
+The `read_all()`, `subscribe_to_all()`, `create_subscription()`
 and `get_commit_position()` methods have `filter_exclude` and `filter_include`
 arguments. This section provides some more details about the values of these
 arguments.
 
-The default value of the `filter_exclude` arguments is designed to exclude
-EventStoreDB "system" and "persistence subscription config" events, which
-otherwise would be included.
+The first thing to note is that these arguments are sequences of regular expressions.
+They are concatenated together by the client as bracketed alternatives in a larger
+regular expression that is anchored to the start and end of the strings being
+matched. So you shouldn't include the `'^'` and `'$'` anchor characters, unless
+these characters are escaped as literal characters to be matched. But you should
+use wildcards if you want to match substrings, for example `'.*Snapshot'` to match
+all strings that end with `'Snapshot`'.
+
+In all methods, the default value of the `filter_exclude` argument is the constant
+`DEFAULT_EXCLUDE_FILTER`, which is designed to exclude EventStoreDB "system" and
+"persistence subscription config" event types, which otherwise would be included.
 
 System events generated by EventStoreDB have `type` strings that start with
 the `$` sign. Persistence subscription events generated when manipulating
 persistence subscriptions have `type` strings that start with `PersistentConfig`.
 
 For example, to match the type of EventStoreDB system events, use the regular
 expression string `r'\$.+'`. Please note, the constant `ESDB_SYSTEM_EVENTS_REGEX` is
@@ -2738,20 +2685,55 @@
 regular expression `r'PersistentConfig\d+'`. The constant `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`
 is set to this value. You can import this constant from `esdbclient`  and use it when
 building longer sequences of regular expressions.
 
 The constant `DEFAULT_EXCLUDE_FILTER` is a sequence of regular expressions that includes
 both `ESDB_SYSTEM_EVENTS_REGEX` and `ESDB_PERSISTENT_CONFIG_EVENTS_REGEX`. It is used
 as the default value of `filter_exclude` so that the events that EventStoreDB generates
-internally are excluded by default, events other than to those which you record using
-the `append_events()` method.
+internally are excluded by default.
+
+For example, if you want to exclude snapshots and system events and persistent subscription
+events, then you may wish to use a appropriately extended copy of `DEFAULT_EXCLUDE_FILTER`
+as the value of the `filter_exclude` arguments, such as `DEFAULT_EXCLUDE_FILTER + ['.*Snapshot']`.
+
+
+### Reconnect and retry method decorators
+
+Please note, nearly all the client methods are decorated with the `@autoreconnect` and
+the `@retrygrpc` decorators.
+
+The `@autoreconnect` decorator will reconnect to a suitable node in the cluster when
+the server to which the client has been connected has become unavailable, or when the
+client's gRPC channel happens to have been closed. The client will also reconnect when
+a method is called that requires a leader, and the client's node preference is to be
+connected to a leader, but the node that the client has been connected to stops being
+the leader. In this case, the client will reconnect to the current leader. After
+reconnecting, the failed operation will be retried.
 
-If you want to exclude, for example, snapshots from the recorded events returned when
-reading events from the database, then you may wish to use a appropriately extended
-copy of `DEFAULT_EXCLUDE_FILTER` as the value of the `filter_exclude` arguments.
+The `@retrygrpc` decorator retries operations that have failed due to a deadline being
+reached (so that the operation times out), and in case the server throws an exception
+when handling a client request.
+
+Please also note, the aspects not covered by the reconnect and retry decorator
+behaviours have to do with methods that return iterators. For example, consider
+the "read response" iterator returned from the `read_all()` method. The
+`read_all()` method will have returned, and the method decorators will therefore
+have exited, before iterating over the "read response" begins. Therefore, if a
+connection issues occurs whilst iterating over the "read response", it isn't possible
+for any decorator on the `read_all()` method to trigger a reconnection.
+
+With the "catch-up subscription" objects, there is an initial "confirmation" response
+from the server which is received and checked by the client. And so, when a call is
+made to `subscribe_to_all()` or `subscribe_to_stream()`, if the server is unavailable,
+or if the channel has somehow been closed, or if the request fails for some other reason,
+then the client will reconnect and retry. However, if an exception is raised when iterating over a
+successfully returned "catch-up subscription" object, the catch-up subscription will
+need to be restarted. Similarly, when reading persistent subscriptions, if there are
+connection issues whilst iterating over a successfully received response, the consumer
+will need to be restarted.
 
 
 ## Contributors
 
 ### Install Poetry
 
 The first thing is to check you have Poetry installed.
@@ -2853,8 +2835,7 @@
 
 Tests belong in `./tests`. Code-under-test belongs in `./esdbclient`.
 
 Edit package dependencies in `pyproject.toml`. Update installed packages (and the
 `poetry.lock` file) using the following command.
 
     $ make update-packages
-
```

