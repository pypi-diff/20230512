# Comparing `tmp/orbax-checkpoint-0.2.2.tar.gz` & `tmp/orbax-checkpoint-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-checkpoint-0.2.2.tar", last modified: Mon May  8 17:57:15 2023, max compression
+gzip compressed data, was "orbax-checkpoint-0.2.3.tar", last modified: Fri May 12 16:00:53 2023, max compression
```

## Comparing `orbax-checkpoint-0.2.2.tar` & `orbax-checkpoint-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/LICENSE
--rw-r--r--   0        0        0      699 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/README.md
--rw-r--r--   0        0        0     2564 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4742 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    33945 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7672 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45137 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    21766 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5234 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0     9406 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    13488 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    22579 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    20450 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7444 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/LICENSE
+-rw-r--r--   0        0        0      699 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/README.md
+-rw-r--r--   0        0        0     2564 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2629 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5348 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4744 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    34823 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0     9920 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     7190 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1465 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7672 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45137 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    22114 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5234 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0     9406 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    13488 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    23003 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    21387 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7444 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.3/PKG-INFO
```

### Comparing `orbax-checkpoint-0.2.2/LICENSE` & `orbax-checkpoint-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/README.md` & `orbax-checkpoint-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/__init__.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.2'
+__version__ = '0.2.3'
```

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/abstract_checkpointer.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/aggregate_handlers.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/array_checkpoint_handler.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpoint_handler.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpointer.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpointer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import functools
 import time
 from typing import Any, Optional
 
 from absl import logging
 from etils import epath
 import jax
-from jax.experimental.gda_serialization.serialization import AsyncManager
+from jax.experimental.array_serialization.serialization import AsyncManager
 from orbax.checkpoint import utils
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
 from orbax.checkpoint.checkpointer import Checkpointer
 
 
 def _on_commit_callback(temp_ckpt_dir: epath.Path, final_ckpt_dir: epath.Path,
                         checkpoint_start_time: float):
```

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_handler.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_manager.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,41 +14,43 @@
 
 """CheckpointManager, a sync implementation of AbstractCheckpointManager."""
 
 import asyncio
 import dataclasses
 import datetime
 import threading
+import time
 from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
 import uuid
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
-from jax.experimental.gda_serialization import serialization
+from jax.experimental.array_serialization import serialization
 from orbax.checkpoint import utils
 from orbax.checkpoint.abstract_checkpointer import AbstractCheckpointer
 from orbax.checkpoint.async_checkpointer import AsyncCheckpointer
 from orbax.checkpoint.checkpointer import Checkpointer
 from orbax.checkpoint.json_checkpoint_handler import JsonCheckpointHandler
 
-
 PyTree = Any
 CheckpointDirs = Tuple[str, str]
 SaveParams = Mapping[str, Any]
 RestoreParams = SaveParams
 
 DEFAULT_ITEM_NAME = 'default'
 DESCRIPTOR_ITEM_NAME = 'descriptor'
 METRIC_ITEM_NAME = 'metrics'
 METADATA_ITEM_NAME = 'metadata'
 
 RESERVED_ITEM_NAMES = [DESCRIPTOR_ITEM_NAME, METRIC_ITEM_NAME]
 
+_INIT_TIME = time.time()
+
 
 def _metrics_file_exists(metrics_item_path: epath.Path) -> bool:
   """True if item directory AND actual file both exist."""
   return (
       metrics_item_path.exists()
       and (metrics_item_path / METRIC_ITEM_NAME).exists()
   )
@@ -590,14 +592,15 @@
           continue
       if item_name not in self._checkpointers:
         raise ValueError(f'Checkpointer for item "{item_name}" not found')
       item = items.get(item_name, None)
       kwargs = restore_kwargs.get(item_name, {})
       restored[item_name] = self._checkpointers[item_name].restore(
           path, item=item, **kwargs)
+
     return restored
 
   def structure(self) -> Union[Any, Mapping[str, Any]]:
     """For all Checkpointers, returns the saved structure.
 
     Calls the `structure` method for each Checkpointer and returns a
     mapping of each item name to the restored structure. If the manager only
@@ -864,41 +867,58 @@
 
     Delegates to underlying Checkpointer.
     """
     for checkpointer in self._checkpointers.values():
       if is_async_checkpointer(checkpointer):
         checkpointer.check_for_errors()  # pytype: disable=attribute-error
 
-  def _finalize_checkpoint(self, temp_ckpt_dir: epath.Path):
+  def _finalize_checkpoint(
+      self, temp_ckpt_dir: epath.Path
+  ) -> Optional[epath.Path]:
     """Moves tmp step checkpoint to final.
 
     Args:
       temp_ckpt_dir: The temporary checkpoint directory. If not None, only
         finalize the checkpoints in `temp_ckpt_dir`. If None, it will iterate
         through all temp checkpoints in `self.directory` and finalize them all.
+
+    Returns:
+      the final checkpoint dir
     """
     if jax.process_index() == 0:
       try:
         self.check_for_errors()
       except Exception as e:  # pylint: disable=broad-except
         logging.error(
             (
                 'Received error: %s from Checkpointer. One or more items may'
                 ' not be finalized. Skipping finalization of step checkpoint.'
             ),
             e,
         )
-        return
-      utils.ensure_atomic_save(
-          temp_ckpt_dir,
-          self._get_save_directory(
-              utils.step_from_checkpoint_name(temp_ckpt_dir.name),
-              self.directory,
-          ),
-      )
+        return None
+      step = utils.step_from_checkpoint_name(temp_ckpt_dir.name)
+      # If at a preemption step, record the time since the previous checkpoint.
+      # This represents training time that would otherwise have been wasted.
+      # If another checkpoint has not been previously saved, measures the time
+      # since program start.
+      if self.reached_preemption(step):
+        if len(self._checkpoints) > 1:
+          previous_time = self._checkpoints[-2].time
+        else:
+          previous_time = _INIT_TIME
+        assert self._last_checkpoint is not None
+        duration = self._last_checkpoint.time - previous_time
+        jax.monitoring.record_event_duration_secs(
+            '/jax/checkpoint/write/preempt/duration_saved_secs',
+            duration.total_seconds(),
+        )
+      final_ckpt_dir = self._get_save_directory(step, self.directory)
+      utils.ensure_atomic_save(temp_ckpt_dir, final_ckpt_dir)
+      return final_ckpt_dir
 
   def _finalize(self, temp_ckpt_dir: epath.Path):
     """Cleans up old checkpoints and synchronizes hosts."""
     if not self._all_checkpointers_are_sync:
       self.wait_until_finished(join_finalize_thread=False)
-    self._finalize_checkpoint(temp_ckpt_dir)
+    final_ckpt_dir = self._finalize_checkpoint(temp_ckpt_dir)
     self._remove_old_checkpoints()
```

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils_test.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpointer.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/conftest.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/future.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/lazy_utils.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils_test.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax-checkpoint-0.2.3/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 
 import asyncio
 import dataclasses
 import functools
 import re
 from typing import Any, Callable, List, Optional, Tuple, Union
 
+from absl import logging
 from etils import epath
 import jax
-from jax.experimental.gda_serialization import serialization
+from jax.experimental.array_serialization import serialization
 import numpy as np
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import lazy_utils
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
@@ -581,10 +582,20 @@
     Raises:
       FileNotFoundError: if the checkpoint is not found.
     """
     checkpoint_path = directory / self._aggregate_filename
     if checkpoint_path.exists():
       return self._aggregate_handler.deserialize(checkpoint_path)
     else:
-      raise FileNotFoundError(
-          f'Checkpoint not found: {checkpoint_path}.'
-      )
+      if self._use_ocdbt:
+        raise ValueError(
+            f'Checkpoint structure file does not exist at {directory}.'
+        )
+      else:
+        logging.error(
+            (
+                'Checkpoint structure file does not exist at %s.'
+                ' Attempting to assume an implicit tree structure.'
+            ),
+            directory,
+        )
+        return utils.pytree_structure(directory)
```

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/test_utils.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils_test.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/type_handlers.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/type_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import dataclasses
 import os
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 from absl import logging
 from etils import epath
 import jax
-from jax.experimental.gda_serialization import serialization
-from jax.experimental.gda_serialization.serialization import get_tensorstore_spec
+from jax.experimental.array_serialization import serialization
+from jax.experimental.array_serialization.serialization import get_tensorstore_spec
 import jax.numpy as jnp
 from jax.sharding import Mesh
 import numpy as np
 from orbax.checkpoint import utils
 from orbax.checkpoint.future import Future
 import tensorstore as ts
 
@@ -480,14 +480,25 @@
     """Gets Tensorstore spec for reading."""
     return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
 
   async def serialize(
       self, value: jax.Array, info: ParamInfo, args: Optional[SaveArgs] = None
   ) -> List[Future]:
     """See superclass documentation."""
+    if (
+        isinstance(value, jax.Array)
+        and jax.process_count() > 1
+        and value.is_fully_addressable
+    ):
+      raise ValueError(
+          'Cannot serialize host local arrays. Arrays like this are typically'
+          ' obtained using pmap. Consider using host_local_to_global_array in'
+          ' orbax/checkpoint/utils.py to convert your arrays into serializable'
+          ' objects.'
+      )
     args = args or SaveArgs()
     tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
     tspec = _get_cast_tspec_serialize(tspec, value, args)
     commit_futures = []
     await serialization.async_serialize(
         value, tspec, commit_future=commit_futures, context=self._ts_context
     )
```

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/utils.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -359,14 +359,15 @@
 
 
 def cleanup_tmp_directories(directory: epath.PathLike,
                             primary_host: Optional[int] = 0):
   """Cleanup steps in `directory` with tmp files, as these are not finalized."""
   directory = epath.Path(directory)
   if primary_host is None or jax.process_index() == primary_host:
+    logging.info('Cleaning up existing temporary directories at %s.', directory)
     tmp_files = tmp_checkpoints(directory)
     for tmp_file in tmp_files:
       (directory / tmp_file).rmtree()
 
   sync_global_devices('cleanup_tmp_dirs')
 
 
@@ -633,7 +634,33 @@
   return False
 
 
 def tmp_checkpoints(checkpoint_dir: epath.PathLike) -> List[str]:
   """Returns a list of tmp checkpoints in the directory."""
   checkpoint_dir = epath.Path(checkpoint_dir)
   return [s.name for s in checkpoint_dir.iterdir() if is_tmp_checkpoint(s)]
+
+
+def fully_replicated_host_local_array_to_global_array(
+    arr: jax.Array,
+) -> jax.Array:
+  """Converts a host local array from to global jax.Array.
+
+  In most cases, the local array is expected to have been produced by pmap.
+
+  Args:
+    arr: Host local array
+
+  Returns:
+    A global array.
+  """
+  if not arr.is_fully_replicated:
+    raise ValueError('Array must be fully replicated.')
+  global_shape = arr.device_buffers[0].shape
+  # Create a 1D mesh to create fully replicated global jax.Array.
+  sharding = jax.sharding.NamedSharding(
+      jax.sharding.Mesh(np.array(jax.devices()), axis_names=('x',)),
+      jax.sharding.PartitionSpec(None),
+  )
+  # pmap-produced Array has a "scrambled" device order.
+  dbs = sorted(arr.device_buffers, key=lambda x: x.device().id)
+  return jax.make_array_from_single_device_arrays(global_shape, sharding, dbs)
```

### Comparing `orbax-checkpoint-0.2.2/orbax/checkpoint/utils_test.py` & `orbax-checkpoint-0.2.3/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.2/pyproject.toml` & `orbax-checkpoint-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 dependencies = [
     'absl-py',
     'cached_property',
     'importlib_resources',
     'etils',
     'typing_extensions',
     'msgpack',
-    'jax >= 0.4.8',
+    'jax >= 0.4.9',
     'jaxlib',
     'numpy',
     'pyyaml',
     'tensorstore >= 0.1.35',
     'nest_asyncio'
 ]
```

### Comparing `orbax-checkpoint-0.2.2/PKG-INFO` & `orbax-checkpoint-0.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.2
+Version: 0.2.3
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: absl-py
 Requires-Dist: cached_property
 Requires-Dist: importlib_resources
 Requires-Dist: etils
 Requires-Dist: typing_extensions
 Requires-Dist: msgpack
-Requires-Dist: jax >= 0.4.8
+Requires-Dist: jax >= 0.4.9
 Requires-Dist: jaxlib
 Requires-Dist: numpy
 Requires-Dist: pyyaml
 Requires-Dist: tensorstore >= 0.1.35
 Requires-Dist: nest_asyncio
 Requires-Dist: flax ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
```

