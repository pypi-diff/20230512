# Comparing `tmp/parshift-0.2.1.tar.gz` & `tmp/parshift-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parshift-0.2.1.tar", last modified: Wed Mar 29 09:28:47 2023, max compression
+gzip compressed data, was "parshift-0.2.2.tar", last modified: Fri May 12 08:46:02 2023, max compression
```

## Comparing `parshift-0.2.1.tar` & `parshift-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:28:47.378987 parshift-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-29 09:28:35.000000 parshift-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-29 09:28:47.378987 parshift-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-29 09:28:35.000000 parshift-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:28:47.378987 parshift-0.2.1/parshift/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-29 09:28:35.000000 parshift-0.2.1/parshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-03-29 09:28:35.000000 parshift-0.2.1/parshift/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-29 09:28:35.000000 parshift-0.2.1/parshift/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-29 09:28:35.000000 parshift-0.2.1/parshift/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:28:47.378987 parshift-0.2.1/parshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-29 09:28:47.000000 parshift-0.2.1/parshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-29 09:28:47.000000 parshift-0.2.1/parshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:28:47.000000 parshift-0.2.1/parshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-29 09:28:47.000000 parshift-0.2.1/parshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 09:28:47.000000 parshift-0.2.1/parshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-29 09:28:35.000000 parshift-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:28:47.378987 parshift-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:28:47.378987 parshift-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-03-29 09:28:35.000000 parshift-0.2.1/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-29 09:28:35.000000 parshift-0.2.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-29 09:28:35.000000 parshift-0.2.1/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-12 08:45:55.000000 parshift-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-12 08:46:02.804889 parshift-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-12 08:45:55.000000 parshift-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/parshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/oo_parshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/parshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-12 08:45:55.000000 parshift-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:46:02.804889 parshift-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_oo_parshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_statistics.py
```

### Comparing `parshift-0.2.1/LICENSE` & `parshift-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parshift-0.2.1/PKG-INFO` & `parshift-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parshift
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package based on Gibson's framework (2003) for turn-taking in group conversation analysis.
 Author-email: Bruno Saraiva <bruno.saraiva@ulusofona.pt>, João Pedro Carvalho <joao.matos.carvalho@ulusofona.pt>, Nuno Fachada <nuno.fachada@ulusofona.pt>, Manuel Pita <manuel.pita@ulusofona.pt>
 License: MIT
 Project-URL: Homepage, https://github.com/bdfsaraiva/parshift
 Project-URL: Bug Tracker, https://github.com/bdfsaraiva/parshift/issues
 Project-URL: Documentation, https://bdfsaraiva.github.io/parshift/
 Keywords: python,conversation-analysis,participation-shifts,turn-taking
```

### Comparing `parshift-0.2.1/README.md` & `parshift-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `parshift-0.2.1/parshift/__init__.py` & `parshift-0.2.2/parshift/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 """API reference for the functions exported by ParShift."""
 
 __all__ = [
     "annotate",
     "cond_probs",
     "frequency_treemap",
     "conv2turns",
-    "pshift_type",
+    "propensities",
+    "pshift_class",
     "read_ccsv",
+    "Parshift",
 ]
 
 
-from parshift.annotation import annotate, conv2turns, pshift_type, read_ccsv
+from parshift.annotation import annotate, conv2turns, pshift_class, read_ccsv
+from parshift.oo_parshift import Parshift
 from parshift.plotting import frequency_treemap
-from parshift.statistics import cond_probs
+from parshift.statistics import cond_probs, propensities
```

### Comparing `parshift-0.2.1/parshift/annotation.py` & `parshift-0.2.2/parshift/annotation.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,34 +26,34 @@
     "A0-AY": "Turn Continuing",
     "AB-A0": "Turn Continuing",
     "AB-AY": "Turn Continuing",
 }
 
 # Expected column types
 _p_shift_cols = {
-    "id": np.int64,
-    "user_id": np.int64,
-    "message_text": str,
-    "reply_id": object,
+    "utterance_id": np.int64,
+    "speaker_id": str,
+    "utterance": str,
+    "reply_to_id": object,
     "target_id": object,
 }
 
 
 def read_ccsv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     **kwargs: Any,
 ) -> pd.DataFrame:
     """Read a conversation file in CSV format, validate it and return a dataframe.
 
     The conversation file should have the following columns:
 
-    - `id`: ID of the message (int)
-    - `user_id`: ID of the user sending the message (int)
-    - `message_text`: The message itself (string)
-    - `reply_id` or `target_id`: The reply ID or the target ID (int)
+    - `utterance_id`: ID of the message (int)
+    - `speaker_id`: ID of the user sending the message (str)
+    - `utterance`: The message itself (string)
+    - `reply_to_id` or `target_id`: The reply ID or the target ID (int)
 
     Arguments:
         filepath_or_buffer: Any valid string path to CSV file, as accepted by
             Pandas [`read_csv()`][pandas.read_csv] function.
         **kwargs: Keyword parameters passed to Pandas
             [`read_csv()`][pandas.read_csv] function.
 
@@ -65,21 +65,31 @@
     # Read the conversation file
     conversation: pd.DataFrame = pd.read_csv(filepath_or_buffer, dtype=_p_shift_cols, **kwargs)  # type: ignore
 
     # Obtain potentially missing columns
     missing = _p_shift_cols.keys() - conversation.columns
 
     # Check if we have missing columns
-    if len(missing) == 1 and "reply_id" not in missing and "target_id" not in missing:
-        # If only one column missing, it can't be other than `reply_id` or `target_id`
+    if (
+        len(missing) == 1
+        and "reply_to_id" not in missing
+        and "target_id" not in missing
+    ):
+        # If only one column missing, it can't be other than `reply_to_id` or `target_id`
         raise ValueError(f"CSV file is missing the `{missing.pop()}` column")
     elif len(missing) > 1:
         # If more than one column missing, we have a problem
         raise ValueError(f"CSV file is missing the `{'`, `'.join(missing)}` columns")
 
+    # Change Nan values to empty strings in the `reply_to_id` or `target_id` column
+    if "reply_to_id" in conversation.columns:
+        conversation["reply_to_id"] = conversation["reply_to_id"].fillna("")
+    else:
+        conversation["target_id"] = conversation["target_id"].fillna("")
+
     return conversation
 
 
 def conv2turns(conv_df: pd.DataFrame) -> List[Dict[str, Any]]:
     """Take a conversation dataframe and group it into conversation turns.
 
     A turn is a group of messages sent by the same user and addressed to the
@@ -89,61 +99,64 @@
         conv_df: The conversation from where to obtain the conversation turns.
 
     Returns:
         A list of dictionaries, each representing a conversation turn.
     """
 
     conv_df = conv_df.reset_index()
-    if "reply_id" in conv_df.columns:
-        last_col = "reply_id"
+    if "reply_to_id" in conv_df.columns:
+        last_col = "reply_to_id"
     elif "target_id" in conv_df.columns:
         last_col = "target_id"
 
     conversation: List[Dict[str, Any]] = []
     turn = 0
 
     for index, row in conv_df.iterrows():
-        # If the row being looped has the same "user_id" and the "last_col" value,
-        # then merge the message text and message IDs into the previous turn.
+        # If the row being looped has the same "speaker_id" and the "last_col" value,
+        # then merge the message text and message utterance_ids into the previous turn.
         if (
             index != 0
-            and conversation[turn - 1]["user_id"] == row["user_id"]
+            and conversation[turn - 1]["speaker_id"] == row["speaker_id"]
             and str(conversation[turn - 1][last_col]) == row[last_col]
         ):
             msg_join = ". ".join(
-                [conversation[turn - 1]["message_text"], row["message_text"]]
+                [conversation[turn - 1]["utterance"], row["utterance"]]
             )
-            list_id = conversation[turn - 1]["ids"] + [row["id"]]
-            conversation[turn - 1]["ids"] = list_id
-            conversation[turn - 1]["message_text"] = msg_join
+            list_id = conversation[turn - 1]["utterance_ids"] + [row["utterance_id"]]
+            conversation[turn - 1]["utterance_ids"] = list_id
+            conversation[turn - 1]["utterance"] = msg_join
 
         # Otherwise, create a new dictionary representing a new turn
         else:
-            id = row["id"]
-            user_id = row["user_id"]
-            message_text = row["message_text"]
+            id = row["utterance_id"]
+            speaker_id = row["speaker_id"]
+            utterance = row["utterance"]
             last_col_val = row[last_col]
 
             conversation.append(
                 {
-                    "ids": [id],
-                    "user_id": user_id,
-                    "message_text": message_text,
-                    last_col: int(last_col_val) if last_col_val != "None" else None,
+                    "utterance_ids": [id],
+                    "speaker_id": speaker_id,
+                    "utterance": utterance,
+                    last_col: int(last_col_val)
+                    if last_col_val != ""
+                    and last_col_val != None
+                    and last_col_val != "None"
+                    else None,
                 }
             )
 
             # Increment the turn counter
             turn += 1
 
     return conversation
 
 
 def _pshift_code(label: str) -> str:
-
     # split the label into 4 parts
     a = label.split(",")[0].split("to")[0].replace(" ", "")
     b = label.split(",")[0].split("to")[1].replace(" ", "")
     c = label.split(",")[1].split("to")[0].replace(" ", "")
     d = label.split(",")[1].split("to")[1].replace(" ", "")
 
     # Part 1 - always starts with A
@@ -196,56 +209,59 @@
 
     # part1 will take the parshift label for the previous turn
     part_1 = ""
 
     # part2 will take the parshift label for the current turn
     part_2 = ""
 
-    if "reply_id" in conv_df.columns:
+    if "reply_to_id" in conv_df.columns:
         annotate_df = pd.DataFrame(
             {
-                "ids": [],
-                "user_id": [],
-                "message_text": [],
-                "reply_id": [],
+                "utterance_ids": [],
+                "speaker_id": [],
+                "utterance": [],
+                "reply_to_id": [],
                 "label_desc": [],
                 "pshift": [],
             }
         )
 
         # calculate the participation shift for each turn
         for idx, msg in enumerate(conversation):
             if (
-                msg["reply_id"] == None
-                or msg["reply_id"] == "None"
-                or msg["reply_id"] == ""
+                msg["reply_to_id"] == None
+                or msg["reply_to_id"] == "None"
+                or msg["reply_to_id"] == ""
             ):
-                part_2 = " " + str(msg["user_id"]) + " to group"
+                part_2 = " " + str(msg["speaker_id"]) + " to group"
             else:
                 for msgPrev in conversation[: idx + 1]:
-                    if msg["reply_id"] in msgPrev["ids"]:
+                    if msg["reply_to_id"] in msgPrev["utterance_ids"]:
                         if (
-                            msgPrev["reply_id"] == None
-                            or msgPrev["reply_id"] == "None"
-                            or msgPrev["reply_id"] == ""
+                            msgPrev["reply_to_id"] == None
+                            or msgPrev["reply_to_id"] == "None"
+                            or msgPrev["reply_to_id"] == ""
                         ):
-                            part_1 = str(msgPrev["user_id"]) + " to group,"
+                            part_1 = str(msgPrev["speaker_id"]) + " to group,"
 
                         else:  # reply - reply
                             for msgPrev2 in conversation[:idx]:
-                                if msgPrev["reply_id"] in msgPrev2["ids"]:
+                                if msgPrev["reply_to_id"] in msgPrev2["utterance_ids"]:
                                     part_1 = (
-                                        str(msgPrev["user_id"])
+                                        str(msgPrev["speaker_id"])
                                         + " to "
-                                        + str(msgPrev2["user_id"])
+                                        + str(msgPrev2["speaker_id"])
                                         + ","
                                     )
 
                         part_2 = (
-                            " " + str(msg["user_id"]) + " to " + str(msgPrev["user_id"])
+                            " "
+                            + str(msg["speaker_id"])
+                            + " to "
+                            + str(msgPrev["speaker_id"])
                         )
 
             # p1p2 takes the parshift label for the previous + current turn
             p1p2 = part_1 + part_2
 
             # part_1 takes the part_2 label for the next iteration
             part_1 = part_2[1:] + ","
@@ -254,47 +270,47 @@
             pshift_label = ""
 
             # we cannot calculate the pshift for the first turn
             if idx != 0:
                 pshift_label = _pshift_code(p1p2)
 
             annotate_df.loc[len(annotate_df.index)] = [  # type: ignore
-                str(msg["ids"]),
-                str(msg["user_id"]),
-                msg["message_text"],
-                str(msg["reply_id"]),
+                str(msg["utterance_ids"]),
+                str(msg["speaker_id"]),
+                msg["utterance"],
+                str(msg["reply_to_id"]),
                 p1p2,
                 pshift_label,
             ]
 
     elif "target_id" in conv_df.columns:
         annotate_df = pd.DataFrame(
             {
-                "ids": [],
-                "user_id": [],
-                "message_text": [],
+                "utterance_ids": [],
+                "speaker_id": [],
+                "utterance": [],
                 "target_id": [],
                 "label_desc": [],
                 "pshift": [],
             }
         )
 
         # calculate the participation shift for each turn
         for idx, msg in enumerate(conversation):
             # if msg has no target, it is directed to the group
             if (
                 msg["target_id"] == None
                 or msg["target_id"] == "None"
                 or msg["target_id"] == ""
             ):
-                part_2 = " " + str(msg["user_id"]) + " to group"
+                part_2 = " " + str(msg["speaker_id"]) + " to group"
 
             # if msg has a target, we save it
             else:
-                part_2 = " " + str(msg["user_id"]) + " to " + str(msg["target_id"])
+                part_2 = " " + str(msg["speaker_id"]) + " to " + str(msg["target_id"])
 
             # p1p2 takes the parshift label for the previous + current turn
             p1p2 = part_1 + part_2
 
             # part_1 takes the part_2 label for the next iteration
             part_1 = part_2[1:] + ","
 
@@ -304,37 +320,37 @@
             # we cannot calculate the pshift for the first turn
             if idx != 0:
                 msg["label"] = p1p2
                 pshift_label = _pshift_code(p1p2)
                 msg["pshift"] = pshift_label
 
             annotate_df.loc[len(annotate_df.index)] = [  # type: ignore
-                str(msg["ids"]),
-                str(msg["user_id"]),
-                msg["message_text"],
+                str(msg["utterance_ids"]),
+                str(msg["speaker_id"]),
+                msg["utterance"],
                 str(msg["target_id"]),
                 p1p2,
                 pshift_label,
             ]
 
     annotate_df.drop(columns=["label_desc"], inplace=True)
 
     return annotate_df
 
 
-def pshift_type(pshift_code: str) -> str:
-    """Returns the participation shift type given a participation shift code.
+def pshift_class(pshift: str) -> str:
+    """Returns the participation shift class given a participation shift code.
 
     Arguments:
-        pshift_code: Participation shift code (e.g A0-XA).
+        pshift: Participation shift code (e.g A0-XA).
 
     Returns:
-        Participation shift type in given the participation shift code (either
+        Participation shift classe in given the participation shift code (either
             "Turn Receiving", "Turn Claiming", "Turn Usurping" or  "Turn Continuing").
     """
 
-    if not isinstance(pshift_code, str):
+    if not isinstance(pshift, str):
         raise TypeError("Parameter pshift_code must be a String")
-    if not re.search("A[B|0]-[A|B|X][A|B|X|Y|0]", pshift_code):
+    if not re.search("A[B|0]-[A|B|X][A|B|X|Y|0]", pshift):
         raise ValueError("Parameter pshift_code must be a parshift code. eg: AB-B0")
 
-    return _p_shift_dict[pshift_code]
+    return _p_shift_dict[pshift]
```

### Comparing `parshift-0.2.1/parshift/plotting.py` & `parshift-0.2.2/parshift/plotting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,88 @@
 # Copyright (c) 2022-2023 Bruno Saraiva and contributors
 # Distributed under the MIT License (See accompanying file LICENSE or copy
 # at http://opensource.org/licenses/MIT)
 
 import matplotlib
 import matplotlib.pyplot as plt
 import pandas as pd
-import seaborn as sns
 import squarify
 
-from .annotation import pshift_type
+from .annotation import pshift_class
 
 
 def frequency_treemap(
     cond_probs_df: pd.DataFrame,
     ax: matplotlib.axes.Axes = None,
-    column_name: str = "pshift",
+    type: str = "Pshift",
 ) -> matplotlib.axes.Axes:
     """Get a matplotlib axes object displaying the conditional probabilities or frequencies.
 
     Arguments:
         cond_probs_df: Dataframe with information about the participation shift
             conditional probabilities. This dataframe can be obtained with
             [`cond_probs()`][parshift.statistics.cond_probs]
-        column_name: Column name to be used to plot the treemap, either `"pshift"`
-            (default) or `"pshift_type"`.
+        type: Column name to be used to plot the treemap, either `"Pshift"`
+            (default) or `"Pshift_class"`.
         ax: Matplotlib axes with the treemap plot.
 
     Returns:
         ax: Matplotlib axes with the participation shifts probabilities or frequency.
     """
 
-    if not isinstance(column_name, str):
+    if not isinstance(type, str):
         raise TypeError("Parameter filename must be a String")
-    if column_name not in ["pshift_type", "pshift"]:
+    if type not in ["Pshift_class", "Pshift"]:
         raise ValueError(
-            "Parameter column_name must be one of the following: `pshift`, `pshift_type`"
+            "Parameter type must be one of the following: `Pshift`, `Pshift_class`"
         )
 
-    if column_name == "pshift_type":
-        cond_probs_df["pshift_type"] = cond_probs_df["pshift"].apply(pshift_type)
+    if type == "Pshift_class":
+        cond_probs_df["Pshift_class"] = cond_probs_df["Pshift"].apply(pshift_class)
 
-    gb_parshift = cond_probs_df.groupby([column_name])["Frequency"].sum()
+    gb_parshift = cond_probs_df.groupby([type])["Frequency"].sum()
 
     data = [
         el
         for el in list(zip(gb_parshift.values, gb_parshift.index.values))
         if el[0] != 0
     ]
     labels = [
         f"{el} \n {round( 100 * (list(zip(*data))[0][idx] / sum(list(list(zip(*data))[0]))),1)}%"
         for idx, el in enumerate(list(zip(*data))[1])
     ]
 
+    color_dict = {
+        "Turn Receiving": "#86d87c",
+        "AB-BA": "#86d87c",
+        "AB-B0": "#c6ecbe",
+        "AB-BY": "#7cd892",
+        "Turn Claiming": "#f4b461",
+        "A0-X0": "#f4b461",
+        "A0-XA": "#fb9948",
+        "A0-XY": "#efa107",
+        "Turn Usurping": "#ff4d4d",
+        "AB-X0": "#ff4d4d",
+        "AB-XA": "#fb7477",
+        "AB-XB": "#ef3b6e",
+        "AB-XY": "#ef483b",
+        "Turn Continuing": "#85eff9",
+        "A0-AY": "#3b61ef",
+        "AB-A0": "#85eff9",
+        "AB-AY": "#b9befb",
+    }
+
+    colors = [color_dict[el] for el in list(zip(*data))[1]]
+
     if ax is None:
         _, ax = plt.subplots()
 
     squarify.plot(
         list(zip(*data))[0],
         label=labels,
         pad=2,
-        color=sns.color_palette("Spectral", len(list(zip(*data))[0])),
+        color=colors,
         ax=ax,
     )
-    plt.title("Participation Shifts Frequency (%)")
+    # plt.title("Participation Shifts Frequency (%)")
     plt.axis("off")
-
     return ax
```

### Comparing `parshift-0.2.1/parshift/statistics.py` & `parshift-0.2.2/parshift/statistics.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,52 @@
     "AB-XY": 11,
     "A0-AY": 3,
     "AB-A0": 9,
     "AB-AY": 12,
 }
 
 
+def _change_of_speaker(ps):
+    _change_of_speaker_dic = {
+        "AB-BA": True,
+        "AB-B0": True,
+        "AB-BY": True,
+        "A0-X0": True,
+        "A0-XA": True,
+        "A0-XY": True,
+        "AB-X0": True,
+        "AB-XA": True,
+        "AB-XB": True,
+        "AB-XY": True,
+        "A0-AY": False,
+        "AB-A0": False,
+        "AB-AY": False,
+    }
+    return _change_of_speaker_dic[ps]
+
+
+def _targeted_remark(ps):
+    _targeted_remark_dic = {
+        "AB-BA": True,
+        "AB-B0": True,
+        "AB-BY": True,
+        "A0-X0": False,
+        "A0-XA": False,
+        "A0-XY": False,
+        "AB-X0": True,
+        "AB-XA": True,
+        "AB-XB": True,
+        "AB-XY": True,
+        "A0-AY": False,
+        "AB-A0": True,
+        "AB-AY": True,
+    }
+    return _targeted_remark_dic[ps]
+
+
 def _frequency_table(parshift_annotation_df) -> list:
     """
     This function takes in a dataframe of ParShift annotations and returns a frequency table of ParShift codes.
 
     Arguments:
         parshift_annotation_df: A Pandas dataframe containing ParShift annotations
 
@@ -57,15 +95,15 @@
     count_start_A0_total = 0
     count_start_AB_total = 0
     count_not_turn_continuing_A0 = 0
     count_not_turn_continuing_AB = 0
 
     for code in parshift_codes:
         count = 0
-        for index, row in parshift_annotation_df.iterrows():
+        for _, row in parshift_annotation_df.iterrows():
             if row["pshift"] == code:
                 count += 1
 
         dict_prob_empirical_count[code] = count
 
         if code.split("-")[0] == "A0":
             count_start_A0_total += count
@@ -92,49 +130,62 @@
         pshift_codes: A sequence of participation shift code obtained with
             [`annotate()`][parshift.annotation.annotate].
 
     Returns:
         A dataframe containing the frequency, probability and conditional probabilities
             (two) for each parshift code. This dataframe is divided into two 'subgroups':
             (1) those beginning with an undirected remark (A0-); and, (2) those beginning
-            with a directed one (AB-). The `CP` (conditional probability) column contains
-            the frequency divided by total occurrences in each subgroup, while the `CPeTC`
-            (Conditional Probability excluding Turn Continuing type) column contains the
-            frequency divided by total occurrences in each subgroup, assuming change of
-            speaker.
+            with a directed one (AB-). The `P(S|D)` (Probability of a participation shift
+            given a Directed or Undirected remark (D)) column contains the frequency divided
+            by total occurrences in each subgroup, while the `P(S|D and C)` (Probability of
+            a participation shift given a Directed or Undirected remark (D) and assuming
+            Change of Speaker (C)) column contains the frequency divided by total occurrences
+            in each subgroup, for each participation shift where the change of speaker occurs.
     """
 
     if not isinstance(pshift_codes, pd.DataFrame):
         raise TypeError("Parameter parshift_annotation_df must be a Dataframe")
 
     frequency_table_and_counts = _frequency_table(pshift_codes)
     freq_table = frequency_table_and_counts[0]
 
     cond_prob = {}
     for key in freq_table:
         if key.split("-")[0] == "A0":
             if key not in ["A0-AY", "AB-A0", "AB-AY", "A0-A0"]:
                 cond_prob[key] = {
-                    "CP": round(freq_table[key] / frequency_table_and_counts[1], 2),
-                    "CPeTC": round(freq_table[key] / frequency_table_and_counts[3], 2),
+                    "CP": round(freq_table[key] / frequency_table_and_counts[1], 2)
+                    if frequency_table_and_counts[1] != 0
+                    else 0,
+                    "CPeTC": round(freq_table[key] / frequency_table_and_counts[3], 2)
+                    if frequency_table_and_counts[3] != 0
+                    else 0,
                 }
             else:
                 cond_prob[key] = {
-                    "CP": round(freq_table[key] / frequency_table_and_counts[1], 2),
+                    "CP": round(freq_table[key] / frequency_table_and_counts[1], 2)
+                    if frequency_table_and_counts[1] != 0
+                    else 0,
                     "CPeTC": "",
                 }
         else:
             if key not in ["A0-AY", "AB-A0", "AB-AY", "A0-A0"]:
                 cond_prob[key] = {
-                    "CP": round(freq_table[key] / frequency_table_and_counts[2], 2),
-                    "CPeTC": round(freq_table[key] / frequency_table_and_counts[4], 2),
+                    "CP": round(freq_table[key] / frequency_table_and_counts[2], 2)
+                    if frequency_table_and_counts[2] != 0
+                    else 0,
+                    "CPeTC": round(freq_table[key] / frequency_table_and_counts[4], 2)
+                    if frequency_table_and_counts[4] != 0
+                    else 0,
                 }
             else:
                 cond_prob[key] = {
-                    "CP": round(freq_table[key] / frequency_table_and_counts[2], 2),
+                    "CP": round(freq_table[key] / frequency_table_and_counts[2], 2)
+                    if frequency_table_and_counts[2] != 0
+                    else 0,
                     "CPeTC": "",
                 }
 
     cond_prob_df = pd.DataFrame.from_dict(cond_prob, orient="index")
     freq = pd.DataFrame.from_dict(freq_table, orient="index", columns=["Frequency"])
     freq["Probability"] = round(freq["Frequency"] / freq["Frequency"].sum(), 2)
 
@@ -144,9 +195,51 @@
         .rename(columns={"index": "pshift"})
     )
 
     result = result.sort_values(
         by=["pshift"], key=lambda x: x.map(_cp_order)
     ).reset_index(drop=True)
 
-    result_ordered = result.iloc[:, [0, 1, 2, 3, 4]]
-    return result_ordered
+    result = result.iloc[:, [0, 1, 2, 3, 4]]
+
+    result["Change of Speaker (C)"] = result["pshift"].apply(
+        lambda ps: _change_of_speaker(ps)
+    )
+
+    result["Directed Remark (D)"] = result["pshift"].apply(
+        lambda ps: _targeted_remark(ps)
+    )
+
+    result.rename(
+        columns={"pshift": "Pshift", "CP": "P(S|D)", "CPeTC": "P(S|D and C)"},
+        inplace=True,
+    )
+
+    return result
+
+
+def propensities(cond_probs_df: pd.DataFrame) -> pd.DataFrame:
+    """Determine the propensities from a conditional probabilities dataframe.
+
+    Arguments:
+        cond_probs_df: A dataframe with statistics obtained with
+            [`cond_probs()`][parshift.statistics.cond_probs].
+
+    Returns:
+        A dataframe containing the propensities proposed by Gibson.
+    """
+
+    dic_propensities = {}
+
+    # turn-receiving propensity -> AB-BA, AB-BO, and AB-BY ( P(S|D) )
+    p_s_d = cond_probs_df["P(S|D)"]
+    p_s_d_c = cond_probs_df["P(S|D and C)"]
+
+    dic_propensities["turn-receiving"] = p_s_d[4] + p_s_d[5] + p_s_d[10]
+
+    # targeting propensity -> AO-XY, AB-BY and AB-XY ( P(S|D and C) )
+    dic_propensities["targeting"] = p_s_d_c[2] + p_s_d_c[10] + p_s_d_c[11]
+
+    # termination propensity -> AO-AY, AB-AO and AB-AY ( P(S|D) )
+    dic_propensities["termination"] = p_s_d[2] + p_s_d[9] + p_s_d[12]
+
+    return pd.DataFrame([dic_propensities])
```

### Comparing `parshift-0.2.1/parshift.egg-info/PKG-INFO` & `parshift-0.2.2/parshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parshift
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package based on Gibson's framework (2003) for turn-taking in group conversation analysis.
 Author-email: Bruno Saraiva <bruno.saraiva@ulusofona.pt>, João Pedro Carvalho <joao.matos.carvalho@ulusofona.pt>, Nuno Fachada <nuno.fachada@ulusofona.pt>, Manuel Pita <manuel.pita@ulusofona.pt>
 License: MIT
 Project-URL: Homepage, https://github.com/bdfsaraiva/parshift
 Project-URL: Bug Tracker, https://github.com/bdfsaraiva/parshift/issues
 Project-URL: Documentation, https://bdfsaraiva.github.io/parshift/
 Keywords: python,conversation-analysis,participation-shifts,turn-taking
```

### Comparing `parshift-0.2.1/pyproject.toml` & `parshift-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["parshift"]
 
 [project]
 name = "parshift"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python package based on Gibson's framework (2003) for turn-taking in group conversation analysis."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "python",
     "conversation-analysis",
     "participation-shifts",
     "turn-taking" ]
 license = {text = "MIT"}
 authors = [
     {name = "Bruno Saraiva", email = "bruno.saraiva@ulusofona.pt"},
     {name = "João Pedro Carvalho", email = "joao.matos.carvalho@ulusofona.pt" },
     {name = "Nuno Fachada", email = "nuno.fachada@ulusofona.pt" },
     {name = "Manuel Pita", email = "manuel.pita@ulusofona.pt" } ]
-dependencies = ["pandas", "matplotlib", "squarify", "seaborn"]
+dependencies = ["pandas", "matplotlib", "squarify"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering" ]
 
@@ -61,15 +61,15 @@
     "__pycache__" ]
 testpaths = ["parshift", "tests"]
 
 [tool.mypy]
 python_version = 3.8
 
 [[tool.mypy.overrides]]
-module = [ "squarify", "matplotlib", "matplotlib.pyplot", "seaborn" ]
+module = [ "squarify", "matplotlib", "matplotlib.pyplot"]
 ignore_missing_imports = true
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
 include = '\.pyi?$'
 exclude = '''
```

### Comparing `parshift-0.2.1/tests/test_annotation.py` & `parshift-0.2.2/tests/test_annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2022-2023 Bruno Saraiva and contributors
 # Distributed under the MIT License (See accompanying file LICENSE or copy
 # at http://opensource.org/licenses/MIT)
 
 import pandas as pd
 import pytest
 
-from parshift import annotate, pshift_type, read_ccsv
+from parshift import annotate, pshift_class, read_ccsv
 
 
 def test_read_ccsv_return(file_csv_good, p_shift_cols_mandatory, p_shift_cols_optional):
     """Test that `read_ccsv()` returns a data frame with the appropriate columns."""
 
     # Get the object read by read_ccsv()
     df_conv = read_ccsv(file_csv_good["csv_in"], **(file_csv_good["kwargs"]))
@@ -92,15 +92,15 @@
         ("A0-AY", "Turn Continuing"),
         ("AB-A0", "Turn Continuing"),
         ("AB-AY", "Turn Continuing"),
     ],
 )
 def test_pshift_type_return(ps, pstype):
     """Test that `pshift_type()` returns the expected type of p-shift."""
-    assert pshift_type(ps) == pstype
+    assert pshift_class(ps) == pstype
 
 
 @pytest.mark.parametrize("ps,expecterr", [(1, TypeError), ("hi", ValueError)])
 def test_pshift_type_errors(ps, expecterr):
     """Test that `pshift_type()` throws the expected errors."""
     with pytest.raises(expecterr):
-        pshift_type(ps)
+        pshift_class(ps)
```

### Comparing `parshift-0.2.1/tests/test_plotting.py` & `parshift-0.2.2/tests/test_plotting.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 def test_frequency_treemap(pshift_freq_table):
     conditional_probabilities_df = cond_probs(pshift_freq_table["df_ps"])
     _, ax = plt.subplots()
     assert type(ax) == type(frequency_treemap(conditional_probabilities_df))
     assert type(ax) == type(
-        frequency_treemap(conditional_probabilities_df, column_name="pshift_type")
+        frequency_treemap(conditional_probabilities_df, type="Pshift_class")
     )
 
 
-@pytest.mark.parametrize("column_name,expecterr", [(1, TypeError), ("Bye", ValueError)])
-def test_frequency_treemap_errors(pshift_freq_table, column_name, expecterr):
+@pytest.mark.parametrize("type,expecterr", [(1, TypeError), ("Bye", ValueError)])
+def test_frequency_treemap_errors(pshift_freq_table, type, expecterr):
     conditional_probabilities_df = cond_probs(pshift_freq_table["df_ps"])
     with pytest.raises(expecterr):
-        frequency_treemap(conditional_probabilities_df, column_name=column_name)
+        frequency_treemap(conditional_probabilities_df, type=type)
```

