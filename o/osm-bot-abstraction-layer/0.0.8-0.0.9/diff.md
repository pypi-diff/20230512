# Comparing `tmp/osm_bot_abstraction_layer-0.0.8.tar.gz` & `tmp/osm_bot_abstraction_layer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/osm_bot_abstraction_layer-0.0.8.tar", last modified: Sat Feb 29 16:12:33 2020, max compression
+gzip compressed data, was "dist/osm_bot_abstraction_layer-0.0.9.tar", last modified: Wed Feb  3 14:00:18 2021, max compression
```

## Comparing `osm_bot_abstraction_layer-0.0.8.tar` & `osm_bot_abstraction_layer-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2020-02-29 16:12:33.000000 osm_bot_abstraction_layer-0.0.8/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     7498 2020-02-29 16:12:33.000000 osm_bot_abstraction_layer-0.0.8/PKG-INFO
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)     5987 2020-02-29 16:05:41.000000 osm_bot_abstraction_layer-0.0.8/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2020-02-29 16:12:33.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       48 2018-10-16 21:39:29.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/__init__.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)     5604 2020-02-29 16:02:42.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/generic_bot_retagging.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)    17023 2020-02-27 17:22:57.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/human_verification_mode.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)     5740 2019-05-29 06:30:25.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/osm_bot_abstraction_layer.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1414 2020-02-28 13:29:12.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/overpass_downloader.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)     2671 2019-03-26 12:23:01.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/split_into_packages.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)     1303 2019-05-28 09:13:49.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/world_data.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2020-02-29 16:12:33.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)     7498 2020-02-29 16:12:32.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/PKG-INFO
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)      597 2020-02-29 16:12:33.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/SOURCES.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)        1 2020-02-29 16:12:32.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/dependency_links.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)       87 2020-02-29 16:12:32.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/requires.txt
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)       26 2020-02-29 16:12:32.000000 osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2020-02-29 16:12:33.000000 osm_bot_abstraction_layer-0.0.8/setup.cfg
--rw-r--r--   0 mateusz   (1000) mateusz   (1001)      887 2020-02-29 16:06:41.000000 osm_bot_abstraction_layer-0.0.8/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2021-02-03 14:00:18.234476 osm_bot_abstraction_layer-0.0.9/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     7498 2021-02-03 14:00:18.234476 osm_bot_abstraction_layer-0.0.9/PKG-INFO
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)     5987 2020-02-29 16:05:41.000000 osm_bot_abstraction_layer-0.0.9/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2021-02-03 14:00:18.234476 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       48 2018-10-16 21:39:29.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/__init__.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)     5604 2020-02-29 16:02:42.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/generic_bot_retagging.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)    17290 2020-05-24 11:23:06.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/human_verification_mode.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)     5805 2020-05-25 17:03:04.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/osm_bot_abstraction_layer.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1700 2021-02-02 19:05:08.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/overpass_downloader.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)     2671 2019-03-26 12:23:01.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/split_into_packages.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)     1504 2020-11-26 12:52:59.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/world_data.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2021-02-03 14:00:18.234476 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)     7498 2021-02-03 14:00:18.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/PKG-INFO
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)      597 2021-02-03 14:00:18.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)        1 2021-02-03 14:00:18.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)      104 2021-02-03 14:00:18.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/requires.txt
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)       26 2021-02-03 14:00:18.000000 osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2021-02-03 14:00:18.234476 osm_bot_abstraction_layer-0.0.9/setup.cfg
+-rw-r--r--   0 mateusz   (1000) mateusz   (1001)      916 2021-02-03 13:58:52.000000 osm_bot_abstraction_layer-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `osm_bot_abstraction_layer-0.0.8/PKG-INFO` & `osm_bot_abstraction_layer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_bot_abstraction_layer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool for easier automation of OSM edits without causing problems.
 Home-page: https://github.com/matkoniecz/osm_bot_abstraction_layer
 Author: Mateusz Konieczny
 Author-email: matkoniecz@gmail.com
 License: UNKNOWN
 Description: OSM bot abstraction layer is a python package making easier to automate OSM edits without causing problems.
```

### Comparing `osm_bot_abstraction_layer-0.0.8/README.md` & `osm_bot_abstraction_layer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/generic_bot_retagging.py` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/generic_bot_retagging.py`

 * *Files identical despite different names*

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/human_verification_mode.py` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/human_verification_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return True
     if is_doctor(tags):
         return True
     if is_food_place(tags):
         return True
     if is_indoor_rentable_sleeping_place(tags):
         return True
-    if tags.get("amenity") in ["bank", "fuel", "post_office"]:
+    if tags.get("amenity") in ["bank", "fuel", "post_office", "cinema", "bureau_de_change"]:
         return True
     if tags.get("tourism") in ["museum"]:
         return True
     return False
 
 def is_rentable_sleeping_place(tags):
     if is_indoor_rentable_sleeping_place(tags):
@@ -137,14 +137,16 @@
         return True
     if check_potential_main_key(key, value, outdoor_rentable_sleeping_place_tag_listing()):
         return True
     if key == "highway" and value in road_types():
         return True
     if key == "building" and value in expected_building_values():
         return True
+    if key == "building:part" and value == "yes":
+        return True
     return False
 
 def is_any_matching_with_tag_listing(tags, tag_info):
     for key, value_list in tag_info.items():
         if tags.get(key) in value_list:
             return True
     return False
@@ -226,15 +228,15 @@
         return True
     if key in ["opening_hours:signed", "toilets", 'wifi', 'drive_through']:
         if value in ["yes", "no"]:
             return True
     if is_valid_wheelchair_tag(key, value):
         return True
     if key in ['building']:
-        if value in ["yes"]:
+        if value in expected_building_values():
             return True
     if is_valid_address_tag(key, value, tags):
         return True
     return False
 
 def is_valid_address_tag(key, value, tags):
     if key in list_of_address_tags():
@@ -243,18 +245,22 @@
 
 def is_valid_wheelchair_tag(key, value):
     if key in ['wheelchair']:
         if value in ["yes", "no", "limited"]:
             return True
     return False
 
-def is_building(tags):
-    return tags.get("building") in expected_building_values()
+def is_building_or_building_part(tags):
+    if tags.get("building:part") in expected_building_values():
+        return True
+    if tags.get("building") in expected_building_values():
+        return True
+    return False
 
-def is_tag_expected_for_building(key, value, tags):
+def is_tag_expected_for_building_or_building_part(key, value, tags):
     if key == "building:levels":
         if value in [str(i) for i in range(1, 20+1)]:
             return True
     if key == "roof:levels":
         if value in ["0", "1", "2"]:
             return True
     if key == "roof:shape":
@@ -328,46 +334,46 @@
         return True
     if is_good_main_tag(key, value):
         return True
     if key in ['source']:
         return True
     if is_expected_name_tag(key, value, tags):
         return True
-    if key == "surface":
-        if tags.get('highway') in road_types():
+    if tags.get('highway') in road_types():
+        if key == "surface":
             if value in (unpaved_road_surfaces() + paved_road_surfaces()):
                 return True
-            if key == "oneway" and value == "yes":
-                return True
-            if key == "lanes" and value == "2":
-                return True
-            if tags.get("oneway") == "yes" and tags.get("highway") != "motorway":
-                return True
-            if key == "bridge" and value in ["yes", "viaduct", "no"]:
-                return True
-            if key == "tunnel" and value in ["yes", "no"]:
-                return True
+        if key == "oneway" and value == "yes":
+            return True
+        if key == "lanes" and value == "2":
+            return True
+        if tags.get("oneway") == "yes" and tags.get("highway") != "motorway":
+            return True
+        if key == "bridge" and value in ["yes", "viaduct", "no"]:
+            return True
+        if key == "tunnel" and value in ["yes", "no"]:
+            return True
     if key == "construction":
         if tags.get("building") == "construction":
             if value in expected_building_values():
                 if value != "construction":
                     return True
         if tags.get("highway") == "construction":
             if value in road_types():
                 if value != "construction":
                     return True
     if is_lit_tag_expected(tags):
         if key == "lit":
-            if lit in ["yes", "no"]:
+            if value in ["yes", "no"]:
                 return True
     if key == "internet_access":
         if value in ["wlan", "yes", "wifi", "wired"]:
             return True
-    if is_building(tags):
-        if is_tag_expected_for_building(key, value, tags):
+    if is_building_or_building_part(tags):
+        if is_tag_expected_for_building_or_building_part(key, value, tags):
             return True
     if is_indoor_poi(tags):
         if is_tag_expected_for_indoor_poi(key, value, tags):
             return True
     if is_indoor_rentable_sleeping_place(tags):
         if key == "stars" and value in ["1", "2", "3", "4", "5"]:
             return True
```

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/osm_bot_abstraction_layer.py` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/osm_bot_abstraction_layer.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,29 +106,29 @@
     builder = ChangesetBuilder(affected_objects_description, comment, automatic_status, discussion_url, osm_wiki_documentation_page, source, other_tags_dict)
     builder.create_changeset(api)
     update_element(api, type, data)
     api.ChangesetClose()
     if sleeping_time != 0:
         sleep(sleeping_time)
 
-def get_and_verify_data(osm_object_url, prerequisites, failure_callback=None):
+def get_and_verify_data(osm_object_url, prerequisites, prerequisite_failure_callback=None):
     type = osm_object_url.split("/")[3]
     id = osm_object_url.split("/")[4]
     data = get_data(id, type)
     if data == None:
         return None
-    failure = prerequisite_failure_reason(osm_object_url, prerequisites, data, failure_callback)
+    failure = prerequisite_failure_reason(osm_object_url, prerequisites, data, prerequisite_failure_callback)
     if failure != None:
         print(failure)
         return None
     return data
 
-def prerequisite_failure_reason(osm_object_url, prerequisites, data, failure_callback=None):
-    if failure_callback != None:
-        failure_reason = failure_callback(data)
+def prerequisite_failure_reason(osm_object_url, prerequisites, data, prerequisite_failure_callback=None):
+    if prerequisite_failure_callback != None:
+        failure_reason = prerequisite_failure_callback(data)
         if failure_reason != None:
             return osm_object_url + " failed with " + failure_reason
 
     for key in prerequisites.keys():
         if prerequisites[key] == None:
             if key in data['tag']:
                 return("failed " + key + " prerequisite, as key " + key + " was present for " + osm_object_url)
```

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/overpass_downloader.py` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/overpass_downloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 import urllib.request, urllib.error, urllib.parse
 import time
+from tqdm import tqdm
+import random
+
+def sleep(time_in_s):
+    for i in tqdm(range(time_in_s*10), ascii=True):
+        time.sleep(0.1)
 
 def download_overpass_query(query, filepath):
     query = urllib.parse.quote(query)
-    #url = "http://overpass-api.de/api/interpreter?data=" + query
-    url = "https://lz4.overpass-api.de/api/interpreter?data=" + query # force faster server
     # see https://github.com/westnordost/StreetComplete/blob/6740a0b03996b929f9cf74ddb0e6afac7e3fc48e/app/src/main/res/xml/preferences.xml#L99
+    faster_server ="https://lz4.overpass-api.de/api/interpreter"
+    alt_server = "http://z.overpass-api.de/api/interpreter"
+    server = random.choice([faster_server, alt_server])
+    url = server +"?data=" + query
     with open(filepath, 'w+') as file:
         file.write(overpass_download(url))
 
 def overpass_download(url):
+    print("sleeping before download")
+    sleep(20)
+    attempt = 0
     while True:
         try:
             print("downloading " + url)
             request = urllib.request.Request(url,headers={'User-Agent': 'overpass downloader for OSM bot'})
             response = urllib.request.urlopen(request, timeout=25000)
             print("succeded with", response.getcode(), "http code")
             return response.read().decode('utf-8')
         except urllib.error.HTTPError as e:
             print(e.getcode())
             if e.getcode() == 429 or e.getcode() == 503:
+                attempt += 1
                 print("sleeping before retry due to", e.getcode(), "error code")
-                time.sleep(60)
+                sleep(100)
                 print("retrying")
                 continue
             raise e
         except urllib.error.URLError as e:
             print(("URLError for url " + url))
             print(e)
             return
```

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/split_into_packages.py` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/split_into_packages.py`

 * *Files identical despite different names*

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer/world_data.py` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer/world_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,29 @@
       name = element.get_tag_value("name")
       if name != None:
         self.names.append(name)
 
     def collected_names (self):
       return self.names
 
-def list_of_area_divisions(area_iso_code, admin_level_of_split, temporary_storage_file):
-    """returns list with names of subdivisions of area with specific iso code
-    (for example PL for Poland), at specified aministrative level"""
-    for iso_tag in ["ISO3166-1", "ISO3166-1:alpha2", "ISO3166-2"]:
-      internal_division_query = """[out:xml][timeout:3600];
+def list_of_area_divisions_query(iso_tag, area_iso_code, admin_level_of_split):
+    return """[out:xml][timeout:3600];
   area
     ['""" + iso_tag + """'='""" + area_iso_code + """'] -> .parent_area;
   (
-    rel
-      (area.parent_area)
-      [admin_level=""" + str(admin_level_of_split) + """][boundary=administrative];
+    relation["admin_level"=""" + str(admin_level_of_split) + """]["boundary"="administrative"](area.parent_area);
   );
   out tags;"""
+
+def list_of_area_divisions(area_iso_code, admin_level_of_split, temporary_storage_file):
+    """returns list with names of subdivisions of area with specific iso code
+    (for example PL for Poland), at specified aministrative level"""
+    for iso_tag in ["ISO3166-1", "ISO3166-1:alpha2", "ISO3166-2"]:
+      internal_division_query = list_of_area_divisions_query(iso_tag, area_iso_code, admin_level_of_split)
+      print(internal_division_query)
       overpass_downloader.download_overpass_query(internal_division_query, temporary_storage_file)
       osm = Data(temporary_storage_file)
       names = NameCollector()
       osm.iterate_over_data(names)
       if names.collected_names() != []:
         return names.collected_names()
     raise area_iso_code + " not found"
```

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/PKG-INFO` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-bot-abstraction-layer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool for easier automation of OSM edits without causing problems.
 Home-page: https://github.com/matkoniecz/osm_bot_abstraction_layer
 Author: Mateusz Konieczny
 Author-email: matkoniecz@gmail.com
 License: UNKNOWN
 Description: OSM bot abstraction layer is a python package making easier to automate OSM edits without causing problems.
```

### Comparing `osm_bot_abstraction_layer-0.0.8/osm_bot_abstraction_layer.egg-info/SOURCES.txt` & `osm_bot_abstraction_layer-0.0.9/osm_bot_abstraction_layer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osm_bot_abstraction_layer-0.0.8/setup.py` & `osm_bot_abstraction_layer-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osm_bot_abstraction_layer",
-    version="0.0.8",
+    version="0.0.9",
     author="Mateusz Konieczny",
     author_email="matkoniecz@gmail.com",
     description="A tool for easier automation of OSM edits without causing problems.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/matkoniecz/osm_bot_abstraction_layer",
     packages=setuptools.find_packages(),
     install_requires = [
         'osmapi>=1.0.2, <2.0',
         'termcolor>=1.1.0, <2.0',
         'urllib3>=1.13.1, <2.0',
         'osm_iterator>=1.1.0, <2.0',
+        'tqdm>4.47.0, <5.0',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
 )
```

