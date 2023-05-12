# Comparing `tmp/nerfvis-0.1.4.tar.gz` & `tmp/nerfvis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfvis-0.1.4.tar", last modified: Fri Sep 16 22:20:18 2022, max compression
+gzip compressed data, was "nerfvis-0.1.5.tar", last modified: Fri May 12 20:16:44 2023, max compression
```

## Comparing `nerfvis-0.1.4.tar` & `nerfvis-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-09-16 22:20:18.496963 nerfvis-0.1.4/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.4/LICENSE.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.4/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)      251 2022-09-16 22:20:18.496963 nerfvis-0.1.4/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     7292 2022-09-11 09:26:48.000000 nerfvis-0.1.4/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-09-16 22:20:18.492963 nerfvis-0.1.4/nerfvis/
--rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.4/nerfvis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.4/nerfvis/index.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    60169 2022-09-16 21:54:39.000000 nerfvis-0.1.4/nerfvis/scene.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-09-16 22:20:18.496963 nerfvis-0.1.4/nerfvis/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.4/nerfvis/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.4/nerfvis/utils/_rotation.c
--rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.4/nerfvis/utils/_rotation.pyx
--rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.4/nerfvis/utils/sh.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2022-09-16 21:53:23.000000 nerfvis-0.1.4/nerfvis/version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2022-09-16 22:20:18.492963 nerfvis-0.1.4/nerfvis.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      251 2022-09-16 22:20:18.000000 nerfvis-0.1.4/nerfvis.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      366 2022-09-16 22:20:18.000000 nerfvis-0.1.4/nerfvis.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2022-09-16 22:20:18.000000 nerfvis-0.1.4/nerfvis.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        8 2022-09-16 22:20:18.000000 nerfvis-0.1.4/nerfvis.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.4/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2022-09-16 22:20:18.496963 nerfvis-0.1.4/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.4/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-02-04 19:47:59.000000 nerfvis-0.1.5/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      337 2022-09-11 08:09:28.000000 nerfvis-0.1.5/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-12 20:16:44.096757 nerfvis-0.1.5/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7483 2022-09-16 22:22:13.000000 nerfvis-0.1.5/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/nerfvis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       94 2022-08-24 01:42:22.000000 nerfvis-0.1.5/nerfvis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)   805091 2022-09-16 22:19:33.000000 nerfvis-0.1.5/nerfvis/index.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    60471 2023-05-12 20:11:07.000000 nerfvis-0.1.5/nerfvis/scene.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/nerfvis/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7202 2022-09-11 01:40:00.000000 nerfvis-0.1.5/nerfvis/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)  2003887 2022-08-23 04:07:45.000000 nerfvis-0.1.5/nerfvis/utils/_rotation.c
+-rw-rw-r--   0 alex      (1000) alex      (1000)    87588 2022-08-23 02:49:39.000000 nerfvis-0.1.5/nerfvis/utils/_rotation.pyx
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12573 2022-02-04 19:47:59.000000 nerfvis-0.1.5/nerfvis/utils/sh.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-05-12 20:11:17.000000 nerfvis-0.1.5/nerfvis/version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 20:16:44.096757 nerfvis-0.1.5/nerfvis.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      251 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      366 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        8 2023-05-12 20:16:44.000000 nerfvis-0.1.5/nerfvis.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2022-08-23 04:10:40.000000 nerfvis-0.1.5/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-05-12 20:16:44.100757 nerfvis-0.1.5/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1742 2022-09-11 08:10:30.000000 nerfvis-0.1.5/setup.py
```

### Comparing `nerfvis-0.1.4/LICENSE.txt` & `nerfvis-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.4/README.md` & `nerfvis-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -149,23 +149,29 @@
 
 Use `display(open_browser=False)` to prevent opening the browser (while serving the website)
 
 You can also add meshes, points, lines (see docs).
 Note that each object e.g. cube, mesh, points, etc. must have a unique name to identify it
 right now. You may programmatically generate this. They will show up in the *layers* pane
 (top right of the html viewer)
-**New in 0.0.6: Use / in the name e.g. cubes/red/cube001 to put meshes into folders in the layers pane.**
 
 
 Please also `pip install torch svox tqdm scipy` for adding NeRF (`set_nerf`)
 or `pip install trimesh` for using `add_mesh_from_file(path)`.
 
 To add cameras (also used for scaling scene, initializing camera etc), use 
 `add_camera_frustum(focal_length=.., image_width=.., image_height=.., z=..,  r=.., t=..)`
 
+## Viewer Controls
+
+- Left click and drag to orbit
+- Right click and drag, or CTRL+left click and drag to pan
+- Mouse wheel, middle click and drag, or ALT+left click and drag to zoom; alternatively use =/SHIFT+=
+- Number keys 1-6 to change coordinate systems: Z up/down Y up/down X up/down resp.
+
 
 ## Source of pre-compiled binaries
 
 This project contains a index.html containing inlined wasm, which comes from  `volrend`, the branch `nerfvis_base`, compiled using Emscripten as per the instructions in that repo.
 
 https://github.com/sxyu/volrend/tree/nerfvis_base
```

### Comparing `nerfvis-0.1.4/nerfvis/index.html` & `nerfvis-0.1.5/nerfvis/index.html`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.4/nerfvis/scene.py` & `nerfvis-0.1.5/nerfvis/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,15 +485,19 @@
         faces[:, 0, 1] = arr + image_size
         faces[:, 0, 2] = arr + image_size + 1
         faces[:, 1, 1] = arr + image_size + 1
         faces[:, 1, 2] = arr + 1
 
         im = np.array(im)[..., :3]
 
-        r = _scipy_rotation_from_auto(_to_np_array(r)).as_matrix()
+        if r.ndim == 2 and r.shape[-1] == 3 and r.shape[-2] == 3:
+            # Shape is good already
+            pass
+        else:
+            r = _scipy_rotation_from_auto(_to_np_array(r)).as_matrix()
         t = _to_np_array(t).astype(np.float32)
 
         grid_i = (r * grid.reshape(-1, 1, 3)).sum(-1) + t
         grid_i = grid_i.astype(np.float32).copy()
         self.add_mesh(
             name,
             grid_i,
@@ -864,15 +868,19 @@
         self._update_bb(center - radius)
         self._update_bb(center + radius)
         print("* Discretizing NeRF (requires torch, tqdm, svox, scipy)")
 
         if r is not None and t is not None:
             c2w = np.eye(4, dtype=np.float32)[None].repeat(r.shape[0], axis=0)
             c2w[:, :3, 3] = t
-            c2w[:, :3, :3] = _scipy_rotation_from_auto(_to_np_array(r)).as_matrix()
+            if r.ndim == 3 and r.shape[-1] == 3 and r.shape[-2] == 3:
+                # No conversion needed
+                c2w[:, :3, :3] = r
+            else:
+                c2w[:, :3, :3] = _scipy_rotation_from_auto(_to_np_array(r)).as_matrix()
             c2w = torch.from_numpy(c2w).to(device=device)
         else:
             c2w = None
 
         import torch
         from tqdm import tqdm
         from svox import N3Tree
@@ -1024,15 +1032,15 @@
                 self.fields[_f(name, k)] = tree_data[k]
 
 
     def write(self, path : str, compress : bool = True):
         """
         Write to drawlist npz which you can open with volrend
         (:code:`volrend --draw <output.npz>`;
-         nerfvis_base branch recommended for more up-to-date experience)
+        nerfvis_base branch recommended for more up-to-date experience)
         as well as in the web viewer. Usually, it's easier to use one of
         :code:`Scene.export()`,
         :code:`Scene.display()`, or
         :code:`Scene.emebd()`
 
         :param path: output npz path
         """
```

### Comparing `nerfvis-0.1.4/nerfvis/utils/__init__.py` & `nerfvis-0.1.5/nerfvis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.4/nerfvis/utils/_rotation.c` & `nerfvis-0.1.5/nerfvis/utils/_rotation.c`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.4/nerfvis/utils/_rotation.pyx` & `nerfvis-0.1.5/nerfvis/utils/_rotation.pyx`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.4/nerfvis/utils/sh.py` & `nerfvis-0.1.5/nerfvis/utils/sh.py`

 * *Files identical despite different names*

### Comparing `nerfvis-0.1.4/setup.py` & `nerfvis-0.1.5/setup.py`

 * *Files identical despite different names*

