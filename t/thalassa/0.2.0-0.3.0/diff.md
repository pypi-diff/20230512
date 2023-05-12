# Comparing `tmp/thalassa-0.2.0.tar.gz` & `tmp/thalassa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thalassa-0.2.0.tar", max compression
+gzip compressed data, was "thalassa-0.3.0.tar", max compression
```

## Comparing `thalassa-0.2.0.tar` & `thalassa-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,8 @@
--rw-r--r--   0        0        0    14138 2023-03-02 09:50:57.249458 thalassa-0.2.0/LICENSE
--rw-r--r--   0        0        0     1967 2023-03-15 09:24:38.558587 thalassa-0.2.0/README.md
--rw-r--r--   0        0        0     3639 2023-05-08 07:29:53.137564 thalassa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-02 09:50:57.249458 thalassa-0.2.0/thalassa/__init__.py
--rw-r--r--   0        0        0    11314 2023-05-08 05:42:04.878122 thalassa-0.2.0/thalassa/api.py
--rw-r--r--   0        0        0     5327 2023-05-08 05:42:04.881456 thalassa-0.2.0/thalassa/normalization.py
--rw-r--r--   0        0        0     5039 2022-11-23 12:15:17.376479 thalassa-0.2.0/thalassa/static/favicon.png
--rw-r--r--   0        0        0     4987 2022-11-22 19:39:04.004846 thalassa-0.2.0/thalassa/static/logo.png
--rw-r--r--   0        0        0    18092 2023-05-08 05:42:04.878122 thalassa-0.2.0/thalassa/ui.py
--rw-r--r--   0        0        0     9720 2023-05-08 05:42:04.878122 thalassa-0.2.0/thalassa/utils.py
--rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 thalassa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    14138 2023-03-02 09:50:57.249458 thalassa-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2392 2023-05-12 15:48:27.668665 thalassa-0.3.0/README.md
+-rw-r--r--   0        0        0     3514 2023-05-12 17:03:10.434827 thalassa-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-02 09:50:57.249458 thalassa-0.3.0/thalassa/__init__.py
+-rw-r--r--   0        0        0    11314 2023-05-08 05:42:04.878122 thalassa-0.3.0/thalassa/api.py
+-rw-r--r--   0        0        0     5510 2023-05-12 14:20:53.774892 thalassa-0.3.0/thalassa/normalization.py
+-rw-r--r--   0        0        0     9438 2023-05-12 14:20:53.768225 thalassa-0.3.0/thalassa/utils.py
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 thalassa-0.3.0/PKG-INFO
```

### Comparing `thalassa-0.2.0/LICENSE` & `thalassa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thalassa-0.2.0/pyproject.toml` & `thalassa-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tool.poetry]
 name = "thalassa"
-version = "0.2.0"  # overwritten by poetry-dynamic-versioning plugin
-description = ""
+version = "0.3.0"  # overwritten by poetry-dynamic-versioning plugin
+description = "A library for visualizing large scale results of hydrodynamic simulations"
 authors = ["Panos Mavrogiorgos <pmav99@gmail.com>"]
-license = 'EUPL v1.2'
+license = 'EUPL-1.2'
 readme = "README.md"
 repository = "https://github.com/ec-jrc/thalassa.git"
 classifiers = [
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Environment :: Other Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Visualization",
@@ -22,33 +21,26 @@
     # Datashader 0.14.4 is not compatible with python 3.11
     # As soon as a new release is made, we should be able to switch back support for 3.11
     # "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-bokeh = "*"
 Cartopy = "*"
 datashader = "*"
 geopandas = "*"
 geoviews = "*"
 holoviews = "*"
-hvplot = "*"
-llvmlite = "*"
-netCDF4 = "*"
 # datashader has fixed the incompatibilities with numpy, but they haven't released a new package
-# As soon as datashader 1.4.5 gets released we should be able to remove the pin
+# As soon as datashader 0.14.5 gets released we should be able to remove the pin
 # https://github.com/holoviz/datashader/issues/1158
 numpy = "<1.24"
 pandas = "*"
 panel = "*"
-"ruamel.yaml" = "*"
-scipy = "*"
 shapely = "*"
-tornado = "*"
 xarray = {version = "*", extras = ["io", "accel"]}
 
 [tool.poetry.group.dev.dependencies]
 covdefaults = "*"
 mypy = ">=1"
 pytest = "*"
 pytest-cov = ">=3.0"
@@ -128,15 +120,15 @@
     "D103",  # undocumented-public-function
     "PD901",  # pandas-df-variable-name
 ]
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["thalassa"]
-omit = ["thalassa/ui.py"]
+omit = []
 concurrency = [
   "multiprocessing",
   "thread",
 ]
 parallel = true
 sigterm = true
```

### Comparing `thalassa-0.2.0/thalassa/api.py` & `thalassa-0.3.0/thalassa/api.py`

 * *Files identical despite different names*

### Comparing `thalassa-0.2.0/thalassa/normalization.py` & `thalassa-0.3.0/thalassa/normalization.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     "triface_nodes",
 }
 _SCHISM_DIMS = {
     "time",
     "nSCHISM_hgrid_edge",
     "nSCHISM_hgrid_face",
     "nSCHISM_hgrid_node",
-    "nSCHISM_vgrid_layers",
     "nMaxSCHISM_hgrid_face_nodes",
 }
 _SCHISM_VARS = {
     "SCHISM_hgrid_node_x",
     "SCHISM_hgrid_node_y",
     "SCHISM_hgrid_face_nodes",
 }
@@ -68,26 +67,26 @@
 _ADCIRC_VARS = {
     "adcirc_mesh",
     "depth",
     "element",
     "ibtype",
     "nbvv",
     "nvell",
-    "zeta",
 }
 # fmt: on
 
 
 def is_generic(ds: xr.Dataset) -> bool:
     total_vars = list(ds.data_vars.keys()) + list(ds.coords.keys())
     return _GENERIC_DIMS.issubset(ds.dims) and _GENERIC_VARS.issubset(total_vars)
 
 
 def is_schism(ds: xr.Dataset) -> bool:
-    return _SCHISM_DIMS.issubset(ds.dims) and _SCHISM_VARS.issubset(ds.data_vars)
+    total_vars = list(ds.data_vars.keys()) + list(ds.coords.keys())
+    return _SCHISM_DIMS.issubset(ds.dims) and _SCHISM_VARS.issubset(total_vars)
 
 
 def is_pyposeidon(ds: xr.Dataset) -> bool:
     return _PYPOSEIDON_DIMS.issubset(ds.dims) and _PYPOSEIDON_VARS.issubset(ds.data_vars)
 
 
 def is_adcirc(ds: xr.Dataset) -> bool:
@@ -129,21 +128,27 @@
 
 def normalize_schism(ds: xr.Dataset) -> xr.Dataset:
     ds = ds.rename(
         {
             "nSCHISM_hgrid_edge": "edge",
             "nSCHISM_hgrid_face": "face",
             "nSCHISM_hgrid_node": "node",
-            "nSCHISM_vgrid_layers": "layer",
             "SCHISM_hgrid_face_nodes": "face_nodes",
             "nMaxSCHISM_hgrid_face_nodes": "max_no_vertices",
             "SCHISM_hgrid_node_x": "lon",
             "SCHISM_hgrid_node_y": "lat",
         },
     )
+    if "nSCHISM_vgrid_layers" in ds.dims:
+        # I.e. OLD Schism IO or "merged" new IO
+        ds = ds.rename(
+            {
+                "nSCHISM_vgrid_layers": "layer",
+            },
+        )
     # SCHISM output uses one-based indices for `face_nodes`
     # Let's ensure that we use zero-based indices everywhere.
     ds["face_nodes"] -= 1
     return ds
 
 
 def normalize_pyposeidon(ds: xr.Dataset) -> xr.Dataset:
```

### Comparing `thalassa-0.2.0/thalassa/utils.py` & `thalassa-0.3.0/thalassa/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,18 @@
 import geoviews as gv
 import holoviews as hv
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import shapely
 import xarray as xr
-from ruamel.yaml import YAML
-
-yaml = YAML(typ="safe", pure=True)
 
 logger = logging.getLogger(__name__)
 
 
-def setup_logging() -> None:
-    with open("config.yml", "rb") as fd:
-        config = yaml.load(fd.read())
-
-    logging.config.dictConfig(config["logging"])
-    logger.debug(logging.getLogger("thalassa").handlers)
-
-
 def generate_thalassa_ds(
     nodes: npt.NDArray[np.int_],
     triface_nodes: npt.NDArray[np.int_],
     lons: npt.NDArray[np.float_] | None = None,
     lats: npt.NDArray[np.float_] | None = None,
     time_range: pd.DateTimeIndex | None = None,
     **kwargs: dict[str, tuple[tuple[str], npt.NDArray[np.float_]]],
```

### Comparing `thalassa-0.2.0/PKG-INFO` & `thalassa-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,119 @@
 Metadata-Version: 2.1
 Name: thalassa
-Version: 0.2.0
-Summary: 
+Version: 0.3.0
+Summary: A library for visualizing large scale results of hydrodynamic simulations
 Home-page: https://github.com/ec-jrc/thalassa.git
-License: EUPL v1.2
+License: EUPL-1.2
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: Cartopy
-Requires-Dist: bokeh
 Requires-Dist: datashader
 Requires-Dist: geopandas
 Requires-Dist: geoviews
 Requires-Dist: holoviews
-Requires-Dist: hvplot
-Requires-Dist: llvmlite
-Requires-Dist: netCDF4
 Requires-Dist: numpy (<1.24)
 Requires-Dist: pandas
 Requires-Dist: panel
-Requires-Dist: ruamel.yaml
-Requires-Dist: scipy
 Requires-Dist: shapely
-Requires-Dist: tornado
 Requires-Dist: xarray[accel,io]
 Project-URL: Repository, https://github.com/ec-jrc/thalassa.git
 Description-Content-Type: text/markdown
 
-Large Scale Sea level visualizations of unstructured mesh data
-===============================================================
+Thalassa
+========
 
-Thalassa is a library/application for visualizing large scale results of hydrodynamic simulations.
+Thalassa ia a library for visualizing unstructured mesh data.
 
+It builds upon [geoviews](https://geoviews.org/) and [datashader](https://datashader.org/)
+and can easily handle meshes with millions of nodes interactively.
 
+<!-- https://user-images.githubusercontent.com/411196/146007390-88e8cc59-9ae9-4a15-83fd-f7f1f2d724c2.mp4 -->
 
-https://user-images.githubusercontent.com/411196/146007390-88e8cc59-9ae9-4a15-83fd-f7f1f2d724c2.mp4
+Thalassa is currently supporting visualization of the output of the following solvers:
 
+- [Schism](https://github.com/schism-dev/schism)
+- [ADCIRC](https://adcirc.org/)
 
+Adding support for new solvers is relatively straight-forward.
 
-## Obtaining Data
-
-You will need some data to visualize. If you don't have any you can download a sample dataset
-created with [pyposeidon](https://github.com/ec-jrc/pyPoseidon/):
-
-```
-mkdir ./data
-wget -O data/dataset.nc https://static.techrad.eu/thalassa/dataset.nc
-```
+## Installation
 
-## Deploying on a server
+### PyPI
 
 1. Install the binary dependencies:
 
-- `python 3.9`
-- `proj < 8`
+- `python >= 3.9`
+- `geos`
 
-2. Install the python dependencies with
+2. Install from PyPI with:
 
 ```
-pip install -r requirements/requirements.txt
+pip install thalassa
 ```
 
-3. Run the panel server with:
+### Conda
 
+You can also install using conda/mamba:
+
+```bash
+mamba install -y -c conda-forge thalassa
 ```
-panel serve ./run.py
-```
 
-For the record, `panel serve` is a thin wrapper around the [bokeh
-server](https://docs.bokeh.org/en/latest/docs/user_guide/server.html#).  It provides lots of
-command line options which can useful in various deployments scenarios.  Of particular interest
-might be `--num-procs` which spawns multiple workers and `--allow-websocket-origin`. Make sure to
-check the docs:
+## Obtaining Data
+
+You will need some data to visualize. You can download sample datasets from the following links:
 
-- https://panel.holoviz.org/user_guide/Deploy_and_Export.html#launching-a-server-on-the-commandline
-- https://docs.bokeh.org/en/latest/docs/user_guide/server.html#basic-reverse-proxy-setup
-- `panel serve --help`
+- 2D Output from the [STOFS-2D Global]() model which uses ADCIRC from [here](https://noaa-gestofs-pds.s3.amazonaws.com/stofs_2d_glo.20230501/stofs_2d_glo.t00z.fields.cwl.nc) (12GB)
+- 3D Output from the [STOFS-3D Atlantic](https://noaa-nos-stofs3d-pds.s3.amazonaws.com/README.html) model which uses Schism 5.9 (old IO) from [here](https://noaa-nos-stofs3d-pds.s3.amazonaws.com/STOFS-3D-Atl-shadow-VIMS/20220430/schout_20220501.nc) (12GB)
+- 2D Output from the [STOFS-3D Atlantic](https://noaa-nos-stofs3d-pds.s3.amazonaws.com/README.html) model which uses Schism 5.10 (new IO) from [here](https://noaa-nos-stofs3d-pds.s3.amazonaws.com/STOFS-3D-Atl/stofs_3d_atl.20230501/stofs_3d_atl.t12z.fields.out2d_nowcast.nc) (3GB)
+
+## Thalassa-server
+
+[thalassa-server](https://github.com/oceanmodeling/thalassa-server) is an web-application leveraging the `thalassa` library
+and [panel](https://panel.holoviz.org/). Check-it out!
 
 ## Developing
 
 ### Prerequisites
 
-For managing dependencies we use poetry.
+For developing we are using [poetry](https://pre-commit.com/) and [pre-commit](https://pre-commit.com/).
+You can install both with [pipx](https://github.com/pypa/pipx):
 
 ```
+# poetry
 pipx install poetry
+pipx inject poetry poetry-dynamic-versioning
+pipx inject poetry poetry-plugin-export
+# pre-commit
+pipx install pre-commit
 ```
 
 ### Install dependencies
 
 Just run:
 
 ```
-poetry install
+make init
 ```
 
-and please make sure to also install the [pre-commit](https://pre-commit.com/) hooks:
-
-```
-pre-commit install
-```
-
-### Running Thalassa
-
-#### As a web application
-
-It should be as simple as:
-
-```
-panel serve ./run.py --autoreload
-```
-
-#### Inside jupyterlab
-
-Open the `Thalassa.ipynb` in jupyterlab
-
 ## License
 
-The project is released under the EUPL v1.2 license.
+The project is released under the EUPL v1.2 license which is compatible with GPL v3
```

