# Comparing `tmp/tracknado-0.2.tar.gz` & `tmp/tracknado-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracknado-0.2.tar", last modified: Wed May  3 11:16:17 2023, max compression
+gzip compressed data, was "tracknado-0.2.1.tar", last modified: Fri May 12 14:46:09 2023, max compression
```

## Comparing `tracknado-0.2.tar` & `tracknado-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.082956 tracknado-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.078956 tracknado-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.078956 tracknado-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 11:16:05.000000 tracknado-0.2/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-03 11:16:05.000000 tracknado-0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-03 11:16:05.000000 tracknado-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-03 11:16:17.082956 tracknado-0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-03 11:16:05.000000 tracknado-0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-03 11:16:05.000000 tracknado-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:16:17.082956 tracknado-0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-03 11:16:05.000000 tracknado-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.078956 tracknado-0.2/tracknado/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 11:16:16.000000 tracknado-0.2/tracknado/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.082956 tracknado-0.2/tracknado/old/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/grouping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/hub_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/make_hub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/old/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-03 11:16:05.000000 tracknado-0.2/tracknado/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:16:17.082956 tracknado-0.2/tracknado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 11:16:17.000000 tracknado-0.2/tracknado.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 14:45:57.000000 tracknado-0.2.1/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-05-12 14:45:57.000000 tracknado-0.2.1/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-12 14:45:57.000000 tracknado-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-12 14:46:09.280572 tracknado-0.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2422 2023-05-12 14:45:57.000000 tracknado-0.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-12 14:45:57.000000 tracknado-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:46:09.280572 tracknado-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-12 14:45:57.000000 tracknado-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/tracknado/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28022 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/tracknado/old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6644 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/grouping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/hub_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6442 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/make_hub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2356 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/old/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-05-12 14:45:57.000000 tracknado-0.2.1/tracknado/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:46:09.280572 tracknado-0.2.1/tracknado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 14:46:09.000000 tracknado-0.2.1/tracknado.egg-info/top_level.txt
```

### Comparing `tracknado-0.2/.github/workflows/python-publish.yml` & `tracknado-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/LICENSE` & `tracknado-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/PKG-INFO` & `tracknado-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.2
+Version: 0.2.1
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tracknado-0.2/README.md` & `tracknado-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/pyproject.toml` & `tracknado-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado/api.py` & `tracknado-0.2.1/tracknado/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,20 +186,21 @@
         subgroup_by: List[str] = None,
         overlay_by: List[str] = None,
         supergroup_by: List[str] = None,
         **kwargs,
     ):
 
         self.details = details
-        self._supertrack_columns = supergroup_by
-        self._overlay_columns = overlay_by
-        self._subgroup_columns = subgroup_by
-        self._color_columns = color_by
+        self._supertrack_columns = list(supergroup_by) if supergroup_by else list()
+        self._overlay_columns = list(overlay_by) if overlay_by else list()
+        self._subgroup_columns = list(subgroup_by) if subgroup_by else list()
+        self.subgroup_definitions = list() if subgroup_by else None
+        self._color_columns = list(color_by) if color_by else list()
 
-        self._add_subgroupings(supergroup_by=supergroup_by, subgroup_by=subgroup_by)
+        self._add_subgroupings(supergroup_by=self._supertrack_columns, subgroup_by=self._subgroup_columns)
 
         self.super_tracks = self._get_super_tracks()
         self._add_supertrack_indicators()
 
         self.composite_tracks = self._get_composite_tracks()
         self._add_composite_track_indicators()
 
@@ -318,14 +319,17 @@
             subgroup_definitions.append(subgroup_definition)
 
         # Add a column to the details dataframe with the subgroup definition for each track
         df["subgroup_names"] = [
             tuple([col for col in subgroup_by]) for i in range(df.shape[0])
         ]
         df["subgroup_definition"] = [subgroup_definitions for i in range(df.shape[0])]
+
+        self.subgroup_definitions.extend(subgroup_definitions)
+
         return df
 
     def _add_subgroupings(
         self, supergroup_by: List[str] = None, subgroup_by: List[str] = None
     ) -> None:
         """Add a column to the details dataframe with a `trackhub.SubGroupDefinition` for each track.
 
@@ -342,15 +346,15 @@
                 [c in self.details.columns for c in subgroup_by]
             ), f"Subgroup-By columns {subgroup_by} missing"
 
             if supergroup_by:
                 assert not any(
                     subgroup in supergroup_by for subgroup in subgroup_by
                 ), f"SubGroup columns {subgroup_by} cannot be in SuperGroup columns {supergroup_by}"
-
+          
                 self.details = self.details.groupby(supergroup_by).apply(
                     self._add_subgroup_definitions_to_df, subgroup_by=subgroup_by
                 )
             else:
                 self.details = self._add_subgroup_definitions_to_df(
                     self.details, subgroup_by=subgroup_by
                 )
@@ -362,16 +366,26 @@
             assert all(
                 [c in self.details.columns for c in self._supertrack_columns]
             ), f"SuperTrack columns {self._supertrack_columns} missing"
 
             supertracks = dict()
             for grouping, df in self.details.groupby(self._supertrack_columns):
                 
-                track_id = tuple(grouping) if not isinstance(grouping, str) else (grouping,)
-                track_name = "_".join(grouping)
+
+                if isinstance(grouping, str):
+                    track_id = (grouping,)
+                elif len(grouping) == 1:
+                    track_id = grouping
+                else:
+                    track_id = tuple(grouping)
+                
+                if len(track_id) == 1:
+                    track_name = track_id[0]
+                else:
+                    track_name = "_".join(track_id)
 
 
                 supertracks[get_hash(track_id)] = trackhub.SuperTrack(
                     name=track_name,
                 )
 
         else:
@@ -391,40 +405,40 @@
     
     def _get_composite_tracks(self) -> Dict[str, trackhub.CompositeTrack]:
         """Generate a dictionary of CompositeTracks from the details dataframe"""
 
         composite_tracks = dict()
         if "supertrack" in self.details.columns:
             for (supertrack, ext) , df in self.details.groupby(["supertrack", "ext"]):
-
-                subgroupings = df.iloc[df["subgroup_names"].drop_duplicates().index, :][
-                    "subgroup_definition"
-                ]
+                
                 dimensions = dict(
                     zip(
                         [f"dim{d}" for d in ["X", "Y", "A", "B", "C", "D"]],
-                        subgroupings,
+                        self._subgroup_columns,
                     )
                 )
 
-                supertrack_name = self.super_tracks[get_hash(supertrack)].name
+                supertrack_name = self.super_tracks[supertrack].name
                 composite_name = "_".join([supertrack_name, ext])
 
+
                 composite = trackhub.CompositeTrack(
                     name=composite_name,
                     tracktype=ext,
                     dimensions=" ".join([f"{k}={v}" for k, v in dimensions.items()])
                     if dimensions
                     else None,
-                    sortOrder=" ".join([f"{k}=+" for k in subgroupings]),
+                    sortOrder=" ".join([f"{k}=+" for k in self._subgroup_columns]),
                     visibility="hide",
                     dragAndDrop="subTracks",
                     allButtonPair="off",
                 )
 
+                composite.add_subgroups(self.subgroup_definitions)
+
                 self.super_tracks[supertrack].add_tracks(composite)
                 composite_tracks[get_hash((supertrack, ext))] = composite
 
         elif self._subgroup_columns:
             for ext, df in self.details.groupby("ext"):
                 composite = trackhub.CompositeTrack(
                     name=ext,
@@ -441,15 +455,15 @@
 
         return composite_tracks
 
     def _add_composite_track_indicators(self):
         """Add a column to the details dataframe with a CompositeTrack indicator for each track"""
 
         if self.composite_tracks:
-            composite_columns = self._supertrack_columns if self._supertrack_columns else []
+            composite_columns = ["supertrack"] if self._supertrack_columns else []
             composite_columns.append("ext")
 
             self.details["composite"] = get_hash_for_df(self.details, composite_columns)
 
             assert self.details["composite"].isin(self.composite_tracks.keys()).all(), (
                 "Composite tracks not found in details dataframe"
             )
@@ -501,15 +515,15 @@
 
     def _add_overlay_track_indicators(self):
         """Add a column to the details dataframe with an OverlayTrack indicator for each track"""
 
         if self._overlay_columns:
 
             overlay_columns = (
-                self._supertrack_columns if self._supertrack_columns else []
+                ["supertrack"] if self._supertrack_columns else []
             )
             overlay_columns.extend(self._overlay_columns)
 
             self.details["overlay"] = get_hash_for_df(self.details, overlay_columns)
 
             assert self.details["overlay"].isin(self.overlay_tracks.keys()).all(), (
                 "Overlay tracks not found in details dataframe"
```

### Comparing `tracknado-0.2/tracknado/cli.py` & `tracknado-0.2.1/tracknado/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import click
+from typing import Literal, Union
 
 class OptionEatAll(click.Option):
 
     def __init__(self, *args, **kwargs):
         self.save_other_options = kwargs.pop('save_other_options', True)
         nargs = kwargs.pop('nargs', -1)
         assert nargs == -1, 'nargs, if set, must be -1 not {}'.format(nargs)
@@ -47,14 +48,36 @@
 
 @click.group()
 def cli():
     """Tracknado: A tool for generating UCSC track hubs
     Tracknado go BRRRR!
     """
 
+@cli.command()
+@click.option("-i", "--input-files", help="Input files", cls=OptionEatAll, type=list)
+@click.option("-o", "--output", help="Design name", required=True)
+@click.option(
+    "--preset",
+    help="Adjust design for specific use cases. Choose from: seqnado",
+    type=click.Choice(["seqnado"]),
+    default=None,
+)
+
+def design(input_files: list, output: str, preset: Union[None, Literal["seqnado"]]):
+
+    from tracknado.api import TrackFiles
+
+    tf = TrackFiles(input_files, infer_subgroups=True, infer_attributes=True)
+
+    if preset == "seqnado":
+        tf.files = tf.files.assign(experiment=lambda df: df["fn"].apply(lambda x: x.parent.parent.parent.name))
+
+    tf.files.to_csv(output)
+
+
 
 @cli.command()
 @click.option("-i", "--input-files", help="Input files", cls=OptionEatAll, type=tuple)
 @click.option("-o", "--output", help="Hub output directory", required=True)
 @click.option("--save-hub-design", help="Save hub design to file", type=str)
 @click.option(
     "-d",
@@ -66,24 +89,27 @@
     help="Infer details from filenames. Requires SAMPLENAME_[ANTIBODY]_[REPLICATE]",
     is_flag=True,
 )
 @click.option(
     "--hub-name",
     help="Name of hub to generate",
     default="HUB",
+    required=True,
 )
 @click.option(
     "--hub-email",
     help="Email address for hub",
     default="alastair.smith@ndcls.ox.ac.uk",
+    required=True,
 )
 @click.option(
     "--genome-name",
     help="Name of genome",
     default="hg19",
+    required=True,
 )
 @click.option(
     "--custom-genome",
     help="Determines if this is a custom genome",
     is_flag=True,
     default=False,
 )
```

### Comparing `tracknado-0.2/tracknado/old/cli.py` & `tracknado-0.2.1/tracknado/old/cli.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado/old/grouping.py` & `tracknado-0.2.1/tracknado/old/grouping.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado/old/hub_setup.py` & `tracknado-0.2.1/tracknado/old/hub_setup.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado/old/make_hub.py` & `tracknado-0.2.1/tracknado/old/make_hub.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado/old/track.py` & `tracknado-0.2.1/tracknado/old/track.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado/utils.py` & `tracknado-0.2.1/tracknado/utils.py`

 * *Files identical despite different names*

### Comparing `tracknado-0.2/tracknado.egg-info/PKG-INFO` & `tracknado-0.2.1/tracknado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracknado
-Version: 0.2
+Version: 0.2.1
 Summary: CLI library to generate UCSC trackhubs from sequencing data
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

