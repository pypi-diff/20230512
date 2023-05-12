# Comparing `tmp/express-pascal-voc-tools-0.6.2.tar.gz` & `tmp/express-pascal-voc-tools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.6.2.tar", last modified: Thu May 11 13:02:11 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.7.0.tar", last modified: Fri May 12 04:44:56 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.6.2.tar` & `express-pascal-voc-tools-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.557399 express-pascal-voc-tools-0.6.2/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     4900 2023-05-11 13:02:11.553400 express-pascal-voc-tools-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4416 2023-05-11 13:01:05.000000 express-pascal-voc-tools-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.504953 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0     4900 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-11 13:02:11.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 13:02:10.000000 express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 13:02:11.558066 express-pascal-voc-tools-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-11 12:55:55.000000 express-pascal-voc-tools-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.538739 express-pascal-voc-tools-0.6.2/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.6.2/voc_tools/__init__.py
--rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.6.2/voc_tools/constants.py
--rw-rw-rw-   0        0        0     4733 2023-05-11 12:00:26.000000 express-pascal-voc-tools-0.6.2/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-11 13:02:11.546739 express-pascal-voc-tools-0.6.2/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.6.2/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     3126 2023-05-11 12:01:39.000000 express-pascal-voc-tools-0.6.2/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0     8858 2023-05-11 12:09:35.000000 express-pascal-voc-tools-0.6.2/voc_tools/utils.py
--rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.6.2/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.6.2/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.946051 express-pascal-voc-tools-0.7.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     4900 2023-05-12 04:44:56.942059 express-pascal-voc-tools-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4416 2023-05-11 13:01:05.000000 express-pascal-voc-tools-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.892233 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0     4900 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 04:44:56.000000 express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 04:44:56.947051 express-pascal-voc-tools-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-12 04:28:46.000000 express-pascal-voc-tools-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.927125 express-pascal-voc-tools-0.7.0/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.7.0/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0      102 2023-05-11 08:12:31.000000 express-pascal-voc-tools-0.7.0/voc_tools/constants.py
+-rw-rw-rw-   0        0        0     5096 2023-05-12 04:28:20.000000 express-pascal-voc-tools-0.7.0/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-12 04:44:56.935124 express-pascal-voc-tools-0.7.0/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.7.0/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     3745 2023-05-12 04:43:55.000000 express-pascal-voc-tools-0.7.0/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0     8858 2023-05-11 12:09:35.000000 express-pascal-voc-tools-0.7.0/voc_tools/utils.py
+-rw-rw-rw-   0        0        0      164 2023-05-11 08:37:02.000000 express-pascal-voc-tools-0.7.0/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.7.0/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.6.2/LICENSE` & `express-pascal-voc-tools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.6.2/PKG-INFO` & `express-pascal-voc-tools-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.6.2
+Version: 0.7.0
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.6.2/README.md` & `express-pascal-voc-tools-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.6.2/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.7.0/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.6.2
+Version: 0.7.0
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `express-pascal-voc-tools-0.6.2/setup.py` & `express-pascal-voc-tools-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=['lxml', 'numpy', 'opencv-python'],
     version_config=True,
-    version="0.6.2"
+    version="0.7.0"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.6.2/voc_tools/reader.py` & `express-pascal-voc-tools-0.7.0/voc_tools/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,32 @@
     """
     Generate a list of Annotation objects for a given image or xml of a PASCAL VOC dataset.
     It also supports captions .txt files
     """
     if file.endswith(".xml"):
         return from_xml(file)
     elif file.endswith(".txt"):
-        return caption_from_file(file)
+        return from_caption(file)
     elif file.endswith(".jpeg") or file.endswith(".jpg"):
         return from_image(file)
     else:
         raise ValueError("Unsupported file format")
 
 
+def from_caption(txt_file: str):
+    """
+    Generate a list of Annotation objects for a given caption of a PASCAL VOC dataset
+    """
+    txt_file = pathlib.Path(txt_file)
+    parent_path = txt_file.parents[1] / "Annotations"
+    file_name = txt_file.name.replace(".txt", ".xml")
+    xml_file = str(parent_path / file_name)
+    return from_xml(xml_file)
+
+
 def from_image(image_file: str):
     """
     Generate a list of Annotation objects for a given image of a PASCAL VOC dataset
     """
     image_file = pathlib.Path(image_file)
     parent_path = image_file.parents[1] / "Annotations"
     file_name = image_file.name.replace(".jpeg", ".xml").replace(".jpg", ".xml")
```

### Comparing `express-pascal-voc-tools-0.6.2/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.7.0/voc_tools/unittest/reader_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,46 +13,50 @@
         self.assertEqual(list(voc_reader.list_dir(str(dataset_path / "train"), fullpath=False)),
                          ["P00002.xml", "P00003.xml", "P00004.xml"], msg="XML files not matched.")
         self.assertEqual(list(voc_reader.list_dir(str(dataset_path / "train"), fullpath=False, images=True)),
                          ["P00002.jpg", "P00003.jpg", "P00004.jpg"], msg="JPEG files not matched.")
         self.assertEqual(Annotation.csv_header(), "file,xmin,ymin,xmax,ymax,center_x,center_y,class_name",
                          msg="CSV header mismatch")
 
-        ["file:P00002.jpg,xmin:274,ymin:232,xmax:610,ymax:460,center_x:442.0,center_y:346.0,class_name:knife",
-         "file:P00002.jpg,xmin:225,ymin:334,xmax:591,ymax:465,center_x:408.0,center_y:399.5,class_name:knife", ]
-        ["P00002.jpg,274,232,610,460,442.0,346.0,knife",
-         "P00002.jpg,225,334,591,465,408.0,399.5,knife",
-         "P00002.jpg,274,232,610,460,442.0,346.0,knife",
-         "P00002.jpg,225,334,591,465,408.0,399.5,knife", ]
-        "P00003.jpg,858,121,918,321,888.0,221.0,knife",
-        "P00004.jpg,83,73,133,425,108.0,249.0,knife",
-        "P00004.jpg,1,162,343,318,172.0,240.0,knife",
-
-        for anno in voc_reader.from_file(r"sixray_data\train\JPEGImages\P00002.jpeg"):
-            print(str(anno))
-        for anno in voc_reader.from_file(r"sixray_data\train\Annotations\P00002.xml"):
-            print(anno.csv())
-        for anno in voc_reader.from_dir(str(dataset_path / "train"), bulk=False):
-            print(anno.csv())
+        test1 = ["file:P00002.jpg,xmin:274,ymin:232,xmax:610,ymax:460,center_x:442.0,center_y:346.0,class_name:knife",
+                 "file:P00002.jpg,xmin:225,ymin:334,xmax:591,ymax:465,center_x:408.0,center_y:399.5,class_name:knife"]
+
+        test2 = [
+            "file:P00002.jpg,xmin:274,ymin:232,xmax:610,ymax:460,center_x:442.0,center_y:346.0,class_name:knife",
+            "file:P00002.jpg,xmin:225,ymin:334,xmax:591,ymax:465,center_x:408.0,center_y:399.5,class_name:knife",
+            "file:P00003.jpg,xmin:858,ymin:121,xmax:918,ymax:321,center_x:888.0,center_y:221.0,class_name:knife",
+            "file:P00004.jpg,xmin:83,ymin:73,xmax:133,ymax:425,center_x:108.0,center_y:249.0,class_name:knife",
+            "file:P00004.jpg,xmin:1,ymin:162,xmax:343,ymax:318,center_x:172.0,center_y:240.0,class_name:knife",
+        ]
+
+        for te, anno in zip(test1, voc_reader.from_file(r"sixray_data\train\JPEGImages\P00002.jpeg")):
+            self.assertEqual(te, str(anno))
+        for te, anno in zip(test1, voc_reader.from_file(r"sixray_data\train\Annotations\P00002.xml")):
+            self.assertEqual(te, str(anno))
+        for te, anno in zip(test1, voc_reader.from_file(r"sixray_data\train\text\P00002.txt")):
+            self.assertEqual(te, str(anno))
+        for te, anno in zip(test2, voc_reader.from_dir(str(dataset_path / "train"), bulk=False)):
+            self.assertEqual(te, str(anno))
         self.assertEqual("file,xmin,ymin,xmax,ymax,center_x,center_y,class_name", Annotation.csv_header())
 
         my_voc = VOCDataset(str(dataset_path))
         my_voc.train.load()
         my_voc.train.unload()
         my_voc.train.to_csv(str(dataset_path / "train.csv"))
         classes1 = my_voc.train.class_names()
         classes2 = "knife",
         self.assertEqual(classes2, classes1)
 
         voc_caption_data = VOCDataset(str(dataset_path), caption_support=True)
-        for caption in voc_caption_data.train.caption.fetch():
-            print(caption)
+        for length, captions in zip([4, 2, 1], voc_caption_data.train.caption.fetch(bulk=True)):
+            self.assertEqual(length, len(captions))
 
-        for anno, jpeg in voc_caption_data.train.fetch():
-            print(anno, jpeg)
+        l = [annotations[0].class_name for annotations, image in VOCDataset(str(dataset_path)).train.fetch(bulk=True)]
+        test3 = ['knife', 'knife', 'knife']
+        self.assertEqual(test3, l)
 
         voc_caption_data.train.caption.to_csv(str(dataset_path / "captions.csv"))
         jpg = from_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
         shape1 = jpg.image.shape
         shape2 = (482, 801, 3)
         self.assertEqual(shape1, shape2)
         # see_jpeg(r"sixray_data\train\JPEGImages\P00002.jpg")
```

### Comparing `express-pascal-voc-tools-0.6.2/voc_tools/utils.py` & `express-pascal-voc-tools-0.7.0/voc_tools/utils.py`

 * *Files identical despite different names*

