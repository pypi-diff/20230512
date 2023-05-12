# Comparing `tmp/grpcio-channelz-1.54.0rc1.tar.gz` & `tmp/grpcio-channelz-1.55.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-channelz-1.54.0rc1.tar", last modified: Fri Mar 31 21:34:14 2023, max compression
+gzip compressed data, was "grpcio-channelz-1.55.0rc1.tar", last modified: Wed Apr 26 10:35:42 2023, max compression
```

## Comparing `grpcio-channelz-1.54.0rc1.tar` & `grpcio-channelz-1.55.0rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:14.719330 grpcio-channelz-1.54.0rc1/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      104 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1162 2023-03-31 21:34:14.719330 grpcio-channelz-1.54.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:14.703328 grpcio-channelz-1.54.0rc1/grpc_channelz/
--rw-r--r--   0 root         (0) root         (0)      580 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:14.715329 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/
--rw-r--r--   0 root         (0) root         (0)      580 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/_async.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/_servicer.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz.py
--rw-r--r--   0 root         (0) root         (0)    15398 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz_pb2.py
--rw-r--r--   0 root         (0) root         (0)    23536 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    13199 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:34:14.715329 grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1162 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      721 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-31 21:34:14.000000 grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 21:34:14.719330 grpcio-channelz-1.54.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3250 2023-03-31 21:09:23.000000 grpcio-channelz-1.54.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:42.543858 grpcio-channelz-1.55.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-04-26 10:35:42.543858 grpcio-channelz-1.55.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:42.531857 grpcio-channelz-1.55.0rc1/grpc_channelz/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:42.539857 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/_async.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/_servicer.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz.py
+-rw-r--r--   0 root         (0) root         (0)    16425 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24126 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    13199 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:35:42.543858 grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      721 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 10:35:42.000000 grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 10:35:42.543858 grpcio-channelz-1.55.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-04-26 10:25:03.000000 grpcio-channelz-1.55.0rc1/setup.py
```

### Comparing `grpcio-channelz-1.54.0rc1/LICENSE` & `grpcio-channelz-1.55.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/PKG-INFO` & `grpcio-channelz-1.55.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.54.0rc1
+Version: 1.55.0rc1
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/__init__.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/__init__.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/_async.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/_async.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/_servicer.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/_servicer.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz_pb2.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,98 +15,99 @@
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fgrpc_channelz/v1/channelz.proto\x12\x10grpc.channelz.v1\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xfe\x01\n\x07\x43hannel\x12)\n\x03ref\x18\x01 \x01(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.grpc.channelz.v1.ChannelData\x12\x31\n\x0b\x63hannel_ref\x18\x03 \x03(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12\x37\n\x0esubchannel_ref\x18\x04 \x03(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12/\n\nsocket_ref\x18\x05 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\x84\x02\n\nSubchannel\x12,\n\x03ref\x18\x01 \x01(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.grpc.channelz.v1.ChannelData\x12\x31\n\x0b\x63hannel_ref\x18\x03 \x03(\x0b\x32\x1c.grpc.channelz.v1.ChannelRef\x12\x37\n\x0esubchannel_ref\x18\x04 \x03(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRef\x12/\n\nsocket_ref\x18\x05 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\xbb\x01\n\x18\x43hannelConnectivityState\x12?\n\x05state\x18\x01 \x01(\x0e\x32\x30.grpc.channelz.v1.ChannelConnectivityState.State\"^\n\x05State\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04IDLE\x10\x01\x12\x0e\n\nCONNECTING\x10\x02\x12\t\n\x05READY\x10\x03\x12\x15\n\x11TRANSIENT_FAILURE\x10\x04\x12\x0c\n\x08SHUTDOWN\x10\x05\"\x8e\x02\n\x0b\x43hannelData\x12\x39\n\x05state\x18\x01 \x01(\x0b\x32*.grpc.channelz.v1.ChannelConnectivityState\x12\x0e\n\x06target\x18\x02 \x01(\t\x12-\n\x05trace\x18\x03 \x01(\x0b\x32\x1e.grpc.channelz.v1.ChannelTrace\x12\x15\n\rcalls_started\x18\x04 \x01(\x03\x12\x17\n\x0f\x63\x61lls_succeeded\x18\x05 \x01(\x03\x12\x14\n\x0c\x63\x61lls_failed\x18\x06 \x01(\x03\x12?\n\x1blast_call_started_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xdb\x02\n\x11\x43hannelTraceEvent\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12>\n\x08severity\x18\x02 \x01(\x0e\x32,.grpc.channelz.v1.ChannelTraceEvent.Severity\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0b\x63hannel_ref\x18\x04 \x01(\x0b\x32\x1c.grpc.channelz.v1.ChannelRefH\x00\x12\x39\n\x0esubchannel_ref\x18\x05 \x01(\x0b\x32\x1f.grpc.channelz.v1.SubchannelRefH\x00\"E\n\x08Severity\x12\x0e\n\nCT_UNKNOWN\x10\x00\x12\x0b\n\x07\x43T_INFO\x10\x01\x12\x0e\n\nCT_WARNING\x10\x02\x12\x0c\n\x08\x43T_ERROR\x10\x03\x42\x0b\n\tchild_ref\"\x96\x01\n\x0c\x43hannelTrace\x12\x19\n\x11num_events_logged\x18\x01 \x01(\x03\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x06\x65vents\x18\x03 \x03(\x0b\x32#.grpc.channelz.v1.ChannelTraceEvent\"R\n\nChannelRef\x12\x12\n\nchannel_id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"X\n\rSubchannelRef\x12\x15\n\rsubchannel_id\x18\x07 \x01(\x03\x12\x0c\n\x04name\x18\x08 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"P\n\tSocketRef\x12\x11\n\tsocket_id\x18\x03 \x01(\x03\x12\x0c\n\x04name\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"P\n\tServerRef\x12\x11\n\tserver_id\x18\x05 \x01(\x03\x12\x0c\n\x04name\x18\x06 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"\x92\x01\n\x06Server\x12(\n\x03ref\x18\x01 \x01(\x0b\x32\x1b.grpc.channelz.v1.ServerRef\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.grpc.channelz.v1.ServerData\x12\x32\n\rlisten_socket\x18\x03 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\"\xc2\x01\n\nServerData\x12-\n\x05trace\x18\x01 \x01(\x0b\x32\x1e.grpc.channelz.v1.ChannelTrace\x12\x15\n\rcalls_started\x18\x02 \x01(\x03\x12\x17\n\x0f\x63\x61lls_succeeded\x18\x03 \x01(\x03\x12\x14\n\x0c\x63\x61lls_failed\x18\x04 \x01(\x03\x12?\n\x1blast_call_started_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xf6\x01\n\x06Socket\x12(\n\x03ref\x18\x01 \x01(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.grpc.channelz.v1.SocketData\x12(\n\x05local\x18\x03 \x01(\x0b\x32\x19.grpc.channelz.v1.Address\x12)\n\x06remote\x18\x04 \x01(\x0b\x32\x19.grpc.channelz.v1.Address\x12,\n\x08security\x18\x05 \x01(\x0b\x32\x1a.grpc.channelz.v1.Security\x12\x13\n\x0bremote_name\x18\x06 \x01(\t\"\xee\x04\n\nSocketData\x12\x17\n\x0fstreams_started\x18\x01 \x01(\x03\x12\x19\n\x11streams_succeeded\x18\x02 \x01(\x03\x12\x16\n\x0estreams_failed\x18\x03 \x01(\x03\x12\x15\n\rmessages_sent\x18\x04 \x01(\x03\x12\x19\n\x11messages_received\x18\x05 \x01(\x03\x12\x18\n\x10keep_alives_sent\x18\x06 \x01(\x03\x12G\n#last_local_stream_created_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12H\n$last_remote_stream_created_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12?\n\x1blast_message_sent_timestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x1flast_message_received_timestamp\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x19local_flow_control_window\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12?\n\x1aremote_flow_control_window\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12.\n\x06option\x18\r \x03(\x0b\x32\x1e.grpc.channelz.v1.SocketOption\"\xe8\x02\n\x07\x41\x64\x64ress\x12?\n\rtcpip_address\x18\x01 \x01(\x0b\x32&.grpc.channelz.v1.Address.TcpIpAddressH\x00\x12;\n\x0buds_address\x18\x02 \x01(\x0b\x32$.grpc.channelz.v1.Address.UdsAddressH\x00\x12?\n\rother_address\x18\x03 \x01(\x0b\x32&.grpc.channelz.v1.Address.OtherAddressH\x00\x1a\x30\n\x0cTcpIpAddress\x12\x12\n\nip_address\x18\x01 \x01(\x0c\x12\x0c\n\x04port\x18\x02 \x01(\x05\x1a\x1e\n\nUdsAddress\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x1a\x41\n\x0cOtherAddress\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyB\t\n\x07\x61\x64\x64ress\"\xbe\x02\n\x08Security\x12-\n\x03tls\x18\x01 \x01(\x0b\x32\x1e.grpc.channelz.v1.Security.TlsH\x00\x12\x39\n\x05other\x18\x02 \x01(\x0b\x32(.grpc.channelz.v1.Security.OtherSecurityH\x00\x1a{\n\x03Tls\x12\x17\n\rstandard_name\x18\x01 \x01(\tH\x00\x12\x14\n\nother_name\x18\x02 \x01(\tH\x00\x12\x19\n\x11local_certificate\x18\x03 \x01(\x0c\x12\x1a\n\x12remote_certificate\x18\x04 \x01(\x0c\x42\x0e\n\x0c\x63ipher_suite\x1a\x42\n\rOtherSecurity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyB\x07\n\x05model\"U\n\x0cSocketOption\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12(\n\nadditional\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\"B\n\x13SocketOptionTimeout\x12+\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\"Q\n\x12SocketOptionLinger\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xae\x05\n\x13SocketOptionTcpInfo\x12\x12\n\ntcpi_state\x18\x01 \x01(\r\x12\x15\n\rtcpi_ca_state\x18\x02 \x01(\r\x12\x18\n\x10tcpi_retransmits\x18\x03 \x01(\r\x12\x13\n\x0btcpi_probes\x18\x04 \x01(\r\x12\x14\n\x0ctcpi_backoff\x18\x05 \x01(\r\x12\x14\n\x0ctcpi_options\x18\x06 \x01(\r\x12\x17\n\x0ftcpi_snd_wscale\x18\x07 \x01(\r\x12\x17\n\x0ftcpi_rcv_wscale\x18\x08 \x01(\r\x12\x10\n\x08tcpi_rto\x18\t \x01(\r\x12\x10\n\x08tcpi_ato\x18\n \x01(\r\x12\x14\n\x0ctcpi_snd_mss\x18\x0b \x01(\r\x12\x14\n\x0ctcpi_rcv_mss\x18\x0c \x01(\r\x12\x14\n\x0ctcpi_unacked\x18\r \x01(\r\x12\x13\n\x0btcpi_sacked\x18\x0e \x01(\r\x12\x11\n\ttcpi_lost\x18\x0f \x01(\r\x12\x14\n\x0ctcpi_retrans\x18\x10 \x01(\r\x12\x14\n\x0ctcpi_fackets\x18\x11 \x01(\r\x12\x1b\n\x13tcpi_last_data_sent\x18\x12 \x01(\r\x12\x1a\n\x12tcpi_last_ack_sent\x18\x13 \x01(\r\x12\x1b\n\x13tcpi_last_data_recv\x18\x14 \x01(\r\x12\x1a\n\x12tcpi_last_ack_recv\x18\x15 \x01(\r\x12\x11\n\ttcpi_pmtu\x18\x16 \x01(\r\x12\x19\n\x11tcpi_rcv_ssthresh\x18\x17 \x01(\r\x12\x10\n\x08tcpi_rtt\x18\x18 \x01(\r\x12\x13\n\x0btcpi_rttvar\x18\x19 \x01(\r\x12\x19\n\x11tcpi_snd_ssthresh\x18\x1a \x01(\r\x12\x15\n\rtcpi_snd_cwnd\x18\x1b \x01(\r\x12\x13\n\x0btcpi_advmss\x18\x1c \x01(\r\x12\x17\n\x0ftcpi_reordering\x18\x1d \x01(\r\"F\n\x15GetTopChannelsRequest\x12\x18\n\x10start_channel_id\x18\x01 \x01(\x03\x12\x13\n\x0bmax_results\x18\x02 \x01(\x03\"Q\n\x16GetTopChannelsResponse\x12*\n\x07\x63hannel\x18\x01 \x03(\x0b\x32\x19.grpc.channelz.v1.Channel\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"A\n\x11GetServersRequest\x12\x17\n\x0fstart_server_id\x18\x01 \x01(\x03\x12\x13\n\x0bmax_results\x18\x02 \x01(\x03\"K\n\x12GetServersResponse\x12(\n\x06server\x18\x01 \x03(\x0b\x32\x18.grpc.channelz.v1.Server\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"%\n\x10GetServerRequest\x12\x11\n\tserver_id\x18\x01 \x01(\x03\"=\n\x11GetServerResponse\x12(\n\x06server\x18\x01 \x01(\x0b\x32\x18.grpc.channelz.v1.Server\"Z\n\x17GetServerSocketsRequest\x12\x11\n\tserver_id\x18\x01 \x01(\x03\x12\x17\n\x0fstart_socket_id\x18\x02 \x01(\x03\x12\x13\n\x0bmax_results\x18\x03 \x01(\x03\"X\n\x18GetServerSocketsResponse\x12/\n\nsocket_ref\x18\x01 \x03(\x0b\x32\x1b.grpc.channelz.v1.SocketRef\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x08\"\'\n\x11GetChannelRequest\x12\x12\n\nchannel_id\x18\x01 \x01(\x03\"@\n\x12GetChannelResponse\x12*\n\x07\x63hannel\x18\x01 \x01(\x0b\x32\x19.grpc.channelz.v1.Channel\"-\n\x14GetSubchannelRequest\x12\x15\n\rsubchannel_id\x18\x01 \x01(\x03\"I\n\x15GetSubchannelResponse\x12\x30\n\nsubchannel\x18\x01 \x01(\x0b\x32\x1c.grpc.channelz.v1.Subchannel\"6\n\x10GetSocketRequest\x12\x11\n\tsocket_id\x18\x01 \x01(\x03\x12\x0f\n\x07summary\x18\x02 \x01(\x08\"=\n\x11GetSocketResponse\x12(\n\x06socket\x18\x01 \x01(\x0b\x32\x18.grpc.channelz.v1.Socket2\x9a\x05\n\x08\x43hannelz\x12\x63\n\x0eGetTopChannels\x12\'.grpc.channelz.v1.GetTopChannelsRequest\x1a(.grpc.channelz.v1.GetTopChannelsResponse\x12W\n\nGetServers\x12#.grpc.channelz.v1.GetServersRequest\x1a$.grpc.channelz.v1.GetServersResponse\x12T\n\tGetServer\x12\".grpc.channelz.v1.GetServerRequest\x1a#.grpc.channelz.v1.GetServerResponse\x12i\n\x10GetServerSockets\x12).grpc.channelz.v1.GetServerSocketsRequest\x1a*.grpc.channelz.v1.GetServerSocketsResponse\x12W\n\nGetChannel\x12#.grpc.channelz.v1.GetChannelRequest\x1a$.grpc.channelz.v1.GetChannelResponse\x12`\n\rGetSubchannel\x12&.grpc.channelz.v1.GetSubchannelRequest\x1a\'.grpc.channelz.v1.GetSubchannelResponse\x12T\n\tGetSocket\x12\".grpc.channelz.v1.GetSocketRequest\x1a#.grpc.channelz.v1.GetSocketResponseBX\n\x13io.grpc.channelz.v1B\rChannelzProtoP\x01Z0google.golang.org/grpc/channelz/grpc_channelz_v1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_channelz.v1.channelz_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_channelz.v1.channelz_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023io.grpc.channelz.v1B\rChannelzProtoP\001Z0google.golang.org/grpc/channelz/grpc_channelz_v1'
-  _CHANNEL._serialized_start=178
-  _CHANNEL._serialized_end=432
-  _SUBCHANNEL._serialized_start=435
-  _SUBCHANNEL._serialized_end=695
-  _CHANNELCONNECTIVITYSTATE._serialized_start=698
-  _CHANNELCONNECTIVITYSTATE._serialized_end=885
-  _CHANNELCONNECTIVITYSTATE_STATE._serialized_start=791
-  _CHANNELCONNECTIVITYSTATE_STATE._serialized_end=885
-  _CHANNELDATA._serialized_start=888
-  _CHANNELDATA._serialized_end=1158
-  _CHANNELTRACEEVENT._serialized_start=1161
-  _CHANNELTRACEEVENT._serialized_end=1508
-  _CHANNELTRACEEVENT_SEVERITY._serialized_start=1426
-  _CHANNELTRACEEVENT_SEVERITY._serialized_end=1495
-  _CHANNELTRACE._serialized_start=1511
-  _CHANNELTRACE._serialized_end=1661
-  _CHANNELREF._serialized_start=1663
-  _CHANNELREF._serialized_end=1745
-  _SUBCHANNELREF._serialized_start=1747
-  _SUBCHANNELREF._serialized_end=1835
-  _SOCKETREF._serialized_start=1837
-  _SOCKETREF._serialized_end=1917
-  _SERVERREF._serialized_start=1919
-  _SERVERREF._serialized_end=1999
-  _SERVER._serialized_start=2002
-  _SERVER._serialized_end=2148
-  _SERVERDATA._serialized_start=2151
-  _SERVERDATA._serialized_end=2345
-  _SOCKET._serialized_start=2348
-  _SOCKET._serialized_end=2594
-  _SOCKETDATA._serialized_start=2597
-  _SOCKETDATA._serialized_end=3219
-  _ADDRESS._serialized_start=3222
-  _ADDRESS._serialized_end=3582
-  _ADDRESS_TCPIPADDRESS._serialized_start=3424
-  _ADDRESS_TCPIPADDRESS._serialized_end=3472
-  _ADDRESS_UDSADDRESS._serialized_start=3474
-  _ADDRESS_UDSADDRESS._serialized_end=3504
-  _ADDRESS_OTHERADDRESS._serialized_start=3506
-  _ADDRESS_OTHERADDRESS._serialized_end=3571
-  _SECURITY._serialized_start=3585
-  _SECURITY._serialized_end=3903
-  _SECURITY_TLS._serialized_start=3703
-  _SECURITY_TLS._serialized_end=3826
-  _SECURITY_OTHERSECURITY._serialized_start=3828
-  _SECURITY_OTHERSECURITY._serialized_end=3894
-  _SOCKETOPTION._serialized_start=3905
-  _SOCKETOPTION._serialized_end=3990
-  _SOCKETOPTIONTIMEOUT._serialized_start=3992
-  _SOCKETOPTIONTIMEOUT._serialized_end=4058
-  _SOCKETOPTIONLINGER._serialized_start=4060
-  _SOCKETOPTIONLINGER._serialized_end=4141
-  _SOCKETOPTIONTCPINFO._serialized_start=4144
-  _SOCKETOPTIONTCPINFO._serialized_end=4830
-  _GETTOPCHANNELSREQUEST._serialized_start=4832
-  _GETTOPCHANNELSREQUEST._serialized_end=4902
-  _GETTOPCHANNELSRESPONSE._serialized_start=4904
-  _GETTOPCHANNELSRESPONSE._serialized_end=4985
-  _GETSERVERSREQUEST._serialized_start=4987
-  _GETSERVERSREQUEST._serialized_end=5052
-  _GETSERVERSRESPONSE._serialized_start=5054
-  _GETSERVERSRESPONSE._serialized_end=5129
-  _GETSERVERREQUEST._serialized_start=5131
-  _GETSERVERREQUEST._serialized_end=5168
-  _GETSERVERRESPONSE._serialized_start=5170
-  _GETSERVERRESPONSE._serialized_end=5231
-  _GETSERVERSOCKETSREQUEST._serialized_start=5233
-  _GETSERVERSOCKETSREQUEST._serialized_end=5323
-  _GETSERVERSOCKETSRESPONSE._serialized_start=5325
-  _GETSERVERSOCKETSRESPONSE._serialized_end=5413
-  _GETCHANNELREQUEST._serialized_start=5415
-  _GETCHANNELREQUEST._serialized_end=5454
-  _GETCHANNELRESPONSE._serialized_start=5456
-  _GETCHANNELRESPONSE._serialized_end=5520
-  _GETSUBCHANNELREQUEST._serialized_start=5522
-  _GETSUBCHANNELREQUEST._serialized_end=5567
-  _GETSUBCHANNELRESPONSE._serialized_start=5569
-  _GETSUBCHANNELRESPONSE._serialized_end=5642
-  _GETSOCKETREQUEST._serialized_start=5644
-  _GETSOCKETREQUEST._serialized_end=5698
-  _GETSOCKETRESPONSE._serialized_start=5700
-  _GETSOCKETRESPONSE._serialized_end=5761
-  _CHANNELZ._serialized_start=5764
-  _CHANNELZ._serialized_end=6430
+  _globals['_CHANNEL']._serialized_start=178
+  _globals['_CHANNEL']._serialized_end=432
+  _globals['_SUBCHANNEL']._serialized_start=435
+  _globals['_SUBCHANNEL']._serialized_end=695
+  _globals['_CHANNELCONNECTIVITYSTATE']._serialized_start=698
+  _globals['_CHANNELCONNECTIVITYSTATE']._serialized_end=885
+  _globals['_CHANNELCONNECTIVITYSTATE_STATE']._serialized_start=791
+  _globals['_CHANNELCONNECTIVITYSTATE_STATE']._serialized_end=885
+  _globals['_CHANNELDATA']._serialized_start=888
+  _globals['_CHANNELDATA']._serialized_end=1158
+  _globals['_CHANNELTRACEEVENT']._serialized_start=1161
+  _globals['_CHANNELTRACEEVENT']._serialized_end=1508
+  _globals['_CHANNELTRACEEVENT_SEVERITY']._serialized_start=1426
+  _globals['_CHANNELTRACEEVENT_SEVERITY']._serialized_end=1495
+  _globals['_CHANNELTRACE']._serialized_start=1511
+  _globals['_CHANNELTRACE']._serialized_end=1661
+  _globals['_CHANNELREF']._serialized_start=1663
+  _globals['_CHANNELREF']._serialized_end=1745
+  _globals['_SUBCHANNELREF']._serialized_start=1747
+  _globals['_SUBCHANNELREF']._serialized_end=1835
+  _globals['_SOCKETREF']._serialized_start=1837
+  _globals['_SOCKETREF']._serialized_end=1917
+  _globals['_SERVERREF']._serialized_start=1919
+  _globals['_SERVERREF']._serialized_end=1999
+  _globals['_SERVER']._serialized_start=2002
+  _globals['_SERVER']._serialized_end=2148
+  _globals['_SERVERDATA']._serialized_start=2151
+  _globals['_SERVERDATA']._serialized_end=2345
+  _globals['_SOCKET']._serialized_start=2348
+  _globals['_SOCKET']._serialized_end=2594
+  _globals['_SOCKETDATA']._serialized_start=2597
+  _globals['_SOCKETDATA']._serialized_end=3219
+  _globals['_ADDRESS']._serialized_start=3222
+  _globals['_ADDRESS']._serialized_end=3582
+  _globals['_ADDRESS_TCPIPADDRESS']._serialized_start=3424
+  _globals['_ADDRESS_TCPIPADDRESS']._serialized_end=3472
+  _globals['_ADDRESS_UDSADDRESS']._serialized_start=3474
+  _globals['_ADDRESS_UDSADDRESS']._serialized_end=3504
+  _globals['_ADDRESS_OTHERADDRESS']._serialized_start=3506
+  _globals['_ADDRESS_OTHERADDRESS']._serialized_end=3571
+  _globals['_SECURITY']._serialized_start=3585
+  _globals['_SECURITY']._serialized_end=3903
+  _globals['_SECURITY_TLS']._serialized_start=3703
+  _globals['_SECURITY_TLS']._serialized_end=3826
+  _globals['_SECURITY_OTHERSECURITY']._serialized_start=3828
+  _globals['_SECURITY_OTHERSECURITY']._serialized_end=3894
+  _globals['_SOCKETOPTION']._serialized_start=3905
+  _globals['_SOCKETOPTION']._serialized_end=3990
+  _globals['_SOCKETOPTIONTIMEOUT']._serialized_start=3992
+  _globals['_SOCKETOPTIONTIMEOUT']._serialized_end=4058
+  _globals['_SOCKETOPTIONLINGER']._serialized_start=4060
+  _globals['_SOCKETOPTIONLINGER']._serialized_end=4141
+  _globals['_SOCKETOPTIONTCPINFO']._serialized_start=4144
+  _globals['_SOCKETOPTIONTCPINFO']._serialized_end=4830
+  _globals['_GETTOPCHANNELSREQUEST']._serialized_start=4832
+  _globals['_GETTOPCHANNELSREQUEST']._serialized_end=4902
+  _globals['_GETTOPCHANNELSRESPONSE']._serialized_start=4904
+  _globals['_GETTOPCHANNELSRESPONSE']._serialized_end=4985
+  _globals['_GETSERVERSREQUEST']._serialized_start=4987
+  _globals['_GETSERVERSREQUEST']._serialized_end=5052
+  _globals['_GETSERVERSRESPONSE']._serialized_start=5054
+  _globals['_GETSERVERSRESPONSE']._serialized_end=5129
+  _globals['_GETSERVERREQUEST']._serialized_start=5131
+  _globals['_GETSERVERREQUEST']._serialized_end=5168
+  _globals['_GETSERVERRESPONSE']._serialized_start=5170
+  _globals['_GETSERVERRESPONSE']._serialized_end=5231
+  _globals['_GETSERVERSOCKETSREQUEST']._serialized_start=5233
+  _globals['_GETSERVERSOCKETSREQUEST']._serialized_end=5323
+  _globals['_GETSERVERSOCKETSRESPONSE']._serialized_start=5325
+  _globals['_GETSERVERSOCKETSRESPONSE']._serialized_end=5413
+  _globals['_GETCHANNELREQUEST']._serialized_start=5415
+  _globals['_GETCHANNELREQUEST']._serialized_end=5454
+  _globals['_GETCHANNELRESPONSE']._serialized_start=5456
+  _globals['_GETCHANNELRESPONSE']._serialized_end=5520
+  _globals['_GETSUBCHANNELREQUEST']._serialized_start=5522
+  _globals['_GETSUBCHANNELREQUEST']._serialized_end=5567
+  _globals['_GETSUBCHANNELRESPONSE']._serialized_start=5569
+  _globals['_GETSUBCHANNELRESPONSE']._serialized_end=5642
+  _globals['_GETSOCKETREQUEST']._serialized_start=5644
+  _globals['_GETSOCKETREQUEST']._serialized_end=5698
+  _globals['_GETSOCKETRESPONSE']._serialized_start=5700
+  _globals['_GETSOCKETRESPONSE']._serialized_end=5761
+  _globals['_CHANNELZ']._serialized_start=5764
+  _globals['_CHANNELZ']._serialized_end=6430
 # @@protoc_insertion_point(module_scope)
```

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz_pb2.pyi` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -6,439 +6,449 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Address(_message.Message):
-    __slots__ = ["other_address", "tcpip_address", "uds_address"]
-    class OtherAddress(_message.Message):
-        __slots__ = ["name", "value"]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        name: str
-        value: _any_pb2.Any
-        def __init__(self, name: _Optional[str] = ..., value: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
-    class TcpIpAddress(_message.Message):
-        __slots__ = ["ip_address", "port"]
-        IP_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-        PORT_FIELD_NUMBER: _ClassVar[int]
-        ip_address: bytes
-        port: int
-        def __init__(self, ip_address: _Optional[bytes] = ..., port: _Optional[int] = ...) -> None: ...
-    class UdsAddress(_message.Message):
-        __slots__ = ["filename"]
-        FILENAME_FIELD_NUMBER: _ClassVar[int]
-        filename: str
-        def __init__(self, filename: _Optional[str] = ...) -> None: ...
-    OTHER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    TCPIP_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    UDS_ADDRESS_FIELD_NUMBER: _ClassVar[int]
-    other_address: Address.OtherAddress
-    tcpip_address: Address.TcpIpAddress
-    uds_address: Address.UdsAddress
-    def __init__(self, tcpip_address: _Optional[_Union[Address.TcpIpAddress, _Mapping]] = ..., uds_address: _Optional[_Union[Address.UdsAddress, _Mapping]] = ..., other_address: _Optional[_Union[Address.OtherAddress, _Mapping]] = ...) -> None: ...
-
 class Channel(_message.Message):
-    __slots__ = ["channel_ref", "data", "ref", "socket_ref", "subchannel_ref"]
-    CHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["ref", "data", "channel_ref", "subchannel_ref", "socket_ref"]
     REF_FIELD_NUMBER: _ClassVar[int]
-    SOCKET_REF_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    CHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
     SUBCHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
-    channel_ref: _containers.RepeatedCompositeFieldContainer[ChannelRef]
-    data: ChannelData
+    SOCKET_REF_FIELD_NUMBER: _ClassVar[int]
     ref: ChannelRef
-    socket_ref: _containers.RepeatedCompositeFieldContainer[SocketRef]
+    data: ChannelData
+    channel_ref: _containers.RepeatedCompositeFieldContainer[ChannelRef]
     subchannel_ref: _containers.RepeatedCompositeFieldContainer[SubchannelRef]
+    socket_ref: _containers.RepeatedCompositeFieldContainer[SocketRef]
     def __init__(self, ref: _Optional[_Union[ChannelRef, _Mapping]] = ..., data: _Optional[_Union[ChannelData, _Mapping]] = ..., channel_ref: _Optional[_Iterable[_Union[ChannelRef, _Mapping]]] = ..., subchannel_ref: _Optional[_Iterable[_Union[SubchannelRef, _Mapping]]] = ..., socket_ref: _Optional[_Iterable[_Union[SocketRef, _Mapping]]] = ...) -> None: ...
 
+class Subchannel(_message.Message):
+    __slots__ = ["ref", "data", "channel_ref", "subchannel_ref", "socket_ref"]
+    REF_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    CHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
+    SUBCHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
+    SOCKET_REF_FIELD_NUMBER: _ClassVar[int]
+    ref: SubchannelRef
+    data: ChannelData
+    channel_ref: _containers.RepeatedCompositeFieldContainer[ChannelRef]
+    subchannel_ref: _containers.RepeatedCompositeFieldContainer[SubchannelRef]
+    socket_ref: _containers.RepeatedCompositeFieldContainer[SocketRef]
+    def __init__(self, ref: _Optional[_Union[SubchannelRef, _Mapping]] = ..., data: _Optional[_Union[ChannelData, _Mapping]] = ..., channel_ref: _Optional[_Iterable[_Union[ChannelRef, _Mapping]]] = ..., subchannel_ref: _Optional[_Iterable[_Union[SubchannelRef, _Mapping]]] = ..., socket_ref: _Optional[_Iterable[_Union[SocketRef, _Mapping]]] = ...) -> None: ...
+
 class ChannelConnectivityState(_message.Message):
     __slots__ = ["state"]
     class State(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    CONNECTING: ChannelConnectivityState.State
+        UNKNOWN: _ClassVar[ChannelConnectivityState.State]
+        IDLE: _ClassVar[ChannelConnectivityState.State]
+        CONNECTING: _ClassVar[ChannelConnectivityState.State]
+        READY: _ClassVar[ChannelConnectivityState.State]
+        TRANSIENT_FAILURE: _ClassVar[ChannelConnectivityState.State]
+        SHUTDOWN: _ClassVar[ChannelConnectivityState.State]
+    UNKNOWN: ChannelConnectivityState.State
     IDLE: ChannelConnectivityState.State
+    CONNECTING: ChannelConnectivityState.State
     READY: ChannelConnectivityState.State
+    TRANSIENT_FAILURE: ChannelConnectivityState.State
     SHUTDOWN: ChannelConnectivityState.State
     STATE_FIELD_NUMBER: _ClassVar[int]
-    TRANSIENT_FAILURE: ChannelConnectivityState.State
-    UNKNOWN: ChannelConnectivityState.State
     state: ChannelConnectivityState.State
     def __init__(self, state: _Optional[_Union[ChannelConnectivityState.State, str]] = ...) -> None: ...
 
 class ChannelData(_message.Message):
-    __slots__ = ["calls_failed", "calls_started", "calls_succeeded", "last_call_started_timestamp", "state", "target", "trace"]
-    CALLS_FAILED_FIELD_NUMBER: _ClassVar[int]
-    CALLS_STARTED_FIELD_NUMBER: _ClassVar[int]
-    CALLS_SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
-    LAST_CALL_STARTED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["state", "target", "trace", "calls_started", "calls_succeeded", "calls_failed", "last_call_started_timestamp"]
     STATE_FIELD_NUMBER: _ClassVar[int]
     TARGET_FIELD_NUMBER: _ClassVar[int]
     TRACE_FIELD_NUMBER: _ClassVar[int]
-    calls_failed: int
-    calls_started: int
-    calls_succeeded: int
-    last_call_started_timestamp: _timestamp_pb2.Timestamp
+    CALLS_STARTED_FIELD_NUMBER: _ClassVar[int]
+    CALLS_SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
+    CALLS_FAILED_FIELD_NUMBER: _ClassVar[int]
+    LAST_CALL_STARTED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     state: ChannelConnectivityState
     target: str
     trace: ChannelTrace
+    calls_started: int
+    calls_succeeded: int
+    calls_failed: int
+    last_call_started_timestamp: _timestamp_pb2.Timestamp
     def __init__(self, state: _Optional[_Union[ChannelConnectivityState, _Mapping]] = ..., target: _Optional[str] = ..., trace: _Optional[_Union[ChannelTrace, _Mapping]] = ..., calls_started: _Optional[int] = ..., calls_succeeded: _Optional[int] = ..., calls_failed: _Optional[int] = ..., last_call_started_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ChannelRef(_message.Message):
-    __slots__ = ["channel_id", "name"]
-    CHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    channel_id: int
-    name: str
-    def __init__(self, channel_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
-
-class ChannelTrace(_message.Message):
-    __slots__ = ["creation_timestamp", "events", "num_events_logged"]
-    CREATION_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-    EVENTS_FIELD_NUMBER: _ClassVar[int]
-    NUM_EVENTS_LOGGED_FIELD_NUMBER: _ClassVar[int]
-    creation_timestamp: _timestamp_pb2.Timestamp
-    events: _containers.RepeatedCompositeFieldContainer[ChannelTraceEvent]
-    num_events_logged: int
-    def __init__(self, num_events_logged: _Optional[int] = ..., creation_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., events: _Optional[_Iterable[_Union[ChannelTraceEvent, _Mapping]]] = ...) -> None: ...
-
 class ChannelTraceEvent(_message.Message):
-    __slots__ = ["channel_ref", "description", "severity", "subchannel_ref", "timestamp"]
+    __slots__ = ["description", "severity", "timestamp", "channel_ref", "subchannel_ref"]
     class Severity(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    CHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
-    CT_ERROR: ChannelTraceEvent.Severity
-    CT_INFO: ChannelTraceEvent.Severity
+        CT_UNKNOWN: _ClassVar[ChannelTraceEvent.Severity]
+        CT_INFO: _ClassVar[ChannelTraceEvent.Severity]
+        CT_WARNING: _ClassVar[ChannelTraceEvent.Severity]
+        CT_ERROR: _ClassVar[ChannelTraceEvent.Severity]
     CT_UNKNOWN: ChannelTraceEvent.Severity
+    CT_INFO: ChannelTraceEvent.Severity
     CT_WARNING: ChannelTraceEvent.Severity
+    CT_ERROR: ChannelTraceEvent.Severity
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     SEVERITY_FIELD_NUMBER: _ClassVar[int]
-    SUBCHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-    channel_ref: ChannelRef
+    CHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
+    SUBCHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
     description: str
     severity: ChannelTraceEvent.Severity
-    subchannel_ref: SubchannelRef
     timestamp: _timestamp_pb2.Timestamp
+    channel_ref: ChannelRef
+    subchannel_ref: SubchannelRef
     def __init__(self, description: _Optional[str] = ..., severity: _Optional[_Union[ChannelTraceEvent.Severity, str]] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., channel_ref: _Optional[_Union[ChannelRef, _Mapping]] = ..., subchannel_ref: _Optional[_Union[SubchannelRef, _Mapping]] = ...) -> None: ...
 
-class GetChannelRequest(_message.Message):
-    __slots__ = ["channel_id"]
+class ChannelTrace(_message.Message):
+    __slots__ = ["num_events_logged", "creation_timestamp", "events"]
+    NUM_EVENTS_LOGGED_FIELD_NUMBER: _ClassVar[int]
+    CREATION_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    EVENTS_FIELD_NUMBER: _ClassVar[int]
+    num_events_logged: int
+    creation_timestamp: _timestamp_pb2.Timestamp
+    events: _containers.RepeatedCompositeFieldContainer[ChannelTraceEvent]
+    def __init__(self, num_events_logged: _Optional[int] = ..., creation_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., events: _Optional[_Iterable[_Union[ChannelTraceEvent, _Mapping]]] = ...) -> None: ...
+
+class ChannelRef(_message.Message):
+    __slots__ = ["channel_id", "name"]
     CHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     channel_id: int
-    def __init__(self, channel_id: _Optional[int] = ...) -> None: ...
-
-class GetChannelResponse(_message.Message):
-    __slots__ = ["channel"]
-    CHANNEL_FIELD_NUMBER: _ClassVar[int]
-    channel: Channel
-    def __init__(self, channel: _Optional[_Union[Channel, _Mapping]] = ...) -> None: ...
-
-class GetServerRequest(_message.Message):
-    __slots__ = ["server_id"]
-    SERVER_ID_FIELD_NUMBER: _ClassVar[int]
-    server_id: int
-    def __init__(self, server_id: _Optional[int] = ...) -> None: ...
-
-class GetServerResponse(_message.Message):
-    __slots__ = ["server"]
-    SERVER_FIELD_NUMBER: _ClassVar[int]
-    server: Server
-    def __init__(self, server: _Optional[_Union[Server, _Mapping]] = ...) -> None: ...
-
-class GetServerSocketsRequest(_message.Message):
-    __slots__ = ["max_results", "server_id", "start_socket_id"]
-    MAX_RESULTS_FIELD_NUMBER: _ClassVar[int]
-    SERVER_ID_FIELD_NUMBER: _ClassVar[int]
-    START_SOCKET_ID_FIELD_NUMBER: _ClassVar[int]
-    max_results: int
-    server_id: int
-    start_socket_id: int
-    def __init__(self, server_id: _Optional[int] = ..., start_socket_id: _Optional[int] = ..., max_results: _Optional[int] = ...) -> None: ...
-
-class GetServerSocketsResponse(_message.Message):
-    __slots__ = ["end", "socket_ref"]
-    END_FIELD_NUMBER: _ClassVar[int]
-    SOCKET_REF_FIELD_NUMBER: _ClassVar[int]
-    end: bool
-    socket_ref: _containers.RepeatedCompositeFieldContainer[SocketRef]
-    def __init__(self, socket_ref: _Optional[_Iterable[_Union[SocketRef, _Mapping]]] = ..., end: bool = ...) -> None: ...
-
-class GetServersRequest(_message.Message):
-    __slots__ = ["max_results", "start_server_id"]
-    MAX_RESULTS_FIELD_NUMBER: _ClassVar[int]
-    START_SERVER_ID_FIELD_NUMBER: _ClassVar[int]
-    max_results: int
-    start_server_id: int
-    def __init__(self, start_server_id: _Optional[int] = ..., max_results: _Optional[int] = ...) -> None: ...
-
-class GetServersResponse(_message.Message):
-    __slots__ = ["end", "server"]
-    END_FIELD_NUMBER: _ClassVar[int]
-    SERVER_FIELD_NUMBER: _ClassVar[int]
-    end: bool
-    server: _containers.RepeatedCompositeFieldContainer[Server]
-    def __init__(self, server: _Optional[_Iterable[_Union[Server, _Mapping]]] = ..., end: bool = ...) -> None: ...
-
-class GetSocketRequest(_message.Message):
-    __slots__ = ["socket_id", "summary"]
-    SOCKET_ID_FIELD_NUMBER: _ClassVar[int]
-    SUMMARY_FIELD_NUMBER: _ClassVar[int]
-    socket_id: int
-    summary: bool
-    def __init__(self, socket_id: _Optional[int] = ..., summary: bool = ...) -> None: ...
-
-class GetSocketResponse(_message.Message):
-    __slots__ = ["socket"]
-    SOCKET_FIELD_NUMBER: _ClassVar[int]
-    socket: Socket
-    def __init__(self, socket: _Optional[_Union[Socket, _Mapping]] = ...) -> None: ...
+    name: str
+    def __init__(self, channel_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
 
-class GetSubchannelRequest(_message.Message):
-    __slots__ = ["subchannel_id"]
+class SubchannelRef(_message.Message):
+    __slots__ = ["subchannel_id", "name"]
     SUBCHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     subchannel_id: int
-    def __init__(self, subchannel_id: _Optional[int] = ...) -> None: ...
-
-class GetSubchannelResponse(_message.Message):
-    __slots__ = ["subchannel"]
-    SUBCHANNEL_FIELD_NUMBER: _ClassVar[int]
-    subchannel: Subchannel
-    def __init__(self, subchannel: _Optional[_Union[Subchannel, _Mapping]] = ...) -> None: ...
-
-class GetTopChannelsRequest(_message.Message):
-    __slots__ = ["max_results", "start_channel_id"]
-    MAX_RESULTS_FIELD_NUMBER: _ClassVar[int]
-    START_CHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
-    max_results: int
-    start_channel_id: int
-    def __init__(self, start_channel_id: _Optional[int] = ..., max_results: _Optional[int] = ...) -> None: ...
+    name: str
+    def __init__(self, subchannel_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
 
-class GetTopChannelsResponse(_message.Message):
-    __slots__ = ["channel", "end"]
-    CHANNEL_FIELD_NUMBER: _ClassVar[int]
-    END_FIELD_NUMBER: _ClassVar[int]
-    channel: _containers.RepeatedCompositeFieldContainer[Channel]
-    end: bool
-    def __init__(self, channel: _Optional[_Iterable[_Union[Channel, _Mapping]]] = ..., end: bool = ...) -> None: ...
+class SocketRef(_message.Message):
+    __slots__ = ["socket_id", "name"]
+    SOCKET_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    socket_id: int
+    name: str
+    def __init__(self, socket_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
 
-class Security(_message.Message):
-    __slots__ = ["other", "tls"]
-    class OtherSecurity(_message.Message):
-        __slots__ = ["name", "value"]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        name: str
-        value: _any_pb2.Any
-        def __init__(self, name: _Optional[str] = ..., value: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
-    class Tls(_message.Message):
-        __slots__ = ["local_certificate", "other_name", "remote_certificate", "standard_name"]
-        LOCAL_CERTIFICATE_FIELD_NUMBER: _ClassVar[int]
-        OTHER_NAME_FIELD_NUMBER: _ClassVar[int]
-        REMOTE_CERTIFICATE_FIELD_NUMBER: _ClassVar[int]
-        STANDARD_NAME_FIELD_NUMBER: _ClassVar[int]
-        local_certificate: bytes
-        other_name: str
-        remote_certificate: bytes
-        standard_name: str
-        def __init__(self, standard_name: _Optional[str] = ..., other_name: _Optional[str] = ..., local_certificate: _Optional[bytes] = ..., remote_certificate: _Optional[bytes] = ...) -> None: ...
-    OTHER_FIELD_NUMBER: _ClassVar[int]
-    TLS_FIELD_NUMBER: _ClassVar[int]
-    other: Security.OtherSecurity
-    tls: Security.Tls
-    def __init__(self, tls: _Optional[_Union[Security.Tls, _Mapping]] = ..., other: _Optional[_Union[Security.OtherSecurity, _Mapping]] = ...) -> None: ...
+class ServerRef(_message.Message):
+    __slots__ = ["server_id", "name"]
+    SERVER_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    server_id: int
+    name: str
+    def __init__(self, server_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
 
 class Server(_message.Message):
-    __slots__ = ["data", "listen_socket", "ref"]
+    __slots__ = ["ref", "data", "listen_socket"]
+    REF_FIELD_NUMBER: _ClassVar[int]
     DATA_FIELD_NUMBER: _ClassVar[int]
     LISTEN_SOCKET_FIELD_NUMBER: _ClassVar[int]
-    REF_FIELD_NUMBER: _ClassVar[int]
+    ref: ServerRef
     data: ServerData
     listen_socket: _containers.RepeatedCompositeFieldContainer[SocketRef]
-    ref: ServerRef
     def __init__(self, ref: _Optional[_Union[ServerRef, _Mapping]] = ..., data: _Optional[_Union[ServerData, _Mapping]] = ..., listen_socket: _Optional[_Iterable[_Union[SocketRef, _Mapping]]] = ...) -> None: ...
 
 class ServerData(_message.Message):
-    __slots__ = ["calls_failed", "calls_started", "calls_succeeded", "last_call_started_timestamp", "trace"]
-    CALLS_FAILED_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["trace", "calls_started", "calls_succeeded", "calls_failed", "last_call_started_timestamp"]
+    TRACE_FIELD_NUMBER: _ClassVar[int]
     CALLS_STARTED_FIELD_NUMBER: _ClassVar[int]
     CALLS_SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
+    CALLS_FAILED_FIELD_NUMBER: _ClassVar[int]
     LAST_CALL_STARTED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-    TRACE_FIELD_NUMBER: _ClassVar[int]
-    calls_failed: int
+    trace: ChannelTrace
     calls_started: int
     calls_succeeded: int
+    calls_failed: int
     last_call_started_timestamp: _timestamp_pb2.Timestamp
-    trace: ChannelTrace
     def __init__(self, trace: _Optional[_Union[ChannelTrace, _Mapping]] = ..., calls_started: _Optional[int] = ..., calls_succeeded: _Optional[int] = ..., calls_failed: _Optional[int] = ..., last_call_started_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ServerRef(_message.Message):
-    __slots__ = ["name", "server_id"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    SERVER_ID_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    server_id: int
-    def __init__(self, server_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
-
 class Socket(_message.Message):
-    __slots__ = ["data", "local", "ref", "remote", "remote_name", "security"]
+    __slots__ = ["ref", "data", "local", "remote", "security", "remote_name"]
+    REF_FIELD_NUMBER: _ClassVar[int]
     DATA_FIELD_NUMBER: _ClassVar[int]
     LOCAL_FIELD_NUMBER: _ClassVar[int]
-    REF_FIELD_NUMBER: _ClassVar[int]
     REMOTE_FIELD_NUMBER: _ClassVar[int]
-    REMOTE_NAME_FIELD_NUMBER: _ClassVar[int]
     SECURITY_FIELD_NUMBER: _ClassVar[int]
+    REMOTE_NAME_FIELD_NUMBER: _ClassVar[int]
+    ref: SocketRef
     data: SocketData
     local: Address
-    ref: SocketRef
     remote: Address
-    remote_name: str
     security: Security
+    remote_name: str
     def __init__(self, ref: _Optional[_Union[SocketRef, _Mapping]] = ..., data: _Optional[_Union[SocketData, _Mapping]] = ..., local: _Optional[_Union[Address, _Mapping]] = ..., remote: _Optional[_Union[Address, _Mapping]] = ..., security: _Optional[_Union[Security, _Mapping]] = ..., remote_name: _Optional[str] = ...) -> None: ...
 
 class SocketData(_message.Message):
-    __slots__ = ["keep_alives_sent", "last_local_stream_created_timestamp", "last_message_received_timestamp", "last_message_sent_timestamp", "last_remote_stream_created_timestamp", "local_flow_control_window", "messages_received", "messages_sent", "option", "remote_flow_control_window", "streams_failed", "streams_started", "streams_succeeded"]
+    __slots__ = ["streams_started", "streams_succeeded", "streams_failed", "messages_sent", "messages_received", "keep_alives_sent", "last_local_stream_created_timestamp", "last_remote_stream_created_timestamp", "last_message_sent_timestamp", "last_message_received_timestamp", "local_flow_control_window", "remote_flow_control_window", "option"]
+    STREAMS_STARTED_FIELD_NUMBER: _ClassVar[int]
+    STREAMS_SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
+    STREAMS_FAILED_FIELD_NUMBER: _ClassVar[int]
+    MESSAGES_SENT_FIELD_NUMBER: _ClassVar[int]
+    MESSAGES_RECEIVED_FIELD_NUMBER: _ClassVar[int]
     KEEP_ALIVES_SENT_FIELD_NUMBER: _ClassVar[int]
     LAST_LOCAL_STREAM_CREATED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-    LAST_MESSAGE_RECEIVED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-    LAST_MESSAGE_SENT_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     LAST_REMOTE_STREAM_CREATED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    LAST_MESSAGE_SENT_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    LAST_MESSAGE_RECEIVED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     LOCAL_FLOW_CONTROL_WINDOW_FIELD_NUMBER: _ClassVar[int]
-    MESSAGES_RECEIVED_FIELD_NUMBER: _ClassVar[int]
-    MESSAGES_SENT_FIELD_NUMBER: _ClassVar[int]
-    OPTION_FIELD_NUMBER: _ClassVar[int]
     REMOTE_FLOW_CONTROL_WINDOW_FIELD_NUMBER: _ClassVar[int]
-    STREAMS_FAILED_FIELD_NUMBER: _ClassVar[int]
-    STREAMS_STARTED_FIELD_NUMBER: _ClassVar[int]
-    STREAMS_SUCCEEDED_FIELD_NUMBER: _ClassVar[int]
+    OPTION_FIELD_NUMBER: _ClassVar[int]
+    streams_started: int
+    streams_succeeded: int
+    streams_failed: int
+    messages_sent: int
+    messages_received: int
     keep_alives_sent: int
     last_local_stream_created_timestamp: _timestamp_pb2.Timestamp
-    last_message_received_timestamp: _timestamp_pb2.Timestamp
-    last_message_sent_timestamp: _timestamp_pb2.Timestamp
     last_remote_stream_created_timestamp: _timestamp_pb2.Timestamp
+    last_message_sent_timestamp: _timestamp_pb2.Timestamp
+    last_message_received_timestamp: _timestamp_pb2.Timestamp
     local_flow_control_window: _wrappers_pb2.Int64Value
-    messages_received: int
-    messages_sent: int
-    option: _containers.RepeatedCompositeFieldContainer[SocketOption]
     remote_flow_control_window: _wrappers_pb2.Int64Value
-    streams_failed: int
-    streams_started: int
-    streams_succeeded: int
+    option: _containers.RepeatedCompositeFieldContainer[SocketOption]
     def __init__(self, streams_started: _Optional[int] = ..., streams_succeeded: _Optional[int] = ..., streams_failed: _Optional[int] = ..., messages_sent: _Optional[int] = ..., messages_received: _Optional[int] = ..., keep_alives_sent: _Optional[int] = ..., last_local_stream_created_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., last_remote_stream_created_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., last_message_sent_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., last_message_received_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., local_flow_control_window: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., remote_flow_control_window: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., option: _Optional[_Iterable[_Union[SocketOption, _Mapping]]] = ...) -> None: ...
 
+class Address(_message.Message):
+    __slots__ = ["tcpip_address", "uds_address", "other_address"]
+    class TcpIpAddress(_message.Message):
+        __slots__ = ["ip_address", "port"]
+        IP_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+        PORT_FIELD_NUMBER: _ClassVar[int]
+        ip_address: bytes
+        port: int
+        def __init__(self, ip_address: _Optional[bytes] = ..., port: _Optional[int] = ...) -> None: ...
+    class UdsAddress(_message.Message):
+        __slots__ = ["filename"]
+        FILENAME_FIELD_NUMBER: _ClassVar[int]
+        filename: str
+        def __init__(self, filename: _Optional[str] = ...) -> None: ...
+    class OtherAddress(_message.Message):
+        __slots__ = ["name", "value"]
+        NAME_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        name: str
+        value: _any_pb2.Any
+        def __init__(self, name: _Optional[str] = ..., value: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
+    TCPIP_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    UDS_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    OTHER_ADDRESS_FIELD_NUMBER: _ClassVar[int]
+    tcpip_address: Address.TcpIpAddress
+    uds_address: Address.UdsAddress
+    other_address: Address.OtherAddress
+    def __init__(self, tcpip_address: _Optional[_Union[Address.TcpIpAddress, _Mapping]] = ..., uds_address: _Optional[_Union[Address.UdsAddress, _Mapping]] = ..., other_address: _Optional[_Union[Address.OtherAddress, _Mapping]] = ...) -> None: ...
+
+class Security(_message.Message):
+    __slots__ = ["tls", "other"]
+    class Tls(_message.Message):
+        __slots__ = ["standard_name", "other_name", "local_certificate", "remote_certificate"]
+        STANDARD_NAME_FIELD_NUMBER: _ClassVar[int]
+        OTHER_NAME_FIELD_NUMBER: _ClassVar[int]
+        LOCAL_CERTIFICATE_FIELD_NUMBER: _ClassVar[int]
+        REMOTE_CERTIFICATE_FIELD_NUMBER: _ClassVar[int]
+        standard_name: str
+        other_name: str
+        local_certificate: bytes
+        remote_certificate: bytes
+        def __init__(self, standard_name: _Optional[str] = ..., other_name: _Optional[str] = ..., local_certificate: _Optional[bytes] = ..., remote_certificate: _Optional[bytes] = ...) -> None: ...
+    class OtherSecurity(_message.Message):
+        __slots__ = ["name", "value"]
+        NAME_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        name: str
+        value: _any_pb2.Any
+        def __init__(self, name: _Optional[str] = ..., value: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
+    TLS_FIELD_NUMBER: _ClassVar[int]
+    OTHER_FIELD_NUMBER: _ClassVar[int]
+    tls: Security.Tls
+    other: Security.OtherSecurity
+    def __init__(self, tls: _Optional[_Union[Security.Tls, _Mapping]] = ..., other: _Optional[_Union[Security.OtherSecurity, _Mapping]] = ...) -> None: ...
+
 class SocketOption(_message.Message):
-    __slots__ = ["additional", "name", "value"]
-    ADDITIONAL_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["name", "value", "additional"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
-    additional: _any_pb2.Any
+    ADDITIONAL_FIELD_NUMBER: _ClassVar[int]
     name: str
     value: str
+    additional: _any_pb2.Any
     def __init__(self, name: _Optional[str] = ..., value: _Optional[str] = ..., additional: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
 
+class SocketOptionTimeout(_message.Message):
+    __slots__ = ["duration"]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
+    duration: _duration_pb2.Duration
+    def __init__(self, duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
+
 class SocketOptionLinger(_message.Message):
     __slots__ = ["active", "duration"]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     DURATION_FIELD_NUMBER: _ClassVar[int]
     active: bool
     duration: _duration_pb2.Duration
     def __init__(self, active: bool = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
 
 class SocketOptionTcpInfo(_message.Message):
-    __slots__ = ["tcpi_advmss", "tcpi_ato", "tcpi_backoff", "tcpi_ca_state", "tcpi_fackets", "tcpi_last_ack_recv", "tcpi_last_ack_sent", "tcpi_last_data_recv", "tcpi_last_data_sent", "tcpi_lost", "tcpi_options", "tcpi_pmtu", "tcpi_probes", "tcpi_rcv_mss", "tcpi_rcv_ssthresh", "tcpi_rcv_wscale", "tcpi_reordering", "tcpi_retrans", "tcpi_retransmits", "tcpi_rto", "tcpi_rtt", "tcpi_rttvar", "tcpi_sacked", "tcpi_snd_cwnd", "tcpi_snd_mss", "tcpi_snd_ssthresh", "tcpi_snd_wscale", "tcpi_state", "tcpi_unacked"]
-    TCPI_ADVMSS_FIELD_NUMBER: _ClassVar[int]
-    TCPI_ATO_FIELD_NUMBER: _ClassVar[int]
-    TCPI_BACKOFF_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["tcpi_state", "tcpi_ca_state", "tcpi_retransmits", "tcpi_probes", "tcpi_backoff", "tcpi_options", "tcpi_snd_wscale", "tcpi_rcv_wscale", "tcpi_rto", "tcpi_ato", "tcpi_snd_mss", "tcpi_rcv_mss", "tcpi_unacked", "tcpi_sacked", "tcpi_lost", "tcpi_retrans", "tcpi_fackets", "tcpi_last_data_sent", "tcpi_last_ack_sent", "tcpi_last_data_recv", "tcpi_last_ack_recv", "tcpi_pmtu", "tcpi_rcv_ssthresh", "tcpi_rtt", "tcpi_rttvar", "tcpi_snd_ssthresh", "tcpi_snd_cwnd", "tcpi_advmss", "tcpi_reordering"]
+    TCPI_STATE_FIELD_NUMBER: _ClassVar[int]
     TCPI_CA_STATE_FIELD_NUMBER: _ClassVar[int]
+    TCPI_RETRANSMITS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_PROBES_FIELD_NUMBER: _ClassVar[int]
+    TCPI_BACKOFF_FIELD_NUMBER: _ClassVar[int]
+    TCPI_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_SND_WSCALE_FIELD_NUMBER: _ClassVar[int]
+    TCPI_RCV_WSCALE_FIELD_NUMBER: _ClassVar[int]
+    TCPI_RTO_FIELD_NUMBER: _ClassVar[int]
+    TCPI_ATO_FIELD_NUMBER: _ClassVar[int]
+    TCPI_SND_MSS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_RCV_MSS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_UNACKED_FIELD_NUMBER: _ClassVar[int]
+    TCPI_SACKED_FIELD_NUMBER: _ClassVar[int]
+    TCPI_LOST_FIELD_NUMBER: _ClassVar[int]
+    TCPI_RETRANS_FIELD_NUMBER: _ClassVar[int]
     TCPI_FACKETS_FIELD_NUMBER: _ClassVar[int]
-    TCPI_LAST_ACK_RECV_FIELD_NUMBER: _ClassVar[int]
+    TCPI_LAST_DATA_SENT_FIELD_NUMBER: _ClassVar[int]
     TCPI_LAST_ACK_SENT_FIELD_NUMBER: _ClassVar[int]
     TCPI_LAST_DATA_RECV_FIELD_NUMBER: _ClassVar[int]
-    TCPI_LAST_DATA_SENT_FIELD_NUMBER: _ClassVar[int]
-    TCPI_LOST_FIELD_NUMBER: _ClassVar[int]
-    TCPI_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_LAST_ACK_RECV_FIELD_NUMBER: _ClassVar[int]
     TCPI_PMTU_FIELD_NUMBER: _ClassVar[int]
-    TCPI_PROBES_FIELD_NUMBER: _ClassVar[int]
-    TCPI_RCV_MSS_FIELD_NUMBER: _ClassVar[int]
     TCPI_RCV_SSTHRESH_FIELD_NUMBER: _ClassVar[int]
-    TCPI_RCV_WSCALE_FIELD_NUMBER: _ClassVar[int]
-    TCPI_REORDERING_FIELD_NUMBER: _ClassVar[int]
-    TCPI_RETRANSMITS_FIELD_NUMBER: _ClassVar[int]
-    TCPI_RETRANS_FIELD_NUMBER: _ClassVar[int]
-    TCPI_RTO_FIELD_NUMBER: _ClassVar[int]
-    TCPI_RTTVAR_FIELD_NUMBER: _ClassVar[int]
     TCPI_RTT_FIELD_NUMBER: _ClassVar[int]
-    TCPI_SACKED_FIELD_NUMBER: _ClassVar[int]
-    TCPI_SND_CWND_FIELD_NUMBER: _ClassVar[int]
-    TCPI_SND_MSS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_RTTVAR_FIELD_NUMBER: _ClassVar[int]
     TCPI_SND_SSTHRESH_FIELD_NUMBER: _ClassVar[int]
-    TCPI_SND_WSCALE_FIELD_NUMBER: _ClassVar[int]
-    TCPI_STATE_FIELD_NUMBER: _ClassVar[int]
-    TCPI_UNACKED_FIELD_NUMBER: _ClassVar[int]
-    tcpi_advmss: int
-    tcpi_ato: int
-    tcpi_backoff: int
+    TCPI_SND_CWND_FIELD_NUMBER: _ClassVar[int]
+    TCPI_ADVMSS_FIELD_NUMBER: _ClassVar[int]
+    TCPI_REORDERING_FIELD_NUMBER: _ClassVar[int]
+    tcpi_state: int
     tcpi_ca_state: int
+    tcpi_retransmits: int
+    tcpi_probes: int
+    tcpi_backoff: int
+    tcpi_options: int
+    tcpi_snd_wscale: int
+    tcpi_rcv_wscale: int
+    tcpi_rto: int
+    tcpi_ato: int
+    tcpi_snd_mss: int
+    tcpi_rcv_mss: int
+    tcpi_unacked: int
+    tcpi_sacked: int
+    tcpi_lost: int
+    tcpi_retrans: int
     tcpi_fackets: int
-    tcpi_last_ack_recv: int
+    tcpi_last_data_sent: int
     tcpi_last_ack_sent: int
     tcpi_last_data_recv: int
-    tcpi_last_data_sent: int
-    tcpi_lost: int
-    tcpi_options: int
+    tcpi_last_ack_recv: int
     tcpi_pmtu: int
-    tcpi_probes: int
-    tcpi_rcv_mss: int
     tcpi_rcv_ssthresh: int
-    tcpi_rcv_wscale: int
-    tcpi_reordering: int
-    tcpi_retrans: int
-    tcpi_retransmits: int
-    tcpi_rto: int
     tcpi_rtt: int
     tcpi_rttvar: int
-    tcpi_sacked: int
-    tcpi_snd_cwnd: int
-    tcpi_snd_mss: int
     tcpi_snd_ssthresh: int
-    tcpi_snd_wscale: int
-    tcpi_state: int
-    tcpi_unacked: int
+    tcpi_snd_cwnd: int
+    tcpi_advmss: int
+    tcpi_reordering: int
     def __init__(self, tcpi_state: _Optional[int] = ..., tcpi_ca_state: _Optional[int] = ..., tcpi_retransmits: _Optional[int] = ..., tcpi_probes: _Optional[int] = ..., tcpi_backoff: _Optional[int] = ..., tcpi_options: _Optional[int] = ..., tcpi_snd_wscale: _Optional[int] = ..., tcpi_rcv_wscale: _Optional[int] = ..., tcpi_rto: _Optional[int] = ..., tcpi_ato: _Optional[int] = ..., tcpi_snd_mss: _Optional[int] = ..., tcpi_rcv_mss: _Optional[int] = ..., tcpi_unacked: _Optional[int] = ..., tcpi_sacked: _Optional[int] = ..., tcpi_lost: _Optional[int] = ..., tcpi_retrans: _Optional[int] = ..., tcpi_fackets: _Optional[int] = ..., tcpi_last_data_sent: _Optional[int] = ..., tcpi_last_ack_sent: _Optional[int] = ..., tcpi_last_data_recv: _Optional[int] = ..., tcpi_last_ack_recv: _Optional[int] = ..., tcpi_pmtu: _Optional[int] = ..., tcpi_rcv_ssthresh: _Optional[int] = ..., tcpi_rtt: _Optional[int] = ..., tcpi_rttvar: _Optional[int] = ..., tcpi_snd_ssthresh: _Optional[int] = ..., tcpi_snd_cwnd: _Optional[int] = ..., tcpi_advmss: _Optional[int] = ..., tcpi_reordering: _Optional[int] = ...) -> None: ...
 
-class SocketOptionTimeout(_message.Message):
-    __slots__ = ["duration"]
-    DURATION_FIELD_NUMBER: _ClassVar[int]
-    duration: _duration_pb2.Duration
-    def __init__(self, duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
+class GetTopChannelsRequest(_message.Message):
+    __slots__ = ["start_channel_id", "max_results"]
+    START_CHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
+    MAX_RESULTS_FIELD_NUMBER: _ClassVar[int]
+    start_channel_id: int
+    max_results: int
+    def __init__(self, start_channel_id: _Optional[int] = ..., max_results: _Optional[int] = ...) -> None: ...
 
-class SocketRef(_message.Message):
-    __slots__ = ["name", "socket_id"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    SOCKET_ID_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    socket_id: int
-    def __init__(self, socket_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
+class GetTopChannelsResponse(_message.Message):
+    __slots__ = ["channel", "end"]
+    CHANNEL_FIELD_NUMBER: _ClassVar[int]
+    END_FIELD_NUMBER: _ClassVar[int]
+    channel: _containers.RepeatedCompositeFieldContainer[Channel]
+    end: bool
+    def __init__(self, channel: _Optional[_Iterable[_Union[Channel, _Mapping]]] = ..., end: bool = ...) -> None: ...
 
-class Subchannel(_message.Message):
-    __slots__ = ["channel_ref", "data", "ref", "socket_ref", "subchannel_ref"]
-    CHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    REF_FIELD_NUMBER: _ClassVar[int]
+class GetServersRequest(_message.Message):
+    __slots__ = ["start_server_id", "max_results"]
+    START_SERVER_ID_FIELD_NUMBER: _ClassVar[int]
+    MAX_RESULTS_FIELD_NUMBER: _ClassVar[int]
+    start_server_id: int
+    max_results: int
+    def __init__(self, start_server_id: _Optional[int] = ..., max_results: _Optional[int] = ...) -> None: ...
+
+class GetServersResponse(_message.Message):
+    __slots__ = ["server", "end"]
+    SERVER_FIELD_NUMBER: _ClassVar[int]
+    END_FIELD_NUMBER: _ClassVar[int]
+    server: _containers.RepeatedCompositeFieldContainer[Server]
+    end: bool
+    def __init__(self, server: _Optional[_Iterable[_Union[Server, _Mapping]]] = ..., end: bool = ...) -> None: ...
+
+class GetServerRequest(_message.Message):
+    __slots__ = ["server_id"]
+    SERVER_ID_FIELD_NUMBER: _ClassVar[int]
+    server_id: int
+    def __init__(self, server_id: _Optional[int] = ...) -> None: ...
+
+class GetServerResponse(_message.Message):
+    __slots__ = ["server"]
+    SERVER_FIELD_NUMBER: _ClassVar[int]
+    server: Server
+    def __init__(self, server: _Optional[_Union[Server, _Mapping]] = ...) -> None: ...
+
+class GetServerSocketsRequest(_message.Message):
+    __slots__ = ["server_id", "start_socket_id", "max_results"]
+    SERVER_ID_FIELD_NUMBER: _ClassVar[int]
+    START_SOCKET_ID_FIELD_NUMBER: _ClassVar[int]
+    MAX_RESULTS_FIELD_NUMBER: _ClassVar[int]
+    server_id: int
+    start_socket_id: int
+    max_results: int
+    def __init__(self, server_id: _Optional[int] = ..., start_socket_id: _Optional[int] = ..., max_results: _Optional[int] = ...) -> None: ...
+
+class GetServerSocketsResponse(_message.Message):
+    __slots__ = ["socket_ref", "end"]
     SOCKET_REF_FIELD_NUMBER: _ClassVar[int]
-    SUBCHANNEL_REF_FIELD_NUMBER: _ClassVar[int]
-    channel_ref: _containers.RepeatedCompositeFieldContainer[ChannelRef]
-    data: ChannelData
-    ref: SubchannelRef
+    END_FIELD_NUMBER: _ClassVar[int]
     socket_ref: _containers.RepeatedCompositeFieldContainer[SocketRef]
-    subchannel_ref: _containers.RepeatedCompositeFieldContainer[SubchannelRef]
-    def __init__(self, ref: _Optional[_Union[SubchannelRef, _Mapping]] = ..., data: _Optional[_Union[ChannelData, _Mapping]] = ..., channel_ref: _Optional[_Iterable[_Union[ChannelRef, _Mapping]]] = ..., subchannel_ref: _Optional[_Iterable[_Union[SubchannelRef, _Mapping]]] = ..., socket_ref: _Optional[_Iterable[_Union[SocketRef, _Mapping]]] = ...) -> None: ...
+    end: bool
+    def __init__(self, socket_ref: _Optional[_Iterable[_Union[SocketRef, _Mapping]]] = ..., end: bool = ...) -> None: ...
 
-class SubchannelRef(_message.Message):
-    __slots__ = ["name", "subchannel_id"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class GetChannelRequest(_message.Message):
+    __slots__ = ["channel_id"]
+    CHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
+    channel_id: int
+    def __init__(self, channel_id: _Optional[int] = ...) -> None: ...
+
+class GetChannelResponse(_message.Message):
+    __slots__ = ["channel"]
+    CHANNEL_FIELD_NUMBER: _ClassVar[int]
+    channel: Channel
+    def __init__(self, channel: _Optional[_Union[Channel, _Mapping]] = ...) -> None: ...
+
+class GetSubchannelRequest(_message.Message):
+    __slots__ = ["subchannel_id"]
     SUBCHANNEL_ID_FIELD_NUMBER: _ClassVar[int]
-    name: str
     subchannel_id: int
-    def __init__(self, subchannel_id: _Optional[int] = ..., name: _Optional[str] = ...) -> None: ...
+    def __init__(self, subchannel_id: _Optional[int] = ...) -> None: ...
+
+class GetSubchannelResponse(_message.Message):
+    __slots__ = ["subchannel"]
+    SUBCHANNEL_FIELD_NUMBER: _ClassVar[int]
+    subchannel: Subchannel
+    def __init__(self, subchannel: _Optional[_Union[Subchannel, _Mapping]] = ...) -> None: ...
+
+class GetSocketRequest(_message.Message):
+    __slots__ = ["socket_id", "summary"]
+    SOCKET_ID_FIELD_NUMBER: _ClassVar[int]
+    SUMMARY_FIELD_NUMBER: _ClassVar[int]
+    socket_id: int
+    summary: bool
+    def __init__(self, socket_id: _Optional[int] = ..., summary: bool = ...) -> None: ...
+
+class GetSocketResponse(_message.Message):
+    __slots__ = ["socket"]
+    SOCKET_FIELD_NUMBER: _ClassVar[int]
+    socket: Socket
+    def __init__(self, socket: _Optional[_Union[Socket, _Mapping]] = ...) -> None: ...
```

### Comparing `grpcio-channelz-1.54.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py` & `grpcio-channelz-1.55.0rc1/grpc_channelz/v1/channelz_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/grpc_version.py` & `grpcio-channelz-1.55.0rc1/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_channelz/grpc_version.py.template`!!!
 
-VERSION = '1.54.0rc1'
+VERSION = '1.55.0rc1'
```

### Comparing `grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/PKG-INFO` & `grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.54.0rc1
+Version: 1.55.0rc1
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-channelz-1.54.0rc1/grpcio_channelz.egg-info/SOURCES.txt` & `grpcio-channelz-1.55.0rc1/grpcio_channelz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.54.0rc1/setup.py` & `grpcio-channelz-1.55.0rc1/setup.py`

 * *Files identical despite different names*

