# Comparing `tmp/pygltflib-1.8.tar.gz` & `tmp/pygltflib-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygltflib-1.8.tar", last modified: Wed Apr  3 20:59:06 2019, max compression
+gzip compressed data, was "dist/pygltflib-1.9.tar", last modified: Thu Apr  4 21:29:11 2019, max compression
```

## Comparing `pygltflib-1.8.tar` & `pygltflib-1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 luke      (1000) luke      (1000)        0 2019-04-03 20:59:06.000000 pygltflib-1.8/
--rw-rw-r--   0 luke      (1000) luke      (1000)       38 2019-04-03 20:59:06.000000 pygltflib-1.8/setup.cfg
--rw-rw-r--   0 luke      (1000) luke      (1000)    10408 2019-04-03 20:59:06.000000 pygltflib-1.8/PKG-INFO
-drwxrwxr-x   0 luke      (1000) luke      (1000)        0 2019-04-03 20:59:06.000000 pygltflib-1.8/pygltflib/
--rw-rw-r--   0 luke      (1000) luke      (1000)    18051 2019-04-03 20:42:10.000000 pygltflib-1.8/pygltflib/__init__.py
--rw-rw-r--   0 luke      (1000) luke      (1000)     3598 2019-03-27 05:08:34.000000 pygltflib-1.8/pygltflib/utils.py
--rw-rw-r--   0 luke      (1000) luke      (1000)     7898 2019-04-03 20:57:25.000000 pygltflib-1.8/README.md
--rw-rw-r--   0 luke      (1000) luke      (1000)      744 2018-10-26 23:42:12.000000 pygltflib-1.8/setup.py
-drwxrwxr-x   0 luke      (1000) luke      (1000)        0 2019-04-03 20:59:06.000000 pygltflib-1.8/pygltflib.egg-info/
--rw-rw-r--   0 luke      (1000) luke      (1000)    10408 2019-04-03 20:59:06.000000 pygltflib-1.8/pygltflib.egg-info/PKG-INFO
--rw-rw-r--   0 luke      (1000) luke      (1000)      191 2019-04-03 20:59:06.000000 pygltflib-1.8/pygltflib.egg-info/SOURCES.txt
--rw-rw-r--   0 luke      (1000) luke      (1000)       10 2019-04-03 20:59:06.000000 pygltflib-1.8/pygltflib.egg-info/top_level.txt
--rw-rw-r--   0 luke      (1000) luke      (1000)        1 2019-04-03 20:59:06.000000 pygltflib-1.8/pygltflib.egg-info/dependency_links.txt
+drwxrwxr-x   0 luke      (1000) luke      (1000)        0 2019-04-04 21:29:11.000000 pygltflib-1.9/
+-rw-rw-r--   0 luke      (1000) luke      (1000)       38 2019-04-04 21:29:11.000000 pygltflib-1.9/setup.cfg
+-rw-rw-r--   0 luke      (1000) luke      (1000)    12739 2019-04-04 21:29:11.000000 pygltflib-1.9/PKG-INFO
+drwxrwxr-x   0 luke      (1000) luke      (1000)        0 2019-04-04 21:29:11.000000 pygltflib-1.9/pygltflib/
+-rw-rw-r--   0 luke      (1000) luke      (1000)    18549 2019-04-04 21:16:02.000000 pygltflib-1.9/pygltflib/__init__.py
+-rw-rw-r--   0 luke      (1000) luke      (1000)     5385 2019-04-04 21:24:30.000000 pygltflib-1.9/pygltflib/utils.py
+-rw-rw-r--   0 luke      (1000) luke      (1000)     9677 2019-04-04 21:28:01.000000 pygltflib-1.9/README.md
+-rw-rw-r--   0 luke      (1000) luke      (1000)      744 2018-10-26 23:42:12.000000 pygltflib-1.9/setup.py
+drwxrwxr-x   0 luke      (1000) luke      (1000)        0 2019-04-04 21:29:11.000000 pygltflib-1.9/pygltflib.egg-info/
+-rw-rw-r--   0 luke      (1000) luke      (1000)    12739 2019-04-04 21:29:11.000000 pygltflib-1.9/pygltflib.egg-info/PKG-INFO
+-rw-rw-r--   0 luke      (1000) luke      (1000)      191 2019-04-04 21:29:11.000000 pygltflib-1.9/pygltflib.egg-info/SOURCES.txt
+-rw-rw-r--   0 luke      (1000) luke      (1000)       10 2019-04-04 21:29:11.000000 pygltflib-1.9/pygltflib.egg-info/top_level.txt
+-rw-rw-r--   0 luke      (1000) luke      (1000)        1 2019-04-04 21:29:11.000000 pygltflib-1.9/pygltflib.egg-info/dependency_links.txt
```

### Comparing `pygltflib-1.8/PKG-INFO` & `pygltflib-1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygltflib
-Version: 1.8
+Version: 1.9
 Summary: Python library for reading, writing and managing 3D objects in the Khronos Group gltf and gltf2 formats. Python 3.6+
 Home-page: https://gitlab.com/dodgyville/pygltflib
 Author: Luke Miller
 Author-email: dodgyville@gmail.com
 License: UNKNOWN
 Description: # pygltflib
         
@@ -40,14 +40,16 @@
         ###### Contributors:
         * Luke Miller
         * Sebastian Höffner
         * Arthur van Hoff
         
         
         ###### Changelog:
+        * 1.9
+            * use factories to create Attributes and Asset objects
         * 1.8
             * allow images to point to bufferViews
         * 1.7
             * preserve order of bufferViews when saving to glb
             * pad binary chunks within embedded data correctly
         * 1.6
             * provide better support for binary (.glb) files (bug fixes)
@@ -102,14 +104,81 @@
         
         >>> scene = Scene()
         >>> gltf.scenes.append(scene)
         >>> len(gltf.scenes)
         1
         
         ```
+        ##### A simple mesh
+        ```python3
+            from pygltflib import *
+            
+            # create gltf objects for a scene with a primitive triangle with indexed geometery
+            gltf = GLTF2()
+            scene = Scene()
+            mesh = Mesh()
+            primitive = Primitive()
+            node = Node()
+            buffer = Buffer()
+            bufferView1 = BufferView()
+            bufferView2 = BufferView()
+            accessor1 = Accessor()
+            accessor2 = Accessor()
+        
+            # add data
+            buffer.uri = "data:application/octet-stream;base64,AAABAAIAAAAAAAAAAAAAAAAAAAAAAIA/AAAAAAAAAAAAAAAAAACAPwAAAAA="
+            buffer.byteLength = 44
+        
+            bufferView1.buffer = 0
+            bufferView1.byteOffset = 0
+            bufferView1.byteLength = 6
+            bufferView1.target = 34963
+        
+            bufferView2.buffer = 0
+            bufferView2.byteOffset = 8
+            bufferView2.byteLength = 36
+            bufferView2.target = 34962
+        
+            accessor1.bufferView = 0
+            accessor1.byteOffset = 0
+            accessor1.componentType = UNSIGNED_SHORT
+            accessor1.count = 3
+            accessor1.type = SCALAR
+            accessor1.max = [2]
+            accessor1.min = [0]
+        
+            accessor2.bufferView = 1
+            accessor2.byteOffset = 0
+            accessor2.componentType = FLOAT
+            accessor2.count = 3
+            accessor2.type = VEC3
+            accessor2.max = [1.0, 1.0, 0.0]
+            accessor2.min = [0.0, 0.0, 0.0]
+        
+            primitive.attributes.POSITION = 1
+            node.mesh = 0
+            scene.nodes = [0]
+        
+            # assemble into a gltf structure
+            gltf.scenes.append(scene)
+            gltf.meshes.append(mesh)
+            gltf.meshes[0].primitives.append(primitive)
+            gltf.nodes.append(node)
+            gltf.buffers.append(buffer)
+            gltf.bufferViews.append(bufferView1)
+            gltf.bufferViews.append(bufferView2)
+            gltf.accessors.append(accessor1)
+            gltf.accessors.append(accessor2)
+        
+            # save to file
+            gltf.save("triangle.gltf")
+        
+        
+        ```
+        
         
         ### Loading and saving
         
         `pygltflib` can load json-based .GLTF files and binary .GLB files, based on the file extension. 
         
         #### GLTF files
```

### Comparing `pygltflib-1.8/pygltflib/__init__.py` & `pygltflib-1.9/pygltflib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 try:
     from dataclasses_json.core import _ExtendedEncoder as JsonEncoder
 except ImportError:  # backwards compat with dataclasses_json 0.0.25 and less
     from dataclasses_json.core import _CollectionEncoder as JsonEncoder
 
 
-__version__ = "1.8"
+__version__ = "1.9"
 
 
 A = TypeVar('A')
 
 
 LINEAR = "LINEAR"
 STEP = "STEP"
@@ -56,14 +56,21 @@
 VEC2 = "VEC2"
 VEC3 = "VEC3"
 VEC4 = "VEC4"
 MAT2 = "MAT2"
 MAT3 = "MAT3"
 MAT4 = "MAT4"
 
+BYTE = 5120  # 1
+UNSIGNED_BYTE = 5121  # 1
+SHORT = 5122  # 2
+UNSIGNED_SHORT = 5123   # 2
+UNSIGNED_INT = 5125  # 4
+FLOAT = 5126  # 4
+
 POSITION = "POSITION"
 NORMAL = "NORMAL"
 TANGENT = "TANGENT"
 TEXCOORD_0 = "TEXCOORD_0"
 TEXCOORD_1 = "TEXCOORD_1"
 COLOR_0 = "COLOR_0"
 JOINTS_0 = "JOINTS_0"
@@ -113,15 +120,15 @@
 # class PrimitiveTarget: #TODO is this the same as Attributes?
 #     POSITION: int = None
 
 
 @dataclass_json
 @dataclass
 class Primitive:
-    attributes: Attributes = Attributes()
+    attributes: Attributes = field(default_factory=Attributes)
     indices: int = None
     mode: int = None
     material: int = None
     targets: List[Attributes] = field(default_factory=list)
 
 
 @dataclass_json
@@ -325,15 +332,15 @@
     samplers: List[Sampler] = field(default_factory=list)
 
 
 @dataclass
 class GLTF2:
     accessors: List[Accessor] = field(default_factory=list)
     animations: List[Animation] = field(default_factory=list)
-    asset: Asset = Asset()
+    asset: Asset = field(default_factory=Asset)
     bufferViews: List[BufferView] = field(default_factory=list)
     buffers: List[Buffer] = field(default_factory=list)
     cameras: List[Camera] = field(default_factory=list)
     extensionsUsed: List[str] = field(default_factory=list)
     extensionsRequired: List[str] = field(default_factory=list)
     images: List[Image] = field(default_factory=list)
     materials: List[Material] = field(default_factory=list)
@@ -444,14 +451,18 @@
             original_buffers = copy.deepcopy(self.buffers)
 
             offset = 0
             new_buffer = Buffer()
             path = getattr(self, "_path", Path())
             for i, bufferView in enumerate(self.bufferViews):
                 buffer = self.buffers[bufferView.buffer]
+                if bufferView.byteStride and bufferView.byteStride > 0:
+                    warnings.warn(
+                        f"padding based on bufferView.byteStride is unsupported and may result in corrupted output. "
+                        "Please open an issue at https://gitlab.com/dodgyville/pygltflib/issues")
                 if buffer.uri == '':  # assume loaded from glb binary file
                     data = self._glb_data
                 elif Path(path.parent, buffer.uri).is_file():
                     with open(Path(path.parent, buffer.uri), 'rb') as fb:
                         data = fb.read()
                 else:
                     warnings.warn(f"Unable to save bufferView {buffer.uri} to glb, skipping. "
```

### Comparing `pygltflib-1.8/setup.py` & `pygltflib-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pygltflib-1.8/pygltflib.egg-info/PKG-INFO` & `pygltflib-1.9/pygltflib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygltflib
-Version: 1.8
+Version: 1.9
 Summary: Python library for reading, writing and managing 3D objects in the Khronos Group gltf and gltf2 formats. Python 3.6+
 Home-page: https://gitlab.com/dodgyville/pygltflib
 Author: Luke Miller
 Author-email: dodgyville@gmail.com
 License: UNKNOWN
 Description: # pygltflib
         
@@ -40,14 +40,16 @@
         ###### Contributors:
         * Luke Miller
         * Sebastian Höffner
         * Arthur van Hoff
         
         
         ###### Changelog:
+        * 1.9
+            * use factories to create Attributes and Asset objects
         * 1.8
             * allow images to point to bufferViews
         * 1.7
             * preserve order of bufferViews when saving to glb
             * pad binary chunks within embedded data correctly
         * 1.6
             * provide better support for binary (.glb) files (bug fixes)
@@ -102,14 +104,81 @@
         
         >>> scene = Scene()
         >>> gltf.scenes.append(scene)
         >>> len(gltf.scenes)
         1
         
         ```
+        ##### A simple mesh
+        ```python3
+            from pygltflib import *
+            
+            # create gltf objects for a scene with a primitive triangle with indexed geometery
+            gltf = GLTF2()
+            scene = Scene()
+            mesh = Mesh()
+            primitive = Primitive()
+            node = Node()
+            buffer = Buffer()
+            bufferView1 = BufferView()
+            bufferView2 = BufferView()
+            accessor1 = Accessor()
+            accessor2 = Accessor()
+        
+            # add data
+            buffer.uri = "data:application/octet-stream;base64,AAABAAIAAAAAAAAAAAAAAAAAAAAAAIA/AAAAAAAAAAAAAAAAAACAPwAAAAA="
+            buffer.byteLength = 44
+        
+            bufferView1.buffer = 0
+            bufferView1.byteOffset = 0
+            bufferView1.byteLength = 6
+            bufferView1.target = 34963
+        
+            bufferView2.buffer = 0
+            bufferView2.byteOffset = 8
+            bufferView2.byteLength = 36
+            bufferView2.target = 34962
+        
+            accessor1.bufferView = 0
+            accessor1.byteOffset = 0
+            accessor1.componentType = UNSIGNED_SHORT
+            accessor1.count = 3
+            accessor1.type = SCALAR
+            accessor1.max = [2]
+            accessor1.min = [0]
+        
+            accessor2.bufferView = 1
+            accessor2.byteOffset = 0
+            accessor2.componentType = FLOAT
+            accessor2.count = 3
+            accessor2.type = VEC3
+            accessor2.max = [1.0, 1.0, 0.0]
+            accessor2.min = [0.0, 0.0, 0.0]
+        
+            primitive.attributes.POSITION = 1
+            node.mesh = 0
+            scene.nodes = [0]
+        
+            # assemble into a gltf structure
+            gltf.scenes.append(scene)
+            gltf.meshes.append(mesh)
+            gltf.meshes[0].primitives.append(primitive)
+            gltf.nodes.append(node)
+            gltf.buffers.append(buffer)
+            gltf.bufferViews.append(bufferView1)
+            gltf.bufferViews.append(bufferView2)
+            gltf.accessors.append(accessor1)
+            gltf.accessors.append(accessor2)
+        
+            # save to file
+            gltf.save("triangle.gltf")
+        
+        
+        ```
+        
         
         ### Loading and saving
         
         `pygltflib` can load json-based .GLTF files and binary .GLB files, based on the file extension. 
         
         #### GLTF files
```

