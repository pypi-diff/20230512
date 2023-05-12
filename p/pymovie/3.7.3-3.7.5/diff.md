# Comparing `tmp/pymovie-3.7.3.tar.gz` & `tmp/pymovie-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymovie-3.7.3.tar", last modified: Sat Feb 11 21:46:35 2023, max compression
+gzip compressed data, was "pymovie-3.7.5.tar", last modified: Fri May 12 16:54:09 2023, max compression
```

## Comparing `pymovie-3.7.3.tar` & `pymovie-3.7.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 21:46:35.273484 pymovie-3.7.3/
--rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.7.3/LICENSE
--rw-rw-rw-   0        0        0     1474 2023-02-11 21:46:35.273484 pymovie-3.7.3/PKG-INFO
--rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.7.3/README.rst
--rw-rw-rw-   0        0        0       80 2023-02-11 21:46:35.276484 pymovie-3.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-11 21:46:35.244919 pymovie-3.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-02-11 21:46:35.268444 pymovie-3.7.3/src/pymovie/
--rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.7.3/src/pymovie/NE3Lut.p
--rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.7.3/src/pymovie/PyMovie-doc.pdf
--rw-rw-rw-   0        0        0   729476 2023-02-11 21:46:20.000000 pymovie-3.7.3/src/pymovie/PyMovie-info.pdf
--rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.7.3/src/pymovie/PyMovie.bat
--rw-rw-rw-   0        0        0     5921 2020-03-09 02:49:37.000000 pymovie-3.7.3/src/pymovie/SER.py
--rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.7.3/src/pymovie/__init__.py
--rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.7.3/src/pymovie/alias_lnk_resolver.py
--rw-rw-rw-   0        0        0     4834 2022-07-28 03:01:01.000000 pymovie-3.7.3/src/pymovie/aperture.py
--rw-rw-rw-   0        0        0    12873 2022-07-10 14:43:28.000000 pymovie-3.7.3/src/pymovie/apertureEdit.py
--rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.7.3/src/pymovie/apertureEditDialog.py
--rw-rw-rw-   0        0        0     2118 2019-08-17 21:54:24.000000 pymovie-3.7.3/src/pymovie/apertureNameDialog.py
--rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.7.3/src/pymovie/aperturesFileTagDialog.py
--rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.7.3/src/pymovie/astrometry_client.py
--rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.7.3/src/pymovie/checkForNewerVersion.py
--rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.7.3/src/pymovie/gammaUtils.py
--rw-rw-rw-   0        0        0   219915 2023-02-09 16:11:29.000000 pymovie-3.7.3/src/pymovie/gui.py
--rw-rw-rw-   0        0        0     2324 2019-06-08 18:46:48.000000 pymovie-3.7.3/src/pymovie/helpDialog.py
--rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.7.3/src/pymovie/hotPixelDialog.py
--rw-rw-rw-   0        0        0   399754 2023-02-10 00:35:02.000000 pymovie-3.7.3/src/pymovie/main.py
--rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.7.3/src/pymovie/ocr.py
--rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.7.3/src/pymovie/ocrCharacterBox.py
--rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.7.3/src/pymovie/ocrProfileNameDialog.py
--rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.7.3/src/pymovie/play-Temp.py
--rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.7.3/src/pymovie/play-introspection.py
--rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.7.3/src/pymovie/run-pymovie-mac.bat
--rw-rw-rw-   0        0        0     3559 2019-10-10 18:10:06.000000 pymovie-3.7.3/src/pymovie/selectHotPixelProfile.py
--rw-rw-rw-   0        0        0     3511 2019-07-06 18:14:37.000000 pymovie-3.7.3/src/pymovie/selectProfile.py
--rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.7.3/src/pymovie/stacker.py
--rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.7.3/src/pymovie/starPositionDialog.py
--rw-rw-rw-   0        0        0       36 2023-02-11 21:45:57.000000 pymovie-3.7.3/src/pymovie/version.py
--rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.7.3/src/pymovie/wcs_helper_functions.py
-drwxrwxrwx   0        0        0        0 2023-02-11 21:46:35.272446 pymovie-3.7.3/src/pymovie.egg-info/
--rw-rw-rw-   0        0        0     1474 2023-02-11 21:46:35.000000 pymovie-3.7.3/src/pymovie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-02-11 21:46:35.000000 pymovie-3.7.3/src/pymovie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 21:46:35.000000 pymovie-3.7.3/src/pymovie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.7.3/src/pymovie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      247 2023-02-11 21:46:35.000000 pymovie-3.7.3/src/pymovie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-11 21:46:35.000000 pymovie-3.7.3/src/pymovie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 16:54:09.180386 pymovie-3.7.5/
+-rw-rw-rw-   0        0        0     1098 2019-04-05 17:09:16.000000 pymovie-3.7.5/LICENSE
+-rw-rw-rw-   0        0        0     1474 2023-05-12 16:54:09.180386 pymovie-3.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2019-04-05 17:32:17.000000 pymovie-3.7.5/README.rst
+-rw-rw-rw-   0        0        0       80 2023-05-12 16:54:09.183395 pymovie-3.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-02-11 21:36:47.000000 pymovie-3.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:54:09.154395 pymovie-3.7.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 16:54:09.176395 pymovie-3.7.5/src/pymovie/
+-rw-rw-rw-   0        0        0      415 2022-01-05 20:02:47.000000 pymovie-3.7.5/src/pymovie/NE3Lut.p
+-rw-rw-rw-   0        0        0  2406045 2019-07-25 01:02:37.000000 pymovie-3.7.5/src/pymovie/PyMovie-doc.pdf
+-rw-rw-rw-   0        0        0   617532 2023-05-12 16:50:13.000000 pymovie-3.7.5/src/pymovie/PyMovie-info.pdf
+-rwxrwxrwx   0        0        0      389 2020-01-12 05:29:48.000000 pymovie-3.7.5/src/pymovie/PyMovie.bat
+-rw-rw-rw-   0        0        0     6074 2023-05-12 16:19:29.000000 pymovie-3.7.5/src/pymovie/SER.py
+-rw-rw-rw-   0        0        0        0 2019-04-05 17:38:51.000000 pymovie-3.7.5/src/pymovie/__init__.py
+-rw-rw-rw-   0        0        0     2247 2019-06-29 16:49:47.000000 pymovie-3.7.5/src/pymovie/alias_lnk_resolver.py
+-rw-rw-rw-   0        0        0     4981 2023-05-12 16:19:29.000000 pymovie-3.7.5/src/pymovie/aperture.py
+-rw-rw-rw-   0        0        0    13197 2023-05-12 16:19:29.000000 pymovie-3.7.5/src/pymovie/apertureEdit.py
+-rw-rw-rw-   0        0        0     3674 2019-08-03 15:46:58.000000 pymovie-3.7.5/src/pymovie/apertureEditDialog.py
+-rw-rw-rw-   0        0        0     2118 2019-08-17 21:54:24.000000 pymovie-3.7.5/src/pymovie/apertureNameDialog.py
+-rw-rw-rw-   0        0        0     3869 2020-02-04 19:29:30.000000 pymovie-3.7.5/src/pymovie/aperturesFileTagDialog.py
+-rw-rw-rw-   0        0        0    10585 2020-01-12 05:29:48.000000 pymovie-3.7.5/src/pymovie/astrometry_client.py
+-rw-rw-rw-   0        0        0     5306 2023-02-08 15:51:31.000000 pymovie-3.7.5/src/pymovie/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0      873 2022-01-03 22:42:29.000000 pymovie-3.7.5/src/pymovie/gammaUtils.py
+-rw-rw-rw-   0        0        0   219915 2023-05-12 16:19:29.000000 pymovie-3.7.5/src/pymovie/gui.py
+-rw-rw-rw-   0        0        0     2324 2019-06-08 18:46:48.000000 pymovie-3.7.5/src/pymovie/helpDialog.py
+-rw-rw-rw-   0        0        0     4236 2019-10-10 00:04:14.000000 pymovie-3.7.5/src/pymovie/hotPixelDialog.py
+-rw-rw-rw-   0        0        0   399960 2023-05-12 16:24:27.000000 pymovie-3.7.5/src/pymovie/main.py
+-rw-rw-rw-   0        0        0    28379 2020-10-13 12:32:19.000000 pymovie-3.7.5/src/pymovie/ocr.py
+-rw-rw-rw-   0        0        0     2129 2022-07-28 03:07:15.000000 pymovie-3.7.5/src/pymovie/ocrCharacterBox.py
+-rw-rw-rw-   0        0        0     2470 2019-06-27 01:59:32.000000 pymovie-3.7.5/src/pymovie/ocrProfileNameDialog.py
+-rw-rw-rw-   0        0        0      749 2019-12-19 02:19:32.000000 pymovie-3.7.5/src/pymovie/play-Temp.py
+-rw-rw-rw-   0        0        0      866 2019-12-29 20:26:21.000000 pymovie-3.7.5/src/pymovie/play-introspection.py
+-rwxrwxrwx   0        0        0      507 2019-06-08 00:30:37.000000 pymovie-3.7.5/src/pymovie/run-pymovie-mac.bat
+-rw-rw-rw-   0        0        0     3559 2019-10-10 18:10:06.000000 pymovie-3.7.5/src/pymovie/selectHotPixelProfile.py
+-rw-rw-rw-   0        0        0     3511 2019-07-06 18:14:37.000000 pymovie-3.7.5/src/pymovie/selectProfile.py
+-rw-rw-rw-   0        0        0    21278 2022-07-23 14:26:50.000000 pymovie-3.7.5/src/pymovie/stacker.py
+-rw-rw-rw-   0        0        0    12852 2022-05-09 22:42:27.000000 pymovie-3.7.5/src/pymovie/starPositionDialog.py
+-rw-rw-rw-   0        0        0       36 2023-05-12 16:49:04.000000 pymovie-3.7.5/src/pymovie/version.py
+-rw-rw-rw-   0        0        0     7574 2020-01-12 05:29:48.000000 pymovie-3.7.5/src/pymovie/wcs_helper_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:54:09.179386 pymovie-3.7.5/src/pymovie.egg-info/
+-rw-rw-rw-   0        0        0     1474 2023-05-12 16:54:08.000000 pymovie-3.7.5/src/pymovie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2023-05-12 16:54:08.000000 pymovie-3.7.5/src/pymovie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:54:08.000000 pymovie-3.7.5/src/pymovie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-04-05 23:49:13.000000 pymovie-3.7.5/src/pymovie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      247 2023-05-12 16:54:08.000000 pymovie-3.7.5/src/pymovie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 16:54:08.000000 pymovie-3.7.5/src/pymovie.egg-info/top_level.txt
```

### Comparing `pymovie-3.7.3/LICENSE` & `pymovie-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/PKG-INFO` & `pymovie-3.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.7.3
+Version: 3.7.5
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.7.3/setup.py` & `pymovie-3.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/PyMovie-doc.pdf` & `pymovie-3.7.5/src/pymovie/PyMovie-doc.pdf`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/SER.py` & `pymovie-3.7.5/src/pymovie/SER.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-import numpy as np
-import os
-from astropy.time import Time
-from datetime import datetime, timedelta
-
-
-SER_HEADER_SIZE = 178
-
-def sharpCapTimestamp(datetime64):
-
-    usecs = int(datetime64 // 10)
-    extra_digit = datetime64 - 10 * usecs
-    ts = (datetime(1, 1, 1) + timedelta(microseconds=usecs))
-
-    timestamp = (f'{ts.year}-{ts.month}-{ts.day}T{ts.hour:02d}:{ts.minute:02d}:{ts.second:02d}.{ts.microsecond:06d}'
-                f'{extra_digit}')
-    return timestamp
-
-def convertNETdatetimeToJD(datetime64):
-    jd = datetime64 / 864000000000 + 1721424.5
-    return jd
-
-
-def convertJDtoTimestamp(jd):
-    t = Time(jd, format='jd', precision=4)
-    return t.isot
-
-
-def stringFromByteArray(byteArray):
-    listOfCharacters = ""
-    for byte in byteArray:
-        listOfCharacters += chr(byte)
-    return "".join(listOfCharacters)
-
-
-def getMetaData(fpath):
-    # Using the SER format description version 3 by Gischa Hahn 2014 Feb 06,
-    # this function puts the meta-data into a dictionary and the timestamps (if any)
-    # into a list and returns both.  All 'endian' requirements are followed EXCEPT
-    # that the prevailing convention now is to treat a value of 0 in the LittleEndian
-    # field is specifying little-endian byte order in 16 bit image data (opposite of 'spec').
-
-    with open(fpath, 'rb') as f:
-
-        ans = {}
-        timestamps = []
-
-        raw_file_ID = np.fromfile(f, dtype='uint8', count=14)
-        FileID = stringFromByteArray(raw_file_ID)
-        ans.update(FileID=FileID)
-
-        # '<i4' specifies a little-endian 32 bit int
-        LuID = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(LuID=LuID)
-
-        ColorID = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(ColorID=ColorID)
-
-        if not ColorID == 0:  # monochrome image
-            raise ValueError("Color SER files not supported.  Only mono")
-
-        LittleEndian = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(LittleEndian=LittleEndian)
-
-        ImageWidth = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(ImageWidth=ImageWidth)
-
-        ImageHeight = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(ImageHeight=ImageHeight)
-
-        PixelDepthPerPlane = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(PixelDepthPerPlane=PixelDepthPerPlane)
-
-        FrameCount = np.fromfile(f, dtype='<i4', count=1)[0]
-        ans.update(FrameCount=FrameCount)
-
-        raw_observer = np.fromfile(f, dtype='uint8', count=40)
-        Observer = stringFromByteArray(raw_observer)
-        ans.update(Observer=Observer)
-
-        raw_instrument = np.fromfile(f, dtype='uint8', count=40)
-        Instrument = stringFromByteArray(raw_instrument)
-        ans.update(Instrument=Instrument)
-
-        raw_telescope = np.fromfile(f, dtype='uint8', count=40)
-        Telescope = stringFromByteArray(raw_telescope)
-        ans.update(Telescope=Telescope)
-
-        # '<i8' specifies a little-endian 64 bit integer
-        datetimeLocal = np.fromfile(f, dtype='<i8', count=1)[0]
-        # DateTimeLocal = convertJDtoTimestamp(convertNETdatetimeToJD(datetimeLocal))
-        DateTimeLocal = sharpCapTimestamp(datetimeLocal)
-        ans.update(DateTimeLocal=DateTimeLocal)
-
-        datetimeUTC = np.fromfile(f, dtype='<i8', count=1)[0]
-        # DateTimeUTC = convertJDtoTimestamp(convertNETdatetimeToJD(datetimeUTC))
-        DateTimeUTC = sharpCapTimestamp(datetimeUTC)
-
-        ans.update(DateTimeUTC=DateTimeUTC)
-
-        if PixelDepthPerPlane > 8:
-            BytesPerPixel = 2
-        else:
-            BytesPerPixel = 1
-        ans.update(BytesPerPixel=BytesPerPixel)
-
-        ImageDataSize = int(FrameCount) * int(ImageWidth) * int(ImageHeight) * int(BytesPerPixel)
-        ans.update(ImageDataSize=ImageDataSize)
-
-        # Two ways to get file size
-        # f.seek(0,2)           # set position to offset=0 from end of file
-        # fileSize = f.tell()   # tell what that position is
-        FileSize = os.path.getsize(fpath)
-        ans.update(FileSize=FileSize)
-
-        NumTimestamps = (FileSize - SER_HEADER_SIZE - ImageDataSize) / 8
-        ans.update(NumTimestamps=NumTimestamps)
-
-        PositionOfTimestamps = ImageDataSize + SER_HEADER_SIZE
-        ans.update(PositionOfTimestamps=PositionOfTimestamps)
-
-        if NumTimestamps > 0:
-            f.seek(PositionOfTimestamps)
-            for i in range(int(NumTimestamps)):
-                datetimeUTC = np.fromfile(f, dtype='<i8', count=1)[0]
-                DateTimeUTC = sharpCapTimestamp(datetimeUTC)
-                # DateTimeUTC = convertJDtoTimestamp(convertNETdatetimeToJD(datetimeUTC))
-                timestamps.append(DateTimeUTC)
-
-    return ans, timestamps
-
-def getSerImage(f, frameNum, bytes_per_pixel, image_width, image_height, little_endian):
-    # height is y axis   width is x axis
-    num_pixels_in_frame = image_height * image_width
-    frame_size = bytes_per_pixel * num_pixels_in_frame
-    frame_start = int(frame_size) * int(frameNum) + SER_HEADER_SIZE
-    f.seek(frame_start)
-    if bytes_per_pixel == 1:
-        img = np.fromfile(f, dtype='uint8', count=num_pixels_in_frame)
-    elif bytes_per_pixel == 2:
-        if little_endian == 0:
-            img = np.fromfile(f, dtype='<u2', count=num_pixels_in_frame)
-        else:
-            img = np.fromfile(f, dtype='>u2', count=num_pixels_in_frame)
-    else:
-        raise ValueError("bytes_per_pixel must be 1 or 2")
-    return img.reshape(image_height, image_width)
-
-#   test_file = r'/Users/bob/Dropbox/SER project/ser-files-from-jan/FireCapture/190822_212734.ser'
-#   meta_data, timestamps = getMetaData(test_file)
-#
-#   f = open(test_file, 'rb') # Leave file handle open to speed repeat reads from file
-#   image = getSerImage(f, 43, meta_data['BytesPerPixel'], meta_data['ImageWidth'], meta_data['ImageHeight'], meta_data['LittleEndian'])
+import numpy as np
+import os
+from astropy.time import Time
+from datetime import datetime, timedelta
+
+
+SER_HEADER_SIZE = 178
+
+def sharpCapTimestamp(datetime64):
+
+    usecs = int(datetime64 // 10)
+    extra_digit = datetime64 - 10 * usecs
+    ts = (datetime(1, 1, 1) + timedelta(microseconds=usecs))
+
+    timestamp = (f'{ts.year}-{ts.month}-{ts.day}T{ts.hour:02d}:{ts.minute:02d}:{ts.second:02d}.{ts.microsecond:06d}'
+                f'{extra_digit}')
+    return timestamp
+
+def convertNETdatetimeToJD(datetime64):
+    jd = datetime64 / 864000000000 + 1721424.5
+    return jd
+
+
+def convertJDtoTimestamp(jd):
+    t = Time(jd, format='jd', precision=4)
+    return t.isot
+
+
+def stringFromByteArray(byteArray):
+    listOfCharacters = ""
+    for byte in byteArray:
+        listOfCharacters += chr(byte)
+    return "".join(listOfCharacters)
+
+
+def getMetaData(fpath):
+    # Using the SER format description version 3 by Gischa Hahn 2014 Feb 06,
+    # this function puts the meta-data into a dictionary and the timestamps (if any)
+    # into a list and returns both.  All 'endian' requirements are followed EXCEPT
+    # that the prevailing convention now is to treat a value of 0 in the LittleEndian
+    # field is specifying little-endian byte order in 16 bit image data (opposite of 'spec').
+
+    with open(fpath, 'rb') as f:
+
+        ans = {}
+        timestamps = []
+
+        raw_file_ID = np.fromfile(f, dtype='uint8', count=14)
+        FileID = stringFromByteArray(raw_file_ID)
+        ans.update(FileID=FileID)
+
+        # '<i4' specifies a little-endian 32 bit int
+        LuID = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(LuID=LuID)
+
+        ColorID = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(ColorID=ColorID)
+
+        if not ColorID == 0:  # monochrome image
+            raise ValueError("Color SER files not supported.  Only mono")
+
+        LittleEndian = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(LittleEndian=LittleEndian)
+
+        ImageWidth = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(ImageWidth=ImageWidth)
+
+        ImageHeight = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(ImageHeight=ImageHeight)
+
+        PixelDepthPerPlane = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(PixelDepthPerPlane=PixelDepthPerPlane)
+
+        FrameCount = np.fromfile(f, dtype='<i4', count=1)[0]
+        ans.update(FrameCount=FrameCount)
+
+        raw_observer = np.fromfile(f, dtype='uint8', count=40)
+        Observer = stringFromByteArray(raw_observer)
+        ans.update(Observer=Observer)
+
+        raw_instrument = np.fromfile(f, dtype='uint8', count=40)
+        Instrument = stringFromByteArray(raw_instrument)
+        ans.update(Instrument=Instrument)
+
+        raw_telescope = np.fromfile(f, dtype='uint8', count=40)
+        Telescope = stringFromByteArray(raw_telescope)
+        ans.update(Telescope=Telescope)
+
+        # '<i8' specifies a little-endian 64 bit integer
+        datetimeLocal = np.fromfile(f, dtype='<i8', count=1)[0]
+        # DateTimeLocal = convertJDtoTimestamp(convertNETdatetimeToJD(datetimeLocal))
+        DateTimeLocal = sharpCapTimestamp(datetimeLocal)
+        ans.update(DateTimeLocal=DateTimeLocal)
+
+        datetimeUTC = np.fromfile(f, dtype='<i8', count=1)[0]
+        # DateTimeUTC = convertJDtoTimestamp(convertNETdatetimeToJD(datetimeUTC))
+        DateTimeUTC = sharpCapTimestamp(datetimeUTC)
+
+        ans.update(DateTimeUTC=DateTimeUTC)
+
+        if PixelDepthPerPlane > 8:
+            BytesPerPixel = 2
+        else:
+            BytesPerPixel = 1
+        ans.update(BytesPerPixel=BytesPerPixel)
+
+        ImageDataSize = int(FrameCount) * int(ImageWidth) * int(ImageHeight) * int(BytesPerPixel)
+        ans.update(ImageDataSize=ImageDataSize)
+
+        # Two ways to get file size
+        # f.seek(0,2)           # set position to offset=0 from end of file
+        # fileSize = f.tell()   # tell what that position is
+        FileSize = os.path.getsize(fpath)
+        ans.update(FileSize=FileSize)
+
+        NumTimestamps = (FileSize - SER_HEADER_SIZE - ImageDataSize) / 8
+        ans.update(NumTimestamps=NumTimestamps)
+
+        PositionOfTimestamps = ImageDataSize + SER_HEADER_SIZE
+        ans.update(PositionOfTimestamps=PositionOfTimestamps)
+
+        if NumTimestamps > 0:
+            f.seek(PositionOfTimestamps)
+            for i in range(int(NumTimestamps)):
+                datetimeUTC = np.fromfile(f, dtype='<i8', count=1)[0]
+                DateTimeUTC = sharpCapTimestamp(datetimeUTC)
+                # DateTimeUTC = convertJDtoTimestamp(convertNETdatetimeToJD(datetimeUTC))
+                timestamps.append(DateTimeUTC)
+
+    return ans, timestamps
+
+def getSerImage(f, frameNum, bytes_per_pixel, image_width, image_height, little_endian):
+    # height is y axis   width is x axis
+    num_pixels_in_frame = image_height * image_width
+    frame_size = bytes_per_pixel * num_pixels_in_frame
+    frame_start = int(frame_size) * int(frameNum) + SER_HEADER_SIZE
+    f.seek(frame_start)
+    if bytes_per_pixel == 1:
+        img = np.fromfile(f, dtype='uint8', count=num_pixels_in_frame)
+    elif bytes_per_pixel == 2:
+        if little_endian == 0:
+            img = np.fromfile(f, dtype='<u2', count=num_pixels_in_frame)
+        else:
+            img = np.fromfile(f, dtype='>u2', count=num_pixels_in_frame)
+    else:
+        raise ValueError("bytes_per_pixel must be 1 or 2")
+    return img.reshape(image_height, image_width)
+
+#   test_file = r'/Users/bob/Dropbox/SER project/ser-files-from-jan/FireCapture/190822_212734.ser'
+#   meta_data, timestamps = getMetaData(test_file)
+#
+#   f = open(test_file, 'rb') # Leave file handle open to speed repeat reads from file
+#   image = getSerImage(f, 43, meta_data['BytesPerPixel'], meta_data['ImageWidth'], meta_data['ImageHeight'], meta_data['LittleEndian'])
 #   f.close() # Remember to close the file handle when no more images need to read from the file
```

### Comparing `pymovie-3.7.3/src/pymovie/alias_lnk_resolver.py` & `pymovie-3.7.5/src/pymovie/alias_lnk_resolver.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/aperture.py` & `pymovie-3.7.5/src/pymovie/aperture.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import pyqtgraph as pg
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.QtWidgets import QDialog
-from pymovie import apertureNameDialog
-import PyQt5
-
-
-class AppNameDialog(QDialog, apertureNameDialog.Ui_Dialog):
-    def __init__(self):
-        super(AppNameDialog, self).__init__()
-        self.setupUi(self)
-
-
-class HorizontalLine(pg.GraphicsObject):
-    def __init__(self, rowNumber, height, width, colorStr):  # Initialize aperture specified by a bounding box
-        self.pen = pg.mkPen(colorStr)
-        self.y0 = rowNumber
-        self.x0 = 0
-        self.x1 = width
-        self.h = height
-        self.w = width
-
-        # note that the use of super() is often avoided because Qt does not
-        # allow to inherit from multiple QObject subclasses.
-        pg.GraphicsObject.__init__(self)
-
-    # All graphics items must have paint() defined.
-    def paint(self, p, *args):
-        _ = args  # Just to satisfy PyCharm code inspector (need to use args in some manner)
-        p.setPen(self.pen)
-        p.drawLine(self.x0, self.y0, self.x1, self.y0)
-
-    # All graphics items must have boundingRect() defined.
-    def boundingRect(self):
-        return PyQt5.QtCore.QRectF(0, 0, self.w, self.h)
-
-    def setRow(self, row):
-        self.y0 = row
-        self.update()
-
-
-class MeasurementAperture(pg.GraphicsObject):
-
-    def __init__(self, name, bbox, max_xpos, max_ypos):  # Initialize aperture specified by a bounding box
-        self.name = name
-        self.thresh = 0
-        self.pen = pg.mkPen('r')
-        self.color = 'red'
-        self.x0, self.y0, self.xsize, self.ysize = bbox
-
-        self.jogging_enabled = False
-        self.auto_display = False
-        self.thumbnail_source = False
-
-        self.default_mask_radius = 3.0
-        self.order_number = 0
-        self.defaultMask = None
-        self.defaultMaskPixelCount = None
-
-        self.theta = None   # Holds angle to yellow #1 (if present)
-        self.dx = None      # Holds x distance from yellow #1
-        self.dy = None      # Holds y distance from yellow #1
-
-        self.xc = None      # Will hold current x value of centroid in image coordinates
-        self.yc = None      # Will hold current y value of centroid in image coordinates
-
-        self.data = []
-
-        # When created, we accept the callers restriction on the placement
-        # of a bbox (bounding box) corner and enforce
-        self.max_xpos = max_xpos
-        self.max_ypos = max_ypos
-
-        # Enforce the restrictions even during creation
-        self.enforcePositioningConstraints(bbox)
-
-        # menu creation is deferred because it is expensive (not really) and often
-        # the user will never see the menu anyway.
-        self.menu = None
-
-        # note that the use of super() is often avoided because Qt does not
-        # allow to inherit from multiple QObject subclasses.
-        pg.GraphicsObject.__init__(self)
-
-    def getBbox(self):
-        return self.x0, self.y0, self.xsize, self.ysize
-
-    def getCenter(self):
-        return self.x0 + int(self.xsize / 2), self.y0 + int(self.ysize / 2)
-
-    def setCenter(self, xc, yc):
-        delta = int(self.xsize / 2)
-        bbox = (xc - delta, yc - delta, self.xsize, self.ysize)
-        self.enforcePositioningConstraints(bbox)
-
-    def addData(self, data_tuple):
-        self.data.append(data_tuple)
-
-    def enforcePositioningConstraints(self, bbox):
-        self.x0, self.y0, self.xsize, self.ysize = bbox
-
-        # Enforce placement constraints
-        if self.x0 < 0:
-            self.x0 = 0
-        if self.x0 > self.max_xpos:
-            self.x0 = self.max_xpos
-
-        if self.y0 < 0:
-            self.y0 = 0
-        if self.y0 > self.max_ypos:
-            self.y0 = self.max_ypos
-
-    def setPos(self, bbox):
-        self.enforcePositioningConstraints(bbox)
-
-    # All graphics items must have boundingRect() defined.
-    def boundingRect(self):
-        return PyQt5.QtCore.QRectF(self.x0, self.y0, self.xsize, self.ysize)
-
-    # All graphics items must have paint() defined.
-    def paint(self, p, *args):
-        _ = args  # Just to satisfy PyCharm code inspector (need to use args in some manner)
-        p.setPen(self.pen)
-        p.drawRect(self.boundingRect())
-        p.setPen(pg.mkPen('y'))
-        p.drawLine(self.x0, self.y0, self.x0 + self.xsize, self.y0 + self.ysize)
-        p.drawLine(self.x0, self.y0 + self.ysize, self.x0 + self.xsize, self.y0)
-
-    def setGreen(self):
-        self.pen = pg.mkPen('g')
-        self.color = 'green'
-        self.update()
-
-    def setRed(self):
-        self.pen = pg.mkPen('r')
-        self.color = 'red'
-        self.update()
-
-    def setWhite(self):
-        self.pen = pg.mkPen('w')
-        self.color = 'white'
-        self.update()
-
-    def setYellowNoCheck(self):
-        self.pen = pg.mkPen('y')
-        self.color = 'yellow'
-        self.update()
+import pyqtgraph as pg
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QDialog
+from pymovie import apertureNameDialog
+import PyQt5
+
+
+class AppNameDialog(QDialog, apertureNameDialog.Ui_Dialog):
+    def __init__(self):
+        super(AppNameDialog, self).__init__()
+        self.setupUi(self)
+
+
+class HorizontalLine(pg.GraphicsObject):
+    def __init__(self, rowNumber, height, width, colorStr):  # Initialize aperture specified by a bounding box
+        self.pen = pg.mkPen(colorStr)
+        self.y0 = rowNumber
+        self.x0 = 0
+        self.x1 = width
+        self.h = height
+        self.w = width
+
+        # note that the use of super() is often avoided because Qt does not
+        # allow to inherit from multiple QObject subclasses.
+        pg.GraphicsObject.__init__(self)
+
+    # All graphics items must have paint() defined.
+    def paint(self, p, *args):
+        _ = args  # Just to satisfy PyCharm code inspector (need to use args in some manner)
+        p.setPen(self.pen)
+        p.drawLine(self.x0, self.y0, self.x1, self.y0)
+
+    # All graphics items must have boundingRect() defined.
+    def boundingRect(self):
+        return PyQt5.QtCore.QRectF(0, 0, self.w, self.h)
+
+    def setRow(self, row):
+        self.y0 = row
+        self.update()
+
+
+class MeasurementAperture(pg.GraphicsObject):
+
+    def __init__(self, name, bbox, max_xpos, max_ypos):  # Initialize aperture specified by a bounding box
+        self.name = name
+        self.thresh = 0
+        self.pen = pg.mkPen('r')
+        self.color = 'red'
+        self.x0, self.y0, self.xsize, self.ysize = bbox
+
+        self.jogging_enabled = False
+        self.auto_display = False
+        self.thumbnail_source = False
+
+        self.default_mask_radius = 3.0
+        self.order_number = 0
+        self.defaultMask = None
+        self.defaultMaskPixelCount = None
+
+        self.theta = None   # Holds angle to yellow #1 (if present)
+        self.dx = None      # Holds x distance from yellow #1
+        self.dy = None      # Holds y distance from yellow #1
+
+        self.xc = None      # Will hold current x value of centroid in image coordinates
+        self.yc = None      # Will hold current y value of centroid in image coordinates
+
+        self.data = []
+
+        # When created, we accept the callers restriction on the placement
+        # of a bbox (bounding box) corner and enforce
+        self.max_xpos = max_xpos
+        self.max_ypos = max_ypos
+
+        # Enforce the restrictions even during creation
+        self.enforcePositioningConstraints(bbox)
+
+        # menu creation is deferred because it is expensive (not really) and often
+        # the user will never see the menu anyway.
+        self.menu = None
+
+        # note that the use of super() is often avoided because Qt does not
+        # allow to inherit from multiple QObject subclasses.
+        pg.GraphicsObject.__init__(self)
+
+    def getBbox(self):
+        return self.x0, self.y0, self.xsize, self.ysize
+
+    def getCenter(self):
+        return self.x0 + int(self.xsize / 2), self.y0 + int(self.ysize / 2)
+
+    def setCenter(self, xc, yc):
+        delta = int(self.xsize / 2)
+        bbox = (xc - delta, yc - delta, self.xsize, self.ysize)
+        self.enforcePositioningConstraints(bbox)
+
+    def addData(self, data_tuple):
+        self.data.append(data_tuple)
+
+    def enforcePositioningConstraints(self, bbox):
+        self.x0, self.y0, self.xsize, self.ysize = bbox
+
+        # Enforce placement constraints
+        if self.x0 < 0:
+            self.x0 = 0
+        if self.x0 > self.max_xpos:
+            self.x0 = self.max_xpos
+
+        if self.y0 < 0:
+            self.y0 = 0
+        if self.y0 > self.max_ypos:
+            self.y0 = self.max_ypos
+
+    def setPos(self, bbox):
+        self.enforcePositioningConstraints(bbox)
+
+    # All graphics items must have boundingRect() defined.
+    def boundingRect(self):
+        return PyQt5.QtCore.QRectF(self.x0, self.y0, self.xsize, self.ysize)
+
+    # All graphics items must have paint() defined.
+    def paint(self, p, *args):
+        _ = args  # Just to satisfy PyCharm code inspector (need to use args in some manner)
+        p.setPen(self.pen)
+        p.drawRect(self.boundingRect())
+        p.setPen(pg.mkPen('y'))
+        p.drawLine(self.x0, self.y0, self.x0 + self.xsize, self.y0 + self.ysize)
+        p.drawLine(self.x0, self.y0 + self.ysize, self.x0 + self.xsize, self.y0)
+
+    def setGreen(self):
+        self.pen = pg.mkPen('g')
+        self.color = 'green'
+        self.update()
+
+    def setRed(self):
+        self.pen = pg.mkPen('r')
+        self.color = 'red'
+        self.update()
+
+    def setWhite(self):
+        self.pen = pg.mkPen('w')
+        self.color = 'white'
+        self.update()
+
+    def setYellowNoCheck(self):
+        self.pen = pg.mkPen('y')
+        self.color = 'yellow'
+        self.update()
```

### Comparing `pymovie-3.7.3/src/pymovie/apertureEdit.py` & `pymovie-3.7.5/src/pymovie/apertureEdit.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-from pymovie import apertureEditDialog
-from PyQt5.QtWidgets import QDialog
-from PyQt5 import QtGui
-from PyQt5 import QtCore
-from PyQt5.QtWidgets import QTableWidgetItem, QMenu, QAction
-import numpy as np
-
-
-class EditApertureDialog(QDialog, apertureEditDialog.Ui_Dialog):
-    def __init__(self, messager, saver, dictList, appSize, threshSpinner, imageUpdate, setThumbnails):
-        super(EditApertureDialog, self).__init__()
-        self.setupUi(self)
-        self.msgRoutine = messager
-        self.settingsSaver = saver
-        self.dictList = dictList
-        self.fillApertureTable()
-        self.appSize = appSize
-        self.threshSpinner = threshSpinner
-        self.imageUpdate = imageUpdate
-        self.tableWidget.cellClicked.connect(self.cellClicked)
-        self.tableWidget.cellChanged.connect(self.cellClicked)
-        self.tableWidget.cellActivated.connect(self.cellClicked)
-        self.tableWidget.itemSelectionChanged.connect(self.selectionChange)
-        self.setThumbnails = setThumbnails
-        self.ignoreCellClick = False
-        self.col = None
-        self.row = None
-        self.menu = None
-
-    def selectionChange(self):
-        row = self.tableWidget.currentRow()
-        col = self.tableWidget.currentColumn()
-        self.cellClicked(row, col)
-
-    def cellClicked(self, row, column):
-        if self.ignoreCellClick:
-            self.ignoreCellClick = False
-            return
-        # self.msgRoutine( f'row {row} column {column} was clicked')
-        aperture = self.dictList[row]['appRef']
-        self.writeTable()
-        showDefaultMaskInThumbnailTwo = column == 3
-        self.setThumbnails(aperture, showDefaultMaskInThumbnailTwo)
-        # The xy position may have changed because of 'snap' when threshold is changed.
-        self.ignoreCellClick = True
-        xc, yc = aperture.getCenter()
-        item = QTableWidgetItem(str(f'({xc},{yc})'))
-        self.tableWidget.setItem(row, 1, item)
-
-    def writeTable(self):
-        self.updateAperturesFromTable()
-
-    def fillApertureTable(self):
-        for rowDict in self.dictList:
-            numRows = self.tableWidget.rowCount()
-            self.tableWidget.insertRow(numRows)
-
-            item = QTableWidgetItem(str(rowDict['name']))
-            self.tableWidget.setItem(numRows, 0, item)
-
-            item = QTableWidgetItem(str(rowDict['xy']))
-            self.tableWidget.setItem(numRows, 1, item)
-
-            item = QTableWidgetItem(str(rowDict['threshDelta']))
-            self.tableWidget.setItem(numRows, 2, item)
-
-            item = QTableWidgetItem(str(rowDict['defMskRadius']))
-            self.tableWidget.setItem(numRows, 3, item)
-
-            color_str = str(rowDict['color'])
-            if color_str.startswith('red'):
-                item = QTableWidgetItem('red (standard)')
-            elif color_str.startswith('green'):
-                item = QTableWidgetItem('green (connect to threshold spinner)')
-            elif color_str.startswith('yellow'):
-                item = QTableWidgetItem('yellow (tracking aperture)')
-            elif color_str.startswith('white'):
-                item = QTableWidgetItem('white (special flash tag aperture')
-            # item = QTableWidgetItem(str(rowDict['color']))
-            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-            self.tableWidget.setItem(numRows, 4, item)
-
-            item = QTableWidgetItem(str(rowDict['joggable']))
-            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-            self.tableWidget.setItem(numRows, 5, item)
-
-            item = QTableWidgetItem(str(rowDict['autoTextOut']))
-            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-            self.tableWidget.setItem(numRows, 6, item)
-
-            item = QTableWidgetItem(str(rowDict['thumbnailSource']))
-            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-            self.tableWidget.setItem(numRows, 7, item)
-
-            item = QTableWidgetItem(str(rowDict['outputOrder']))
-            self.tableWidget.setItem(numRows, 8, item)
-
-    def createDefaultMask(self, radius):
-        mask = np.zeros((self.appSize, self.appSize), 'int16')
-        maskPixelCount = 0
-        roi_center = int(self.appSize / 2)
-        c = roi_center
-        r = int(np.ceil(radius))
-        if r > c - 1:
-            r = c - 1
-            radius = r
-        for i in range(c - r - 1, c + r + 2):
-            for j in range(c - r - 1, c + r + 2):
-                if (i - c) ** 2 + (j - c) ** 2 <= radius ** 2:
-                    maskPixelCount += 1
-                    mask[i, j] = 1
-        return mask, maskPixelCount, radius
-
-    def closeEvent(self, event):
-        self.settingsSaver.setValue('appEditDialogSize', self.size())
-        self.settingsSaver.setValue('appEditDialogPos', self.pos())
-        self.updateAperturesFromTable()
-
-    def parseXY(self, xyText):
-        # noinspection PyBroadException
-        try:
-            parts = xyText.split(",")
-            xc = int(parts[0].strip().strip("(").strip())
-            yc = int(parts[1].strip().strip(")").strip())
-        except:
-            self.msgRoutine(f'"{xyText}" is an invalid format for x,y')
-            return None, None
-        return xc, yc
-
-    def updateAperturesFromTable(self):
-
-        # Now comes the hard work of validating and using the tableWidget data
-        # to update the aperture properties
-
-        for row in range(self.tableWidget.rowCount()):
-
-            aperture = self.dictList[row]['appRef']
-
-            xyText = self.tableWidget.item(row, 1).text()
-            xc, yc = self.parseXY(xyText=xyText)
-            if xc is not None:
-                aperture.setCenter(xc, yc)
-                self.imageUpdate()
-
-            aperture.name = self.tableWidget.item(row, 0).text()
-
-            # Enforce that thresh is a positive integer
-            text = self.tableWidget.item(row, 2).text()
-            try:
-                thresh = int(text)
-            except ValueError:
-                self.msgRoutine(f'In {aperture.name}(thresh): {text} is not a valid integer')
-                return
-            if thresh < 0:
-                self.msgRoutine(f'In {aperture.name}(thresh): {text} is not a positive integer')
-                return
-            aperture.thresh = thresh
-
-            # Enforce that def mask radius has value between 2.0 and 24.0
-            text = self.tableWidget.item(row, 3).text()
-            try:
-                radius = float(text)
-            except ValueError:
-                self.msgRoutine(f'In {aperture.name}(def mask radius): {text} is not a valid float')
-                return
-            if radius < 2.0:
-                self.msgRoutine(f'In {aperture.name}(def mask radius): {text} cannot be less than 2.0')
-                return
-            aperture.default_mask_radius = radius
-
-            aperture.defaultMask, aperture.defaultMaskPixelCount, aperture.default_mask_radius = \
-                self.createDefaultMask(radius)
-
-            aperture.color = self.tableWidget.item(row, 4).text()
-            if aperture.color.startswith('green'):
-                aperture.setGreen()
-                self.updateSpinnersFromRow(row)
-            elif aperture.color.startswith('red'):
-                aperture.setRed()
-            elif aperture.color.startswith('white'):
-                aperture.setWhite()
-            elif aperture.color.startswith('yellow'):
-                aperture.setYellowNoCheck()
-
-            text = self.tableWidget.item(row, 5).text()
-            if text == 'True':
-                aperture.jogging_enabled = True
-            else:
-                aperture.jogging_enabled = False
-
-            text = self.tableWidget.item(row, 6).text()
-            if text == 'True':
-                aperture.auto_display = True
-            else:
-                aperture.auto_display = False
-
-            text = self.tableWidget.item(row, 7).text()
-            if text == 'True':
-                aperture.thumbnail_source = True
-            else:
-                aperture.thumbnail_source = False
-
-            # Enforce that output order is a positive integer
-            text = self.tableWidget.item(row, 8).text()
-            try:
-                order = int(text)
-            except ValueError:
-                self.msgRoutine(f'In {aperture.name}(order): {text} is not a valid integer')
-                return
-            if order < 0:
-                self.msgRoutine(f'In {aperture.name}(order): {text} is not a positive integer')
-                return
-            aperture.order_number = order
-
-    def contextMenuEvent(self, event):
-        # self.msgRoutine("Got a right-click event")
-        self.col = self.tableWidget.currentColumn()
-        self.row = self.tableWidget.currentRow()
-        items = self.tableWidget.selectedItems()
-        if not items:
-            self.msgRoutine('Nothing selected')
-            return
-        # self.msgRoutine(f'row: {self.row}  column: {self.col} items: {items[0]}')
-
-        if 5 <= self.col <= 7:
-            self.menu = QMenu()
-            # self.menu = QtGui.QMenu()
-            doTrue = QAction("Set True", self)
-            doTrue.triggered.connect(self.setTrue)
-            self.menu.addAction(doTrue)
-
-            doFalse = QAction("Set False", self)
-            doFalse.triggered.connect(self.setFalse)
-            self.menu.addAction(doFalse)
-
-            self.menu.popup(QtGui.QCursor.pos())
-        elif self.col == 4:
-            self.menu = QMenu()
-            # self.menu = QtGui.QMenu()
-
-            setRed = QAction("Set red (standard)", self)
-            setRed.triggered.connect(self.setRed)
-            self.menu.addAction(setRed)
-
-            setGreen = QAction("Set green (connect to threshold spinner)", self)
-            setGreen.triggered.connect(self.setGreen)
-            self.menu.addAction(setGreen)
-
-            setYellow = QAction("Set yellow (tracking aperture)", self)
-            setYellow.triggered.connect(self.setYellow)
-            self.menu.addAction(setYellow)
-
-            setWhite = QAction("Set white (special flash tag aperture)", self)
-            setWhite.triggered.connect(self.setWhite)
-            self.menu.addAction(setWhite)
-
-            self.menu.popup(QtGui.QCursor.pos())
-
-    def setTrue(self):
-        if self.col == 7:
-            # We enforce the condition that only one aperture
-            # can have True for this property
-            for row in range(self.tableWidget.rowCount()):
-                item = QTableWidgetItem('False')
-                item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-                self.tableWidget.setItem(row, self.col, item)
-
-        item = QTableWidgetItem('True')
-        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-        self.tableWidget.setItem(self.row, self.col, item)
-
-    def setFalse(self):
-        item = QTableWidgetItem('False')
-        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-        self.tableWidget.setItem(self.row, self.col, item)
-
-    def setRed(self):
-        item = QTableWidgetItem('red (standard)')
-        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-        self.tableWidget.setItem(self.row, self.col, item)
-
-    def setGreen(self):
-        for row in range(self.tableWidget.rowCount()):
-            # To automatically enforce the 'only one green' policy, turn any existing
-            # 'green' to 'red'
-            if self.tableWidget.item(row, self.col).text().startswith('green'):
-                item = QTableWidgetItem('red (standard)')
-                item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-                self.tableWidget.setItem(row, self.col, item)
-        item = QTableWidgetItem('green (connect to threshold spinner)')
-        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-        self.tableWidget.setItem(self.row, self.col, item)
-
-        self.updateSpinnersFromRow(self.row)
-
-    def updateSpinnersFromRow(self, row):
-
-        try:
-            thresh = int(self.tableWidget.item(row, 2).text())
-        except ValueError:
-            thresh = 0
-        if thresh < 0:
-            thresh = 0
-
-        self.threshSpinner.setValue(thresh)
-
-    def setYellow(self):
-        numYellow = 0
-        for row in range(self.tableWidget.rowCount()):
-            if self.tableWidget.item(row, self.col).text().startswith('yellow'):
-                numYellow += 1
-
-        if numYellow == 2:
-            self.msgRoutine(f'!!! There can only be a max of two yellow apertures !!!')
-            return
-
-        item = QTableWidgetItem('yellow (tracking aperture)')
-        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-        self.tableWidget.setItem(self.row, self.col, item)
-
-    def setWhite(self):
-        item = QTableWidgetItem('white (special flash tag aperture)')
-        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
-        self.tableWidget.setItem(self.row, self.col, item)
+from pymovie import apertureEditDialog
+from PyQt5.QtWidgets import QDialog
+from PyQt5 import QtGui
+from PyQt5 import QtCore
+from PyQt5.QtWidgets import QTableWidgetItem, QMenu, QAction
+import numpy as np
+
+
+class EditApertureDialog(QDialog, apertureEditDialog.Ui_Dialog):
+    def __init__(self, messager, saver, dictList, appSize, threshSpinner, imageUpdate, setThumbnails):
+        super(EditApertureDialog, self).__init__()
+        self.setupUi(self)
+        self.msgRoutine = messager
+        self.settingsSaver = saver
+        self.dictList = dictList
+        self.fillApertureTable()
+        self.appSize = appSize
+        self.threshSpinner = threshSpinner
+        self.imageUpdate = imageUpdate
+        self.tableWidget.cellClicked.connect(self.cellClicked)
+        self.tableWidget.cellChanged.connect(self.cellClicked)
+        self.tableWidget.cellActivated.connect(self.cellClicked)
+        self.tableWidget.itemSelectionChanged.connect(self.selectionChange)
+        self.setThumbnails = setThumbnails
+        self.ignoreCellClick = False
+        self.col = None
+        self.row = None
+        self.menu = None
+
+    def selectionChange(self):
+        row = self.tableWidget.currentRow()
+        col = self.tableWidget.currentColumn()
+        self.cellClicked(row, col)
+
+    def cellClicked(self, row, column):
+        if self.ignoreCellClick:
+            self.ignoreCellClick = False
+            return
+        # self.msgRoutine( f'row {row} column {column} was clicked')
+        aperture = self.dictList[row]['appRef']
+        self.writeTable()
+        showDefaultMaskInThumbnailTwo = column == 3
+        self.setThumbnails(aperture, showDefaultMaskInThumbnailTwo)
+        # The xy position may have changed because of 'snap' when threshold is changed.
+        self.ignoreCellClick = True
+        xc, yc = aperture.getCenter()
+        item = QTableWidgetItem(str(f'({xc},{yc})'))
+        self.tableWidget.setItem(row, 1, item)
+
+    def writeTable(self):
+        self.updateAperturesFromTable()
+
+    def fillApertureTable(self):
+        for rowDict in self.dictList:
+            numRows = self.tableWidget.rowCount()
+            self.tableWidget.insertRow(numRows)
+
+            item = QTableWidgetItem(str(rowDict['name']))
+            self.tableWidget.setItem(numRows, 0, item)
+
+            item = QTableWidgetItem(str(rowDict['xy']))
+            self.tableWidget.setItem(numRows, 1, item)
+
+            item = QTableWidgetItem(str(rowDict['threshDelta']))
+            self.tableWidget.setItem(numRows, 2, item)
+
+            item = QTableWidgetItem(str(rowDict['defMskRadius']))
+            self.tableWidget.setItem(numRows, 3, item)
+
+            color_str = str(rowDict['color'])
+            if color_str.startswith('red'):
+                item = QTableWidgetItem('red (standard)')
+            elif color_str.startswith('green'):
+                item = QTableWidgetItem('green (connect to threshold spinner)')
+            elif color_str.startswith('yellow'):
+                item = QTableWidgetItem('yellow (tracking aperture)')
+            elif color_str.startswith('white'):
+                item = QTableWidgetItem('white (special flash tag aperture')
+            # item = QTableWidgetItem(str(rowDict['color']))
+            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+            self.tableWidget.setItem(numRows, 4, item)
+
+            item = QTableWidgetItem(str(rowDict['joggable']))
+            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+            self.tableWidget.setItem(numRows, 5, item)
+
+            item = QTableWidgetItem(str(rowDict['autoTextOut']))
+            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+            self.tableWidget.setItem(numRows, 6, item)
+
+            item = QTableWidgetItem(str(rowDict['thumbnailSource']))
+            item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+            self.tableWidget.setItem(numRows, 7, item)
+
+            item = QTableWidgetItem(str(rowDict['outputOrder']))
+            self.tableWidget.setItem(numRows, 8, item)
+
+    def createDefaultMask(self, radius):
+        mask = np.zeros((self.appSize, self.appSize), 'int16')
+        maskPixelCount = 0
+        roi_center = int(self.appSize / 2)
+        c = roi_center
+        r = int(np.ceil(radius))
+        if r > c - 1:
+            r = c - 1
+            radius = r
+        for i in range(c - r - 1, c + r + 2):
+            for j in range(c - r - 1, c + r + 2):
+                if (i - c) ** 2 + (j - c) ** 2 <= radius ** 2:
+                    maskPixelCount += 1
+                    mask[i, j] = 1
+        return mask, maskPixelCount, radius
+
+    def closeEvent(self, event):
+        self.settingsSaver.setValue('appEditDialogSize', self.size())
+        self.settingsSaver.setValue('appEditDialogPos', self.pos())
+        self.updateAperturesFromTable()
+
+    def parseXY(self, xyText):
+        # noinspection PyBroadException
+        try:
+            parts = xyText.split(",")
+            xc = int(parts[0].strip().strip("(").strip())
+            yc = int(parts[1].strip().strip(")").strip())
+        except:
+            self.msgRoutine(f'"{xyText}" is an invalid format for x,y')
+            return None, None
+        return xc, yc
+
+    def updateAperturesFromTable(self):
+
+        # Now comes the hard work of validating and using the tableWidget data
+        # to update the aperture properties
+
+        for row in range(self.tableWidget.rowCount()):
+
+            aperture = self.dictList[row]['appRef']
+
+            xyText = self.tableWidget.item(row, 1).text()
+            xc, yc = self.parseXY(xyText=xyText)
+            if xc is not None:
+                aperture.setCenter(xc, yc)
+                self.imageUpdate()
+
+            aperture.name = self.tableWidget.item(row, 0).text()
+
+            # Enforce that thresh is a positive integer
+            text = self.tableWidget.item(row, 2).text()
+            try:
+                thresh = int(text)
+            except ValueError:
+                self.msgRoutine(f'In {aperture.name}(thresh): {text} is not a valid integer')
+                return
+            if thresh < 0:
+                self.msgRoutine(f'In {aperture.name}(thresh): {text} is not a positive integer')
+                return
+            aperture.thresh = thresh
+
+            # Enforce that def mask radius has value between 2.0 and 24.0
+            text = self.tableWidget.item(row, 3).text()
+            try:
+                radius = float(text)
+            except ValueError:
+                self.msgRoutine(f'In {aperture.name}(def mask radius): {text} is not a valid float')
+                return
+            if radius < 2.0:
+                self.msgRoutine(f'In {aperture.name}(def mask radius): {text} cannot be less than 2.0')
+                return
+            aperture.default_mask_radius = radius
+
+            aperture.defaultMask, aperture.defaultMaskPixelCount, aperture.default_mask_radius = \
+                self.createDefaultMask(radius)
+
+            aperture.color = self.tableWidget.item(row, 4).text()
+            if aperture.color.startswith('green'):
+                aperture.setGreen()
+                self.updateSpinnersFromRow(row)
+            elif aperture.color.startswith('red'):
+                aperture.setRed()
+            elif aperture.color.startswith('white'):
+                aperture.setWhite()
+            elif aperture.color.startswith('yellow'):
+                aperture.setYellowNoCheck()
+
+            text = self.tableWidget.item(row, 5).text()
+            if text == 'True':
+                aperture.jogging_enabled = True
+            else:
+                aperture.jogging_enabled = False
+
+            text = self.tableWidget.item(row, 6).text()
+            if text == 'True':
+                aperture.auto_display = True
+            else:
+                aperture.auto_display = False
+
+            text = self.tableWidget.item(row, 7).text()
+            if text == 'True':
+                aperture.thumbnail_source = True
+            else:
+                aperture.thumbnail_source = False
+
+            # Enforce that output order is a positive integer
+            text = self.tableWidget.item(row, 8).text()
+            try:
+                order = int(text)
+            except ValueError:
+                self.msgRoutine(f'In {aperture.name}(order): {text} is not a valid integer')
+                return
+            if order < 0:
+                self.msgRoutine(f'In {aperture.name}(order): {text} is not a positive integer')
+                return
+            aperture.order_number = order
+
+    def contextMenuEvent(self, event):
+        # self.msgRoutine("Got a right-click event")
+        self.col = self.tableWidget.currentColumn()
+        self.row = self.tableWidget.currentRow()
+        items = self.tableWidget.selectedItems()
+        if not items:
+            self.msgRoutine('Nothing selected')
+            return
+        # self.msgRoutine(f'row: {self.row}  column: {self.col} items: {items[0]}')
+
+        if 5 <= self.col <= 7:
+            self.menu = QMenu()
+            # self.menu = QtGui.QMenu()
+            doTrue = QAction("Set True", self)
+            doTrue.triggered.connect(self.setTrue)
+            self.menu.addAction(doTrue)
+
+            doFalse = QAction("Set False", self)
+            doFalse.triggered.connect(self.setFalse)
+            self.menu.addAction(doFalse)
+
+            self.menu.popup(QtGui.QCursor.pos())
+        elif self.col == 4:
+            self.menu = QMenu()
+            # self.menu = QtGui.QMenu()
+
+            setRed = QAction("Set red (standard)", self)
+            setRed.triggered.connect(self.setRed)
+            self.menu.addAction(setRed)
+
+            setGreen = QAction("Set green (connect to threshold spinner)", self)
+            setGreen.triggered.connect(self.setGreen)
+            self.menu.addAction(setGreen)
+
+            setYellow = QAction("Set yellow (tracking aperture)", self)
+            setYellow.triggered.connect(self.setYellow)
+            self.menu.addAction(setYellow)
+
+            setWhite = QAction("Set white (special flash tag aperture)", self)
+            setWhite.triggered.connect(self.setWhite)
+            self.menu.addAction(setWhite)
+
+            self.menu.popup(QtGui.QCursor.pos())
+
+    def setTrue(self):
+        if self.col == 7:
+            # We enforce the condition that only one aperture
+            # can have True for this property
+            for row in range(self.tableWidget.rowCount()):
+                item = QTableWidgetItem('False')
+                item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+                self.tableWidget.setItem(row, self.col, item)
+
+        item = QTableWidgetItem('True')
+        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+        self.tableWidget.setItem(self.row, self.col, item)
+
+    def setFalse(self):
+        item = QTableWidgetItem('False')
+        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+        self.tableWidget.setItem(self.row, self.col, item)
+
+    def setRed(self):
+        item = QTableWidgetItem('red (standard)')
+        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+        self.tableWidget.setItem(self.row, self.col, item)
+
+    def setGreen(self):
+        for row in range(self.tableWidget.rowCount()):
+            # To automatically enforce the 'only one green' policy, turn any existing
+            # 'green' to 'red'
+            if self.tableWidget.item(row, self.col).text().startswith('green'):
+                item = QTableWidgetItem('red (standard)')
+                item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+                self.tableWidget.setItem(row, self.col, item)
+        item = QTableWidgetItem('green (connect to threshold spinner)')
+        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+        self.tableWidget.setItem(self.row, self.col, item)
+
+        self.updateSpinnersFromRow(self.row)
+
+    def updateSpinnersFromRow(self, row):
+
+        try:
+            thresh = int(self.tableWidget.item(row, 2).text())
+        except ValueError:
+            thresh = 0
+        if thresh < 0:
+            thresh = 0
+
+        self.threshSpinner.setValue(thresh)
+
+    def setYellow(self):
+        numYellow = 0
+        for row in range(self.tableWidget.rowCount()):
+            if self.tableWidget.item(row, self.col).text().startswith('yellow'):
+                numYellow += 1
+
+        if numYellow == 2:
+            self.msgRoutine(f'!!! There can only be a max of two yellow apertures !!!')
+            return
+
+        item = QTableWidgetItem('yellow (tracking aperture)')
+        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+        self.tableWidget.setItem(self.row, self.col, item)
+
+    def setWhite(self):
+        item = QTableWidgetItem('white (special flash tag aperture)')
+        item.setFlags(item.flags() ^ QtCore.Qt.ItemIsEditable)
+        self.tableWidget.setItem(self.row, self.col, item)
```

### Comparing `pymovie-3.7.3/src/pymovie/apertureEditDialog.py` & `pymovie-3.7.5/src/pymovie/apertureEditDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/apertureNameDialog.py` & `pymovie-3.7.5/src/pymovie/apertureNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/aperturesFileTagDialog.py` & `pymovie-3.7.5/src/pymovie/aperturesFileTagDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/astrometry_client.py` & `pymovie-3.7.5/src/pymovie/astrometry_client.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/checkForNewerVersion.py` & `pymovie-3.7.5/src/pymovie/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/gammaUtils.py` & `pymovie-3.7.5/src/pymovie/gammaUtils.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/gui.py` & `pymovie-3.7.5/src/pymovie/gui.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/helpDialog.py` & `pymovie-3.7.5/src/pymovie/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/hotPixelDialog.py` & `pymovie-3.7.5/src/pymovie/hotPixelDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/main.py` & `pymovie-3.7.5/src/pymovie/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -6535,25 +6535,32 @@
                        (signal, appsum, mean, std, threshold, max_area, '    NA', '    NA', minpx, maxpx)
             self.showMsg(line)
 
         # xc_roi and yc_roi are used by centerAperture() to recenter the aperture
         # The remaining outputs are used in writing the lightcurve information
         # !!! ANY CHANGE TO THE TYPE OR ORDERING OF THIS OUTPUT MUST BE REFLECTED IN writeCsvFile() !!!
         if self.processAsFieldsCheckBox.isChecked():
-            top_mask = mask[0::2, :]
+            if y0 % 2 == 0:
+                top_index = 0
+                bot_index = 1
+            else:
+                top_index = 1
+                bot_index = 0
+
+            top_mask = mask[top_index::2, :]
             top_mask_pixel_count = np.sum(top_mask)
-            top_thumbnail = thumbnail[0::2, :]
+            top_thumbnail = thumbnail[top_index::2, :]
             top_appsum = np.sum(top_mask * top_thumbnail)
             top_signal = top_appsum - int(round(top_mask_pixel_count * mean_top))
             if default_mask_used:
                 top_mask_pixel_count = -top_mask_pixel_count
 
-            bottom_mask = mask[1::2, :]
+            bottom_mask = mask[bot_index::2, :]
             bottom_mask_pixel_count = np.sum(bottom_mask)
-            bottom_thumbnail = thumbnail[1::2, :]
+            bottom_thumbnail = thumbnail[bot_index::2, :]
             bottom_appsum = np.sum(bottom_mask * bottom_thumbnail)
             bottom_signal = bottom_appsum - int(round(bottom_mask_pixel_count * mean_bot))
             if default_mask_used:
                 bottom_mask_pixel_count = -bottom_mask_pixel_count
 
             if aperture.color == 'white':
                 top_signal = top_appsum
```

### Comparing `pymovie-3.7.3/src/pymovie/ocr.py` & `pymovie-3.7.5/src/pymovie/ocr.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/ocrCharacterBox.py` & `pymovie-3.7.5/src/pymovie/ocrCharacterBox.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/ocrProfileNameDialog.py` & `pymovie-3.7.5/src/pymovie/ocrProfileNameDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/play-Temp.py` & `pymovie-3.7.5/src/pymovie/play-Temp.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/play-introspection.py` & `pymovie-3.7.5/src/pymovie/play-introspection.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/selectHotPixelProfile.py` & `pymovie-3.7.5/src/pymovie/selectHotPixelProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/selectProfile.py` & `pymovie-3.7.5/src/pymovie/selectProfile.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/stacker.py` & `pymovie-3.7.5/src/pymovie/stacker.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/starPositionDialog.py` & `pymovie-3.7.5/src/pymovie/starPositionDialog.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie/wcs_helper_functions.py` & `pymovie-3.7.5/src/pymovie/wcs_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pymovie-3.7.3/src/pymovie.egg-info/PKG-INFO` & `pymovie-3.7.5/src/pymovie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymovie
-Version: 3.7.3
+Version: 3.7.5
 Summary: pymovie is a lightcurve extractor for astronomical videos
 Home-page: https://github.com/bob-anderson-ok/pymovie
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pymovie-3.7.3/src/pymovie.egg-info/SOURCES.txt` & `pymovie-3.7.5/src/pymovie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

