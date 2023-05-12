# Comparing `tmp/terka-1.8.2.tar.gz` & `tmp/terka-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.8.2.tar", last modified: Thu May 11 15:33:46 2023, max compression
+gzip compressed data, was "terka-1.8.3.tar", last modified: Fri May 12 15:54:44 2023, max compression
```

## Comparing `terka-1.8.2.tar` & `terka-1.8.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-11 15:33:46.780932 terka-1.8.2/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-11 15:33:46.780932 terka-1.8.2/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-11 15:33:42.000000 terka-1.8.2/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.776928 terka-1.8.2/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.2/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.2/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.8.2/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.8.2/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    44867 2023-05-11 15:30:51.000000 terka-1.8.2/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.8.2/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.8.2/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.8.2/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.8.2/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.8.2/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.8.2/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.2/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.8.2/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.2/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    31687 2023-05-11 15:29:58.000000 terka-1.8.2/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.8.2/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.8.2/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.8.2/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.8.2/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7800 2023-05-11 15:27:57.000000 terka-1.8.2/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-11 15:33:46.780932 terka-1.8.2/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-11 15:33:46.000000 terka-1.8.2/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-11 15:33:46.000000 terka-1.8.2/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-11 15:33:46.000000 terka-1.8.2/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-11 15:33:46.000000 terka-1.8.2/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-11 15:33:46.000000 terka-1.8.2/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-11 15:33:46.000000 terka-1.8.2/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.953602 terka-1.8.3/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-12 15:54:44.953602 terka-1.8.3/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-12 15:54:44.953602 terka-1.8.3/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-12 15:54:38.000000 terka-1.8.3/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.949602 terka-1.8.3/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.3/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.953602 terka-1.8.3/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.3/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.8.3/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.8.3/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.953602 terka-1.8.3/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    44867 2023-05-11 15:30:51.000000 terka-1.8.3/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.8.3/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.953602 terka-1.8.3/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.8.3/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.8.3/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.8.3/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.8.3/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.8.3/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.953602 terka-1.8.3/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.3/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.8.3/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.953602 terka-1.8.3/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.3/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    32005 2023-05-11 20:45:27.000000 terka-1.8.3/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.8.3/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.8.3/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.8.3/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.8.3/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7800 2023-05-11 15:27:57.000000 terka-1.8.3/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-12 15:54:44.949602 terka-1.8.3/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-12 15:54:44.000000 terka-1.8.3/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-12 15:54:44.000000 terka-1.8.3/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-12 15:54:44.000000 terka-1.8.3/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-12 15:54:44.000000 terka-1.8.3/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-12 15:54:44.000000 terka-1.8.3/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-12 15:54:44.000000 terka-1.8.3/terka.egg-info/top_level.txt
```

### Comparing `terka-1.8.2/setup.py` & `terka-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.8.2",
+    version="1.8.3",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.8.2/terka/adapters/orm.py` & `terka-1.8.3/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/adapters/repository.py` & `terka-1.8.3/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/collaborators.py` & `terka-1.8.3/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/commands.py` & `terka-1.8.3/terka/domain/commands.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/commentary.py` & `terka-1.8.3/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/epic.py` & `terka-1.8.3/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/event_history.py` & `terka-1.8.3/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/project.py` & `terka-1.8.3/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/sprint.py` & `terka-1.8.3/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/story.py` & `terka-1.8.3/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/tag.py` & `terka-1.8.3/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/task.py` & `terka-1.8.3/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/domain/time_tracker.py` & `terka-1.8.3/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/entrypoints/cli.py` & `terka-1.8.3/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/service_layer/printer.py` & `terka-1.8.3/terka/service_layer/printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,15 +459,16 @@
                 table=table,
                 entities=completed_tasks,
                 default_columns=default_columns,
                 repo=repo,
                 story_points=completed_story_points,
                 show_window=show_window,
                 all_tasks=False,
-                view_level=view_level)
+                view_level=view_level,
+                custom_sort=custom_sort)
             if table.row_count:
                 self.console.print(f"[green]****COMPLETED TASKS*****[/green]")
                 self.console.print(table)
 
     def _get_attributes(self, obj) -> List[Tuple[str, str]]:
         import inspect
         attributes = []
@@ -566,28 +567,37 @@
                     custom_sort=None):
         if all_tasks:
             completed_tasks = []
         else:
             completed_tasks = None
             completed_story_points = None
         if not custom_sort:
-            custom_sort = "status.value"
-            reverse=True
+            custom_sort = "status"
+            reverse = True
+        elif custom_sort == "priority":
+            reverse = True
         else:
-            reverse=False
+            reverse = False
+        sorting = attrgetter(custom_sort)
+
+        def sorting_fn(x):
+            if hasattr(sorting(x), "value"):
+                return sorting(x).value
+            return sorting(x)
+
         if story_points:
             completed_story_points = []
-            sorting = attrgetter(custom_sort)
             entities = [
                 (entity, story_point)
                 for entity, story_point in sorted(zip(entities, story_points),
-                                                  key=lambda x: sorting(x[0]),
+                                                  key=lambda x: sorting_fn(x),
                                                   reverse=reverse)
             ]
         else:
+            entities.sort(key=lambda x: sorting_fn(x), reverse=reverse)
             completed_story_points = None
         for column in default_columns:
             table.add_column(column)
         for entity in entities:
             if story_points:
                 story_point = entity[1]
                 entity = entity[0]
```

### Comparing `terka-1.8.2/terka/service_layer/services.py` & `terka-1.8.3/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/service_layer/ui.py` & `terka-1.8.3/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/service_layer/vertical_layout.css` & `terka-1.8.3/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/service_layer/views.py` & `terka-1.8.3/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka/utils.py` & `terka-1.8.3/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.8.2/terka.egg-info/SOURCES.txt` & `terka-1.8.3/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

