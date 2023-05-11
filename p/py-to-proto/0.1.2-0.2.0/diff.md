# Comparing `tmp/py_to_proto-0.1.2-py39-none-any.whl.zip` & `tmp/py_to_proto-0.2.0-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 31558 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1174 b- defN 23-May-01 23:14 py_to_proto/__init__.py
--rw-r--r--  2.0 unx      251 b- defN 23-May-01 23:14 py_to_proto/compat_annotated.py
--rw-r--r--  2.0 unx    26041 b- defN 23-May-01 23:14 py_to_proto/converter_base.py
--rw-r--r--  2.0 unx    12097 b- defN 23-May-01 23:14 py_to_proto/dataclass_to_proto.py
--rw-r--r--  2.0 unx     9686 b- defN 23-May-01 23:14 py_to_proto/descriptor_to_file.py
--rw-r--r--  2.0 unx     4799 b- defN 23-May-01 23:14 py_to_proto/descriptor_to_message_class.py
--rw-r--r--  2.0 unx     9092 b- defN 23-May-01 23:14 py_to_proto/json_to_service.py
--rw-r--r--  2.0 unx     8288 b- defN 23-May-01 23:14 py_to_proto/jtd_to_proto.py
--rw-r--r--  2.0 unx    12660 b- defN 23-May-01 23:14 py_to_proto/utils.py
--rw-r--r--  2.0 unx    14885 b- defN 23-May-01 23:14 py_to_proto/validation.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     6777 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1272 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/RECORD
-15 files, 108215 bytes uncompressed, 29452 bytes compressed:  72.8%
+Zip file size: 32208 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1174 b- defN 23-May-11 22:59 py_to_proto/__init__.py
+-rw-r--r--  2.0 unx      251 b- defN 23-May-11 22:59 py_to_proto/compat_annotated.py
+-rw-r--r--  2.0 unx    26041 b- defN 23-May-11 22:59 py_to_proto/converter_base.py
+-rw-r--r--  2.0 unx    12097 b- defN 23-May-11 22:59 py_to_proto/dataclass_to_proto.py
+-rw-r--r--  2.0 unx     9686 b- defN 23-May-11 22:59 py_to_proto/descriptor_to_file.py
+-rw-r--r--  2.0 unx     5265 b- defN 23-May-11 22:59 py_to_proto/descriptor_to_message_class.py
+-rw-r--r--  2.0 unx    12474 b- defN 23-May-11 22:59 py_to_proto/json_to_service.py
+-rw-r--r--  2.0 unx     8288 b- defN 23-May-11 22:59 py_to_proto/jtd_to_proto.py
+-rw-r--r--  2.0 unx    12660 b- defN 23-May-11 22:59 py_to_proto/utils.py
+-rw-r--r--  2.0 unx    14885 b- defN 23-May-11 22:59 py_to_proto/validation.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-11 23:00 py_to_proto-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6777 b- defN 23-May-11 23:00 py_to_proto-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-May-11 23:00 py_to_proto-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-11 23:00 py_to_proto-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1273 b- defN 23-May-11 23:00 py_to_proto-0.2.0.dist-info/RECORD
+15 files, 112064 bytes uncompressed, 30102 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: py_to_proto/utils.py
 Comment: 
 
 Filename: py_to_proto/validation.py
 Comment: 
 
-Filename: py_to_proto-0.1.2.dist-info/LICENSE
+Filename: py_to_proto-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: py_to_proto-0.1.2.dist-info/METADATA
+Filename: py_to_proto-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: py_to_proto-0.1.2.dist-info/WHEEL
+Filename: py_to_proto-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: py_to_proto-0.1.2.dist-info/top_level.txt
+Filename: py_to_proto-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: py_to_proto-0.1.2.dist-info/RECORD
+Filename: py_to_proto-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py_to_proto/descriptor_to_message_class.py

```diff
@@ -41,17 +41,25 @@
         # Check to see whether this descriptor already has a concrete class.
         # NOTE: The MessageFactory already does this for newer versions of
         #   proto, but in order to maintain compatibility with older versions,
         #   this is needed here.
         try:
             message_class = descriptor._concrete_class
         except (TypeError, SystemError, AttributeError):
-            message_class = reflection.message_factory.MessageFactory().GetPrototype(
-                descriptor
-            )
+            # protobuf version compatibility
+            if hasattr(reflection.message_factory, "GetMessageClass"):
+                # Newer protobuf versions use GetMessageClass
+                message_class = reflection.message_factory.GetMessageClass(
+                    descriptor
+                )  # pragma: no cover
+            else:
+                # Older protobuf versions require creating an instance of a MessageFactory
+                message_class = (
+                    reflection.message_factory.MessageFactory().GetPrototype(descriptor)
+                )  # pragma: no cover
 
         # Recursively add nested messages
         for nested_message_descriptor in descriptor.nested_types:
             nested_message_class = descriptor_to_message_class(
                 nested_message_descriptor
             )
             setattr(message_class, nested_message_descriptor.name, nested_message_class)
```

## py_to_proto/json_to_service.py

```diff
@@ -1,18 +1,17 @@
 # Standard
 from typing import Callable, Dict, List, Optional, Type
 import dataclasses
 import types
 
 # Third Party
-from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pb2
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message, service
-from google.protobuf.descriptor import ServiceDescriptor
+from google.protobuf import service
+from google.protobuf.descriptor import MethodDescriptor, ServiceDescriptor
 from google.protobuf.service import Service
 from google.protobuf.service_reflection import GeneratedServiceType
 import grpc
 
 # First Party
 import alog
 
@@ -32,15 +31,19 @@
             "properties": {
                 "rpcs": {
                     "elements": {
                         "properties": {
                             "input_type": {"type": "string"},
                             "name": {"type": "string"},
                             "output_type": {"type": "string"},
-                        }
+                        },
+                        "optionalProperties": {
+                            "server_streaming": {"type": "boolean"},
+                            "client_streaming": {"type": "boolean"},
+                        },
                     }
                 }
             }
         }
     }
 }
 
@@ -48,22 +51,30 @@
     bytes=lambda x: isinstance(x, bytes), **JTD_TYPE_VALIDATORS
 )
 
 # Python type hint equivalent of jtd service schema
 ServiceJsonType = Dict[str, Dict[str, List[Dict[str, str]]]]
 
 
+@dataclasses.dataclass
+class GRPCService:
+    descriptor: ServiceDescriptor
+    registration_function: Callable[[Service, grpc.Server], None]
+    client_stub_class: Type
+    service_class: Type[service.Service]
+
+
 def json_to_service(
     name: str,
     package: str,
     json_service_def: ServiceJsonType,
     *,
     descriptor_pool: Optional[_descriptor_pool.DescriptorPool] = None,
-) -> _descriptor.ServiceDescriptor:
-    """Convert a JSON representation of an RPC service into a ServiceDescriptor.
+) -> GRPCService:
+    """Convert a JSON representation of an RPC service into a GRPCService.
 
     Reference: https://jsontypedef.com/docs/jtd-in-5-minutes/
 
     Args:
         name:  str
             The name for the top-level service object
         package:  str
@@ -73,43 +84,95 @@
 
     Kwargs:
         descriptor_pool:  Optional[descriptor_pool.DescriptorPool]
             If given, this DescriptorPool will be used to aggregate the set of
             message descriptors
 
     Returns:
-        descriptor:  google.protobuf.descriptor.ServiceDescriptor
-            The ServiceDescriptor corresponding to this json definition
+        grpc_service:  GRPCService
+            The GRPCService container with the service descriptor and other associated
+            grpc bits required to boot a server:
+            - Servicer registration function
+            - Client stub class
+            - Servicer base class
     """
     # Ensure we have a valid service spec
     log.debug2("Validating service json")
     if not validate_jtd(json_service_def, SERVICE_JTD_SCHEMA, EXTENDED_TYPE_VALIDATORS):
         raise ValueError("Invalid service json")
 
-    method_descriptor_protos: List[descriptor_pb2.MethodDescriptorProto] = []
-    imports: List[str] = []
-
+    # And descriptor pool
     if descriptor_pool is None:
         log.debug2("Using the default descriptor pool")
         descriptor_pool = _descriptor_pool.Default()
 
+    # First get the descriptor proto:
+    service_fd_proto = _json_to_service_file_descriptor_proto(
+        name, package, json_service_def, descriptor_pool=descriptor_pool
+    )
+    assert (
+        len(service_fd_proto.service) == 1
+    ), f"File Descriptor {service_fd_proto.name} should only have one service"
+    service_descriptor_proto = service_fd_proto.service[0]
+
+    # Then put that in the pool to get the real descriptor back
+    log.debug("Adding Descriptors to DescriptorPool")
+    safe_add_fd_to_pool(service_fd_proto, descriptor_pool)
+    service_fullname = name if not package else ".".join([package, name])
+    service_descriptor = descriptor_pool.FindServiceByName(service_fullname)
+
+    # Then the client stub:
+    client_stub = _service_descriptor_to_client_stub(
+        service_descriptor, service_descriptor_proto
+    )
+
+    # And the registration function:
+    registration_function = _service_descriptor_to_server_registration_function(
+        service_descriptor, service_descriptor_proto
+    )
+
+    # And service class!
+    service_class = _service_descriptor_to_service(service_descriptor)
+
+    return GRPCService(
+        descriptor=service_descriptor,
+        service_class=service_class,
+        client_stub_class=client_stub,
+        registration_function=registration_function,
+    )
+
+
+def _json_to_service_file_descriptor_proto(
+    name: str,
+    package: str,
+    json_service_def: ServiceJsonType,
+    *,
+    descriptor_pool: Optional[_descriptor_pool.DescriptorPool] = None,
+) -> descriptor_pb2.FileDescriptorProto:
+    """Creates the FileDescriptorProto for the service definition"""
+
+    method_descriptor_protos: List[descriptor_pb2.MethodDescriptorProto] = []
+    imports: List[str] = []
+
     json_service = json_service_def["service"]
     rpcs_def = json_service["rpcs"]
     for rpc_def in rpcs_def:
         rpc_input_type = rpc_def["input_type"]
         input_descriptor = descriptor_pool.FindMessageTypeByName(rpc_input_type)
 
         rpc_output_type = rpc_def["output_type"]
         output_descriptor = descriptor_pool.FindMessageTypeByName(rpc_output_type)
 
         method_descriptor_protos.append(
             descriptor_pb2.MethodDescriptorProto(
                 name=rpc_def["name"],
                 input_type=input_descriptor.full_name,
                 output_type=output_descriptor.full_name,
+                client_streaming=rpc_def.get("client_streaming", False),
+                server_streaming=rpc_def.get("server_streaming", False),
             )
         )
         imports.append(input_descriptor.file.name)
         imports.append(output_descriptor.file.name)
 
     imports = sorted(list(set(imports)))
 
@@ -122,153 +185,159 @@
         package=package,
         syntax="proto3",
         dependency=imports,
         # **proto_kwargs,
         service=[service_descriptor_proto],
     )
 
-    # Add the FileDescriptorProto to the Descriptor Pool
-    log.debug("Adding Descriptors to DescriptorPool")
-    safe_add_fd_to_pool(fd_proto, descriptor_pool)
-
-    # Return the descriptor for the top-level message
-    fullname = name if not package else ".".join([package, name])
-
-    return descriptor_pool.FindServiceByName(fullname)
+    return fd_proto
 
 
-def service_descriptor_to_service(
-    service_descriptor: _descriptor.ServiceDescriptor,
+def _service_descriptor_to_service(
+    service_descriptor: ServiceDescriptor,
 ) -> Type[service.Service]:
     """Create a service class from a service descriptor
 
     Args:
         service_descriptor:  google.protobuf.descriptor.ServiceDescriptor
             The ServiceDescriptor to generate a service interface for
 
     Returns:
         Type[google.protobuf.service.Service]
-            A new class with metaclass google.protobuf.service_reflection.GeneratedServiceType containing the methods
-            from the service_descriptor
+            A new class with metaclass google.protobuf.service_reflection.GeneratedServiceType
+            containing the methods from the service_descriptor
     """
     service_class = types.new_class(
         service_descriptor.name,
         (service.Service,),
         {"metaclass": GeneratedServiceType},
         lambda ns: ns.update({"DESCRIPTOR": service_descriptor}),
     )
     service_class = _add_protobuf_serializers(service_class, service_descriptor)
 
     return service_class
 
 
-def service_descriptor_to_client_stub(
-    service_descriptor: _descriptor.ServiceDescriptor,
+def _service_descriptor_to_client_stub(
+    service_descriptor: ServiceDescriptor,
+    service_descriptor_proto: descriptor_pb2.ServiceDescriptorProto,
 ) -> Type:
     """Generates a new client stub class from the service descriptor
 
     Args:
-        service_descriptor (google.protobuf.descriptor.ServiceDescriptor):
+        service_descriptor:  google.protobuf.descriptor.ServiceDescriptor
             The ServiceDescriptor to generate a service interface for
+        service_descriptor_proto:  google.protobuf.descriptor_pb2.ServiceDescriptorProto
+            The descriptor proto for that service. This holds the I/O streaming information
+            for each method
     """
-    methods = _get_rpc_methods(service_descriptor)
+    _assert_method_lists_same(service_descriptor, service_descriptor_proto)
+
+    def _get_channel_func(
+        channel: grpc.Channel, method: descriptor_pb2.MethodDescriptorProto
+    ) -> Callable:
+        if method.client_streaming and method.server_streaming:
+            return channel.stream_stream
+        if not method.client_streaming and method.server_streaming:
+            return channel.unary_stream
+        if method.client_streaming and not method.server_streaming:
+            return channel.stream_unary
+        return channel.unary_unary
 
     # Initializer
-    def initializer(self, channel):
+    def initializer(self, channel: grpc.Channel):
         f"""Initializes a client stub with for the {service_descriptor.name} Service"""
-        for method in methods:
+        for method, method_proto in zip(
+            service_descriptor.methods, service_descriptor_proto.method
+        ):
             setattr(
                 self,
                 method.name,
-                channel.unary_unary(
-                    method.fullname,
-                    request_serializer=method.input_message_class.SerializeToString,
-                    response_deserializer=method.output_message_class.FromString,
+                _get_channel_func(channel, method_proto)(
+                    _get_method_fullname(method),
+                    request_serializer=descriptor_to_message_class(
+                        method.input_type
+                    ).SerializeToString,
+                    response_deserializer=descriptor_to_message_class(
+                        method.output_type
+                    ).FromString,
                 ),
             )
 
     # Creating class dynamically
     return type(
         f"{service_descriptor.name}Stub",
         (object,),
         {
             "__init__": initializer,
         },
     )
 
 
-def service_descriptor_to_server_registration_function(
-    service_descriptor: _descriptor.ServiceDescriptor,
+def _service_descriptor_to_server_registration_function(
+    service_descriptor: ServiceDescriptor,
+    service_descriptor_proto: descriptor_pb2.ServiceDescriptorProto,
 ) -> Callable[[Service, grpc.Server], None]:
     """Generates a server registration function from the service descriptor
 
     Args:
         service_descriptor:  google.protobuf.descriptor.ServiceDescriptor
             The ServiceDescriptor to generate a service interface for
+        service_descriptor_proto:  google.protobuf.descriptor_pb2.ServiceDescriptorProto
+            The descriptor proto for that service. This holds the I/O streaming information
+            for each method
 
     Returns:
         function:  Server registration function to add service handlers to a server
     """
-    methods = _get_rpc_methods(service_descriptor)
+    _assert_method_lists_same(service_descriptor, service_descriptor_proto)
+
+    def _get_handler(method: descriptor_pb2.MethodDescriptorProto):
+        if method.client_streaming and method.server_streaming:
+            return grpc.stream_stream_rpc_method_handler
+        if not method.client_streaming and method.server_streaming:
+            return grpc.unary_stream_rpc_method_handler
+        if method.client_streaming and not method.server_streaming:
+            return grpc.stream_unary_rpc_method_handler
+        return grpc.unary_unary_rpc_method_handler
 
     def registration_function(servicer: Service, server: grpc.Server):
         """Server registration function"""
         rpc_method_handlers = {
-            method.name: grpc.unary_unary_rpc_method_handler(
+            method.name: _get_handler(method_proto)(
                 getattr(servicer, method.name),
-                request_deserializer=method.input_message_class.FromString,
-                response_serializer=method.output_message_class.SerializeToString,
+                request_deserializer=descriptor_to_message_class(
+                    method.input_type
+                ).FromString,
+                response_serializer=descriptor_to_message_class(
+                    method.output_type
+                ).SerializeToString,
+            )
+            for method, method_proto in zip(
+                service_descriptor.methods, service_descriptor_proto.method
             )
-            for method in methods
         }
         generic_handler = grpc.method_handlers_generic_handler(
             service_descriptor.full_name, rpc_method_handlers
         )
         server.add_generic_rpc_handlers((generic_handler,))
 
     return registration_function
 
 
-@dataclasses.dataclass
-class _RPCMethod:
-    name: str
-    fullname: str
-    input_message_class: Type[message.Message]
-    output_message_class: Type[message.Message]
-
-
-def _get_rpc_methods(service_descriptor: ServiceDescriptor) -> List[_RPCMethod]:
-    """Get list of RPC methods from a service descriptor
+def _get_method_fullname(method: MethodDescriptor):
+    method_name_parts = method.full_name.split(".")
+    return f"/{'.'.join(method_name_parts[:-1])}/{method_name_parts[-1]}"
 
-    Args:
-        service_descriptor:  google.protobuf.descriptor.ServiceDescriptor
-            The ServiceDescriptor to get RPC methods for
-
-    Returns:
-        List of RPC methods
-    """
-    # For each method, need to know input / output message
-    methods: List[_RPCMethod] = []
-
-    for method in service_descriptor.methods:
-        method: _descriptor.MethodDescriptor
 
-        input_descriptor: _descriptor.Descriptor = method.input_type
-        output_descriptor: _descriptor.Descriptor = method.output_type
-
-        input_message_class = descriptor_to_message_class(input_descriptor)
-        output_message_class = descriptor_to_message_class(output_descriptor)
-
-        method_name_parts = method.full_name.split(".")
-        method_full_name = (
-            f"/{'.'.join(method_name_parts[:-1])}/{method_name_parts[-1]}"
-        )
-        methods.append(
-            _RPCMethod(
-                name=method.name,
-                fullname=method_full_name,
-                input_message_class=input_message_class,
-                output_message_class=output_message_class,
-            )
-        )
+def _assert_method_lists_same(
+    service_descriptor: ServiceDescriptor,
+    service_descriptor_proto: descriptor_pb2.ServiceDescriptorProto,
+):
+    assert len(service_descriptor.methods) == len(service_descriptor_proto.method), (
+        f"Method count mismatch: {service_descriptor.full_name} has"
+        f" {len(service_descriptor.methods)} methods but proto descriptor"
+        f" {service_descriptor_proto.name} has {len(service_descriptor_proto.method)} methods"
+    )
 
-    return methods
+    for m1, m2 in zip(service_descriptor.methods, service_descriptor_proto.method):
+        assert m1.name == m2.name, f"Method mismatch: {m1.name}, {m2.name}"
```

## Comparing `py_to_proto-0.1.2.dist-info/LICENSE` & `py_to_proto-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py_to_proto-0.1.2.dist-info/METADATA` & `py_to_proto-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-to-proto
-Version: 0.1.2
+Version: 0.2.0
 Summary: A tool to dynamically create protobuf message classes from python data schemas
 Home-page: https://github.com/IBM/py-to-proto
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: json,json typedef,jtd,protobuf,proto,dataclass
 Platform: UNKNOWN
```

## Comparing `py_to_proto-0.1.2.dist-info/RECORD` & `py_to_proto-0.2.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 py_to_proto/__init__.py,sha256=0xvSrTlGuMSPzey0U_v2i1ehBcFVzQRk3Z2qbFZiXO4,1174
 py_to_proto/compat_annotated.py,sha256=-JMeTz4v2hSkrRKVfQVqOlI1Az6IVqXoIC3ma2Fu2XI,251
 py_to_proto/converter_base.py,sha256=M_fO8qin-dklE19hPs9gyDTnjmjYvrRlwHdBOgzGLEw,26041
 py_to_proto/dataclass_to_proto.py,sha256=e2sjalvr03_aaclbpXHiby5PFSuS_EOaZs_Gvb_hJxk,12097
 py_to_proto/descriptor_to_file.py,sha256=aVOJGMulF_xppS1n3MdjB8hStRXdnSH7Fkmhui6Xd2Q,9686
-py_to_proto/descriptor_to_message_class.py,sha256=GLk9Uh3j66ADzb_HIy_fswm6WSOp23wgvEPJlBSnuv8,4799
-py_to_proto/json_to_service.py,sha256=yI3pyM99rWBbx63jhmSHi6M-_55ERPBmKtSg8tegQes,9092
+py_to_proto/descriptor_to_message_class.py,sha256=2gJfz38W0_XLS4I3XI4Vtycok0-9q6kfSK7A_OYW2X4,5265
+py_to_proto/json_to_service.py,sha256=zzbJnXnXLeCPwRQsFYWnbzSKFgUBe-SpUeWYIKd7HCU,12474
 py_to_proto/jtd_to_proto.py,sha256=dmRj35Z5rfFgfeP2QRTaJ2sF1tZrYBD7KsyNY5yrCQ0,8288
 py_to_proto/utils.py,sha256=SU9A7S3yFN5EgRFu2gibVbebsng_2uF2wF4zPjedGMk,12660
 py_to_proto/validation.py,sha256=ssTE17roJwMYwTkRSuDUKL_JGAf1C3Ua0bcAsSPEtLE,14885
-py_to_proto-0.1.2.dist-info/LICENSE,sha256=t-ZkY-vak1QWjzid8VIzMds6wT0xEafbk406cLmdj_Q,1088
-py_to_proto-0.1.2.dist-info/METADATA,sha256=ePYaUZkVRqGCxznMVhSbejgdfMDG5Rx7nyFJtFVKQj0,6777
-py_to_proto-0.1.2.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
-py_to_proto-0.1.2.dist-info/top_level.txt,sha256=AScY99r2vRxOMZGEg6sfYg7B5BlIyy9sXKc6CrlBR5s,12
-py_to_proto-0.1.2.dist-info/RECORD,,
+py_to_proto-0.2.0.dist-info/LICENSE,sha256=t-ZkY-vak1QWjzid8VIzMds6wT0xEafbk406cLmdj_Q,1088
+py_to_proto-0.2.0.dist-info/METADATA,sha256=lqstt1THvLYHnaRryGnV5pq4huq6AeuqGgRvJgzmnTE,6777
+py_to_proto-0.2.0.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
+py_to_proto-0.2.0.dist-info/top_level.txt,sha256=AScY99r2vRxOMZGEg6sfYg7B5BlIyy9sXKc6CrlBR5s,12
+py_to_proto-0.2.0.dist-info/RECORD,,
```

