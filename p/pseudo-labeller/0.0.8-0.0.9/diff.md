# Comparing `tmp/pseudo_labeller-0.0.8.tar.gz` & `tmp/pseudo_labeller-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudo_labeller-0.0.8.tar", last modified: Tue May  2 12:50:47 2023, max compression
+gzip compressed data, was "pseudo_labeller-0.0.9.tar", last modified: Fri May 12 15:17:44 2023, max compression
```

## Comparing `pseudo_labeller-0.0.8.tar` & `pseudo_labeller-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/pseudo_labeller/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/pseudo_labeller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/pseudo_labeller/model/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/pseudo_labeller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/pseudo_labeller/model/idam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/pseudo_labeller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/pseudo_labeller/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/pseudo_labeller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-02 12:50:47.000000 pseudo_labeller-0.0.8/pseudo_labeller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 12:50:47.000000 pseudo_labeller-0.0.8/pseudo_labeller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:50:47.000000 pseudo_labeller-0.0.8/pseudo_labeller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 12:50:47.000000 pseudo_labeller-0.0.8/pseudo_labeller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 12:50:47.000000 pseudo_labeller-0.0.8/pseudo_labeller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:50:47.086291 pseudo_labeller-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 12:50:27.000000 pseudo_labeller-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:17:44.051752 pseudo_labeller-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-12 15:17:44.051752 pseudo_labeller-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:17:44.047752 pseudo_labeller-0.0.9/pseudo_labeller/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/pseudo_labeller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:17:44.051752 pseudo_labeller-0.0.9/pseudo_labeller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/pseudo_labeller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/pseudo_labeller/model/idam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:17:44.051752 pseudo_labeller-0.0.9/pseudo_labeller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/pseudo_labeller/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:17:44.051752 pseudo_labeller-0.0.9/pseudo_labeller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-12 15:17:44.000000 pseudo_labeller-0.0.9/pseudo_labeller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 15:17:44.000000 pseudo_labeller-0.0.9/pseudo_labeller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:17:44.000000 pseudo_labeller-0.0.9/pseudo_labeller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 15:17:44.000000 pseudo_labeller-0.0.9/pseudo_labeller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 15:17:44.000000 pseudo_labeller-0.0.9/pseudo_labeller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:17:44.051752 pseudo_labeller-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-12 15:17:28.000000 pseudo_labeller-0.0.9/setup.py
```

### Comparing `pseudo_labeller-0.0.8/LICENSE` & `pseudo_labeller-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pseudo_labeller-0.0.8/pseudo_labeller/model/idam.py` & `pseudo_labeller-0.0.9/pseudo_labeller/model/idam.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,16 +76,14 @@
                 nn.Conv3d(
                     in_channels=conv3d_channels,
                     out_channels=conv3d_channels,
                     kernel_size=(kernel_size, kernel_size, kernel_size),
                     padding="same",
                 )
             )
-            #if i % 2 == 0:
-            #    self.layers.append(nn.BatchNorm3d(conv3d_channels))
 
         # Map to output latent variables, per timestep
 
         # Map the output to the latent variables
         # Latent head should be number of output steps + latent channels
         self.latent_head = nn.Conv2d(
             in_channels=input_steps * conv3d_channels,
@@ -93,28 +91,26 @@
             kernel_size=(1, 1),
             padding="same",
         )
 
         # Small head model to convert from latent space to PV generation for training
         # Input is per-pixel input data, this will be
         # reshaped to the same output steps as the latent head
-        self.pv_meta_input = nn.Conv2d(
-            pv_meta_input_channels, out_channels=hidden_dim, kernel_size=(1, 1)
+        self.pv_meta_input = nn.Conv1d(
+            pv_meta_input_channels, out_channels=hidden_dim, kernel_size=1
         )
-        self.batch_norm_meta = nn.Identity()
 
         # Output is forecast steps channels, each channel is a timestep
         # For labelling, this should be 1, forecasting the middle
         # timestep, for forecasting, the number of steps
         # This is done by putting the meta inputs to each timestep
-        self.batch_norm_output_meta = nn.Identity()
-        self.pv_meta_output = nn.Conv2d(
+        self.pv_meta_output = nn.Conv1d(
             in_channels=(output_steps * output_channels) + hidden_dim,
             out_channels=output_steps,
-            kernel_size=(1, 1),
+            kernel_size=1,
             padding="same",
         )
 
     def forward(self, x: torch.Tensor, pv_meta: torch.Tensor = None, output_latents: bool = True):
         """
         Compute either just the latent psuedo irradience, or the PV generation
 
@@ -132,16 +128,17 @@
         x = einops.rearrange(x, "b c t h w -> b (c t) h w")
         x = self.latent_head(x)
         if output_latents:
             # Rearrange back to timeseries of latent variables
             x = einops.rearrange(x, "b (c t) h w -> b c t h w", c=self.output_channels)
             return x
         pv_meta = self.pv_meta_input(pv_meta)
-        pv_meta = self.batch_norm_meta(pv_meta)
         pv_meta = F.relu(pv_meta)
+        # Scale down to 1 size
+        x = F.adaptive_avg_pool2d(x, (1, 1))
         # Reshape to fit into 3DCNN
         x = torch.cat([x, pv_meta], dim=1)
         # Get pv_meta_output
         x = F.relu(
-            self.pv_meta_output(self.batch_norm_output_meta(x))
+            self.pv_meta_output(x)
         )  # Generation can only be positive or 0, so ReLU
         return x
```

### Comparing `pseudo_labeller-0.0.8/setup.py` & `pseudo_labeller-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="pseudo_labeller",
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     description="Psuedo PV/Irradience Labeller",
     author="Jacob Bieker",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

