# Comparing `tmp/irene_pro-0.0.27.tar.gz` & `tmp/irene_pro-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.27.tar", last modified: Fri May 12 08:12:09 2023, max compression
+gzip compressed data, was "irene_pro-0.0.28.tar", last modified: Fri May 12 08:52:41 2023, max compression
```

## Comparing `irene_pro-0.0.27.tar` & `irene_pro-0.0.28.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 08:12:09.313984 irene_pro-0.0.27/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.27/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.27/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-05-12 08:12:09.311989 irene_pro-0.0.27/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.27/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 08:12:09.293039 irene_pro-0.0.27/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.27/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.27/irene_pro/logic.py
--rw-rw-rw-   0        0        0    24847 2023-05-12 07:47:01.000000 irene_pro-0.0.27/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:12:09.308997 irene_pro-0.0.27/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-05-12 08:12:09.000000 irene_pro-0.0.27/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-12 08:12:09.000000 irene_pro-0.0.27/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 08:12:09.000000 irene_pro-0.0.27/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-12 08:12:09.000000 irene_pro-0.0.27/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 08:12:09.000000 irene_pro-0.0.27/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 08:12:09.313984 irene_pro-0.0.27/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-12 08:07:52.000000 irene_pro-0.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:52:41.923066 irene_pro-0.0.28/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.28/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.28/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-05-12 08:52:41.920072 irene_pro-0.0.28/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.28/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 08:52:41.872201 irene_pro-0.0.28/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.28/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.28/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    24927 2023-05-12 08:49:53.000000 irene_pro-0.0.28/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:52:41.909103 irene_pro-0.0.28/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-05-12 08:52:41.000000 irene_pro-0.0.28/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-12 08:52:41.000000 irene_pro-0.0.28/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 08:52:41.000000 irene_pro-0.0.28/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-12 08:52:41.000000 irene_pro-0.0.28/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 08:52:41.000000 irene_pro-0.0.28/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 08:52:41.924062 irene_pro-0.0.28/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-12 08:50:20.000000 irene_pro-0.0.28/setup.py
```

### Comparing `irene_pro-0.0.27/PKG-INFO` & `irene_pro-0.0.28/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.27
+Version: 0.0.28
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.27/README.md` & `irene_pro-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.27/irene_pro/logic.py` & `irene_pro-0.0.28/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.27/irene_pro/widgets.py` & `irene_pro-0.0.28/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
                         self.choosen_date.delete(0.0, END)
                         self.choosen_date.insert(END, final_datetime)
                     except Exception:
                         pass
             self.datetime_fr.destroy()
             
             
-        set_date = btn(master=self.datetime_fr3, text = "set & copy", command = set_selected)
+        set_date = btn(master=self.datetime_fr3, text = "set date", command = set_selected)
         set_date.pack(side=LEFT, fill=X, expand=True)
         close = btn(master=self.datetime_fr3, text = "close", 
                          command = lambda: self.datetime_fr.destroy())
         close.pack(side=LEFT, fill=X, expand = True)
 
 class Browse:
     def __init__(self):
@@ -528,18 +528,18 @@
         self.base_frame = frame(parent)
         self.base_frame.pack(fill = X, expand = True, padx = w(1), pady = h(1), side = LEFT)
 
         self.btn_frame = frame(self.base_frame)
         self.btn_frame.pack(side = BOTTOM, fill = X, expand = True, padx = w(1), pady = h(1))
 
         self.row = btn(self.btn_frame, text = "add row", command=self.make_row)
-        self.row.pack(side = LEFT, padx = w(1), pady = h(1), fill = X, expand = True)
+        self.row.pack(side = LEFT, padx = w(1), pady = h(1), anchor=W)
 
         self.col = btn(self.btn_frame, text = "add column", command= lambda: self.make_column(self.base_frame))
-        self.col.pack(side = LEFT, padx = w(1), pady = h(1), fill = X, expand = True)
+        self.col.pack(side = LEFT, padx = w(1), pady = h(1), anchor=W)
 
         # INITIAL COLUMN AT START
         self.make_column(self.base_frame)
     
     def entry(self, frame:Frame):
         e = entry(frame)
         e.bind("<KeyRelease>", lambda e: replace_empty_in_data())
@@ -591,7 +591,12 @@
     
     def final_data(self):
         # BY NOW, THE DATAFRAME WILL BE BEING DISLPLAY IN THE TERMINAL
         nd = np.array(self.data)
         transposed_data = nd.T
         return transposed_data
 
+
+# CONSTANTS
+comb_syle = 'comb.TCombobox'
+check_style = "TCheckbutton"
+radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.27/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.28/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.27
+Version: 0.0.28
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.27/setup.py` & `irene_pro-0.0.28/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3237 270d 0a44 4553 4352   '0.0.27'..DESCR
+00000100: 2027 302e 302e 3238 270d 0a44 4553 4352   '0.0.28'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

