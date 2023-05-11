# Comparing `tmp/keypoint-moseq-0.1.0.tar.gz` & `tmp/keypoint-moseq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.1.0.tar", last modified: Thu May  4 15:20:07 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.1.1.tar", last modified: Thu May 11 22:14:11 2023, max compression
```

## Comparing `keypoint-moseq-0.1.0.tar` & `keypoint-moseq-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:20:07.196150 keypoint-moseq-0.1.0/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.0/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.0/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-04 15:20:07.196308 keypoint-moseq-0.1.0/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1613 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:20:07.197762 keypoint-moseq-0.1.0/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      878 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-04 15:20:07.197863 keypoint-moseq-0.1.0/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-21 10:40:06.000000 keypoint-moseq-0.1.0/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17369 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    32958 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    27288 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    67128 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-04 15:20:07.195621 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      143 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-04 15:20:07.000000 keypoint-moseq-0.1.0/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      723 2023-05-04 15:20:07.197316 keypoint-moseq-0.1.0/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.0/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-11 22:14:11.779245 keypoint-moseq-0.1.1/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.1/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.1/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-11 22:14:11.779396 keypoint-moseq-0.1.1/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-11 19:57:02.000000 keypoint-moseq-0.1.1/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-11 22:14:11.780825 keypoint-moseq-0.1.1/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.1/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-11 22:14:11.780952 keypoint-moseq-0.1.1/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.1/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.1/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17318 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.1/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    41843 2023-05-11 21:25:41.000000 keypoint-moseq-0.1.1/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    27401 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.1/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    68316 2023-05-11 21:54:06.000000 keypoint-moseq-0.1.1/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-11 22:14:11.778779 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      152 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      733 2023-05-11 22:14:11.780345 keypoint-moseq-0.1.1/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.1/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.1/versioneer.py
```

### Comparing `keypoint-moseq-0.1.0/LICENSE.md` & `keypoint-moseq-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.0/NOTICE.md` & `keypoint-moseq-0.1.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.0/keypoint_moseq/analysis.py` & `keypoint-moseq-0.1.1/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.0/keypoint_moseq/calibration.py` & `keypoint-moseq-0.1.1/keypoint_moseq/calibration.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.0/keypoint_moseq/fitting.py` & `keypoint-moseq-0.1.1/keypoint_moseq/fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import joblib
 import os
 import numpy as np
 import tqdm
 import jax
 import warnings
-warnings.formatwarning = lambda msg, *a: str(msg)
 from textwrap import fill
 from datetime import datetime
 
 from keypoint_moseq.viz import plot_progress
 from keypoint_moseq.io import save_checkpoint, format_data, save_hdf5
 from keypoint_moseq.util import get_durations, get_frequencies, pad_along_axis, reindex_by_frequency
 from jax_moseq.models.keypoint_slds import estimate_coordinates, resample_model, init_model
@@ -209,15 +208,14 @@
     model = init_model(data, states, params, hypparams,
                        noise_prior, seed, **kwargs)
 
     return fit_model(model, data, labels, start_iter=iteration+1, 
                      num_iters=num_iters, **kwargs)
 
 
-
 def extract_results(*, params, states, labels, save_results=True, 
                     project_dir=None, name=None, results_path=None, 
                     **kwargs): 
     """
     Extract model outputs and [optionally] save them to disk.
 
     Model outputs are saved to disk as a .h5 file, either at `results_path`
```

### Comparing `keypoint-moseq-0.1.0/keypoint_moseq/io.py` & `keypoint-moseq-0.1.1/keypoint_moseq/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 import os
 import cv2
 import re
 import pandas as pd
 from datetime import datetime
 from textwrap import fill
 from vidio.read import OpenCVReader
-warnings.formatwarning = lambda msg, *a: str(msg)
+import matplotlib.pyplot as plt
+import tabulate
+
 
 from jax_moseq.utils import batch
 from keypoint_moseq.util import (
     reindex_by_bodyparts, 
     list_files_with_exts, 
     interpolate_keypoints,
 )
@@ -301,20 +303,20 @@
             
             if dlc_config is None:
                 raise RuntimeError(
                     f'{deeplabcut_config} does not exists or is not a'
                     ' valid yaml file')
                 
             if 'multianimalproject' in dlc_config and dlc_config['multianimalproject']:
-                raise NotImplementedError(
-                    'Config initialization from multi-animal deeplabcut'
-                    ' projects is not yet supported')
-                
-            dlc_options['bodyparts'] = dlc_config['bodyparts']
-            dlc_options['use_bodyparts'] = dlc_config['bodyparts']
+                dlc_options['bodyparts'] = dlc_config['multianimalbodyparts']
+                dlc_options['use_bodyparts'] = dlc_config['multianimalbodyparts']
+            else:
+                dlc_options['bodyparts'] = dlc_config['bodyparts']
+                dlc_options['use_bodyparts'] = dlc_config['bodyparts']
+
             dlc_options['skeleton'] = dlc_config['skeleton']
             dlc_options['video_dir'] = os.path.join(dlc_config['project_path'],'videos')
 
         options = {**dlc_options, **options}
 
     elif sleap_file is not None:
         sleap_options = {}
@@ -364,31 +366,30 @@
     confidences: dict, default=None
         Nonnegative confidence values for the keypoints in 
         `coordinates` as numpy arrays of shape (T,K).
         
     keys: list of str, default=None
         (See :py:func:`keypoint_moseq.util.batch`)
         
-    seg_length: int default=None
-        (See :py:func:`keypoint_moseq.util.batch`)
-        
     bodyparts: list, default=None
         Label for each keypoint represented in `coordinates`. Required
         to reindex coordinates and confidences according to `use_bodyparts`.
 
     use_bodyparts: list, default=None
         Ordered subset of keypoint labels to be used for modeling.
         If `use_bodyparts=None`, then all keypoints are used.
 
     conf_pseudocount: float, default=1e-3
         Pseudocount used to augment keypoint confidences.
     
     seg_length: int, default=None
         Length of each segment. If `seg_length=None`, a length is 
         chosen so that no time-series are broken into multiple segments.
+        If all time-series are shorter than `seg_length`, then
+        `seg_length` is set to the length of the shortest time-series.
         
     Returns
     -------
     data: dict with the following items
     
         Y: jax array with shape (n_segs, seg_length, K, D)
             Keypoint coordinates from all sessions broken into 
@@ -405,14 +406,31 @@
             
     labels: list of tuples (object, int, int)
         Label for each row of `Y` and `conf` 
         (see :py:func:`keypoint_moseq.util.batch`).
     """    
     if keys is None: 
         keys = sorted(coordinates.keys()) 
+    else: 
+        bad_keys = set(keys) - set(coordinates.keys())
+        assert len(bad_keys) == 0, fill(
+            f'Keys {bad_keys} not found in coordinates')
+
+    assert len(keys) > 0, 'No sessions found'
+
+    num_keypoints = [coordinates[key].shape[-2] for key in keys]
+    assert len(set(num_keypoints)) == 1, fill(
+        f'All sessions must have the same number of keypoints, but '
+        f'found {set(num_keypoints)} keypoints across sessions.')
+    
+    if bodyparts is not None:
+        assert len(bodyparts) == num_keypoints[0], fill(
+            f'The number of keypoints in `coordinates` ({num_keypoints[0]}) '
+            f'does not match the number of labels in `bodyparts` '
+            f'({len(bodyparts)})')
 
     if any(['/' in key for key in keys]): 
         warnings.warn(fill(
             'WARNING: Session names should not contain "/", this will cause '
             'problems with saving/loading hdf5 files.'))
         
     if confidences is None:
@@ -422,14 +440,18 @@
         coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
         confidences = reindex_by_bodyparts(confidences, bodyparts, use_bodyparts)
 
     for key in keys:
         outliers = np.isnan(coordinates[key]).any(-1)
         coordinates[key] = interpolate_keypoints(coordinates[key], outliers)
         confidences[key] = np.where(outliers, 0, np.nan_to_num(confidences[key]))
+    
+    if seg_length is not None:
+        max_session_length = max([coordinates[key].shape[0] for key in keys])
+        seg_length = min(seg_length, max_session_length)
 
     Y,mask,labels = batch(coordinates, seg_length=seg_length, keys=keys)
     Y = Y.astype(float)
 
     conf = batch(confidences, seg_length=seg_length, keys=keys)[0]
     if np.min(conf) < 0: 
         conf = np.maximum(conf,0) 
@@ -657,34 +679,207 @@
     if path is None: 
         assert project_dir is not None and name is not None, fill(
             '`name` and `project_dir` are required if no `path` is given.')
         path = os.path.join(project_dir,name,'results.h5')
     return load_hdf5(path)
 
 
+def save_results_as_csv(project_dir=None, name=None, h5_path=None, 
+                        save_dir=None, use_bodyparts=None,
+                        path_sep='-', **kwargs):
+    """
+    Convert modeling results from h5 to csv format.
+
+    The input h5 file is assumed to contain modeling outputs for one
+    or more recordings. This function creates a directory and then
+    saves a separate csv file for each.
+
+    The path to the input h5 file can be specified directly via
+    `results_path`. Otherwise it is assumed to be
+    `{project_dir}/{name}/results.h5`. The path to the output
+    directory can be specified directly via `save_dir`. Otherwise
+    it will be set to `{project_dir}/{name}/results`. Any files
+    already in the output directory will be overwritten.
+    
+    Parameters
+    ----------
+    project_dir: str, default=None
+        Project directory; required if `h5_path` or `save_dir` is not provided.
+
+    name: str, default=None
+        Name of the model; required if `h5_path` or `save_dir` is not provided.
+
+    h5_path: str, default=None
+        Path to the h5 file containing modeling results.
+
+    save_dir: str, default=None
+        Path to the directory where the csv files will be saved.
+
+    use_bodyparts: list, default=None
+        List of bodyparts that were used for modeling. If provided,
+        will be used for the csv column names corresponding to 
+        `estimated_coordinates`. Otherwise, the bodyparts will be
+        named `bodypart0`, `bodypart1` etc.
+
+    path_sep: str, default='-'
+        If a path separator ("/" or "\") is present in the recording name, 
+        it will be replaced with `path_sep` when saving the csv file.
+    """
+
+    if h5_path is None:
+        assert project_dir is not None and name is not None, fill(
+            'Provide either a `h5_path` or a `project_dir` and `name`')
+        h5_path = os.path.join(project_dir, name, 'results.h5')
+
+    if save_dir is None:
+        assert project_dir is not None and name is not None, fill(
+            'Provide either a `save_dir` or a `project_dir` and `name`')
+        save_dir = os.path.join(project_dir, name, 'results')
+
+    if not os.path.exists(save_dir): 
+        os.makedirs(save_dir)
+
+    with h5py.File(h5_path, 'r') as results:
+        for key in tqdm.tqdm(results.keys(), desc='Saving to csv'):
+            column_names, data = [], []
+
+            if 'syllables_reindexed' in results[key].keys():
+                column_names.append(['syllables reindexed'])
+                data.append(results[key]['syllables_reindexed'][()].reshape(-1,1))
+
+            if 'syllables' in results[key].keys():
+                column_names.append(['syllables non-reindexed'])
+                data.append(results[key]['syllables'][()].reshape(-1,1))
+
+            if 'centroid' in results[key].keys():
+                d = results[key]['centroid'].shape[1]
+                column_names.append(['centroid x', 'centroid y', 'centroid z'][:d])
+                data.append(results[key]['centroid'][()])
+
+            if 'heading' in results[key].keys():
+                column_names.append(['heading'])
+                data.append(results[key]['heading'][()].reshape(-1,1))
+
+            if 'estimated_coordinates' in results[key].keys():
+                k,d = results[key]['estimated_coordinates'].shape[1:]
+                if use_bodyparts is None:
+                    use_bodyparts = [f'bodypart{i}' for i in range(k)]
+                for i, bp in enumerate(use_bodyparts):
+                    column_names.append([f'estimated {bp} x', f'estimated {bp} y', f'{bp} z'][:d])
+                    data.append(results[key]['estimated_coordinates'][:,i,:])
+
+            if 'latent_state' in results[key].keys():
+                latent_dim = results[key]['latent_state'].shape[1]
+                column_names.append([f'latent_state {i}' for i in range(latent_dim)])
+                data.append(results[key]['latent_state'][()])
+
+            dfs = [pd.DataFrame(arr, columns=cols) for arr,cols in zip(data,column_names)]
+            df = pd.concat(dfs, axis=1)
+
+            for col in df.select_dtypes(include=[np.floating]).columns:
+                df[col] = df[col].astype(float).round(4)
+
+            save_name = key.replace(os.path.sep, path_sep)
+            save_path = os.path.join(save_dir, save_name)
+            df.to_csv(f'{save_path}.csv', index=False)
+
+
+
+
 def _name_from_path(filepath, path_in_name, path_sep, remove_extension):
     """
     Create a name from a filepath. Either return the name of the file
     (with the extension removed) or return the full filepath, where the
     path separators are replaced with `path_sep`.
     """
     if remove_extension:
         filepath = os.path.splitext(filepath)[0]
     if path_in_name:
         return filepath.replace(os.path.sep, path_sep)
     else:
         return os.path.basename(filepath)
 
 
+def _print_colored_table(row_labels, col_labels, values):
+    try:
+        from IPython.display import display
+        display_available = True
+    except ImportError:
+        display_available = False
+
+    title = 'Proportion of NaNs'
+    df = pd.DataFrame(values, index=row_labels, columns=col_labels)
+    
+    if display_available:
+        def colorize(val):
+            color = plt.get_cmap("Reds")(val*0.8)
+            return f'background-color: rgba({int(color[0]*255)}, {int(color[1]*255)}, {int(color[2]*255)}, {color[3]})'  
+        colored_df = df.style.applymap(colorize).set_caption('Proportion of NaNs')
+        display(colored_df)
+        return colored_df
+    else:
+        print(title)
+        print(tabulate(df, headers='keys', tablefmt="simple_grid", showindex=True))
+
+
+def check_nan_proportions(coordinates, bodyparts, 
+                          warning_threshold=0.5,
+                          breakdown=False, **kwargs):
+    """
+    Check if any bodyparts have a high proportion of NaNs.
+    
+    Parameters
+    ----------
+    coordinates: dict
+        Dictionary mapping filenames to keypoint coordinates as ndarrays
+        of shape (n_frames, n_bodyparts, 2)
+
+    bodyparts: list of str
+        Name of each bodypart. The order of the names should match the
+        order of the bodyparts in `coordinates`.
+
+    warning_threshold: float, default=0.5
+        If the proportion of NaNs for a bodypart is greater than
+        `warning_threshold`, then a warning is printed.
+        
+    breakdown: bool, default=False
+        Whether to print a table detailing the proportion of NaNs
+        for each bodyparts in each array of `coordinates`.
+    """
+    if breakdown:
+        keys = sorted(coordinates.keys())
+        nan_props = [np.isnan(coordinates[k]).any(-1).mean(0) for k in keys]
+        _print_colored_table(keys, bodyparts, nan_props)
+    else:
+        all_coords = np.concatenate(list(coordinates.values()))
+        nan_props = np.isnan(all_coords).any(-1).mean(0)
+        if np.any(nan_props > warning_threshold):
+            bps = [bp for bp,p in zip(bodyparts,nan_props) if p > warning_threshold]
+            warnings.warn(
+                 '\nCoordinates for the following bodyparts are missing (set to NaN) in at least '
+                 '{}% of frames:\n - {}\n\n'.format(warning_threshold*100, '\n - '.join(bps)))
+            warnings.warn(
+                'This may cause problems during modeling. See '
+                'https://keypoint-moseq.readthedocs.io/en/latest/FAQs.html#high-proportion-of-nans'
+                ' for additional information.')
+
+
+
 def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
-                            path_in_name=False, remove_extension=True, 
-                            return_bodyparts=False):
+                            path_in_name=False, remove_extension=True):
     """
     Load tracking results from deeplabcut csv or hdf5 files.
 
+    For single-animal tracking, each file yields a single key/value 
+    pair in the returned `coordinates` and `confidences` dictionaries. For
+    multi-animal tracking, a key/vaue pair will be generated for each
+    tracked individual. For example a single file called `two_mice.h5`
+    with individuals "mouseA" and "mouseB" will yield the pair of
+    keys `'two_mice_mouseA', 'two_mice_mouseB'`. 
+
     Parameters
     ----------
     filepath_pattern: str or list of str
         Filepath pattern for a set of deeplabcut csv or hdf5 files, 
         or a list of such patterns. Filepath patterns can be:
 
             - single file (e.g. `/path/to/file.csv`) 
@@ -707,63 +902,74 @@
         `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
     remove_extension: bool, default=True
         Whether to remove the file extension from the name of the tracking
         results.
 
-    return_bodyparts: bool, default=False
-        Whether to return a list of bodypart names.
-
     Returns
     -------
     coordinates: dict
         Dictionary mapping filenames to keypoint coordinates as ndarrays
         of shape (n_frames, n_bodyparts, 2)
 
     confidences: dict
         Dictionary mapping filenames to `likelihood` scores as ndarrays
         of shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
-        List of bodypart names. Only returned if `return_bodyparts` is True.
+        List of bodypart names. The order of the names matches the order
+        of the bodyparts in `coordinates` and `confidences`.
     """
     filepaths = list_files_with_exts(
         filepath_pattern, ['.csv','.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No deeplabcut csv or hdf5 files found for {filepath_pattern}')
 
     coordinates,confidences = {},{}
     for filepath in tqdm.tqdm(filepaths, desc='Loading from deeplabcut'):
-        try: 
-            ext = os.path.splitext(filepath)[1]
-            if ext=='.h5': df = pd.read_hdf(filepath)
-            if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
 
-            bodyparts = list(list(zip(*df.columns.to_list()))[1][::3])      
+        ext = os.path.splitext(filepath)[1]
+        if ext=='.h5': df = pd.read_hdf(filepath)
+        if ext=='.csv': df = pd.read_csv(filepath, header=[0,1,2], index_col=0) 
+        
+        name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
+        bodyparts = df.columns.get_level_values('bodyparts').unique().tolist()   
+        
+        if 'individuals' in df.columns.names:
+            for ind in df.columns.get_level_values('individuals').unique():
+                ind_df = df.xs(ind, axis=1, level='individuals')
+                arr = ind_df.to_numpy().reshape(len(ind_df), -1, 3)
+                coordinates[f'{name}_{ind}'] = arr[:,:,:-1]
+                confidences[f'{name}_{ind}'] = arr[:,:,-1]
+        else:
             arr = df.to_numpy().reshape(len(df), -1, 3)
-
-            name = _name_from_path(filepath, path_in_name, path_sep, remove_extension)
             coordinates[name] = arr[:,:,:-1]
             confidences[name] = arr[:,:,-1]
 
-        except Exception as e: 
-            print(fill(f'Error loading {filepath}: {e}'))
+        # except Exception as e: 
+        #     print(fill(f'Error loading {filepath}: {e}'))
     
-    if return_bodyparts: 
-        return coordinates,confidences,bodyparts
-    else: return coordinates,confidences
+    if len(coordinates) > 0:
+        check_nan_proportions(coordinates, bodyparts)
+
+    return coordinates,confidences,bodyparts
 
 
 
 def load_sleap_results(filepath_pattern, recursive=True, path_sep='-',
-                       path_in_name=False, return_bodyparts=False,
-                       remove_extension=True):
+                       path_in_name=False, remove_extension=True):
     """
-    Load keypoints from sleap hdf5 files.
+    Load keypoints from sleap hdf5 files. 
+
+    For single-animal tracking, each file yields a single key/value 
+    pair in the returned `coordinates` and `confidences` dictionaries. For
+    multi-animal tracking, a key/vaue pair will be generated for each track.
+    For example a single file called `two_mice.h5` will yield the pair of
+    keys `'two_mice_track0', 'two_mice_track1'`.
 
     Parameters
     ----------
     filepath_pattern: str, default=None
         Filepath pattern for a set of sleap hdf5 files, or a list of 
         such patterns. Filepath patterns can be:
 
@@ -786,30 +992,28 @@
         file `/path/to/file.csv` will be named `path-to-file`. Using
         `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
     remove_extension: bool, default=True
         Whether to remove the file extension from the name of the tracking
         results.
-    
-    return_bodyparts: bool, default=False
-        Whether to return a list of bodypart names.
 
     Returns
     -------
     coordinates: dict
         Dictionary mapping filenames to keypoint coordinates as ndarrays
         of shape (n_frames, n_bodyparts, 2)
 
     confidences: dict
         Dictionary mapping filenames to `likelihood` scores as ndarrays
         of shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
-        List of bodypart names. Only returned if `return_bodyparts` is True.
+        List of bodypart names. The order of the names matches the order
+        of the bodyparts in `coordinates` and `confidences`.
     """
     filepaths = list_files_with_exts(
         filepath_pattern, ['.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No sleap hdf5 files found for {filepath_pattern}.')
 
     coordinates,confidences = {},{}
@@ -826,17 +1030,18 @@
                 else:
                     for i in range(coords.shape[0]):
                         coordinates[f'{name}_track{i}'] = coords[i].T
                         confidences[f'{name}_track{i}'] = confs[i].T
         except Exception as e: 
             print(fill(f'Error loading {filepath}: {e}'))
 
-    if return_bodyparts: 
-        return coordinates,confidences,bodyparts
-    else: return coordinates,confidences
+    if len(coordinates) > 0:
+        check_nan_proportions(coordinates, bodyparts)
+
+    return coordinates,confidences,bodyparts
 
 # hdf5 save/load routines modified from
 # https://gist.github.com/nirum/b119bbbd32d22facee3071210e08ecdf
 
 def save_hdf5(filepath, save_dict):
     """
     Save a dict of pytrees to an hdf5 file.
```

### Comparing `keypoint-moseq-0.1.0/keypoint_moseq/util.py` & `keypoint-moseq-0.1.1/keypoint_moseq/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import os
 import glob
 import tqdm
+import warnings
 from textwrap import fill
 import jax, jax.numpy as jnp, jax.random as jr
 from jax.tree_util import tree_map
 from itertools import groupby
 from functools import partial
 from scipy.ndimage import median_filter, convolve1d
 from sklearn.decomposition import PCA
@@ -687,14 +688,15 @@
     -------
     x_interp: ndarray
         The interpolated values, with the same shape as fp except
         along the interpolation axis.
     """
     assert len(xp.shape)==len(x.shape)==1
     assert fp.shape[axis]==len(xp)
+    assert len(xp)>0, 'xp must be non-empty; cannot interpolate without datapoints'
     
     fp = np.moveaxis(fp, axis, 0)
     shape = fp.shape[1:]
     fp = fp.reshape(fp.shape[0],-1)
 
     x_interp = np.zeros((len(x),fp.shape[1]))
     for i in range(fp.shape[1]):
@@ -718,18 +720,18 @@
     Returns
     -------
     interpolated_coordinates : ndarray with same shape as `coordinates`
         Keypoint observations with outliers imputed.
     """  
     interpolated_coordinates = np.zeros_like(coordinates)
     for i in range(coordinates.shape[1]):
-        interpolated_coordinates[:,i,:] = interpolate_along_axis(
-            np.arange(coordinates.shape[0]),
-            np.nonzero(~outliers[:,i])[0],
-            coordinates[~outliers[:,i],i,:])
+        xp = np.nonzero(~outliers[:,i])[0]
+        if len(xp) > 0: 
+            interpolated_coordinates[:,i,:] = interpolate_along_axis(
+                np.arange(coordinates.shape[0]), xp, coordinates[xp,i,:])
     return interpolated_coordinates
 
 
 
 def filtered_derivative(Y_flat, ksize, axis=0):
     """
     Compute the filtered derivative of a signal along a given axis.
```

### Comparing `keypoint-moseq-0.1.0/keypoint_moseq/viz.py` & `keypoint-moseq-0.1.1/keypoint_moseq/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     find_matching_videos, get_syllable_instances, sample_instances,
     filter_centroids_headings, get_trajectories, interpolate_keypoints,
     interpolate_along_axis
 )
 from keypoint_moseq.io import load_results
 from jax_moseq.models.keypoint_slds import center_embedding
 
-# simple warning formatting
-warnings.formatwarning = lambda msg, *a: str(msg)
 
 # suppress warnings from imageio
 logging.getLogger().setLevel(logging.ERROR)
 
 
 def crop_image(image, centroid, crop_size):
     """
@@ -63,16 +61,15 @@
     padded = np.zeros((h,w,*image.shape[2:]), dtype=image.dtype)
     pad_x = (w - cropped.shape[1]) // 2
     pad_y = (h - cropped.shape[0]) // 2
     padded[pad_y:pad_y+cropped.shape[0], pad_x:pad_x+cropped.shape[1]] = cropped
     return padded
 
 
-def plot_scree(pca, savefig=True, project_dir=None, fig_size=(3,2),
-              ):
+def plot_scree(pca, savefig=True, project_dir=None, fig_size=(3,2)):
     """
     Plot explained variance as a function of the number of PCs.
 
     Parameters
     ----------
     pca : :py:func:`sklearn.decomposition.PCA`
         Fitted PCA model
@@ -89,15 +86,16 @@
 
     Returns 
     -------
     fig : :py:class:`matplotlib.figure.Figure`
         Figure handle
     """
     fig = plt.figure()
-    plt.plot(np.arange(len(pca.mean_))+1,np.cumsum(pca.explained_variance_ratio_))
+    num_pcs = len(pca.components_)
+    plt.plot(np.arange(num_pcs)+1,np.cumsum(pca.explained_variance_ratio_))
     plt.xlabel('PCs')
     plt.ylabel('Explained variance')
     plt.gcf().set_size_inches(fig_size)
     plt.grid()
     plt.tight_layout()
     
     if savefig:
@@ -169,14 +167,18 @@
     if d==3: dims_list,names = [[0,1],[0,2]],['xy','xz']
     
     magnitude = np.sqrt((pca.mean_**2).mean()) * scale
     for dims,name in zip(dims_list,names):
         nrows = int(np.ceil(plot_n_pcs/ncols))
         fig,axs = plt.subplots(nrows, ncols, sharex=True, sharey=True)
         for i,ax in enumerate(axs.flat):
+            if i >= plot_n_pcs:
+                ax.axis('off')
+                continue
+
             ymean = Gamma @ pca.mean_.reshape(k-1,d)[:,dims]
             y = Gamma @ (pca.mean_ + magnitude*pca.components_[i]).reshape(k-1,d)[:,dims]
             
             for e in edges:  
                 ax.plot(*ymean[e].T, color=cmap(e[0]/(k-1)), 
                         zorder=0, alpha=0.25, linewidth=linewidth)
                 ax.plot(*y[e].T, color='k', 
@@ -346,15 +348,15 @@
     ax.set_yticks([])
     if show_median: ax.axvline(np.median(durations), color='k', linestyle='--')
     return fig, ax
         
 
 def plot_progress(model, data, history, iteration, path=None,
                   project_dir=None, name=None, savefig=True,
-                  fig_size=None, seq_length=600, min_frequency=.001, 
+                  fig_size=None, window_size=600, min_frequency=.001, 
                   min_histogram_length=10, **kwargs):
     """
     Plot the progress of the model during fitting.
 
     The figure shows the following plots:
         - Duration distribution: 
             The distribution of state durations for the most recent
@@ -386,16 +388,16 @@
         Whether to save the figure to a file. If true, the figure is
         either saved to `path` or, to `{project_dir}/{name}-progress.pdf`
         if `path` is None.
 
     fig_size : tuple of float, default=None
         Size of the figure in inches. 
         
-    seq_length : int, default=600
-        Length of the state sequence history plot.
+    window_size : int, default=600
+        Window size for state sequence history plot.
 
     min_frequency : float, default=.001
         Minimum frequency for including a state in the frequency 
         distribution plot.
 
     min_histogram_length : int, default=10
         Minimum x-axis length of the frequency distribution plot.
@@ -452,17 +454,18 @@
         med_durs = [np.median(get_durations(z,mask)) for z in past_stateseqs]
         axs[2].scatter(history_iters,med_durs)
         axs[2].set_ylim([-1,np.max(med_durs)*1.1])
         axs[2].set_xlabel('iteration')
         axs[2].set_ylabel('duration')
         axs[2].set_title('Median duration')
         
-        nz = np.stack(np.array(mask[:,seq_length:]).nonzero(),axis=1)
+        window_size = int(min(window_size,mask.max(0).sum()-1))
+        nz = np.stack(np.array(mask[:,window_size:]).nonzero(),axis=1)
         batch_ix,start = nz[np.random.randint(nz.shape[0])]
-        seq_hist = np.stack([z[batch_ix,start:start+seq_length] for z in past_stateseqs])
+        seq_hist = np.stack([z[batch_ix,start:start+window_size] for z in past_stateseqs])
         axs[3].imshow(seq_hist, cmap=plt.cm.jet, aspect='auto', interpolation='nearest')
         axs[3].set_xlabel('Time (frames)')
         axs[3].set_ylabel('Iterations')
         axs[3].set_title('State sequence history')
         
         yticks = [int(y) for y in axs[3].get_yticks() if y < len(history_iters) and y > 0]
         yticklabels = history_iters[yticks]
@@ -510,39 +513,39 @@
         path, pixelformat='yuv420p', 
         fps=fps, quality=quality) as writer:
         for frame in frames: 
             writer.append_data(frame)
 
 
 def _grid_movie_tile(key, start, end, videos, centroids, headings, 
-                     dot_color=(255,255,255), window_size=112,
-                     pre=30, post=60, dot_radius=4):
-            
-        cs = centroids[key][start-pre:start+post]
-        h,c = headings[key][start],cs[pre]
-        r = np.float32([[np.cos(h), np.sin(h)],[-np.sin(h), np.cos(h)]])
-        c = r @ c - window_size//2
-        M = [[ np.cos(h), np.sin(h),-c[0]], [-np.sin(h), np.cos(h),-c[1]]]
-        
-        tile = []
-        frames = videos[key][start-pre:start+post]
-        for ii,(frame,c) in enumerate(zip(frames,cs)):
-            frame = cv2.warpAffine(frame,np.float32(M),(window_size,window_size))
-            if 0 <= ii-pre <= end-start and dot_radius>0:
-                pos = tuple([int(x) for x in M@np.append(c,1)])
-                cv2.circle(frame, pos, dot_radius, dot_color, -1, cv2.LINE_AA)
-            tile.append(frame)  
-        return np.stack(tile)
+                     dot_color, window_size, scaled_window_size,
+                     pre, post, dot_radius):
+    
+    scale_factor = scaled_window_size/window_size
+    cs = centroids[key][start-pre:start+post]
+    h,c = headings[key][start],cs[pre]
+    r = np.float32([[np.cos(h), np.sin(h)],[-np.sin(h), np.cos(h)]])
+    c = r @ c - window_size//2
+    M = [[ np.cos(h), np.sin(h),-c[0]], [-np.sin(h), np.cos(h),-c[1]]]
+    
+    tile = []
+    frames = videos[key][start-pre:start+post]
+    for ii,(frame,c) in enumerate(zip(frames,cs)):
+        frame = cv2.warpAffine(frame,np.float32(M),(window_size,window_size))
+        frame = cv2.resize(frame, (scaled_window_size,scaled_window_size))
+        if 0 <= ii-pre <= end-start and dot_radius>0:
+            pos = tuple([int(x) for x in M@np.append(c,1)*scale_factor])
+            cv2.circle(frame, pos, dot_radius, dot_color, -1, cv2.LINE_AA)
+        tile.append(frame)  
+    return np.stack(tile)
 
 
-    
 def grid_movie(instances, rows, cols, videos, centroids, headings,
-               dot_color=(255,255,255), dot_radius=4, window_size=112, 
-               pre=30, post=60, coordinates=None, overlay_trajectory=False,
-               plot_options={}, overlay_options={}):
+               window_size, dot_color=(255,255,255), dot_radius=4,
+               pre=30, post=60, scaled_window_size=None):
     
     """Generate a grid movie and return it as an array of frames.
 
     Grid movies show many instances of a syllable. Each instance
     contains a snippet of a video, centered on the animal and synchronized
     to the onset of the syllable. A dot appears at syllable onset and 
     disappears at syllable offset.
@@ -566,87 +569,117 @@
         Dictionary mapping video names to arrays of shape `(n_frames, 2)`
         with the x,y coordinates of animal centroid on each frame
 
     headings: dict
         Dictionary mapping video names to arrays of shape `(n_frames,)`
         with the heading of the animal on each frame (in radians)
 
+    window_size: int
+        Size of the window around the animal. This should be a multiple
+        of 16 or imageio will complain.
+
     dot_color: tuple of ints, default=(255,255,255)
         RGB color of the dot indicating syllable onset and offset
 
     dot_radius: int, default=4
         Radius of the dot indicating syllable onset and offset
 
-    window_size: int, default=112
-        Size of the window around the animal. This should be a multiple
-        of 16 or imageio will complain.
-
     pre: int, default=30
         Number of frames before syllable onset to include in the movie
 
     post: int, default=60
         Number of frames after syllable onset to include in the movie
 
-    coordinates: dict, default=None
-        Dictionary mapping session names to keypoint coordinates as 
-        ndarrays of shape (n_frames, n_bodyparts, 2). Required when
-        `overlay_trajectory=True`
-
-    overlay_trajectory: bool, default=False
-        Whether to overlay trajectory of keypoints on the grid movie. 
-        If True, `coordinates` must be provided.
-
-    overlay_options: dict, default={}
-        Dictionary of options for overlaying trajectory (see
-        :py:func:`keypoint_moseq.viz.overlay_trajectory_on_video`).
-
-    plot_options: dict, default={}
-        Dictionary of options for overlaying trajectory (see 
-        :py:func:`keypoint_moseq.viz.overlay_keypoints_on_image`).
+    scaled_window_size: int, default=None
+        Window size after scaling the video. If None, the no scaling
+        is performed (i.e. `scaled_window_size = window_size`)
 
     Returns
     -------
-    frames: array of shape `(rows, cols, post+pre, window_size, window_size, 3)`
-        Array of frames in the grid movie
-    """
-    if overlay_trajectory:
-        assert coordinates is not None, fill(
-            '`coordinates` must be provided if `overlay_trajectory` is True')
+    frames: array of shape `(post+pre, width, height, 3)`
+        Array of frames in the grid movie where:: 
+
+            width = rows * scaled_window_size
+            height = cols * scaled_window_size
+    """     
+    if scaled_window_size is None:
+        scaled_window_size = window_size
 
-        trajectories = get_trajectories(
-            instances, coordinates, pre=pre, post=post, 
-            centroids=centroids, headings=headings)
-            
     tiles = []
     for i,(key,start,end) in enumerate(instances):
-        tile = _grid_movie_tile(
+        tiles.append(_grid_movie_tile(
             key, start, end, videos, centroids, headings, 
-            dot_color=dot_color, window_size=window_size,
-            pre=pre, post=post, dot_radius=dot_radius)
-        
-        if overlay_trajectory:
-            trajectory = trajectories[i] + window_size//2
-            tile = overlay_trajectory_on_video(
-                tile, trajectory, pre, plot_options=plot_options, **overlay_options)
-        tiles.append(tile)
+            dot_color, window_size, scaled_window_size,
+            pre, post, dot_radius))
 
-    tiles = np.stack(tiles).reshape(rows, cols, post+pre, window_size, window_size, 3)
+    tiles = np.stack(tiles).reshape(rows, cols, post+pre, scaled_window_size, scaled_window_size, 3)
     frames = np.concatenate(np.concatenate(tiles,axis=2),axis=2)
     return frames
 
 
+def get_grid_movie_window_size(sampled_instances, centroids, headings,
+                               coordinates, pre, post, pctl=90, 
+                               fudge_factor=1.1, blocksize=16):
+    """
+    Automatically determine the window size for a grid movie.
+
+    The window size is set such that across all sampled instances,
+    the animal is fully visible in at least `pctl` percent of frames.
+
+    Parameters
+    ----------
+    sampled_instances: dict
+        Dictionary mapping syllables to lists of instances, where each
+        instance is specified as a tuple with the video name, start frame
+        and end frame. 
+
+    centroids: dict
+        Dictionary mapping video names to arrays of shape `(n_frames, 2)`
+        with the x,y coordinates of animal centroid on each frame
+
+    headings: dict
+        Dictionary mapping video names to arrays of shape `(n_frames,)`
+        with the heading of the animal on each frame (in radians)
+
+    coordinates: dict
+        Dictionary mapping session names to keypoint coordinates as 
+        ndarrays of shape (n_frames, n_bodyparts, 2). 
+
+    pre, post: int
+        Number of frames before/after syllable onset that are included 
+        in the grid movies.
+
+    pctl: int, default=95
+        Percentile of frames in which the animal should be fully visible.
+
+    fudge_factor: float, default=1.1
+        Factor by which to multiply the window size. 
+
+    blocksize: int, default=16
+        Window size is rounded up to the nearest multiple of `blocksize`.
+    """
+    all_trajectories = get_trajectories(
+        sum(sampled_instances.values(), []), coordinates, pre=pre, 
+        post=post, centroids=centroids, headings=headings)
+    
+    all_trajectories = np.concatenate(all_trajectories, axis=0)
+    ax_distances = np.max(np.abs(all_trajectories), axis=1)
+    window_size = np.percentile(ax_distances, pctl) * fudge_factor * 2
+    window_size = int(np.ceil(window_size / blocksize) * blocksize)
+    return window_size
+
+
 def generate_grid_movies(
     results=None, output_dir=None, name=None, project_dir=None,
     results_path=None, video_dir=None, video_paths=None, rows=4, 
     cols=6, filter_size=9, pre=30, post=60, min_frequency=0.005, 
-    min_duration=3, dot_radius=4, dot_color=(255,255,255), 
-    window_size=112, use_reindexed=True, coordinates=None, 
-    bodyparts=None, use_bodyparts=None, skeleton=[], quality=7, 
-    sampling_options={},  overlay_trajectory=False, plot_options={},
-    overlay_options={}, video_extension=None, **kwargs):
+    min_duration=3, dot_radius=4, dot_color=(255,255,255), quality=7,
+    window_size=None, use_reindexed=True, coordinates=None, 
+    bodyparts=None, use_bodyparts=None, sampling_options={},  
+    video_extension=None, max_video_size=1920, **kwargs):
     
     """
     Generate grid movies for a modeled dataset.
 
     Grid movies show many instances of a syllable and are useful in
     figuring out what behavior the syllable captures 
     (see :py:func:`keypoint_moseq.viz.grid_movie`). This method
@@ -727,60 +760,57 @@
     sampling_options: dict, default={}
         Dictionary of options for sampling syllable instances (see
         :py:func:`keypoint_moseq.util.sample_instances`).
     
     coordinates: dict, default=None
         Dictionary mapping session names to keypoint coordinates as 
         ndarrays of shape (n_frames, n_bodyparts, 2). Required when
-        `overlay_trajectory=True`, and for density-based sampling 
-        (i.e. when `sampling_options['mode']=='density'`; see 
+        `window_size=None`, and for density-based sampling (i.e. when 
+        `sampling_options['mode']=='density'`; see 
         :py:func:`keypoint_moseq.util.sample_instances`).
 
     bodyparts: list of str, default=None
         List of bodypart names in `coordinates`. Required when 
         `coordinates` is provided and bodyparts were reindexed 
         for modeling. 
 
     use_bodyparts: list of str, default=None
         Ordered list of bodyparts used for modeling. Required when 
         `coordinates` is provided and bodyparts were reindexed 
         for modeling. 
 
-    skeleton : list, default=[]
-        List of edges that define the skeleton, where each edge is a
-        pair of bodypart names or a pair of indexes.
-
-    overlay_trajectory: bool, default=False
-        Whether to overlay trajectory of keypoints on the grid movie. 
-        If True, `coordinates` must be provided.
-
-    overlay_options: dict, default={}
-        Dictionary of options for overlaying trajectory (see
-        :py:func:`keypoint_moseq.viz.overlay_trajectory_on_video`).
-
-    plot_options: dict, default={}
-        Dictionary of options for overlaying trajectory (see 
-        :py:func:`keypoint_moseq.viz.overlay_keypoints_on_image`).
-
     quality: int, default=7
         Quality of the grid movies. Higher values result in higher
         quality movies but larger file sizes.
 
     rows, cols, pre, post, dot_radius, dot_color, window_size
         See :py:func:`keypoint_moseq.viz.grid_movie`
 
     video_extension: str, default=None
         Preferred video extension (passed to :py:func:`keypoint_moseq.util.find_matching_videos`)
+
+    window_size: int, default=None
+        Size of the window around the animal. If None, the window
+        size is determined automatically based on the size of the
+        animal. If provided explicitly, `window_size` should be a
+        multiple of 16 or imageio will complain.
+
+    max_video_size: int, default=4000
+        Maximum size of the grid movie in pixels. If the grid movie
+        is larger than this, it will be downsampled.
+
+        
+    See :py:func:`keypoint_moseq.viz.grid_movie` for the remaining parameters.
     """
     assert (video_dir is not None) or (video_paths is not None), fill(
         'You must provide either `video_dir` or `video_paths`') 
 
-    if overlay_trajectory:
+    if window_size is None:
         assert coordinates is not None, fill(
-            '`coordinates` must be provided if `overlay_trajectory` is True')     
+            '`coordinates` must be provided if `window_size` is None')     
     
     if output_dir is None:
         assert project_dir is not None and name is not None, fill(
             'Either specify the `output_dir` where grid movies should '
             'be saved or include a `project_dir` and `name`')
         output_dir = os.path.join(project_dir,name, 'grid_movies')
     if not os.path.exists(output_dir): os.makedirs(output_dir)
@@ -792,18 +822,18 @@
     if results is None: results = load_results(
         name=name, project_dir=project_dir, path=results_path)
     
     if video_paths is None:
         video_paths = find_matching_videos(
             results.keys(), video_dir, as_dict=True, 
             video_extension=video_extension)
-
+        
     videos = {k: OpenCVReader(path) for k,path in video_paths.items()}
     fps = list(videos.values())[0].fps
-    
+
     syllable_key = 'syllables' + ('_reindexed' if use_reindexed else '')
     syllables = {k:v[syllable_key] for k,v in results.items()}
     centroids = {k:v['centroid'] for k,v in results.items()}
     headings = {k:v['heading'] for k,v in results.items()}
 
     syllable_instances = get_syllable_instances(
         syllables, pre=pre, post=post, min_duration=min_duration,
@@ -819,31 +849,38 @@
     sampled_instances = sample_instances(
         syllable_instances, rows*cols, coordinates=coordinates, 
         centroids=centroids, headings=headings, **sampling_options)
 
     centroids,headings = filter_centroids_headings(
         centroids, headings, filter_size=filter_size)
     
-    if len(skeleton)>0 and overlay_trajectory: 
-        if isinstance(skeleton[0][0],str):
-            assert use_bodyparts is not None, fill(
-                'If skeleton edges are specified using bodypart names, '
-                '`use_bodyparts` must be specified')
-            plot_options['edges'] = get_edges(use_bodyparts, skeleton)
-        else: plot_options['edges'] = skeleton
-    
+    if window_size is None:
+        window_size = get_grid_movie_window_size(
+            sampled_instances, centroids, headings, 
+            coordinates, pre, post)
+        
+    # in practice we may need a smaller window...
+    scaled_window_size = max_video_size/max(rows,cols)
+    scaled_window_size = int(np.floor(scaled_window_size / 16) * 16)
+    scaled_window_size = min(scaled_window_size, window_size)
+    scale_factor = scaled_window_size / window_size
+
+    if scale_factor < 1:
+        warnings.warn('\n'+fill(
+            f'Videos will be downscaled by a factor of {scale_factor:.2f} '
+            f'so that the grid movies are under {max_video_size} pixels. '
+            'Use `max_video_size` to increase or decrease this size limit.')+'\n\n')
+        
     for syllable,instances in tqdm.tqdm(
         sampled_instances.items(), desc='Generating grid movies'):
         
         frames = grid_movie(
             instances, rows, cols, videos, centroids, headings,
-            window_size=window_size, dot_color=dot_color, pre=pre, post=post,
-            dot_radius=dot_radius, overlay_trajectory=overlay_trajectory,
-            coordinates=coordinates, plot_options=plot_options,
-            overlay_options=overlay_options)
+            window_size=window_size, scaled_window_size=scaled_window_size,
+            dot_color=dot_color, pre=pre, post=post, dot_radius=dot_radius)
 
         path = os.path.join(output_dir, f'syllable{syllable}.mp4')
         write_video_clip(frames, path, fps=fps, quality=quality)
 
         
 def get_limits(coordinates, pctl=1, blocksize=None,
                left=0.2, right=0.2, top=0.2, bottom=0.2):
```

### Comparing `keypoint-moseq-0.1.0/setup.cfg` & `keypoint-moseq-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 	statsmodels
 	pyyaml
 	vidio
 	holoviews[recommended]
 	bokeh
 	pandas
 	tables
+	tabulate
 	jax-moseq==0.0.3
 
 [options.package_data]
 * = *.md
 
 [versioneer]
 VCS = git
```

### Comparing `keypoint-moseq-0.1.0/versioneer.py` & `keypoint-moseq-0.1.1/versioneer.py`

 * *Files identical despite different names*

