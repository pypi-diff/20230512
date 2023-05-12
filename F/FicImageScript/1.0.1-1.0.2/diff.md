# Comparing `tmp/FicImageScript-1.0.1.tar.gz` & `tmp/FicImageScript-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FicImageScript-1.0.1.tar", last modified: Thu May 11 13:34:29 2023, max compression
+gzip compressed data, was "FicImageScript-1.0.2.tar", last modified: Fri May 12 16:34:55 2023, max compression
```

## Comparing `FicImageScript-1.0.1.tar` & `FicImageScript-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-11 13:34:29.647168 FicImageScript-1.0.1/FicImage/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        0 2023-05-06 04:09:38.000000 FicImageScript-1.0.1/FicImage/__init__.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5514 2023-05-08 22:25:50.000000 FicImageScript-1.0.1/FicImage/image.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     4629 2023-05-11 13:28:32.000000 FicImageScript-1.0.1/FicImage/main.py
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     2271 2023-05-08 22:25:50.000000 FicImageScript-1.0.1/FicImage/utils.py
-drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/FicImageScript.egg-info/
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7747 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      345 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/SOURCES.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/dependency_links.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/entry_points.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/requires.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-11 13:34:29.000000 FicImageScript-1.0.1/FicImageScript.egg-info/top_level.txt
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImageScript-1.0.1/LICENSE
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     7747 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/PKG-INFO
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     5698 2023-05-08 23:07:54.000000 FicImageScript-1.0.1/README.md
--rw-rw-r--   0 nonso     (1000) nonso     (1001)      927 2023-05-11 11:38:32.000000 FicImageScript-1.0.1/pyproject.toml
--rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-11 13:34:29.651168 FicImageScript-1.0.1/setup.cfg
--rw-rw-r--   0 nonso     (1000) nonso     (1001)     1249 2023-05-11 11:38:33.000000 FicImageScript-1.0.1/setup.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-12 16:34:55.014353 FicImageScript-1.0.2/
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-12 16:34:55.002352 FicImageScript-1.0.2/FicImage/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       22 2023-05-12 16:34:10.000000 FicImageScript-1.0.2/FicImage/__init__.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5514 2023-05-08 22:25:50.000000 FicImageScript-1.0.2/FicImage/image.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     4648 2023-05-12 15:10:31.000000 FicImageScript-1.0.2/FicImage/main.py
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     2265 2023-05-12 13:41:09.000000 FicImageScript-1.0.2/FicImage/utils.py
+drwxrwxr-x   0 nonso     (1000) nonso     (1001)        0 2023-05-12 16:34:55.010353 FicImageScript-1.0.2/FicImageScript.egg-info/
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     6811 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      361 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/SOURCES.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        1 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/dependency_links.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       48 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/entry_points.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      182 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/requires.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)        9 2023-05-12 16:34:54.000000 FicImageScript-1.0.2/FicImageScript.egg-info/top_level.txt
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1075 2023-04-28 12:48:04.000000 FicImageScript-1.0.2/LICENSE
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     6811 2023-05-12 16:34:55.010353 FicImageScript-1.0.2/PKG-INFO
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     6087 2023-05-12 15:54:55.000000 FicImageScript-1.0.2/PYPI_README.rst
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     5698 2023-05-08 23:07:54.000000 FicImageScript-1.0.2/README.md
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)      955 2023-05-12 16:11:28.000000 FicImageScript-1.0.2/pyproject.toml
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)       38 2023-05-12 16:34:55.014353 FicImageScript-1.0.2/setup.cfg
+-rw-rw-r--   0 nonso     (1000) nonso     (1001)     1252 2023-05-12 16:34:10.000000 FicImageScript-1.0.2/setup.py
```

### Comparing `FicImageScript-1.0.1/FicImage/image.py` & `FicImageScript-1.0.2/FicImage/image.py`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.1/FicImage/main.py` & `FicImageScript-1.0.2/FicImage/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 		images_downloaded = {}
 
 		for item in book.get_items_of_type(ebooklib.ITEM_DOCUMENT):
 			try:
 				soup = BeautifulSoup(item.content, "lxml-xml")
 				p_tags = soup.find_all('p')
 				images = [i for i in p_tags if '[img:' in i.text]
-				print(f'Found {len(images)} images in {item.file_name}')
+				if debug:
+					print(f'Found {len(images)} images in {item.file_name}')
 				item_file_name = item.file_name.split('.')[0]
 				images_downloaded[item.file_name] = [0, len(images)]
 				# Clean up the images link
 				# Right now they look like this: <p>[img: <a
 				# href="https://i.imgur.com/ABCDEF.jpg" rel="noopener noreferrer">data:image/gif;base64,R0lGODlhA</a>]</p>
 				# But we want to get the link in the href attribute:
 				try:
@@ -98,16 +99,16 @@
 			epub.write_epub(f"[FicImage]{file_name}.epub", book)
 			total_number_of_images_downloaded = 0
 			number_of_all_images_found = 0
 			for _, chapter_image_list in images_downloaded.items():
 				total_number_of_images_downloaded += chapter_image_list[0]
 				number_of_all_images_found += chapter_image_list[1]
 
-			print(f'Wrote [FicImage]{file_name}.epub')
-			print(f"Image overview of {file_name}")
+			print(f'\nWrote [FicImage]{file_name}.epub')
+			print(f"\nImage overview of {file_name}")
 			print("=" * 54)
 			for k, v in images_downloaded.items():
 				print(f"{k}{' ' * (18 - len(k))}\t{v[0]} out of {v[1]} images downloaded")
 			print("=" * 54)
 			print(f"Total images downloaded: {total_number_of_images_downloaded}"
 			      f" out of {number_of_all_images_found}")
 			print("=" * 54)
```

### Comparing `FicImageScript-1.0.1/FicImage/utils.py` & `FicImageScript-1.0.2/FicImage/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,12 +55,12 @@
 	"""
 	default_settings = {
 		"compress_images": True,
 		"default_image_format": "JPEG",
 		"max_image_size": 100000
 	}
 	default_settings_str = '\n'.join([f"{key}: {value}" for key, value in default_settings.items()])
-	print(f"Using default config settings:"
-	      f"\n\n============================\n"
+	print(f"\nDefault config settings:"
+	      f"\n============================\n"
 	      f"{default_settings_str}"
 	      f"\n============================\n")
 	return default_settings
```

### Comparing `FicImageScript-1.0.1/FicImageScript.egg-info/PKG-INFO` & `FicImageScript-1.0.2/FicImageScript.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,187 +1,202 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 1.0.1
+Version: 1.0.2
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
-Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Emmanuel C. Jemeni
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/Jemeni11/FicImage
+Author-email: jemenichinonso11@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jemeni11/FicImage/issues
-Keywords: fanfiction,fichub,ficimage,image
+Keywords: fanfiction fichub ficimage image download epub
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# FicImage/FicImageScript
+FicImage (aka FicImageScript)
+=============================
 
-## Introduction
-FicImage is an application designed to enhance the reading experience of FicHub epubs. With FicImage, users can easily add missing images to their FicHub epubs, bringing the stories to life with vibrant visuals. This user-friendly tool allows readers to fully immerse themselves in their favorite fan fiction stories and enjoy them in a whole new way.
+FicImage is an application designed to enhance the reading experience of
+FicHub epubs. With FicImage, users can easily add missing images to
+their FicHub epubs, bringing the stories to life with vibrant visuals.
+This user-friendly tool allows readers to fully immerse themselves in
+their favorite fan fiction stories and enjoy them in a whole new way.
+
+How to Use
+----------
+
+Installation with PIP
+~~~~~~~~~~~~~~~~~~~~~
+
+1. Install FicImage using ``pip install FicImageScript``.
+2. After installation, run the program using
+   ``ficimage path/to/epub -c path/to/ficimage/json`` where
+   ``path/to/epub`` is the path to the **FicHub epub** you want to add
+   images to and ``path/to/ficimage/json`` is the path to a file called
+   **ficimage.json** . ficimage.json lets you configure FicImage. See
+   more `in the configuration section below <#configuration>`__.
+
+.. code:: shell
+
+   (virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
+   usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+
+   Update a FicHub epub file with images.
+
+   positional arguments:
+     path_to_epub          The path to the FicHub epub file.
+
+   optional arguments:
+     -h, --help            show this help message and exit
+     -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                           The path to the ficimage.json file.
+     -d, --debug           Enable debug mode.
 
-## How to Use
+Image Support
+~~~~~~~~~~~~~
 
-### Installation with PIP
-1. Install FicImage using `pip install FicImageScript`.
-2.  After installation, run the program using `ficimage path/to/epub -c path/to/ficimage/json` 
-where `path/to/epub` is the path to the **FicHub epub** you want to add 
-images to and `path/to/ficimage/json` is the path to a file called **ficimage.json** . 
-ficimage.json lets you configure FicImage. See more [below](#configuration).
+`FicHub <https://fichub.net/>`__ creates EPUB 3.3 files, which means
+that FicImage only save images in the following file format:
 
-
-```shell
-(virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
-usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
-
-Update a FicHub epub file with images.
-
-positional arguments:
-  path_to_epub          The path to the FicHub epub file.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
-                        The path to the ficimage.json file.
-  -d, --debug           Enable debug mode.
-
-```
-
-### Image Support
-
-[FicHub](https://fichub.net/) creates EPUB 3.3 files, which means that FicImage only save images 
-in the following file format:
 - JPEG
 - PNG
 - GIF
 - WEBP
 - SVG
 
-See the [Core Media Types Section of the EPUB Version 3.3 Specification](https://www.w3.org/TR/epub-33/#sec-core-media-types) for more information.
-
-While FicImage can save SVG images, it can not compress them because SVGs are not supported by Pillow.
-
-FicImage uses [Pillow](https://pillow.readthedocs.io/en/stable/index.html) for image manipulation and conversion. 
+See the `Core Media Types Section of the EPUB Version 3.3
+Specification <https://www.w3.org/TR/epub-33/#sec-core-media-types>`__
+for more information.
+
+While FicImage can save SVG images, it can not compress them because
+SVGs are not supported by Pillow.
+
+FicImage uses
+`Pillow <https://pillow.readthedocs.io/en/stable/index.html>`__ for
+image manipulation and conversion.
 
 By default, FicImage will try and save all non-animated images as JPEGs.
 
 The only animated images that FicImage will save are GIFs and WEBPs.
 
-FicImage does little to no processing on GIFs and WEBPs images. 
-This is to avoid breaking the animation.
+FicImage does little to no processing on GIFs and WEBPs images. This is
+to avoid breaking the animation.
 
-If FicImage can not download an image, it leaves the image url 
-paragraph the same way it met it.
+If FicImage can not download an image, it leaves the image url paragraph
+the same way it met it.
 
-To configure image support, you will need to create a file called `ficimage.json`. 
-See the section below for more information.
+To configure image support, you will need to create a file called
+``ficimage.json``. See the section below for more information.
 
+Configuration
+~~~~~~~~~~~~~
 
-### Configuration
-FicImage comes with a configuration file that allows you to customize the program to your liking.
+FicImage comes with a configuration file that allows you to customize
+the program to your liking.
 
-The configuration file is in the [JSON file format](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON) 
+The configuration file is in the `JSON file
+format <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON>`__
 and contains the following options:
 
+-  ``compress_images``: A boolean that tells FicImage whether to
+   compress images. This is only supported for ``jpeg`` and ``png``
+   images.
+-  ``default_image_format``: A string that tells FicImage what default
+   format to convert and save images in. This is only supported for
+   ``jpeg`` and ``png`` images.
+-  ``max_image_size``: An integer that tells FicImage the maximum size
+   of an image in bytes. If an image is larger than this value, FicImage
+   will compress it.
+
+FicImage checks for a configuration file in the given directory path. If
+no directory path is given, FicImage checks the current directory and
+then the Operating System’s home directory.
 
-- `compress_images`: A boolean that tells FicImage whether to compress images. 
-    This is only supported for `jpeg` and `png` images.
-- `default_image_format`: A string that tells FicImage what default format to convert and save images in. This is only supported for `jpeg` and `png` images.
-- `max_image_size`: An integer that tells FicImage the maximum size of an image in bytes. 
-    If an image is larger than this value, FicImage will compress it.
+If it does not find one, it uses the following defaults:
 
+.. code:: json
 
-FicImage checks for a configuration file in the given directory path. If no directory 
-path is given, FicImage checks the current directory and then the Operating System's 
-home directory.
+   {
+       "compress_images": true,
+       "default_image_format": "JPEG",
+       "max_image_size": 100000
+   }
 
-If it does not find one, it uses the following defaults:
-    
-```json
-{
-    "compress_images": true,
-    "default_image_format": "JPEG",
-    "max_image_size": 100000
-}
-```
+..
+
+   Note: The ``compress_images`` key is a boolean and can only be
+   ``true`` or ``false``. Booleans in JSON are written in lowercase.
+
+   Note: If the ``default_image_format`` key does not exist, FicImage
+   will default to ``jpeg``. The two image formats are ``jpeg`` and
+   ``png``. The ``default_image_format`` key is case-insensitive.
+
+..
 
-> Note: The `compress_images` key is a boolean and can only be `true` or `false`. 
-> Booleans in JSON are written in lowercase.
+   Note: The ``compress_images`` key tells FicImage to compress images.
+   This is only supported for ``jpeg`` and ``png`` images. This also
+   goes hand-in-hand with the ``max_image_size`` key. If the
+   ``compress_images`` key is ``true`` but there’s no ``max_image_size``
+   key, FicImage will compress the image to a size less than 1MB
+   (1000000 bytes). If the ``max_image_size`` key is present, FicImage
+   will compress the image to a size less than the value of the
+   ``max_image_size`` key. The ``max_image_size`` key is in bytes.
 
-> Note: If the `default_image_format` key does not exist, FicImage will default to `jpeg`.
-> The two image formats are `jpeg` and `png`. 
-> The `default_image_format` key is case-insensitive.
+   If ``compress_images`` is ``false``, FicImage will ignore the
+   ``max_image_size`` key.
 
-> Note: The `compress_images` key tells FicImage to compress images. 
-> This is only supported for `jpeg` and `png` images.
-> This also goes hand-in-hand with the `max_image_size` key. 
-> If the `compress_images` key is `true` but there's no `max_image_size` key,
-> FicImage will compress the image to a size less than 1MB (1000000 bytes). 
-> If the `max_image_size` key is present, FicImage will compress the image
-> to a size less than the value of the `max_image_size` key. 
-> The `max_image_size` key is in bytes.
+..
 
-> If `compress_images` is `false`, FicImage will ignore the `max_image_size` key.
+   Warning: Compressing images might make the image quality worse.
 
-> Warning: Compressing images might make the image quality worse.
+   Warning: ``max_image_size`` is not a hard limit. FicImage will try to
+   compress the image to the size of the ``max_image_size`` key, but it
+   might not be able to compress the image to the exact size of the
+   ``max_image_size`` key.
 
-> Warning: `max_image_size` is not a hard limit. FicImage will try to compress the
-> image to the size of the `max_image_size` key, but it might
-> not be able to compress the image to the exact size of the `max_image_size` key.
+..
 
-> Warning: `max_image_size` should not be too small. 
-> For instance, if you set `max_image_size` to 1 000, FicImage will 
-> probably not be able to compress the image to 1 000 bytes (1 KB). 
-> If you set `max_image_size` to 1 000 000, FicImage will probably be able to
-> compress the image to 1 000 000 bytes (1 MB).
+   Warning: ``max_image_size`` should not be too small. For instance, if
+   you set ``max_image_size`` to 1 000, FicImage will probably not be
+   able to compress the image to 1 000 bytes (1 KB). If you set
+   ``max_image_size`` to 1 000 000, FicImage will probably be able to
+   compress the image to 1 000 000 bytes (1 MB).
 
-> Warning: FicImage will not compress GIFs or WEBPs, that might damage the animation.
+   Warning: FicImage will not compress GIFs or WEBPs, that might damage
+   the animation.
 
+TODO
+----
 
-## TODO
-- [x] Improve logs
-- [ ] Conversion to other FicHub supported formats from ePub.
-- [ ] More testing 
+-  ☒ Improve logs
+-  ☐ Conversion to other FicHub supported formats from ePub.
+-  ☐ More testing
 
+Contributing
+------------
 
-## Contributing
-Fork the repo and get started!
+Fork `this repo <https://github.com/Jemeni11/FicImage>`__ and get
+started!
 
+Links
+-----
 
-## Links
+-  Me
 
-- Me
-  
-    [LinkedIn](https://www.linkedin.com/in/emmanuel-jemeni) • [GitHub](https://github.com/Jemeni11) • [Twitter](https://twitter.com/Jemeni11_)
+   `LinkedIn <https://www.linkedin.com/in/emmanuel-jemeni>`__ •
+   `GitHub <https://github.com/Jemeni11>`__ •
+   `Twitter <https://twitter.com/Jemeni11_>`__
 
-- FicHub
+-  FicHub
 
-  Without FicHub, this project would (obviously lol) not exist.
+   `Website <https://fichub.net/>`__ •
+   `GitHub <https://github.com/FicHub/fichub.net>`__ •
+   `Discord <https://discord.gg/sByBAhX>`__
 
-  [Website](https://fichub.net/) • [GitHub](https://github.com/FicHub/fichub.net) • [Discord](https://discord.gg/sByBAhX)
+   Without FicHub, this project would (obviously lol) not exist.
 
-  Thanks to [iris](https://github.com/iridescent-beacon) for helping me with this project as well.
+   Thanks to `iris <https://github.com/iridescent-beacon>`__ for helping
+   me with this project as well.
```

### Comparing `FicImageScript-1.0.1/LICENSE` & `FicImageScript-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.1/PKG-INFO` & `FicImageScript-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,187 +1,202 @@
 Metadata-Version: 2.1
 Name: FicImageScript
-Version: 1.0.1
+Version: 1.0.2
 Summary: FicImage is an application designed to enhance the reading experience of FicHub epubs.
 Home-page: https://github.com/Jemeni11/FicImage
 Author: Emmanuel C. Jemeni
-Author-email: "Emmanuel C. Jemeni" <jemenichinonso11@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Emmanuel C. Jemeni
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/Jemeni11/FicImage
+Author-email: jemenichinonso11@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jemeni11/FicImage/issues
-Keywords: fanfiction,fichub,ficimage,image
+Keywords: fanfiction fichub ficimage image download epub
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# FicImage/FicImageScript
+FicImage (aka FicImageScript)
+=============================
 
-## Introduction
-FicImage is an application designed to enhance the reading experience of FicHub epubs. With FicImage, users can easily add missing images to their FicHub epubs, bringing the stories to life with vibrant visuals. This user-friendly tool allows readers to fully immerse themselves in their favorite fan fiction stories and enjoy them in a whole new way.
+FicImage is an application designed to enhance the reading experience of
+FicHub epubs. With FicImage, users can easily add missing images to
+their FicHub epubs, bringing the stories to life with vibrant visuals.
+This user-friendly tool allows readers to fully immerse themselves in
+their favorite fan fiction stories and enjoy them in a whole new way.
+
+How to Use
+----------
+
+Installation with PIP
+~~~~~~~~~~~~~~~~~~~~~
+
+1. Install FicImage using ``pip install FicImageScript``.
+2. After installation, run the program using
+   ``ficimage path/to/epub -c path/to/ficimage/json`` where
+   ``path/to/epub`` is the path to the **FicHub epub** you want to add
+   images to and ``path/to/ficimage/json`` is the path to a file called
+   **ficimage.json** . ficimage.json lets you configure FicImage. See
+   more `in the configuration section below <#configuration>`__.
+
+.. code:: shell
+
+   (virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
+   usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
+
+   Update a FicHub epub file with images.
+
+   positional arguments:
+     path_to_epub          The path to the FicHub epub file.
+
+   optional arguments:
+     -h, --help            show this help message and exit
+     -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
+                           The path to the ficimage.json file.
+     -d, --debug           Enable debug mode.
 
-## How to Use
+Image Support
+~~~~~~~~~~~~~
 
-### Installation with PIP
-1. Install FicImage using `pip install FicImageScript`.
-2.  After installation, run the program using `ficimage path/to/epub -c path/to/ficimage/json` 
-where `path/to/epub` is the path to the **FicHub epub** you want to add 
-images to and `path/to/ficimage/json` is the path to a file called **ficimage.json** . 
-ficimage.json lets you configure FicImage. See more [below](#configuration).
+`FicHub <https://fichub.net/>`__ creates EPUB 3.3 files, which means
+that FicImage only save images in the following file format:
 
-
-```shell
-(virt) nonso@HPEnvy:~/Documents/Code$ ficimage -h
-usage: ficimage [-h] [-c CONFIG_FILE_PATH] [-d] path_to_epub
-
-Update a FicHub epub file with images.
-
-positional arguments:
-  path_to_epub          The path to the FicHub epub file.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG_FILE_PATH, --config_file_path CONFIG_FILE_PATH
-                        The path to the ficimage.json file.
-  -d, --debug           Enable debug mode.
-
-```
-
-### Image Support
-
-[FicHub](https://fichub.net/) creates EPUB 3.3 files, which means that FicImage only save images 
-in the following file format:
 - JPEG
 - PNG
 - GIF
 - WEBP
 - SVG
 
-See the [Core Media Types Section of the EPUB Version 3.3 Specification](https://www.w3.org/TR/epub-33/#sec-core-media-types) for more information.
-
-While FicImage can save SVG images, it can not compress them because SVGs are not supported by Pillow.
-
-FicImage uses [Pillow](https://pillow.readthedocs.io/en/stable/index.html) for image manipulation and conversion. 
+See the `Core Media Types Section of the EPUB Version 3.3
+Specification <https://www.w3.org/TR/epub-33/#sec-core-media-types>`__
+for more information.
+
+While FicImage can save SVG images, it can not compress them because
+SVGs are not supported by Pillow.
+
+FicImage uses
+`Pillow <https://pillow.readthedocs.io/en/stable/index.html>`__ for
+image manipulation and conversion.
 
 By default, FicImage will try and save all non-animated images as JPEGs.
 
 The only animated images that FicImage will save are GIFs and WEBPs.
 
-FicImage does little to no processing on GIFs and WEBPs images. 
-This is to avoid breaking the animation.
+FicImage does little to no processing on GIFs and WEBPs images. This is
+to avoid breaking the animation.
 
-If FicImage can not download an image, it leaves the image url 
-paragraph the same way it met it.
+If FicImage can not download an image, it leaves the image url paragraph
+the same way it met it.
 
-To configure image support, you will need to create a file called `ficimage.json`. 
-See the section below for more information.
+To configure image support, you will need to create a file called
+``ficimage.json``. See the section below for more information.
 
+Configuration
+~~~~~~~~~~~~~
 
-### Configuration
-FicImage comes with a configuration file that allows you to customize the program to your liking.
+FicImage comes with a configuration file that allows you to customize
+the program to your liking.
 
-The configuration file is in the [JSON file format](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON) 
+The configuration file is in the `JSON file
+format <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON>`__
 and contains the following options:
 
+-  ``compress_images``: A boolean that tells FicImage whether to
+   compress images. This is only supported for ``jpeg`` and ``png``
+   images.
+-  ``default_image_format``: A string that tells FicImage what default
+   format to convert and save images in. This is only supported for
+   ``jpeg`` and ``png`` images.
+-  ``max_image_size``: An integer that tells FicImage the maximum size
+   of an image in bytes. If an image is larger than this value, FicImage
+   will compress it.
+
+FicImage checks for a configuration file in the given directory path. If
+no directory path is given, FicImage checks the current directory and
+then the Operating System’s home directory.
 
-- `compress_images`: A boolean that tells FicImage whether to compress images. 
-    This is only supported for `jpeg` and `png` images.
-- `default_image_format`: A string that tells FicImage what default format to convert and save images in. This is only supported for `jpeg` and `png` images.
-- `max_image_size`: An integer that tells FicImage the maximum size of an image in bytes. 
-    If an image is larger than this value, FicImage will compress it.
+If it does not find one, it uses the following defaults:
 
+.. code:: json
 
-FicImage checks for a configuration file in the given directory path. If no directory 
-path is given, FicImage checks the current directory and then the Operating System's 
-home directory.
+   {
+       "compress_images": true,
+       "default_image_format": "JPEG",
+       "max_image_size": 100000
+   }
 
-If it does not find one, it uses the following defaults:
-    
-```json
-{
-    "compress_images": true,
-    "default_image_format": "JPEG",
-    "max_image_size": 100000
-}
-```
+..
+
+   Note: The ``compress_images`` key is a boolean and can only be
+   ``true`` or ``false``. Booleans in JSON are written in lowercase.
+
+   Note: If the ``default_image_format`` key does not exist, FicImage
+   will default to ``jpeg``. The two image formats are ``jpeg`` and
+   ``png``. The ``default_image_format`` key is case-insensitive.
+
+..
 
-> Note: The `compress_images` key is a boolean and can only be `true` or `false`. 
-> Booleans in JSON are written in lowercase.
+   Note: The ``compress_images`` key tells FicImage to compress images.
+   This is only supported for ``jpeg`` and ``png`` images. This also
+   goes hand-in-hand with the ``max_image_size`` key. If the
+   ``compress_images`` key is ``true`` but there’s no ``max_image_size``
+   key, FicImage will compress the image to a size less than 1MB
+   (1000000 bytes). If the ``max_image_size`` key is present, FicImage
+   will compress the image to a size less than the value of the
+   ``max_image_size`` key. The ``max_image_size`` key is in bytes.
 
-> Note: If the `default_image_format` key does not exist, FicImage will default to `jpeg`.
-> The two image formats are `jpeg` and `png`. 
-> The `default_image_format` key is case-insensitive.
+   If ``compress_images`` is ``false``, FicImage will ignore the
+   ``max_image_size`` key.
 
-> Note: The `compress_images` key tells FicImage to compress images. 
-> This is only supported for `jpeg` and `png` images.
-> This also goes hand-in-hand with the `max_image_size` key. 
-> If the `compress_images` key is `true` but there's no `max_image_size` key,
-> FicImage will compress the image to a size less than 1MB (1000000 bytes). 
-> If the `max_image_size` key is present, FicImage will compress the image
-> to a size less than the value of the `max_image_size` key. 
-> The `max_image_size` key is in bytes.
+..
 
-> If `compress_images` is `false`, FicImage will ignore the `max_image_size` key.
+   Warning: Compressing images might make the image quality worse.
 
-> Warning: Compressing images might make the image quality worse.
+   Warning: ``max_image_size`` is not a hard limit. FicImage will try to
+   compress the image to the size of the ``max_image_size`` key, but it
+   might not be able to compress the image to the exact size of the
+   ``max_image_size`` key.
 
-> Warning: `max_image_size` is not a hard limit. FicImage will try to compress the
-> image to the size of the `max_image_size` key, but it might
-> not be able to compress the image to the exact size of the `max_image_size` key.
+..
 
-> Warning: `max_image_size` should not be too small. 
-> For instance, if you set `max_image_size` to 1 000, FicImage will 
-> probably not be able to compress the image to 1 000 bytes (1 KB). 
-> If you set `max_image_size` to 1 000 000, FicImage will probably be able to
-> compress the image to 1 000 000 bytes (1 MB).
+   Warning: ``max_image_size`` should not be too small. For instance, if
+   you set ``max_image_size`` to 1 000, FicImage will probably not be
+   able to compress the image to 1 000 bytes (1 KB). If you set
+   ``max_image_size`` to 1 000 000, FicImage will probably be able to
+   compress the image to 1 000 000 bytes (1 MB).
 
-> Warning: FicImage will not compress GIFs or WEBPs, that might damage the animation.
+   Warning: FicImage will not compress GIFs or WEBPs, that might damage
+   the animation.
 
+TODO
+----
 
-## TODO
-- [x] Improve logs
-- [ ] Conversion to other FicHub supported formats from ePub.
-- [ ] More testing 
+-  ☒ Improve logs
+-  ☐ Conversion to other FicHub supported formats from ePub.
+-  ☐ More testing
 
+Contributing
+------------
 
-## Contributing
-Fork the repo and get started!
+Fork `this repo <https://github.com/Jemeni11/FicImage>`__ and get
+started!
 
+Links
+-----
 
-## Links
+-  Me
 
-- Me
-  
-    [LinkedIn](https://www.linkedin.com/in/emmanuel-jemeni) • [GitHub](https://github.com/Jemeni11) • [Twitter](https://twitter.com/Jemeni11_)
+   `LinkedIn <https://www.linkedin.com/in/emmanuel-jemeni>`__ •
+   `GitHub <https://github.com/Jemeni11>`__ •
+   `Twitter <https://twitter.com/Jemeni11_>`__
 
-- FicHub
+-  FicHub
 
-  Without FicHub, this project would (obviously lol) not exist.
+   `Website <https://fichub.net/>`__ •
+   `GitHub <https://github.com/FicHub/fichub.net>`__ •
+   `Discord <https://discord.gg/sByBAhX>`__
 
-  [Website](https://fichub.net/) • [GitHub](https://github.com/FicHub/fichub.net) • [Discord](https://discord.gg/sByBAhX)
+   Without FicHub, this project would (obviously lol) not exist.
 
-  Thanks to [iris](https://github.com/iridescent-beacon) for helping me with this project as well.
+   Thanks to `iris <https://github.com/iridescent-beacon>`__ for helping
+   me with this project as well.
```

### Comparing `FicImageScript-1.0.1/README.md` & `FicImageScript-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FicImageScript-1.0.1/pyproject.toml` & `FicImageScript-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[project]
-name = "FicImageScript"
-version = "1.0.1"
-authors = [
-  { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
-]
-description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
-readme = "README.md"
-requires-python = ">=3.6"
-license = {file = "LICENSE"}
-keywords = ["fanfiction", "fichub", "ficimage", "image"]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Topic :: Internet :: WWW/HTTP",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Jemeni11/FicImage"
-"Bug Tracker" = "https://github.com/Jemeni11/FicImage/issues"
+#[project]
+#name = "FicImageScript"
+#version = "1.0.1"
+#authors = [
+#  { name="Emmanuel C. Jemeni", email="jemenichinonso11@gmail.com" }
+#]
+#description = "FicImage is an application designed to enhance the reading experience of FicHub epubs."
+#readme = "PYPI_README.rst"
+#requires-python = ">=3.6"
+#license = {file = "LICENSE"}
+#keywords = ["fanfiction", "fichub", "ficimage", "image"]
+#classifiers = [
+#    "Development Status :: 5 - Production/Stable",
+#    "Programming Language :: Python :: 3",
+#    "License :: OSI Approved :: MIT License",
+#    "Operating System :: OS Independent",
+#    "Topic :: Internet :: WWW/HTTP",
+#]
+#
+#[project.urls]
+#"Homepage" = "https://github.com/Jemeni11/FicImage"
+#"Bug Tracker" = "https://github.com/Jemeni11/FicImage/issues"
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
```

### Comparing `FicImageScript-1.0.1/setup.py` & `FicImageScript-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("PYPI_README.rst", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="FicImageScript",
-	version="1.0.1",
+	version="1.0.2",
 	author="Emmanuel C. Jemeni",
 	author_email="jemenichinonso11@gmail.com",
 	description="FicImage is an application designed to enhance the reading experience of FicHub epubs.",
 	long_description=long_description,
-	long_description_content_type="text/markdown",
+	long_description_content_type="text/x-rst",
 	url="https://github.com/Jemeni11/FicImage",
 	project_urls={
 		"Bug Tracker": "https://github.com/Jemeni11/FicImage/issues",
 	},
 	entry_points={
 		'console_scripts': [
 			'ficimage=FicImage.main:main'
```

