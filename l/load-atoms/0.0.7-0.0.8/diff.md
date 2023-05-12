# Comparing `tmp/load-atoms-0.0.7.tar.gz` & `tmp/load-atoms-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "load-atoms-0.0.7.tar", last modified: Wed Apr 12 12:37:17 2023, max compression
+gzip compressed data, was "load-atoms-0.0.8.tar", last modified: Fri May 12 13:57:17 2023, max compression
```

## Comparing `load-atoms-0.0.7.tar` & `load-atoms-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-12 12:37:17.909505 load-atoms-0.0.7/
--rw-r--r--   0 john       (504) staff       (20)     1069 2023-04-04 12:18:14.000000 load-atoms-0.0.7/LICENSE
--rw-r--r--   0 john       (504) staff       (20)       48 2023-03-07 08:55:19.000000 load-atoms-0.0.7/MANIFEST.in
--rw-r--r--   0 john       (504) staff       (20)     2767 2023-04-12 12:37:17.909044 load-atoms-0.0.7/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)      972 2023-04-12 10:09:54.000000 load-atoms-0.0.7/README.md
--rw-r--r--   0 john       (504) staff       (20)     1309 2023-04-12 12:36:57.000000 load-atoms-0.0.7/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-04-12 12:37:17.909579 load-atoms-0.0.7/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-12 12:37:17.904689 load-atoms-0.0.7/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-12 12:37:17.906307 load-atoms-0.0.7/src/load_atoms/
--rw-r--r--   0 john       (504) staff       (20)      127 2023-04-12 12:36:57.000000 load-atoms-0.0.7/src/load_atoms/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     1727 2023-04-05 06:56:03.000000 load-atoms-0.0.7/src/load_atoms/api.py
--rw-r--r--   0 john       (504) staff       (20)     3304 2023-04-05 08:42:48.000000 load-atoms-0.0.7/src/load_atoms/backend.py
--rw-r--r--   0 john       (504) staff       (20)      535 2023-04-05 08:42:48.000000 load-atoms-0.0.7/src/load_atoms/checksums.py
--rw-r--r--   0 john       (504) staff       (20)     2051 2023-04-05 08:42:48.000000 load-atoms-0.0.7/src/load_atoms/database.py
--rw-r--r--   0 john       (504) staff       (20)     3747 2023-04-12 12:36:53.000000 load-atoms-0.0.7/src/load_atoms/dataset.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-12 12:37:17.907930 load-atoms-0.0.7/src/load_atoms/datasets/
--rw-r--r--   0 john       (504) staff       (20)     1040 2023-04-06 09:55:36.000000 load-atoms-0.0.7/src/load_atoms/datasets/C-GAP-17.yaml
--rw-r--r--   0 john       (504) staff       (20)     1166 2023-04-12 12:15:55.000000 load-atoms-0.0.7/src/load_atoms/datasets/C-GAP-20.yaml
--rw-r--r--   0 john       (504) staff       (20)      760 2023-04-12 09:41:52.000000 load-atoms-0.0.7/src/load_atoms/datasets/C-SYNTH-1M.yaml
--rw-r--r--   0 john       (504) staff       (20)     1356 2023-03-07 08:55:19.000000 load-atoms-0.0.7/src/load_atoms/datasets/QM7.yaml
--rw-r--r--   0 john       (504) staff       (20)     1222 2023-03-07 16:02:25.000000 load-atoms-0.0.7/src/load_atoms/datasets/amorphous-grahpene.yaml
--rw-r--r--   0 john       (504) staff       (20)     1240 2023-02-18 11:49:24.000000 load-atoms-0.0.7/src/load_atoms/manipulations.py
--rw-r--r--   0 john       (504) staff       (20)     1618 2023-04-06 10:09:05.000000 load-atoms-0.0.7/src/load_atoms/util.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-12 12:37:17.907027 load-atoms-0.0.7/src/load_atoms.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2767 2023-04-12 12:37:17.000000 load-atoms-0.0.7/src/load_atoms.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)      755 2023-04-12 12:37:17.000000 load-atoms-0.0.7/src/load_atoms.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-04-12 12:37:17.000000 load-atoms-0.0.7/src/load_atoms.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      157 2023-04-12 12:37:17.000000 load-atoms-0.0.7/src/load_atoms.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       11 2023-04-12 12:37:17.000000 load-atoms-0.0.7/src/load_atoms.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-12 12:37:17.908815 load-atoms-0.0.7/tests/
--rw-r--r--   0 john       (504) staff       (20)     1581 2023-04-06 09:06:34.000000 load-atoms-0.0.7/tests/test_backend.py
--rw-r--r--   0 john       (504) staff       (20)     1965 2023-04-06 09:14:35.000000 load-atoms-0.0.7/tests/test_database.py
--rw-r--r--   0 john       (504) staff       (20)     2094 2023-04-06 09:14:52.000000 load-atoms-0.0.7/tests/test_dataset.py
--rw-r--r--   0 john       (504) staff       (20)      857 2023-04-05 06:56:03.000000 load-atoms-0.0.7/tests/test_manipulations.py
--rw-r--r--   0 john       (504) staff       (20)      441 2023-04-05 08:42:48.000000 load-atoms-0.0.7/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.953891 load-atoms-0.0.8/
+-rw-r--r--   0 john       (504) staff       (20)     1069 2023-04-04 12:18:14.000000 load-atoms-0.0.8/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)       48 2023-03-07 08:55:19.000000 load-atoms-0.0.8/MANIFEST.in
+-rw-r--r--   0 john       (504) staff       (20)     2767 2023-05-12 13:57:17.953662 load-atoms-0.0.8/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)      972 2023-04-12 10:09:54.000000 load-atoms-0.0.8/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1376 2023-05-12 13:56:11.000000 load-atoms-0.0.8/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-12 13:57:17.953951 load-atoms-0.0.8/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.941360 load-atoms-0.0.8/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.944636 load-atoms-0.0.8/src/load_atoms/
+-rw-r--r--   0 john       (504) staff       (20)      127 2023-05-12 13:56:11.000000 load-atoms-0.0.8/src/load_atoms/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     1727 2023-04-05 06:56:03.000000 load-atoms-0.0.8/src/load_atoms/api.py
+-rw-r--r--   0 john       (504) staff       (20)     4663 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/backend.py
+-rw-r--r--   0 john       (504) staff       (20)      535 2023-04-05 08:42:48.000000 load-atoms-0.0.8/src/load_atoms/checksums.py
+-rw-r--r--   0 john       (504) staff       (20)     2104 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/database.py
+-rw-r--r--   0 john       (504) staff       (20)     3924 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/dataset.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.947656 load-atoms-0.0.8/src/load_atoms/datasets/
+-rw-r--r--   0 john       (504) staff       (20)     1040 2023-04-06 09:55:36.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-17.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1166 2023-04-12 12:15:55.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-20.yaml
+-rw-r--r--   0 john       (504) staff       (20)      760 2023-04-12 09:41:52.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-1M.yaml
+-rw-r--r--   0 john       (504) staff       (20)    24624 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-23M.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1356 2023-03-07 08:55:19.000000 load-atoms-0.0.8/src/load_atoms/datasets/QM7.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1222 2023-03-07 16:02:25.000000 load-atoms-0.0.8/src/load_atoms/datasets/amorphous-grahpene.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1279 2023-05-12 08:34:41.000000 load-atoms-0.0.8/src/load_atoms/manipulations.py
+-rw-r--r--   0 john       (504) staff       (20)      946 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.945287 load-atoms-0.0.8/src/load_atoms.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2767 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)      796 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      180 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       11 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.952329 load-atoms-0.0.8/tests/
+-rw-r--r--   0 john       (504) staff       (20)     1706 2023-05-12 13:55:30.000000 load-atoms-0.0.8/tests/test_backend.py
+-rw-r--r--   0 john       (504) staff       (20)     2141 2023-05-12 13:55:30.000000 load-atoms-0.0.8/tests/test_database.py
+-rw-r--r--   0 john       (504) staff       (20)     2094 2023-04-06 09:14:52.000000 load-atoms-0.0.8/tests/test_dataset.py
+-rw-r--r--   0 john       (504) staff       (20)      853 2023-05-12 08:34:41.000000 load-atoms-0.0.8/tests/test_manipulations.py
+-rw-r--r--   0 john       (504) staff       (20)      441 2023-04-05 08:42:48.000000 load-atoms-0.0.8/tests/test_util.py
```

### Comparing `load-atoms-0.0.7/LICENSE` & `load-atoms-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/PKG-INFO` & `load-atoms-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-atoms
-Version: 0.0.7
+Version: 0.0.8
 Summary: Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `load-atoms-0.0.7/README.md` & `load-atoms-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/pyproject.toml` & `load-atoms-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "load-atoms"
-version = "0.0.7"
+version = "0.0.8"
 description = "Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)"
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["chemistry", "machine learning", "datasets"]
-dependencies = ["ase", "pyyaml", "requests", "numpy", "pydantic"]
+dependencies = [
+    "ase",
+    "pyyaml",
+    "requests",
+    "numpy",
+    "pydantic",
+    "aiohttp",
+    "nest_asyncio",
+    "rich",
+]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = [
     "notebook",
     "pytest",
+    "pytest-asyncio",
     "black",
     "isort",
     "sphinx",
     "furo",
     "nbsphinx",
     "sphinx-autobuild",
-    "sphinx-copybutton",
     "pytest-cov",
     "build",
     "bumpver",
     "twine",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/load-atoms"
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `load-atoms-0.0.7/src/load_atoms/api.py` & `load-atoms-0.0.8/src/load_atoms/api.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/checksums.py` & `load-atoms-0.0.8/src/load_atoms/checksums.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/database.py` & `load-atoms-0.0.8/src/load_atoms/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Dict, List
 
 import yaml
 from pydantic import BaseModel, validator
 
 from load_atoms.checksums import valid_checksum
-from load_atoms.util import DATASETS_DIR
+from load_atoms.util import BASE_REMOTE_URL, DATASETS_DIR
 
 
 def is_bibtex(data: str) -> bool:
     data = data.strip()
     return data.startswith("@") and data.endswith("}")
 
 
@@ -19,14 +19,15 @@
     files: Dict[str, str]
     citation: str = None
     license: str = None
     representative_structures: List[int] = None
     long_description: str = None
     per_atom_properties: dict = None
     per_structure_properties: dict = None
+    url_root: str = BASE_REMOTE_URL
 
     @validator("license")
     def validate_license(cls, v):
         valid_licences = ["MIT", "CC-BY-4.0", "CC BY-NC-SA 4.0"]
         if v not in valid_licences:
             raise ValueError(f"Invalid license: {v}. Must be one of {valid_licences}")
         return v
```

### Comparing `load-atoms-0.0.7/src/load_atoms/dataset.py` & `load-atoms-0.0.8/src/load_atoms/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,26 @@
         self.structures = [*structures]
         self._description = description
 
     def __len__(self):
         return len(self.structures)
 
     def __getitem__(self, slice):
-        if isinstance(slice, int):
-            # return a single structure
+        # if the slice can be cast to an int (e.g. is an np.int64), then
+        # return a single structure
+        try:
+            slice = int(slice)
             return self.structures[slice]
-        else:
-            # return a new Dataset
-            return Dataset(self.structures[slice])
+        except TypeError:
+            pass
+
+        # otherwise, our slice is a slice object,
+        # and we should return a new Dataset
+        sliced_structres = self.structures[slice]
+        return Dataset(sliced_structres)
 
     def __iter__(self):
         return iter(self.structures)
 
     def __repr__(self):
         return summarise_dataset(self.structures, self._description)
 
@@ -43,47 +49,47 @@
         structures = read(path, index=":")
         return cls(structures, path.stem)
 
     @classmethod
     def from_id(cls, dataset_id: str, root: Path = None, verbose: bool = True):
         if not is_known_dataset(dataset_id):
             raise ValueError(f"Dataset {dataset_id} is not known.")
+
         dataset_info = DATASETS[dataset_id]
         all_structures = backend.get_structures(dataset_info, root)
         if verbose:
             print(usage_info(dataset_info))
         return cls(all_structures, dataset_info)
 
     @classmethod
     def from_structures(cls, structures: Iterable[Atoms]):
         return cls(structures)
 
     @classmethod
     def from_file(cls, path: Path):
         structures = read(path, index=":")
-        return cls(structures, path.stem)
+        return cls(structures)
 
 
 def usage_info(dataset: DatasetDescription) -> str:
     info = []
     if dataset.license is not None:
         info.append(f"This dataset is covered by the {dataset.license} license.")
     if dataset.citation is not None:
         info.append(f"Please cite this dataset if you use it in your work.")
 
     _url = frontend_url(dataset)
-    info.append(f"For more information about this dataset, see here {_url}")
+    info.append(f"For more information, visit:\n{_url}")
 
     return "\n".join(info)
 
 
 def summarise_dataset(
     structures: List[Atoms], description: DatasetDescription = None
 ) -> str:
-
     name = description.name if description is not None else "Dataset"
     N = len(structures)
     number_atoms = sum([len(structure) for structure in structures])
 
     per_atom_properties = intersection(
         structure.arrays.keys() for structure in structures
     )
```

### Comparing `load-atoms-0.0.7/src/load_atoms/datasets/C-GAP-17.yaml` & `load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-17.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/datasets/C-GAP-20.yaml` & `load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-20.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/datasets/C-SYNTH-1M.yaml` & `load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-1M.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/datasets/QM7.yaml` & `load-atoms-0.0.8/src/load_atoms/datasets/QM7.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/datasets/amorphous-grahpene.yaml` & `load-atoms-0.0.8/src/load_atoms/datasets/amorphous-grahpene.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/src/load_atoms/manipulations.py` & `load-atoms-0.0.8/src/load_atoms/manipulations.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 FilterFunction = Callable[[Atoms], bool]
 
 
 def filter_by(
     dataset: Union[Dataset, Sequence[Atoms]],
     *functions: Sequence[FilterFunction],
-    **kwargs
+    **kwargs,
 ) -> Dataset:
     """Filter a dataset by a given property."""
 
     structures_filtered_by_kwargs = [
         structure
         for structure in dataset
         if all(structure.info.get(key, None) == value for key, value in kwargs.items())
@@ -27,23 +27,23 @@
             for structure in structures_filtered_by_kwargs
             if all(func(structure) for func in functions)
         ]
     )
 
 
 def cross_validate_split(
-    dataset: Dataset, fold, folds=5, n_test: int = None, seed: int = 0
+    dataset: Dataset, fold, k=5, n_test: int = None, seed: int = 0
 ) -> Dataset:
     """Generate a shuffled train/test split for cross-validation."""
 
     if n_test is None:
-        n_test = len(dataset) // folds
+        n_test = len(dataset) // k
 
     idxs = np.arange(len(dataset))
     np.random.RandomState(seed).shuffle(idxs)
-    idxs = np.roll(idxs, fold * len(idxs) // folds)
+    idxs = np.roll(idxs, fold * len(idxs) // k)
     train, test = idxs[:-n_test], idxs[-n_test:]
 
     return (
-        [dataset[t] for t in train],
-        [dataset[t] for t in test],
+        Dataset.from_structures([dataset[t] for t in train]),
+        Dataset.from_structures([dataset[t] for t in test]),
     )
```

### Comparing `load-atoms-0.0.7/src/load_atoms.egg-info/PKG-INFO` & `load-atoms-0.0.8/src/load_atoms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-atoms
-Version: 0.0.7
+Version: 0.0.8
 Summary: Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `load-atoms-0.0.7/src/load_atoms.egg-info/SOURCES.txt` & `load-atoms-0.0.8/src/load_atoms.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/load_atoms.egg-info/SOURCES.txt
 src/load_atoms.egg-info/dependency_links.txt
 src/load_atoms.egg-info/requires.txt
 src/load_atoms.egg-info/top_level.txt
 src/load_atoms/datasets/C-GAP-17.yaml
 src/load_atoms/datasets/C-GAP-20.yaml
 src/load_atoms/datasets/C-SYNTH-1M.yaml
+src/load_atoms/datasets/C-SYNTH-23M.yaml
 src/load_atoms/datasets/QM7.yaml
 src/load_atoms/datasets/amorphous-grahpene.yaml
 tests/test_backend.py
 tests/test_database.py
 tests/test_dataset.py
 tests/test_manipulations.py
 tests/test_util.py
```

### Comparing `load-atoms-0.0.7/tests/test_database.py` & `load-atoms-0.0.8/tests/test_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from load_atoms.checksums import generate_checksum
 from load_atoms.database import (
     DATASETS,
     DatasetDescription,
     find_all_descriptor_files,
     get_description_of,
 )
+from load_atoms.util import BASE_REMOTE_URL
 
 _local_path_to_datasets = Path(__file__).parent.parent / "src/load_atoms/datasets"
 
 
 def test_all_loaded():
     """
     test that all datasets are loaded
@@ -24,14 +25,18 @@
 
 @pytest.mark.parametrize("dataset", DATASETS.values(), ids=lambda x: x.name)
 def test_checksums(dataset):
     """
     test that all dataset checksums are correct
     """
 
+    # we don't want to download all datasets each time we run the tests
+    if dataset.url_root != BASE_REMOTE_URL:
+        return
+
     for path, checksum in dataset.files.items():
         path = _local_path_to_datasets / path
         assert checksum == generate_checksum(path)
 
 
 def test_description():
     desc = get_description_of("C-GAP-17")
```

### Comparing `load-atoms-0.0.7/tests/test_dataset.py` & `load-atoms-0.0.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.7/tests/test_manipulations.py` & `load-atoms-0.0.8/tests/test_manipulations.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,10 +20,10 @@
         structures,
         name="water",
     )
     assert len(filtered) == 1, "The filtered dataset should contain one structure"
 
 
 def test_cv():
-    train, test = cross_validate_split(structures, fold=1, folds=3)
+    train, test = cross_validate_split(structures, fold=1, k=3)
     assert len(train) == 2, "The train dataset should contain two structures"
     assert len(test) == 1, "The test dataset should contain one structure"
```

