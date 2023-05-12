# Comparing `tmp/rapid_videocr-2.1.6-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12191 bytes, number of entries: 9
--rw-r--r--  2.0 unx      133 b- defN 23-Mar-27 10:42 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx    13283 b- defN 23-Mar-27 10:42 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     1880 b- defN 23-Mar-27 10:42 rapid_videocr/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-27 10:43 rapid_videocr-2.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4133 b- defN 23-Mar-27 10:43 rapid_videocr-2.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 10:43 rapid_videocr-2.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 23-Mar-27 10:43 rapid_videocr-2.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Mar-27 10:43 rapid_videocr-2.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      766 b- defN 23-Mar-27 10:43 rapid_videocr-2.1.6.dist-info/RECORD
-9 files, 31726 bytes uncompressed, 10861 bytes compressed:  65.8%
+Zip file size: 12203 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      133 b- defN 23-May-12 02:06 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx    13354 b- defN 23-May-12 02:06 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     1880 b- defN 23-May-12 02:06 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4133 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      766 b- defN 23-May-12 02:06 rapid_videocr-2.1.7.dist-info/RECORD
+9 files, 31797 bytes uncompressed, 10873 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: rapid_videocr/rapid_videocr.py
 Comment: 
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
-Filename: rapid_videocr-2.1.6.dist-info/LICENSE
+Filename: rapid_videocr-2.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.1.6.dist-info/METADATA
+Filename: rapid_videocr-2.1.7.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.1.6.dist-info/WHEEL
+Filename: rapid_videocr-2.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.1.6.dist-info/entry_points.txt
+Filename: rapid_videocr-2.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.1.6.dist-info/top_level.txt
+Filename: rapid_videocr-2.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.1.6.dist-info/RECORD
+Filename: rapid_videocr-2.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/rapid_videocr.py

```diff
@@ -34,15 +34,16 @@
         self.batch_size = concat_batch
         self.is_concat_rec = is_concat_rec
         self.out_format = out_format
         self.is_print_console = is_print_console
 
     def __call__(self,
                  video_sub_finder_dir: Union[str, Path],
-                 save_dir: Union[str, Path]) -> None:
+                 save_dir: Union[str, Path],
+                 save_name: str = 'result') -> None:
         """call
 
         Args:
             video_sub_finder_dir (Union[str, Path]): RGBImages or TXTImages from VideoSubFinder app.
             save_dir (Union[str, Path]): The directory of saving the srt/txt file.
 
         Raises:
@@ -55,27 +56,27 @@
         dir_name = Path(video_sub_finder_dir).name
         is_txt_dir = 'TXTImages' in dir_name
 
         save_dir = Path(save_dir)
         mkdir(save_dir)
 
         img_list = list(Path(video_sub_finder_dir).glob('*.jpeg'))
-        img_list = sorted(img_list, key=lambda x: self.get_sort_key(x))
+        img_list = sorted(img_list, key=self.get_sort_key)
         if not img_list:
             raise RapidVideOCRError(
                 f'{video_sub_finder_dir} has not images with jpeg as suffix.')
 
         if self.is_concat_rec:
             print('Running with concat recognition.')
             srt_result, txt_result = self.concat_rec(img_list, is_txt_dir)
         else:
             print('Running with single recognition.')
             srt_result, txt_result = self.single_rec(img_list)
 
-        self.export_file(save_dir, srt_result, txt_result)
+        self.export_file(save_dir, save_name, srt_result, txt_result)
 
         if self.is_print_console:
             self.print_console(txt_result)
 
     @staticmethod
     def get_sort_key(x):
         return int(''.join(str(x.stem).split('_')[:4]))
@@ -238,21 +239,22 @@
                 final_res.append(' '.join(concat_str))
             else:
                 for v in pair_point:
                     if not used[v]:
                         final_res.append(rec_res[v])
         return '\n'.join(final_res)
 
-    def export_file(self, save_dir: Union[str, Path],
+    def export_file(self, save_dir: Union[str, Path], save_name: str,
                     srt_result: List, txt_result: List) -> None:
         if isinstance(save_dir, str):
             save_dir = Path(save_dir)
 
-        srt_path = save_dir / 'result.srt'
-        txt_path = save_dir / 'result.txt'
+        srt_path = save_dir / f'{save_name}.srt'
+        txt_path = save_dir / f'{save_name}.txt'
+
         if self.out_format == 'txt':
             self.save_file(txt_path, txt_result)
         elif self.out_format == 'srt':
             self.save_file(srt_path, srt_result)
         elif self.out_format == 'all':
             self.save_file(txt_path, txt_result)
             self.save_file(srt_path, srt_result)
```

## Comparing `rapid_videocr-2.1.6.dist-info/LICENSE` & `rapid_videocr-2.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.1.6.dist-info/METADATA` & `rapid_videocr-2.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.1.6
+Version: 2.1.7
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.1.6 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.1.7 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7,<=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

