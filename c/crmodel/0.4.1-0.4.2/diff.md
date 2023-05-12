# Comparing `tmp/crmodel-0.4.1.tar.gz` & `tmp/crmodel-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crmodel-0.4.1.tar", last modified: Thu Mar  2 21:28:15 2023, max compression
+gzip compressed data, was "crmodel-0.4.2.tar", last modified: Fri May 12 13:22:28 2023, max compression
```

## Comparing `crmodel-0.4.1.tar` & `crmodel-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-03-02 21:28:15.535603 crmodel-0.4.1/
--rw-r--r--   0 jeremy     (501) staff       (20)    35147 2023-01-16 12:55:21.000000 crmodel-0.4.1/LICENSE
--rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-01-16 12:55:21.000000 crmodel-0.4.1/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-03-02 21:28:15.535402 crmodel-0.4.1/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)     1111 2023-01-16 12:55:21.000000 crmodel-0.4.1/README.md
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-03-02 21:28:15.533927 crmodel-0.4.1/crmodel/
--rw-r--r--   0 jeremy     (501) staff       (20)     1059 2023-01-16 12:55:21.000000 crmodel-0.4.1/crmodel/config.py
--rw-r--r--   0 jeremy     (501) staff       (20)    18389 2023-03-02 21:22:54.000000 crmodel-0.4.1/crmodel/crmodel.py
--rw-r--r--   0 jeremy     (501) staff       (20)     7796 2023-03-01 15:55:33.000000 crmodel-0.4.1/crmodel/model.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1769 2023-01-16 12:55:21.000000 crmodel-0.4.1/crmodel/segmentationReader.py
--rw-r--r--   0 jeremy     (501) staff       (20)     8394 2023-03-02 21:22:47.000000 crmodel-0.4.1/crmodel/utils.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-03-02 21:28:15.535111 crmodel-0.4.1/crmodel.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-03-02 21:28:15.000000 crmodel-0.4.1/crmodel.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      310 2023-03-02 21:28:15.000000 crmodel-0.4.1/crmodel.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-03-02 21:28:15.000000 crmodel-0.4.1/crmodel.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       90 2023-03-02 21:28:15.000000 crmodel-0.4.1/crmodel.egg-info/requires.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        8 2023-03-02 21:28:15.000000 crmodel-0.4.1/crmodel.egg-info/top_level.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       96 2023-03-01 15:55:33.000000 crmodel-0.4.1/requirements.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-03-02 21:28:15.535681 crmodel-0.4.1/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)     1092 2023-03-02 21:27:56.000000 crmodel-0.4.1/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-12 13:22:28.212648 crmodel-0.4.2/
+-rw-r--r--   0 jeremy     (501) staff       (20)    35147 2023-01-16 12:55:21.000000 crmodel-0.4.2/LICENSE
+-rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-01-16 12:55:21.000000 crmodel-0.4.2/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-05-12 13:22:28.212494 crmodel-0.4.2/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)     1111 2023-01-16 12:55:21.000000 crmodel-0.4.2/README.md
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-12 13:22:28.211490 crmodel-0.4.2/crmodel/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-05-12 12:29:12.000000 crmodel-0.4.2/crmodel/config.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    18474 2023-05-12 13:20:50.000000 crmodel-0.4.2/crmodel/crmodel.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     7859 2023-05-12 13:09:16.000000 crmodel-0.4.2/crmodel/model.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1769 2023-01-16 12:55:21.000000 crmodel-0.4.2/crmodel/segmentationReader.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     8394 2023-03-02 21:22:47.000000 crmodel-0.4.2/crmodel/utils.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-12 13:22:28.212292 crmodel-0.4.2/crmodel.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      310 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        8 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/top_level.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-05-12 12:16:26.000000 crmodel-0.4.2/requirements.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-05-12 13:22:28.212754 crmodel-0.4.2/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)     1092 2023-05-12 13:22:08.000000 crmodel-0.4.2/setup.py
```

### Comparing `crmodel-0.4.1/LICENSE` & `crmodel-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.1/PKG-INFO` & `crmodel-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crmodel
-Version: 0.4.1
+Version: 0.4.2
 Summary: crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.
 Home-page: https://github.com/jeremyk6/crmodel
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crmodel-0.4.1/README.md` & `crmodel-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.1/crmodel/config.py` & `crmodel-0.4.2/crmodel/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 node_tags_to_keep = [
     # general informations
     'highway',
     # crosswalk informations
     'crossing',
     'tactile_paving',
+    'foot',
     # traffic signals informations
     'traffic_signals',
     'traffic_signals:direction',
     'traffic_signals:sound',
     'button_operated'
     #sidewalk informations
     'kerb',
```

### Comparing `crmodel-0.4.1/crmodel/crmodel.py` & `crmodel-0.4.2/crmodel/crmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -342,53 +342,53 @@
         branches_ways = []
         for branch in self.crossroad.branches:
             for way in branch.ways:
                 n1 = way.junctions[0]
                 n2 = way.junctions[1]
                 features.append(Feature(geometry=LineString([(n1.x, n1.y), (n2.x, n2.y)]), properties={
                     "id" : str(branch.number),
-                    "osm_node_ids" : [n1.id, n2.id],
-                    "osm_way_id" : way.osmid[0],
+                    "osm_node_ids" : [str(n1.id), str(n2.id)],
+                    "osm_way_id" : str(way.osmid[0]),
                     "type" : "branch",
                     "name" : way.name,
                     "lanes" : [{"type" : channel.__class__.__name__, "direction" : channel.direction} for channel in way.channels],
-                    "left_sidewalk" : way.sidewalks[0].id if way.sidewalks[0] else None,
-                    "right_sidewalk" : way.sidewalks[1].id if way.sidewalks[1] else None,
-                    "left_island" : way.islands[0].id if way.islands[0] else None,
-                    "right_island" : way.islands[1].id if way.islands[1] else None
+                    "left_sidewalk" : str(way.sidewalks[0].id) if way.sidewalks[0] else None,
+                    "right_sidewalk" : str(way.sidewalks[1].id) if way.sidewalks[1] else None,
+                    "left_island" : str(way.islands[0].id) if way.islands[0] else None,
+                    "right_island" : str(way.islands[1].id) if way.islands[1] else None
                 }))
                 branches_ways.append(way)
         
         # Crossroad ways
         for way in self.crossroad.ways.values():
             if way not in branches_ways:
                 n1 = way.junctions[0]
                 n2 = way.junctions[1]
                 features.append(Feature(geometry=LineString([(n1.x, n1.y), (n2.x, n2.y)]), properties={
                     "id" : str(way.id),
-                    "osm_node_ids" : [n1.id, n2.id],
-                    "osm_way_id" : way.osmid[0],
+                    "osm_node_ids" : [str(n1.id), str(n2.id)],
+                    "osm_way_id" : str(way.osmid[0]),
                     "type" : "way",
                     "name" : way.name,
                     "lanes" : [{"type" : channel.__class__.__name__, "direction" : channel.direction} for channel in way.channels],
-                    "left_sidewalk" : way.sidewalks[0].id if way.sidewalks[0] else None,
-                    "right_sidewalk" : way.sidewalks[1].id if way.sidewalks[1] else None,
-                    "left_island" : way.islands[0].id if way.islands[0] else None,
-                    "right_island" : way.islands[1].id if way.islands[1] else None
+                    "left_sidewalk" : str(way.sidewalks[0].id) if way.sidewalks[0] else None,
+                    "right_sidewalk" : str(way.sidewalks[1].id) if way.sidewalks[1] else None,
+                    "left_island" : str(way.islands[0].id) if way.islands[0] else None,
+                    "right_island" : str(way.islands[1].id) if way.islands[1] else None
                 }))
 
         # Single crosswalks
         crosswalks = []
         for junction in self.crossroad.junctions.values():
             if "Crosswalk" in junction.type:
                 crosswalks.append(junction)
         for crosswalk in crosswalks:
             features.append(Feature(geometry=Point([crosswalk.x, crosswalk.y]), properties={
                 "id" : str(crosswalk.id),
-                "osm_node_id" : crosswalk.id,
+                "osm_node_id" : str(crosswalk.id),
                 "type" : "crosswalk",
                 "tactile_paving" : crosswalk.cw_tactile_paving,
                 "pedestrian_traffic_light" : "yes" if "Pedestrian_traffic_light" in crosswalk.type else "no",
                 "pedestrian_traffic_light:sound" : crosswalk.ptl_sound if "Pedestrian_traffic_light" in crosswalk.type else "unknown"
             }))
 
         # Crossings 
@@ -399,17 +399,17 @@
             crosswalks = crossing.crosswalks
             geom = None
             id = None
             if len(crosswalks) > 1:
                 id = ";".join(map(str,[crosswalks[i].id for i in range(len(crosswalks))]))
                 geom = LineString([(crosswalks[i].x, crosswalks[i].y) for i in range(len(crosswalks))])
             else:
-                id = crosswalks[0].id
+                id = str(crosswalks[0].id)
                 geom = Point([crosswalks[0].x, crosswalks[0].y])
             features.append(Feature(geometry=geom, properties={
                 "id" : str(id),
-                "osm_node_ids" : [crosswalk.id for crosswalk in crosswalks],
+                "osm_node_ids" : [str(crosswalk.id) for crosswalk in crosswalks],
                 "type" : "crossing",
                 "branch": branch.number
             }))
 
         return(dumps(FeatureCollection(features)))
```

### Comparing `crmodel-0.4.1/crmodel/model.py` & `crmodel-0.4.2/crmodel/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,16 @@
     if node_id in Junction._junctions.keys():
         junction = Junction._junctions[node_id]
     else :
         junction = Junction(node_id, node["x"], node["y"])
             
         # is it a crosswalk ?
         if "crossing" in node and node["crossing"] != "no":
-            junction = createCrosswalk(junction, node)
+            if "foot" not in node or node["foot"] != "no":
+                junction = createCrosswalk(junction, node)
 
         # is it a traffic light ?
         if "traffic_signals" in node:
             junction = createTrafficSignal(junction, node)
 
         Junction._junctions[node_id] = junction
```

### Comparing `crmodel-0.4.1/crmodel/segmentationReader.py` & `crmodel-0.4.2/crmodel/segmentationReader.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.1/crmodel/utils.py` & `crmodel-0.4.2/crmodel/utils.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.1/crmodel.egg-info/PKG-INFO` & `crmodel-0.4.2/crmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crmodel
-Version: 0.4.1
+Version: 0.4.2
 Summary: crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.
 Home-page: https://github.com/jeremyk6/crmodel
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crmodel-0.4.1/setup.py` & `crmodel-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # The requirements file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="crmodel",
-    version="0.4.1",
+    version="0.4.2",
     description="crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jeremyk6/crmodel",
     author="Jérémy Kalsron",
     author_email="jeremy.kalsron@gmail.com  ",
     license="AGPL-3.0",
```

