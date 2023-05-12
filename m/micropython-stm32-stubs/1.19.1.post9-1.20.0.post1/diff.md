# Comparing `tmp/micropython_stm32_stubs-1.19.1.post9.tar.gz` & `tmp/micropython_stm32_stubs-1.20.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_stm32_stubs-1.19.1.post9.tar", max compression
+gzip compressed data, was "micropython_stm32_stubs-1.20.0.post1.tar", max compression
```

## Comparing `micropython_stm32_stubs-1.19.1.post9.tar` & `micropython_stm32_stubs-1.20.0.post1.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0     1070 2023-01-16 08:09:06.719668 micropython_stm32_stubs-1.19.1.post9/LICENSE.md
--rw-r--r--   0        0        0     2030 2023-01-16 08:09:06.719668 micropython_stm32_stubs-1.19.1.post9/README.md
--rw-r--r--   0        0        0      269 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/_onewire.pyi
--rw-r--r--   0        0        0      353 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/_uasyncio.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/array.pyi
--rw-r--r--   0        0        0     1365 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/binascii.pyi
--rw-r--r--   0        0        0     1385 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/cmath.pyi
--rw-r--r--   0        0        0      329 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/dht.pyi
--rw-r--r--   0        0        0      676 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/errno.pyi
--rw-r--r--   0        0        0     4787 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/framebuf.pyi
--rw-r--r--   0        0        0     1935 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/gc.pyi
--rw-r--r--   0        0        0     1335 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/hashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/heapq.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/json.pyi
--rw-r--r--   0        0        0     3553 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/lcd160cr.pyi
--rw-r--r--   0        0        0      187 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/lcd160cr_test.pyi
--rw-r--r--   0        0        0    46828 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/machine.pyi
--rw-r--r--   0        0        0     4400 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/math.pyi
--rw-r--r--   0        0        0     7055 2023-01-16 08:08:33.968085 micropython_stm32_stubs-1.19.1.post9/micropython.pyi
--rw-r--r--   0        0        0     1235 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/network.pyi
--rw-r--r--   0        0        0      596 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/onewire.pyi
--rw-r--r--   0        0        0     9144 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/os.pyi
--rw-r--r--   0        0        0      157 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/platform.pyi
--rw-r--r--   0        0        0    84144 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/pyb.pyi
--rw-r--r--   0        0        0     3118 2023-01-16 08:09:07.219661 micropython_stm32_stubs-1.19.1.post9/pyproject.toml
--rw-r--r--   0        0        0     2553 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/random.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/select.pyi
--rw-r--r--   0        0        0     9304 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/socket.pyi
--rw-r--r--   0        0        0     3900 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/stm.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/struct.pyi
--rw-r--r--   0        0        0      838 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/sys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/time.pyi
--rw-r--r--   0        0        0     1017 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uarray.pyi
--rw-r--r--   0        0        0      125 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/__init__.pyi
--rw-r--r--   0        0        0     1478 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/core.pyi
--rw-r--r--   0        0        0      577 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/event.pyi
--rw-r--r--   0        0        0      377 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/funcs.pyi
--rw-r--r--   0        0        0      407 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/lock.pyi
--rw-r--r--   0        0        0     1394 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/stream.pyi
--rw-r--r--   0        0        0      760 2023-01-16 08:08:34.280081 micropython_stm32_stubs-1.19.1.post9/uasyncio/task.pyi
--rw-r--r--   0        0        0     1365 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/ubinascii.pyi
--rw-r--r--   0        0        0     3526 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/ucollections.pyi
--rw-r--r--   0        0        0     2277 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uctypes.pyi
--rw-r--r--   0        0        0      676 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uerrno.pyi
--rw-r--r--   0        0        0     1335 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uhashlib.pyi
--rw-r--r--   0        0        0      897 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uheapq.pyi
--rw-r--r--   0        0        0     3914 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uio.pyi
--rw-r--r--   0        0        0     1339 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/ujson.pyi
--rw-r--r--   0        0        0    46828 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/umachine.pyi
--rw-r--r--   0        0        0     9144 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uos.pyi
--rw-r--r--   0        0        0      157 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uplatform.pyi
--rw-r--r--   0        0        0     2553 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/urandom.pyi
--rw-r--r--   0        0        0      181 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/ure.pyi
--rw-r--r--   0        0        0     3760 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uselect.pyi
--rw-r--r--   0        0        0     9304 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/usocket.pyi
--rw-r--r--   0        0        0     1521 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/ustruct.pyi
--rw-r--r--   0        0        0      838 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/usys.pyi
--rw-r--r--   0        0        0    12180 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/utime.pyi
--rw-r--r--   0        0        0      238 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/utimeq.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/uzlib.pyi
--rw-r--r--   0        0        0     1503 2023-01-16 08:08:34.292081 micropython_stm32_stubs-1.19.1.post9/zlib.pyi
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.19.1.post9/setup.py
--rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.19.1.post9/PKG-INFO
+-rw-r--r--   0        0        0      277 2023-05-12 07:15:43.241810 micropython_stm32_stubs-1.20.0.post1/_onewire.pyi
+-rw-r--r--   0        0        0      848 2023-05-12 07:15:46.137399 micropython_stm32_stubs-1.20.0.post1/_thread.pyi
+-rw-r--r--   0        0        0      364 2023-05-12 07:15:43.243316 micropython_stm32_stubs-1.20.0.post1/_uasyncio.pyi
+-rw-r--r--   0        0        0     1003 2023-05-12 07:15:58.913810 micropython_stm32_stubs-1.20.0.post1/array.pyi
+-rw-r--r--   0        0        0     1408 2023-05-12 07:15:58.792096 micropython_stm32_stubs-1.20.0.post1/binascii.pyi
+-rw-r--r--   0        0        0     1454 2023-05-12 07:15:58.813895 micropython_stm32_stubs-1.20.0.post1/cmath.pyi
+-rw-r--r--   0        0        0     3640 2023-05-12 07:15:58.827952 micropython_stm32_stubs-1.20.0.post1/collections.pyi
+-rw-r--r--   0        0        0      344 2023-05-05 19:51:02.978948 micropython_stm32_stubs-1.20.0.post1/dht.pyi
+-rw-r--r--   0        0        0      709 2023-05-12 07:15:46.940344 micropython_stm32_stubs-1.20.0.post1/errno.pyi
+-rw-r--r--   0        0        0     6349 2023-05-12 07:15:58.874726 micropython_stm32_stubs-1.20.0.post1/framebuf.pyi
+-rw-r--r--   0        0        0     1993 2023-05-12 07:15:58.863196 micropython_stm32_stubs-1.20.0.post1/gc.pyi
+-rw-r--r--   0        0        0     1368 2023-05-12 07:15:58.849147 micropython_stm32_stubs-1.20.0.post1/hashlib.pyi
+-rw-r--r--   0        0        0      930 2023-05-12 07:15:58.866213 micropython_stm32_stubs-1.20.0.post1/heapq.pyi
+-rw-r--r--   0        0        0     2471 2023-05-12 07:15:58.925863 micropython_stm32_stubs-1.20.0.post1/io.pyi
+-rw-r--r--   0        0        0     1384 2023-05-12 07:15:58.879733 micropython_stm32_stubs-1.20.0.post1/json.pyi
+-rw-r--r--   0        0        0    15648 2023-05-12 07:15:59.035817 micropython_stm32_stubs-1.20.0.post1/lcd160cr.pyi
+-rw-r--r--   0        0        0     1092 2023-05-12 09:24:03.793899 micropython_stm32_stubs-1.20.0.post1/LICENSE.md
+-rw-r--r--   0        0        0    51100 2023-05-12 07:16:01.476404 micropython_stm32_stubs-1.20.0.post1/machine.pyi
+-rw-r--r--   0        0        0     4654 2023-05-12 07:15:59.023187 micropython_stm32_stubs-1.20.0.post1/math.pyi
+-rw-r--r--   0        0        0     7213 2023-04-05 11:07:45.360315 micropython_stm32_stubs-1.20.0.post1/micropython.pyi
+-rw-r--r--   0        0        0     1359 2023-05-12 07:15:50.462206 micropython_stm32_stubs-1.20.0.post1/network.pyi
+-rw-r--r--   0        0        0      617 2023-05-05 19:51:02.981472 micropython_stm32_stubs-1.20.0.post1/onewire.pyi
+-rw-r--r--   0        0        0     9396 2023-05-12 07:15:59.054853 micropython_stm32_stubs-1.20.0.post1/os.pyi
+-rw-r--r--   0        0        0      162 2023-05-12 07:15:43.274041 micropython_stm32_stubs-1.20.0.post1/platform.pyi
+-rw-r--r--   0        0        0    88587 2023-05-12 07:16:03.843741 micropython_stm32_stubs-1.20.0.post1/pyb.pyi
+-rw-r--r--   0        0        0     3177 2023-05-12 09:24:04.932010 micropython_stm32_stubs-1.20.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2638 2023-05-12 07:15:59.069379 micropython_stm32_stubs-1.20.0.post1/random.pyi
+-rw-r--r--   0        0        0     2011 2023-05-12 09:24:03.793899 micropython_stm32_stubs-1.20.0.post1/README.md
+-rw-r--r--   0        0        0     3853 2023-05-12 07:15:53.098617 micropython_stm32_stubs-1.20.0.post1/select.pyi
+-rw-r--r--   0        0        0     9529 2023-05-12 07:15:59.160567 micropython_stm32_stubs-1.20.0.post1/socket.pyi
+-rw-r--r--   0        0        0     4169 2023-05-12 07:15:53.724419 micropython_stm32_stubs-1.20.0.post1/stm.pyi
+-rw-r--r--   0        0        0     4241 2023-05-12 07:15:59.172103 micropython_stm32_stubs-1.20.0.post1/struct.pyi
+-rw-r--r--   0        0        0      875 2023-05-12 07:15:59.189143 micropython_stm32_stubs-1.20.0.post1/sys.pyi
+-rw-r--r--   0        0        0    12515 2023-05-12 07:15:59.232246 micropython_stm32_stubs-1.20.0.post1/time.pyi
+-rw-r--r--   0        0        0     1003 2023-05-12 07:15:59.199664 micropython_stm32_stubs-1.20.0.post1/uarray.pyi
+-rw-r--r--   0        0        0      132 2023-05-05 19:51:02.935761 micropython_stm32_stubs-1.20.0.post1/uasyncio/__init__.pyi
+-rw-r--r--   0        0        0     1530 2023-05-05 19:51:02.948379 micropython_stm32_stubs-1.20.0.post1/uasyncio/core.pyi
+-rw-r--r--   0        0        0      625 2023-05-05 19:51:02.952597 micropython_stm32_stubs-1.20.0.post1/uasyncio/event.pyi
+-rw-r--r--   0        0        0      390 2023-05-05 19:51:02.956666 micropython_stm32_stubs-1.20.0.post1/uasyncio/funcs.pyi
+-rw-r--r--   0        0        0      414 2023-05-05 19:51:02.964713 micropython_stm32_stubs-1.20.0.post1/uasyncio/lock.pyi
+-rw-r--r--   0        0        0     1410 2023-05-05 19:52:08.156723 micropython_stm32_stubs-1.20.0.post1/uasyncio/stream.pyi
+-rw-r--r--   0        0        0      789 2023-05-05 19:51:02.973021 micropython_stm32_stubs-1.20.0.post1/uasyncio/task.pyi
+-rw-r--r--   0        0        0     1408 2023-05-12 07:15:59.269519 micropython_stm32_stubs-1.20.0.post1/ubinascii.pyi
+-rw-r--r--   0        0        0     3640 2023-05-12 07:15:59.306737 micropython_stm32_stubs-1.20.0.post1/ucollections.pyi
+-rw-r--r--   0        0        0     2363 2023-05-12 07:15:59.314264 micropython_stm32_stubs-1.20.0.post1/uctypes.pyi
+-rw-r--r--   0        0        0      709 2023-05-12 07:15:54.774402 micropython_stm32_stubs-1.20.0.post1/uerrno.pyi
+-rw-r--r--   0        0        0     1368 2023-05-12 07:15:59.326324 micropython_stm32_stubs-1.20.0.post1/uhashlib.pyi
+-rw-r--r--   0        0        0      930 2023-05-12 07:15:59.335227 micropython_stm32_stubs-1.20.0.post1/uheapq.pyi
+-rw-r--r--   0        0        0     2471 2023-05-12 07:15:59.420836 micropython_stm32_stubs-1.20.0.post1/uio.pyi
+-rw-r--r--   0        0        0     1384 2023-05-12 07:15:59.340235 micropython_stm32_stubs-1.20.0.post1/ujson.pyi
+-rw-r--r--   0        0        0    51100 2023-05-12 07:16:05.691736 micropython_stm32_stubs-1.20.0.post1/umachine.pyi
+-rw-r--r--   0        0        0     9396 2023-05-12 07:15:59.543674 micropython_stm32_stubs-1.20.0.post1/uos.pyi
+-rw-r--r--   0        0        0      162 2023-05-12 07:15:43.303196 micropython_stm32_stubs-1.20.0.post1/uplatform.pyi
+-rw-r--r--   0        0        0     2638 2023-05-12 07:15:59.484480 micropython_stm32_stubs-1.20.0.post1/urandom.pyi
+-rw-r--r--   0        0        0      187 2023-05-12 07:15:43.305658 micropython_stm32_stubs-1.20.0.post1/ure.pyi
+-rw-r--r--   0        0        0     3853 2023-05-12 07:15:57.203703 micropython_stm32_stubs-1.20.0.post1/uselect.pyi
+-rw-r--r--   0        0        0     9529 2023-05-12 07:15:59.595730 micropython_stm32_stubs-1.20.0.post1/usocket.pyi
+-rw-r--r--   0        0        0     4241 2023-05-12 07:15:59.556205 micropython_stm32_stubs-1.20.0.post1/ustruct.pyi
+-rw-r--r--   0        0        0      875 2023-05-12 07:15:59.577684 micropython_stm32_stubs-1.20.0.post1/usys.pyi
+-rw-r--r--   0        0        0    12515 2023-05-12 07:15:59.635636 micropython_stm32_stubs-1.20.0.post1/utime.pyi
+-rw-r--r--   0        0        0      245 2023-05-12 07:15:43.313177 micropython_stm32_stubs-1.20.0.post1/utimeq.pyi
+-rw-r--r--   0        0        0     1535 2023-05-12 07:15:59.615066 micropython_stm32_stubs-1.20.0.post1/uzlib.pyi
+-rw-r--r--   0        0        0     1535 2023-05-12 07:15:59.632108 micropython_stm32_stubs-1.20.0.post1/zlib.pyi
+-rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.20.0.post1/setup.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 micropython_stm32_stubs-1.20.0.post1/PKG-INFO
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/README.md` & `micropython_stm32_stubs-1.20.0.post1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# micropython-stm32-stubs
-
-
-This is a stub-only package for MicroPython.
-It is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.
-
-The version of this package is alligned the the version of the MicroPython firmware.
- - Major, Minor and Patch levels are alligned to the same version as the firmware.  
- - The post release level is used to publish new releases of the stubs.
-
-For `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  
-for `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  
-
-To install the latest stubs:  
-`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.
-
-To install the stubs for an older version, such as MicroPython 1.17:  
-`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.
-
-
-As the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.
-To upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`
-
-If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
-
-For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
- * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
-
-Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-stm32-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/stm32/GENERIC`
-* Core Stubs from `stubs/cpython_core-pycopy`
-
-
-origin | Family | Port | Board | Version
--------|--------|------|-------|--------
-Firmware | micropython | stm32 | PYBv1.1 with STM32F405RG | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | stm32 | - | v1.19.1 
+# micropython-stm32-stubs
+
+
+This is a stub-only package for MicroPython.
+It is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.
+
+The version of this package is alligned the the version of the MicroPython firmware.
+ - Major, Minor and Patch levels are alligned to the same version as the firmware.  
+ - The post release level is used to publish new releases of the stubs.
+
+For `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  
+for `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  
+
+To install the latest stubs:  
+`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.
+
+To install the stubs for an older version, such as MicroPython 1.17:  
+`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.
+
+
+As the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.
+To upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`
+
+If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
+
+For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
+ * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
+
+Included stubs:
+* StubSource.MERGED from `stubs/micropython-v1_20_0-stm32-merged`
+* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`
+* StubSource.CORE from `stubs/micropython-core`
+
+
+origin | Family | Port | Board | Version
+-------|--------|------|-------|--------
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | stm32 | - | v1.20.0
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/array.pyi` & `micropython_stm32_stubs-1.20.0.post1/array.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.19.1/library/array.html
-
-|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
-
-Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
-``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
-floating-point support).
-"""
-from typing import Optional, Any
-
-class array:
-    """
-    Create array with elements of given type. Initial contents of the
-    array are given by *iterable*. If it is not provided, an empty
-    array is created.
-    """
-
-    def extend(self, iterable) -> Any:
-        """
-        Append new elements as contained in *iterable* to the end of
-        array, growing it.
-        """
-        ...
-    def decode(self, *args, **kwargs) -> Any: ...
-    def append(self, val) -> Any:
-        """
-        Append new element *val* to the end of array, growing it.
-        """
-        ...
-    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
+"""
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
+
+|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
+
+Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
+``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
+floating-point support).
+"""
+from typing import List, Optional, Any
+
+class array:
+    """
+    Create array with elements of given type. Initial contents of the
+    array are given by *iterable*. If it is not provided, an empty
+    array is created.
+    """
+
+    def extend(self, iterable) -> Any:
+        """
+        Append new elements as contained in *iterable* to the end of
+        array, growing it.
+        """
+        ...
+    def append(self, val) -> Any:
+        """
+        Append new element *val* to the end of array, growing it.
+        """
+        ...
+    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/binascii.pyi` & `micropython_stm32_stubs-1.20.0.post1/binascii.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
-
-|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
-
-This module implements conversions between binary data and various
-encodings of it in ASCII form (in both directions).
-"""
-from typing import Optional, Any
-
-def crc32(*args, **kwargs) -> Any: ...
-def hexlify(data, sep: Optional[Any] = None) -> bytes:
-    """
-    Convert the bytes in the *data* object to a hexadecimal representation.
-    Returns a bytes object.
-
-    If the additional argument *sep* is supplied it is used as a separator
-    between hexadecimal values.
-    """
-    ...
-
-def unhexlify(data) -> bytes:
-    """
-    Convert hexadecimal data to binary representation. Returns bytes string.
-    (i.e. inverse of hexlify)
-    """
-    ...
-
-def b2a_base64(data, *, newline=True) -> bytes:
-    """
-    Encode binary data in base64 format, as in `RFC 3548
-    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
-    followed by a newline character if newline is true, as a bytes object.
-    """
-    ...
-
-def a2b_base64(data) -> bytes:
-    """
-    Decode base64-encoded data, ignoring invalid characters in the input.
-    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
-    Returns a bytes object.
-    """
-    ...
+"""
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
+
+|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
+
+This module implements conversions between binary data and various
+encodings of it in ASCII form (in both directions).
+"""
+from typing import Optional, Any
+
+def crc32(*args, **kwargs) -> Any: ...
+def hexlify(data, sep: Optional[Any] = None) -> bytes:
+    """
+    Convert the bytes in the *data* object to a hexadecimal representation.
+    Returns a bytes object.
+
+    If the additional argument *sep* is supplied it is used as a separator
+    between hexadecimal values.
+    """
+    ...
+
+def unhexlify(data) -> bytes:
+    """
+    Convert hexadecimal data to binary representation. Returns bytes string.
+    (i.e. inverse of hexlify)
+    """
+    ...
+
+def b2a_base64(data, *, newline=True) -> bytes:
+    """
+    Encode binary data in base64 format, as in `RFC 3548
+    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
+    followed by a newline character if newline is true, as a bytes object.
+    """
+    ...
+
+def a2b_base64(data) -> bytes:
+    """
+    Decode base64-encoded data, ignoring invalid characters in the input.
+    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
+    Returns a bytes object.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/framebuf.pyi` & `micropython_stm32_stubs-1.20.0.post1/framebuf.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,140 @@
-"""
-Frame buffer manipulation. See: https://docs.micropython.org/en/v1.19.1/library/framebuf.html
-
-This module provides a general frame buffer which can be used to create
-bitmap images, which can then be sent to a display.
-"""
-from typing import Optional, Any
-
-MONO_HMSB: int
-MONO_HLSB: int
-RGB565: int
-MONO_VLSB: int
-MVLSB: int
-GS2_HMSB: int
-GS8: int
-GS4_HMSB: int
-
-def FrameBuffer1(*args, **kwargs) -> Any: ...
-
-class FrameBuffer:
-    """
-    Construct a FrameBuffer object.  The parameters are:
-
-        - *buffer* is an object with a buffer protocol which must be large
-          enough to contain every pixel defined by the width, height and
-          format of the FrameBuffer.
-        - *width* is the width of the FrameBuffer in pixels
-        - *height* is the height of the FrameBuffer in pixels
-        - *format* specifies the type of pixel used in the FrameBuffer;
-          permissible values are listed under Constants below. These set the
-          number of bits used to encode a color value and the layout of these
-          bits in *buffer*.
-          Where a color value c is passed to a method, c is a small integer
-          with an encoding that is dependent on the format of the FrameBuffer.
-        - *stride* is the number of pixels between each horizontal line
-          of pixels in the FrameBuffer. This defaults to *width* but may
-          need adjustments when implementing a FrameBuffer within another
-          larger FrameBuffer or screen. The *buffer* size must accommodate
-          an increased step size.
-
-    One must specify valid *buffer*, *width*, *height*, *format* and
-    optionally *stride*.  Invalid *buffer* size or dimensions may lead to
-    unexpected errors.
-    """
-
-    def rect(self, x, y, w, h, c) -> Any: ...
-    def pixel(self, x, y, c: Optional[Any] = None) -> Any:
-        """
-        If *c* is not given, get the color value of the specified pixel.
-        If *c* is given, set the specified pixel to the given color.
-        """
-        ...
-    def vline(self, x, y, h, c) -> Any: ...
-    def scroll(self, xstep, ystep) -> Any:
-        """
-        Shift the contents of the FrameBuffer by the given vector. This may
-        leave a footprint of the previous colors in the FrameBuffer.
-        """
-        ...
-    def text(self, s, x, y, c: Optional[Any] = None) -> None:
-        """
-        Write text to the FrameBuffer using the the coordinates as the upper-left
-        corner of the text. The color of the text can be defined by the optional
-        argument but is otherwise a default value of 1. All characters have
-        dimensions of 8x8 pixels and there is currently no way to change the font.
-
-        """
-        ...
-    def fill(self, c) -> None:
-        """
-        Fill the entire FrameBuffer with the specified color.
-        """
-        ...
-    def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
-        """
-        Draw another FrameBuffer on top of the current one at the given coordinates.
-        If *key* is specified then it should be a color integer and the
-        corresponding color will be considered transparent: all pixels with that
-        color value will not be drawn.
-
-        The *palette* argument enables blitting between FrameBuffers with differing
-        formats. Typical usage is to render a monochrome or grayscale glyph/icon to
-        a color display. The *palette* is a FrameBuffer instance whose format is
-        that of the current FrameBuffer. The *palette* height is one pixel and its
-        pixel width is the number of colors in the source FrameBuffer. The *palette*
-        for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
-        would have 2 pixels representing background and foreground colors. The
-        application assigns a color to each pixel in the *palette*. The color of the
-        current pixel will be that of that *palette* pixel whose x position is the
-        color of the corresponding source pixel.
-        """
-        ...
-    def line(self, x1, y1, x2, y2, c) -> None:
-        """
-        Draw a line from a set of coordinates using the given color and
-        a thickness of 1 pixel. The `line` method draws the line up to
-        a second set of coordinates whereas the `hline` and `vline`
-        methods draw horizontal and vertical lines respectively up to
-        a given length.
-        """
-        ...
-    def fill_rect(self, x, y, w, h, c) -> None:
-        """
-        Draw a rectangle at the given location, size and color. The `rect`
-        method draws only a 1 pixel outline whereas the `fill_rect` method
-        draws both the outline and interior.
-        """
-        ...
-    def hline(self, x, y, w, c) -> Any: ...
-    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
+"""
+Frame buffer manipulation. See: https://docs.micropython.org/en/v1.20.0/library/framebuf.html
+
+This module provides a general frame buffer which can be used to create
+bitmap images, which can then be sent to a display.
+"""
+from typing import Optional, Any
+
+MONO_HMSB: int
+MONO_HLSB: int
+RGB565: int
+MONO_VLSB: int
+MVLSB: int
+GS2_HMSB: int
+GS8: int
+GS4_HMSB: int
+
+def FrameBuffer1(*args, **kwargs) -> Any: ...
+
+class FrameBuffer:
+    """
+    Construct a FrameBuffer object.  The parameters are:
+
+        - *buffer* is an object with a buffer protocol which must be large
+          enough to contain every pixel defined by the width, height and
+          format of the FrameBuffer.
+        - *width* is the width of the FrameBuffer in pixels
+        - *height* is the height of the FrameBuffer in pixels
+        - *format* specifies the type of pixel used in the FrameBuffer;
+          permissible values are listed under Constants below. These set the
+          number of bits used to encode a color value and the layout of these
+          bits in *buffer*.
+          Where a color value c is passed to a method, c is a small integer
+          with an encoding that is dependent on the format of the FrameBuffer.
+        - *stride* is the number of pixels between each horizontal line
+          of pixels in the FrameBuffer. This defaults to *width* but may
+          need adjustments when implementing a FrameBuffer within another
+          larger FrameBuffer or screen. The *buffer* size must accommodate
+          an increased step size.
+
+    One must specify valid *buffer*, *width*, *height*, *format* and
+    optionally *stride*.  Invalid *buffer* size or dimensions may lead to
+    unexpected errors.
+    """
+
+    def poly(self, x, y, coords, c, f: Optional[Any] = None) -> Any:
+        """
+        Given a list of coordinates, draw an arbitrary (convex or concave) closed
+        polygon at the given x, y location using the given color.
+
+        The *coords* must be specified as a :mod:`array` of integers, e.g.
+        ``array('h', [x0, y0, x1, y1, ... xn, yn])``.
+
+        The optional *f* parameter can be set to ``True`` to fill the polygon.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def vline(self, x, y, h, c) -> Any: ...
+    def pixel(self, x, y, c: Optional[Any] = None) -> Any:
+        """
+        If *c* is not given, get the color value of the specified pixel.
+        If *c* is given, set the specified pixel to the given color.
+        """
+        ...
+    def text(self, s, x, y, c: Optional[Any] = None) -> None:
+        """
+        Write text to the FrameBuffer using the the coordinates as the upper-left
+        corner of the text. The color of the text can be defined by the optional
+        argument but is otherwise a default value of 1. All characters have
+        dimensions of 8x8 pixels and there is currently no way to change the font.
+
+        """
+        ...
+    def rect(self, x, y, w, h, c, f: Optional[Any] = None) -> None:
+        """
+        Draw a rectangle at the given location, size and color.
+
+        The optional *f* parameter can be set to ``True`` to fill the rectangle.
+        Otherwise just a one pixel outline is drawn.
+        """
+        ...
+    def scroll(self, xstep, ystep) -> Any:
+        """
+        Shift the contents of the FrameBuffer by the given vector. This may
+        leave a footprint of the previous colors in the FrameBuffer.
+        """
+        ...
+    def ellipse(self, x, y, xr, yr, c, f, m: Optional[Any] = None) -> None:
+        """
+        Draw an ellipse at the given location. Radii *xr* and *yr* define the
+        geometry; equal values cause a circle to be drawn. The *c* parameter
+        defines the color.
+
+        The optional *f* parameter can be set to ``True`` to fill the ellipse.
+        Otherwise just a one pixel outline is drawn.
+
+        The optional *m* parameter enables drawing to be restricted to certain
+        quadrants of the ellipse. The LS four bits determine which quadrants are
+        to be drawn, with bit 0 specifying Q1, b1 Q2, b2 Q3 and b3 Q4. Quadrants
+        are numbered counterclockwise with Q1 being top right.
+        """
+        ...
+    def line(self, x1, y1, x2, y2, c) -> None:
+        """
+        Draw a line from a set of coordinates using the given color and
+        a thickness of 1 pixel. The `line` method draws the line up to
+        a second set of coordinates whereas the `hline` and `vline`
+        methods draw horizontal and vertical lines respectively up to
+        a given length.
+        """
+        ...
+    def blit(self, fbuf, x, y, key=-1, palette=None) -> None:
+        """
+        Draw another FrameBuffer on top of the current one at the given coordinates.
+        If *key* is specified then it should be a color integer and the
+        corresponding color will be considered transparent: all pixels with that
+        color value will not be drawn. (If the *palette* is specified then the *key*
+        is compared to the value from *palette*, not to the value directly from
+        *fbuf*.)
+
+        The *palette* argument enables blitting between FrameBuffers with differing
+        formats. Typical usage is to render a monochrome or grayscale glyph/icon to
+        a color display. The *palette* is a FrameBuffer instance whose format is
+        that of the current FrameBuffer. The *palette* height is one pixel and its
+        pixel width is the number of colors in the source FrameBuffer. The *palette*
+        for an N-bit source needs 2**N pixels; the *palette* for a monochrome source
+        would have 2 pixels representing background and foreground colors. The
+        application assigns a color to each pixel in the *palette*. The color of the
+        current pixel will be that of that *palette* pixel whose x position is the
+        color of the corresponding source pixel.
+        """
+        ...
+    def hline(self, x, y, w, c) -> Any: ...
+    def fill(self, c) -> None:
+        """
+        Fill the entire FrameBuffer with the specified color.
+        """
+        ...
+    def fill_rect(self, *args, **kwargs) -> Any: ...
+    def __init__(self, buffer, width, height, format, stride=-1, /) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/gc.pyi` & `micropython_stm32_stubs-1.20.0.post1/gc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""
-control the garbage collector. See: https://docs.micropython.org/en/v1.19.1/library/gc.html
-
-|see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
-"""
-from typing import Optional, Any
-
-def mem_alloc() -> int:
-    """
-    Return the number of bytes of heap RAM that are allocated.
-    """
-    ...
-
-def isenabled(*args, **kwargs) -> Any: ...
-def mem_free() -> int:
-    """
-    Return the number of bytes of available heap RAM, or -1 if this amount
-    is not known.
-    """
-    ...
-
-def threshold(amount: Optional[Any] = None) -> Any:
-    """
-    Set or query the additional GC allocation threshold. Normally, a collection
-    is triggered only when a new allocation cannot be satisfied, i.e. on an
-    out-of-memory (OOM) condition. If this function is called, in addition to
-    OOM, a collection will be triggered each time after *amount* bytes have been
-    allocated (in total, since the previous time such an amount of bytes
-    have been allocated). *amount* is usually specified as less than the
-    full heap size, with the intention to trigger a collection earlier than when the
-    heap becomes exhausted, and in the hope that an early collection will prevent
-    excessive memory fragmentation. This is a heuristic measure, the effect
-    of which will vary from application to application, as well as
-    the optimal value of the *amount* parameter.
-
-    Calling the function without argument will return the current value of
-    the threshold. A value of -1 means a disabled allocation threshold.
-    """
-    ...
-
-def collect() -> None:
-    """
-    Run a garbage collection.
-    """
-    ...
-
-def enable() -> None:
-    """
-    Enable automatic garbage collection.
-    """
-    ...
-
-def disable() -> None:
-    """
-    Disable automatic garbage collection.  Heap memory can still be allocated,
-    and garbage collection can still be initiated manually using :meth:`gc.collect`.
-    """
-    ...
+"""
+control the garbage collector. See: https://docs.micropython.org/en/v1.20.0/library/gc.html
+
+|see_cpython_module| :mod:`python:gc` https://docs.python.org/3/library/gc.html .
+"""
+from typing import Optional, Any
+
+def mem_alloc() -> int:
+    """
+    Return the number of bytes of heap RAM that are allocated.
+    """
+    ...
+
+def isenabled(*args, **kwargs) -> Any: ...
+def mem_free() -> int:
+    """
+    Return the number of bytes of available heap RAM, or -1 if this amount
+    is not known.
+    """
+    ...
+
+def threshold(amount: Optional[Any] = None) -> Any:
+    """
+    Set or query the additional GC allocation threshold. Normally, a collection
+    is triggered only when a new allocation cannot be satisfied, i.e. on an
+    out-of-memory (OOM) condition. If this function is called, in addition to
+    OOM, a collection will be triggered each time after *amount* bytes have been
+    allocated (in total, since the previous time such an amount of bytes
+    have been allocated). *amount* is usually specified as less than the
+    full heap size, with the intention to trigger a collection earlier than when the
+    heap becomes exhausted, and in the hope that an early collection will prevent
+    excessive memory fragmentation. This is a heuristic measure, the effect
+    of which will vary from application to application, as well as
+    the optimal value of the *amount* parameter.
+
+    Calling the function without argument will return the current value of
+    the threshold. A value of -1 means a disabled allocation threshold.
+    """
+    ...
+
+def collect() -> None:
+    """
+    Run a garbage collection.
+    """
+    ...
+
+def enable() -> None:
+    """
+    Enable automatic garbage collection.
+    """
+    ...
+
+def disable() -> None:
+    """
+    Disable automatic garbage collection.  Heap memory can still be allocated,
+    and garbage collection can still be initiated manually using :meth:`gc.collect`.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/hashlib.pyi` & `micropython_stm32_stubs-1.20.0.post1/hashlib.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
-
-|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
-
-This module implements binary data hashing algorithms. The exact inventory
-of available algorithms depends on a board. Among the algorithms which may
-be implemented:
-
-* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
-  It is suitable for cryptographically-secure purposes. Included in the
-  MicroPython core and any board is recommended to provide this, unless
-  it has particular code size constraints.
-
-* SHA1 - A previous generation algorithm. Not recommended for new usages,
-  but SHA1 is a part of number of Internet standards and existing
-  applications, so boards targeting network connectivity and
-  interoperability will try to provide this.
-
-* MD5 - A legacy algorithm, not considered cryptographically secure. Only
-  selected boards, targeting interoperability with legacy applications,
-  will offer this.
-"""
-from typing import Optional, Any
-
-class sha256:
-    """
-    Create an SHA256 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
+"""
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
+
+|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
+
+This module implements binary data hashing algorithms. The exact inventory
+of available algorithms depends on a board. Among the algorithms which may
+be implemented:
+
+* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
+  It is suitable for cryptographically-secure purposes. Included in the
+  MicroPython core and any board is recommended to provide this, unless
+  it has particular code size constraints.
+
+* SHA1 - A previous generation algorithm. Not recommended for new usages,
+  but SHA1 is a part of number of Internet standards and existing
+  applications, so boards targeting network connectivity and
+  interoperability will try to provide this.
+
+* MD5 - A legacy algorithm, not considered cryptographically secure. Only
+  selected boards, targeting interoperability with legacy applications,
+  will offer this.
+"""
+from typing import Optional, Any
+
+class sha256:
+    """
+    Create an SHA256 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/heapq.pyi` & `micropython_stm32_stubs-1.20.0.post1/heapq.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
-
-|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
-
-This module implements the
-`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
-
-A heap queue is essentially a list that has its elements stored in such a way
-that the first item of the list is always the smallest.
-"""
-from typing import Any
-
-def heappop(heap) -> Any:
-    """
-    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
-    ``heap`` is empty.
-
-    The returned item will be the smallest item in the ``heap``.
-    """
-    ...
-
-def heappush(heap, item) -> Any:
-    """
-    Push the ``item`` onto the ``heap``.
-    """
-    ...
-
-def heapify(x) -> Any:
-    """
-    Convert the list ``x`` into a heap.  This is an in-place operation.
-    """
-    ...
+"""
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
+
+|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
+
+This module implements the
+`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
+
+A heap queue is essentially a list that has its elements stored in such a way
+that the first item of the list is always the smallest.
+"""
+from typing import Any
+
+def heappop(heap) -> Any:
+    """
+    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
+    ``heap`` is empty.
+
+    The returned item will be the smallest item in the ``heap``.
+    """
+    ...
+
+def heappush(heap, item) -> Any:
+    """
+    Push the ``item`` onto the ``heap``.
+    """
+    ...
+
+def heapify(x) -> Any:
+    """
+    Convert the list ``x`` into a heap.  This is an in-place operation.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/machine.pyi` & `micropython_stm32_stubs-1.20.0.post1/machine.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,1204 +1,1273 @@
-"""
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
-
-The ``machine`` module contains specific functions related to the hardware
-on a particular board. Most functions in this module allow to achieve direct
-and unrestricted access to and control of hardware blocks on a system
-(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
-malfunction, lockups, crashes of your board, and in extreme cases, hardware
-damage.
-"""
-from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
-
-HARD_RESET: int
-PWRON_RESET: int
-SOFT_RESET: int
-DEEPSLEEP_RESET: int
-WDT_RESET: int
-
-def idle() -> Any:
-    """
-    Gates the clock to the CPU, useful to reduce power consumption at any time during
-    short or long periods. Peripherals continue working and execution resumes as soon
-    as any interrupt is triggered (on many ports this includes system timer
-    interrupt occurring at regular intervals on the order of millisecond).
-    """
-    ...
-
-def freq(hz: Optional[Any] = None) -> Any:
-    """
-    Returns the CPU frequency in hertz.
-
-    On some ports this can also be used to set the CPU frequency by passing in *hz*.
-    """
-    ...
-
-def info(*args, **kwargs) -> Any: ...
-def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def enable_irq(state) -> Any:
-    """
-    Re-enable interrupt requests.
-    The *state* parameter should be the value that was returned from the most
-    recent call to the `disable_irq()` function.
-    """
-    ...
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-def unique_id() -> bytes:
-    """
-    Returns a byte string with a unique identifier of a board/SoC. It will vary
-    from a board/SoC instance to another, if underlying hardware allows. Length
-    varies by hardware (so use substring of a full value if you expect a short
-    ID). In some MicroPython ports, ID corresponds to the network MAC address.
-    """
-    ...
-
-def soft_reset() -> NoReturn:
-    """
-    Performs a soft reset of the interpreter, deleting all Python objects and
-    resetting the Python heap.  It tries to retain the method by which the user
-    is connected to the MicroPython REPL (eg serial, USB, Wifi).
-    """
-    ...
-
-def sleep() -> Any:
-    """
-    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
-    """
-    ...
-
-def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
-    """
-    Time a pulse on the given *pin*, and return the duration of the pulse in
-    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
-    or 1 to time a high pulse.
-
-    If the current input value of the pin is different to *pulse_level*,
-    the function first (*) waits until the pin input becomes equal to *pulse_level*,
-    then (**) times the duration that the pin is equal to *pulse_level*.
-    If the pin is already equal to *pulse_level* then timing starts straight away.
-
-    The function will return -2 if there was timeout waiting for condition marked
-    (*) above, and -1 if there was timeout during the main measurement, marked (**)
-    above. The timeout is the same for both cases and given by *timeout_us* (which
-    is in microseconds).
-    """
-    ...
-
-def lightsleep(time_ms: Optional[Any] = None) -> Any:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def reset() -> NoReturn:
-    """
-    Resets the device in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-def rng() -> int:
-    """
-    Return a 24-bit software generated random number.
-
-    Availability: WiPy.
-    """
-    ...
-
-def reset_cause() -> int:
-    """
-    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
-    """
-    ...
-
-def bootloader(value: Optional[Any] = None) -> None:
-    """
-    Reset the device and enter its bootloader.  This is typically used to put the
-    device into a state where it can be programmed with new firmware.
-
-    Some ports support passing in an optional *value* argument which can control
-    which bootloader to enter, what to pass to it, or other things.
-    """
-    ...
-
-def bitstream(pin, encoding, timing, data, /) -> Any:
-    """
-    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
-    specifies how the bits are encoded, and *timing* is an encoding-specific timing
-    specification.
-
-    The supported encodings are:
-
-      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
-        1 bits as timed pulses, starting with the most significant bit.
-        The *timing* must be a four-tuple of nanoseconds in the format
-        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
-        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
-        at 800kHz.
-
-    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
-    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
-    will be closer to +/-30ns.
-
-    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
-       module for a higher-level API.
-    """
-    ...
-
-class Pin:
-    """
-    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
-    additional arguments are given in the constructor then they are used to initialise
-    the pin.  Any settings that are not specified will remain in their previous state.
-
-    The arguments are:
-
-      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
-        types are: int (an internal Pin identifier), str (a Pin name), and tuple
-        (pair of [port, pin]).
-
-      - ``mode`` specifies the pin mode, which can be one of:
-
-        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
-          is in high-impedance state.
-
-        - ``Pin.OUT`` - Pin is configured for (normal) output.
-
-        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
-          output works in the following way: if the output value is set to 0 the pin
-          is active at a low level; if the output value is 1 the pin is in a high-impedance
-          state.  Not all ports implement this mode, or some might only on certain pins.
-
-        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
-          port specific.  For a pin configured in such a way any other Pin methods
-          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
-          or a hardware-specific, result).  Not all ports implement this mode.
-
-        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
-          open-drain.  Not all ports implement this mode.
-
-        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
-
-      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
-        one of:
-
-        - ``None`` - No pull up or down resistor.
-        - ``Pin.PULL_UP`` - Pull up resistor enabled.
-        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
-
-      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
-        output pin value if given, otherwise the state of the pin peripheral remains
-        unchanged.
-
-      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
-        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
-        capabilities are port dependent.  Not all ports implement this argument.
-
-      - ``alt`` specifies an alternate function for the pin and the values it can take are
-        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
-        modes.  It may be used when a pin supports more than one alternate function.  If only
-        one pin alternate function is supported the this argument is not required.  Not all
-        ports implement this argument.
-
-    As specified above, the Pin class allows to set an alternate function for a particular
-    pin, but it does not specify any further operations on such a pin.  Pins configured in
-    alternate-function mode are usually not used as GPIO but are instead driven by other
-    hardware peripherals.  The only operation supported on such a pin is re-initialising,
-    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
-    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
-    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
-    """
-
-    AF_OD: int
-    AF9_TIM14: int
-    ALT_OPEN_DRAIN: int
-    AF_PP: int
-    ALT: int
-    AF9_CAN1: int
-    AF8_USART6: int
-    AF9_TIM13: int
-    AF9_CAN2: int
-    AF9_TIM12: int
-    PULL_UP: int
-    OUT_PP: int
-    OUT_OD: int
-    ANALOG: int
-    PULL_DOWN: int
-    PULL_NONE: int
-    IRQ_FALLING: int
-    IN: int
-    OUT: int
-    IRQ_RISING: int
-    OPEN_DRAIN: int
-    AF2_TIM5: int
-    AF3_TIM10: int
-    AF3_TIM11: int
-    AF3_TIM8: int
-    AF3_TIM9: int
-    AF2_TIM4: int
-    AF1_TIM1: int
-    AF1_TIM2: int
-    AF2_TIM3: int
-    AF8_UART4: int
-    AF6_I2S2: int
-    AF7_USART1: int
-    AF7_USART2: int
-    AF7_USART3: int
-    AF4_I2C1: int
-    AF5_SPI2: int
-    AF4_I2C2: int
-    AF5_I2S2: int
-    AF5_SPI1: int
-    def mode(self, mode: Optional[Any] = None) -> Any:
-        """
-        Get or set the pin mode.
-        See the constructor documentation for details of the ``mode`` argument.
-
-        Availability: cc3200, stm32 ports.
-        """
-        ...
-    def name(self, *args, **kwargs) -> Any: ...
-    def pull(self, pull: Optional[Any] = None) -> Any:
-        """
-        Get or set the pin pull state.
-        See the constructor documentation for details of the ``pull`` argument.
-
-        Availability: cc3200, stm32 ports.
-        """
-        ...
-    def low(self) -> None:
-        """
-        Set pin to "0" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
-        """
-           Configure an interrupt handler to be called when the trigger source of the
-           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
-           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
-           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
-           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
-           state '0' and the external pin value for state '1'.
-
-           The arguments are:
-
-             - ``handler`` is an optional function to be called when the interrupt
-               triggers. The handler must take exactly one argument which is the
-               ``Pin`` instance.
-
-             - ``trigger`` configures the event which can generate an interrupt.
-               Possible values are:
-
-               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
-               - ``Pin.IRQ_RISING`` interrupt on rising edge.
-               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
-               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
-
-               These values can be OR'ed together to trigger on multiple events.
-
-             - ``priority`` sets the priority level of the interrupt.  The values it
-               can take are port-specific, but higher values always represent higher
-               priorities.
-
-             - ``wake`` selects the power mode in which this interrupt can wake up the
-               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
-               These values can also be OR'ed together to make a pin generate interrupts in
-               more than one power mode.
-
-             - ``hard`` if true a hardware interrupt is used. This reduces the delay
-               between the pin change and the handler being called. Hard interrupt
-               handlers may not allocate memory; see :ref:`isr_rules`.
-               Not all ports support this argument.
-
-           This method returns a callback object.
-
-        The following methods are not part of the core Pin API and only implemented on certain ports.
-        """
-        ...
-    def pin(self, *args, **kwargs) -> Any: ...
-    def port(self, *args, **kwargs) -> Any: ...
-    def names(self, *args, **kwargs) -> Any: ...
-    def on(self) -> None:
-        """
-        Set pin to "1" output level.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Set pin to "0" output level.
-        """
-        ...
-    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        """
-        Re-initialise the pin using the given parameters.  Only those arguments that
-        are specified will be set.  The rest of the pin peripheral state will remain
-        unchanged.  See the constructor documentation for details of the arguments.
-
-        Returns ``None``.
-        """
-        ...
-    def af_list(self, *args, **kwargs) -> Any: ...
-    def af(self, *args, **kwargs) -> Any: ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the pin, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the digital logic level of
-        the pin, returning 0 or 1 corresponding to low and high voltage signals
-        respectively.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The method returns the actual input value currently present
-            on the pin.
-          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
-          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
-            return value of the method is undefined.  Otherwise, if the pin is in
-            state '1', the method returns the actual input value currently present
-            on the pin.
-
-        If the argument is supplied then this method sets the digital logic level of
-        the pin.  The argument ``x`` can be anything that converts to a boolean.
-        If it converts to ``True``, the pin is set to state '1', otherwise it is set
-        to state '0'.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
-            pin state does not change, it remains in the high-impedance state.  The
-            stored value will become active on the pin as soon as it is changed to
-            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
-          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
-          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
-            state.  Otherwise the pin is set to high-impedance state.
-
-        When setting the value this method returns ``None``.
-        """
-        ...
-    def high(self) -> None:
-        """
-        Set pin to "1" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def gpio(self, *args, **kwargs) -> Any: ...
-    @classmethod
-    def dict(cls, *args, **kwargs) -> Any: ...
-    @classmethod
-    def debug(cls, *args, **kwargs) -> Any: ...
-
-    class cpu:
-        B9: Any
-        B8: Any
-        B7: Any
-        C0: Any
-        C1: Any
-        C10: Any
-        B3: Any
-        B2: Any
-        B6: Any
-        B4: Any
-        B5: Any
-        B15: Any
-        C7: Any
-        C6: Any
-        C5: Any
-        C8: Any
-        C9: Any
-        C11: Any
-        C13: Any
-        C12: Any
-        C4: Any
-        C2: Any
-        C3: Any
-        D2: Any
-        A15: Any
-        A14: Any
-        A13: Any
-        A2: Any
-        A3: Any
-        A4: Any
-        A1: Any
-        A0: Any
-        A12: Any
-        A10: Any
-        A11: Any
-        B14: Any
-        B11: Any
-        B10: Any
-        B1: Any
-        B12: Any
-        B13: Any
-        A5: Any
-        A7: Any
-        A6: Any
-        B0: Any
-        A8: Any
-        A9: Any
-        def __init__(self, *argv, **kwargs) -> None: ...
-
-    @classmethod
-    def mapper(cls, *args, **kwargs) -> Any: ...
-
-    class board:
-        X5: Any
-        X18: Any
-        X4: Any
-        X8: Any
-        X6: Any
-        X7: Any
-        X2: Any
-        X3: Any
-        X19: Any
-        X22: Any
-        X20: Any
-        X21: Any
-        Y5: Any
-        X9: Any
-        Y4: Any
-        Y8: Any
-        Y6: Any
-        Y7: Any
-        Y10: Any
-        Y3: Any
-        Y1: Any
-        Y2: Any
-        Y11: Any
-        Y12: Any
-        Y9: Any
-        SD_CK: Any
-        X17: Any
-        SD: Any
-        SD_D1: Any
-        SD_CMD: Any
-        SD_D0: Any
-        LED_GREEN: Any
-        MMA_INT: Any
-        LED_BLUE: Any
-        MMA_AVDD: Any
-        LED_RED: Any
-        LED_YELLOW: Any
-        X1: Any
-        SD_D2: Any
-        USB_VBUS: Any
-        X12: Any
-        X10: Any
-        X11: Any
-        SD_SW: Any
-        USB_ID: Any
-        SD_D3: Any
-        USB_DP: Any
-        SW: Any
-        USB_DM: Any
-        def __init__(self, *argv, **kwargs) -> None: ...
-
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
-
-class I2S:
-    """
-    Construct an I2S object of the given id:
-
-    - ``id`` identifies a particular I2S bus; it is board and port specific
-
-    Keyword-only parameters that are supported on all ports:
-
-      - ``sck`` is a pin object for the serial clock line
-      - ``ws`` is a pin object for the word select line
-      - ``sd`` is a pin object for the serial data line
-      - ``mck`` is a pin object for the master clock line;
-        master clock frequency is sampling rate * 256
-      - ``mode`` specifies receive or transmit
-      - ``bits`` specifies sample size (bits), 16 or 32
-      - ``format`` specifies channel format, STEREO or MONO
-      - ``rate`` specifies audio sampling rate (Hz);
-        this is the frequency of the ``ws`` signal
-      - ``ibuf`` specifies internal buffer length (bytes)
-
-    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
-    sample data is transfered between the internal buffer and the I2S peripheral unit.
-    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
-    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
-    """
-
-    RX: int
-    MONO: int
-    STEREO: int
-    TX: int
-    @staticmethod
-    def shift(*, buf, bits, shift) -> Any:
-        """
-        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
-        Positive for left shift, negative for right shift.
-        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
-        """
-        ...
-    def init(self, sck, *args, **kwargs) -> Any:
-        """
-        see Constructor for argument descriptions
-        """
-        ...
-    def irq(self, handler) -> Any:
-        """
-        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
-        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
-        ``handler`` is called in the context of the MicroPython scheduler.
-        """
-        ...
-    def readinto(self, buf) -> int:
-        """
-        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the left channel sample data is used.
-        Returns number of bytes read
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        Deinitialize the I2S bus
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the sample data is written to both the right and left channels.
-        Returns number of bytes written
-        """
-        ...
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus, *id*. Values of *id* depend
-    on a particular port and its hardware. Values 0, 1, etc. are commonly used
-    to select hardware SPI block #0, #1, etc.
-
-    With no additional parameters, the SPI object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def init(
-        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
-    ) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``baudrate`` is the SCK clock rate.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
-            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
-            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
-            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
-            (``id`` = -1).
-          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
-            specify them as a tuple of ``pins`` parameter.
-
-        In the case of hardware SPI the actual clock frequency may be lower than the
-        requested baudrate. This is dependant on the platform hardware. The actual
-        rate may be determined by printing the SPI object.
-        """
-        ...
-    def write_readinto(self, write_buf, read_buf) -> int:
-        """
-        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
-        buffers can be the same or different, but both buffers must have the
-        same length.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def read(self, nbytes, write=0x00) -> bytes:
-        """
-        Read a number of bytes specified by ``nbytes`` while continuously writing
-        the single byte given by ``write``.
-        Returns a ``bytes`` object with the data that was read.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes contained in ``buf``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def readinto(self, buf, write=0x00) -> int:
-        """
-        Read into the buffer specified by ``buf`` while continuously writing the
-        single byte given by ``write``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes read.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-mem8: Any
-
-class RTC:
-    """
-    Create an RTC object. See init for parameters of initialization.
-    """
-
-    def info(self, *args, **kwargs) -> Any: ...
-    def init(self, datetime) -> None:
-        """
-        Initialise the RTC. Datetime is a tuple of the form:
-
-           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
-        """
-        ...
-    def wakeup(self, *args, **kwargs) -> Any: ...
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time.
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        The meaning of the ``subseconds`` field is hardware dependent.
-        """
-        ...
-    def calibration(self, *args, **kwargs) -> Any: ...
-    def __init__(self, id=0, *args, **kwargs) -> None: ...
-
-class I2C:
-    """
-    Construct and return a new I2C object using the following parameters:
-
-       - *id* identifies a particular I2C peripheral.  Allowed values for
-         depend on the particular port/board
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-
-    Note that some ports/boards will have default values of *scl* and *sda*
-    that can be changed in this constructor.  Others will have fixed values
-    of *scl* and *sda* that cannot be changed.
-    """
-
-    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.  The number of bytes read is the
-        length of *buf*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_into(self, addr, buf, stop=True, /) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr*.
-        The number of bytes read will be the length of *buf*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr* starting from the memory
-        address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Write *buf* to the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
-        those that respond.  A device responds if it pulls the SDA line low after
-        its address (including a write bit) is sent on the bus.
-        """
-        ...
-    def writeto(self, addr, buf, stop=True, /) -> int:
-        """
-        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
-        NACK is received following the write of a byte from *buf* then the
-        remaining bytes are not sent.  If *stop* is true then a STOP condition is
-        generated at the end of the transfer, even if a NACK is received.
-        The function returns the number of ACKs that were received.
-        """
-        ...
-    def writevto(self, addr, vector, stop=True, /) -> int:
-        """
-        Write the bytes contained in *vector* to the peripheral specified by *addr*.
-        *vector* should be a tuple or list of objects with the buffer protocol.
-        The *addr* is sent once and then the bytes from each object in *vector*
-        are written out sequentially.  The objects in *vector* may be zero bytes
-        in length in which case they don't contribute to the output.
-
-        If a NACK is received following the write of a byte from one of the
-        objects in *vector* then the remaining bytes, and any remaining objects,
-        are not sent.  If *stop* is true then a STOP condition is generated at
-        the end of the transfer, even if a NACK is received.  The function
-        returns the number of ACKs that were received.
-        """
-        ...
-    def start(self) -> None:
-        """
-        Generate a START condition on the bus (SDA transitions to low while SCL is high).
-        """
-        ...
-    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def readinto(self, buf, nack=True, /) -> Any:
-        """
-        Reads bytes from the bus and stores them into *buf*.  The number of bytes
-        read is the length of *buf*.  An ACK will be sent on the bus after
-        receiving all but the last byte.  After the last byte is received, if *nack*
-        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
-        case the peripheral assumes more bytes are going to be read in a later call).
-        """
-        ...
-    def init(self, scl, sda, *, freq=400000) -> None:
-        """
-        Initialise the I2C bus with the given arguments:
-
-           - *scl* is a pin object for the SCL line
-           - *sda* is a pin object for the SDA line
-           - *freq* is the SCL clock rate
-        """
-        ...
-    def stop(self) -> None:
-        """
-        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from *buf* to the bus.  Checks that an ACK is received
-        after each byte and stops transmitting the remaining bytes if a NACK is
-        received.  The function returns the number of ACKs that were received.
-        """
-        ...
-    def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None: ...
-
-class ADC:
-    """
-    Access the ADC associated with a source identified by *id*.  This
-    *id* may be an integer (usually specifying a channel number), a
-    :ref:`Pin <machine.Pin>` object, or other value supported by the
-    underlying machine.
-
-    If additional keyword-arguments are given then they will configure
-    various aspects of the ADC.  If not given, these settings will take
-    previous or default values.  The settings are:
-
-      - *sample_ns* is the sampling time in nanoseconds.
-
-      - *atten* specifies the input attenuation.
-    """
-
-    VREF: int
-    CORE_VREF: int
-    CORE_VBAT: int
-    CORE_TEMP: int
-    def read_u16(self) -> int:
-        """
-        Take an analog reading and return an integer in the range 0-65535.
-        The return value represents the raw reading taken by the ADC, scaled
-        such that the minimum value is 0 and the maximum value is 65535.
-        """
-        ...
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
-        """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
-        """
-        ...
-    def __init__(self, id=0, timeout=5000) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
-    virtual timer (if supported by a board).
-    ``id`` shall not be passed as a keyword argument.
-
-    See ``init`` for parameters of initialisation.
-    """
-
-    PERIODIC: int
-    ONE_SHOT: int
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
-        """
-        Initialise the timer. Example::
-
-            def mycallback(t):
-                pass
-
-            # periodic with 100ms period
-            tim.init(period=100, callback=mycallback)
-
-            # one shot firing after 1000ms
-            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
-              period of the channel expires.
-            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
-              frequency of the channel.
-
-          - ``period`` - The timer period, in milliseconds.
-
-          - ``callback`` - The callable to call upon expiration of the timer period.
-            The callback must take one argument, which is passed the Timer object.
-            The ``callback`` argument shall be specified. Otherwise an exception
-            will occurr upon timer expiration:
-            ``TypeError: 'NoneType' object isn't callable``
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def __init__(self, id=-1, *args, **kwargs) -> None: ...
-
-class SoftSPI:
-    """
-    Construct a new software SPI object.  Additional parameters must be
-    given, usually at least *sck*, *mosi* and *miso*, and these are used
-    to initialise the bus.  See `SPI.init` for a description of the parameters.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
-
-class UART:
-    """
-    Construct a UART object of the given id.
-    """
-
-    CTS: int
-    RTS: int
-    IRQ_RXIDLE: int
-    def readchar(self, *args, **kwargs) -> Any: ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
-        """
-        ...
-    def irq(self, trigger, priority=1, handler=None, wake=IDLE) -> Any:
-        """
-        Create a callback to be triggered when data is received on the UART.
-
-            - *trigger* can only be ``UART.RX_ANY``
-            - *priority* level of the interrupt. Can take values in the range 1-7.
-              Higher values represent higher priorities.
-            - *handler* an optional function to be called when new characters arrive.
-            - *wake* can only be ``machine.IDLE``.
-
-        .. note::
-
-           The handler will be called whenever any of the following two conditions are met:
-
-               - 8 new characters have been received.
-               - At least 1 new character is waiting in the Rx buffer and the Rx line has been
-                 silent for the duration of 1 complete frame.
-
-           This means that when the handler function is called there will be between 1 to 8
-           characters waiting.
-
-        Returns an irq object.
-
-        Availability: WiPy.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - *baudrate* is the clock rate.
-          - *bits* is the number of bits per character, 7, 8 or 9.
-          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
-          - *stop* is the number of stop bits, 1 or 2.
-
-        Additional keyword-only parameters that may be supported by a port are:
-
-          - *tx* specifies the TX pin to use.
-          - *rx* specifies the RX pin to use.
-          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
-          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
-          - *txbuf* specifies the length in characters of the TX buffer.
-          - *rxbuf* specifies the length in characters of the RX buffer.
-          - *timeout* specifies the time to wait for the first character (in ms).
-          - *timeout_char* specifies the time to wait between characters (in ms).
-          - *invert* specifies which lines to invert.
-
-              - ``0`` will not invert lines (idle state of both lines is logic high).
-              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
-              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
-              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
-
-          - *flow* specifies which hardware flow control signals to use. The value
-            is a bitmask.
-
-              - ``0`` will ignore hardware flow control signals.
-              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
-                signal if the receive FIFO has sufficient space to accept more data.
-              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
-                CTS input pin signals that the receiver is running low on buffer space.
-              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
-
-        On the WiPy only the following keyword-only parameter is supported:
-
-          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
-            Any of the pins can be None if one wants the UART to operate with limited functionality.
-            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
-            When no pins are given, then the default set of TX and RX pins is taken, and hardware
-            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
-        """
-        ...
-    def writechar(self, *args, **kwargs) -> Any: ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
-        otherwise read as much data as possible. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns an integer counting the number of characters that can be read without
-        blocking.  It will return 0 if there are no characters available and a positive
-        number if there are characters.  The method may return 1 even if there is more
-        than one character available for reading.
-
-        For more sophisticated querying of available characters use select.poll::
-
-         poll = select.poll()
-         poll.register(uart, select.POLLIN)
-         poll.poll(timeout)
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.
-
-        Return value: number of bytes written or ``None`` on timeout.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: the line read or ``None`` on timeout.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-mem32: Any
-mem16: Any
-
-class SoftI2C:
-    """
-    Construct a new software I2C object.  The parameters are:
-
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
-    """
-
-    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_mem(self, *args, **kwargs) -> Any: ...
-    def writeto_mem(self, *args, **kwargs) -> Any: ...
-    def scan(self, *args, **kwargs) -> Any: ...
-    def writeto(self, *args, **kwargs) -> Any: ...
-    def writevto(self, *args, **kwargs) -> Any: ...
-    def start(self, *args, **kwargs) -> Any: ...
-    def readfrom(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def stop(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-    def __init__(self, pin_obj, *args, invert=False) -> None: ...
+"""
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
+
+The ``machine`` module contains specific functions related to the hardware
+on a particular board. Most functions in this module allow to achieve direct
+and unrestricted access to and control of hardware blocks on a system
+(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
+malfunction, lockups, crashes of your board, and in extreme cases, hardware
+damage.
+"""
+from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
+
+HARD_RESET: int
+PWRON_RESET: int
+SOFT_RESET: int
+DEEPSLEEP_RESET: int
+WDT_RESET: int
+
+def idle() -> Any:
+    """
+    Gates the clock to the CPU, useful to reduce power consumption at any time during
+    short or long periods. Peripherals continue working and execution resumes as soon
+    as any interrupt is triggered (on many ports this includes system timer
+    interrupt occurring at regular intervals on the order of millisecond).
+    """
+    ...
+
+def freq(hz: Optional[Any] = None) -> Any:
+    """
+    Returns the CPU frequency in hertz.
+
+    On some ports this can also be used to set the CPU frequency by passing in *hz*.
+    """
+    ...
+
+def info(*args, **kwargs) -> Any: ...
+def dht_readinto(*args, **kwargs) -> Any: ...
+def enable_irq(state) -> Any:
+    """
+    Re-enable interrupt requests.
+    The *state* parameter should be the value that was returned from the most
+    recent call to the `disable_irq()` function.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
+
+def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def soft_reset() -> NoReturn:
+    """
+    Performs a soft reset of the interpreter, deleting all Python objects and
+    resetting the Python heap.  It tries to retain the method by which the user
+    is connected to the MicroPython REPL (eg serial, USB, Wifi).
+    """
+    ...
+
+def sleep() -> Any:
+    """
+    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
+    """
+    ...
+
+def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
+    """
+    Time a pulse on the given *pin*, and return the duration of the pulse in
+    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
+    or 1 to time a high pulse.
+
+    If the current input value of the pin is different to *pulse_level*,
+    the function first (*) waits until the pin input becomes equal to *pulse_level*,
+    then (**) times the duration that the pin is equal to *pulse_level*.
+    If the pin is already equal to *pulse_level* then timing starts straight away.
+
+    The function will return -2 if there was timeout waiting for condition marked
+    (*) above, and -1 if there was timeout during the main measurement, marked (**)
+    above. The timeout is the same for both cases and given by *timeout_us* (which
+    is in microseconds).
+    """
+    ...
+
+def lightsleep(time_ms: Optional[Any] = None) -> Any:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def reset() -> NoReturn:
+    """
+    Resets the device in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def rng() -> int:
+    """
+    Return a 24-bit software generated random number.
+
+    Availability: WiPy.
+    """
+    ...
+
+def reset_cause() -> int:
+    """
+    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
+    """
+    ...
+
+def unique_id() -> bytes:
+    """
+    Returns a byte string with a unique identifier of a board/SoC. It will vary
+    from a board/SoC instance to another, if underlying hardware allows. Length
+    varies by hardware (so use substring of a full value if you expect a short
+    ID). In some MicroPython ports, ID corresponds to the network MAC address.
+    """
+    ...
+
+def bootloader(value: Optional[Any] = None) -> None:
+    """
+    Reset the device and enter its bootloader.  This is typically used to put the
+    device into a state where it can be programmed with new firmware.
+
+    Some ports support passing in an optional *value* argument which can control
+    which bootloader to enter, what to pass to it, or other things.
+    """
+    ...
+
+def bitstream(pin, encoding, timing, data, /) -> Any:
+    """
+    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
+    specifies how the bits are encoded, and *timing* is an encoding-specific timing
+    specification.
+
+    The supported encodings are:
+
+      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
+        1 bits as timed pulses, starting with the most significant bit.
+        The *timing* must be a four-tuple of nanoseconds in the format
+        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
+        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
+        at 800kHz.
+
+    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
+    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
+    will be closer to +/-30ns.
+
+    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
+       module for a higher-level API.
+    """
+    ...
+
+class Pin:
+    """
+    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
+    additional arguments are given in the constructor then they are used to initialise
+    the pin.  Any settings that are not specified will remain in their previous state.
+
+    The arguments are:
+
+      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
+        types are: int (an internal Pin identifier), str (a Pin name), and tuple
+        (pair of [port, pin]).
+
+      - ``mode`` specifies the pin mode, which can be one of:
+
+        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
+          is in high-impedance state.
+
+        - ``Pin.OUT`` - Pin is configured for (normal) output.
+
+        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
+          output works in the following way: if the output value is set to 0 the pin
+          is active at a low level; if the output value is 1 the pin is in a high-impedance
+          state.  Not all ports implement this mode, or some might only on certain pins.
+
+        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
+          port specific.  For a pin configured in such a way any other Pin methods
+          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
+          or a hardware-specific, result).  Not all ports implement this mode.
+
+        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
+          open-drain.  Not all ports implement this mode.
+
+        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
+
+      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
+        one of:
+
+        - ``None`` - No pull up or down resistor.
+        - ``Pin.PULL_UP`` - Pull up resistor enabled.
+        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
+
+      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
+        output pin value if given, otherwise the state of the pin peripheral remains
+        unchanged.
+
+      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
+        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
+        capabilities are port dependent.  Not all ports implement this argument.
+
+      - ``alt`` specifies an alternate function for the pin and the values it can take are
+        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
+        modes.  It may be used when a pin supports more than one alternate function.  If only
+        one pin alternate function is supported the this argument is not required.  Not all
+        ports implement this argument.
+
+    As specified above, the Pin class allows to set an alternate function for a particular
+    pin, but it does not specify any further operations on such a pin.  Pins configured in
+    alternate-function mode are usually not used as GPIO but are instead driven by other
+    hardware peripherals.  The only operation supported on such a pin is re-initialising,
+    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
+    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
+    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
+    """
+
+    AF_OD: int
+    AF9_TIM14: int
+    ALT_OPEN_DRAIN: int
+    AF_PP: int
+    ALT: int
+    AF9_CAN1: int
+    AF8_USART6: int
+    AF9_TIM13: int
+    AF9_CAN2: int
+    AF9_TIM12: int
+    PULL_UP: int
+    OUT_PP: int
+    OUT_OD: int
+    ANALOG: int
+    PULL_DOWN: int
+    PULL_NONE: int
+    IRQ_FALLING: int
+    IN: int
+    OUT: int
+    IRQ_RISING: int
+    OPEN_DRAIN: int
+    AF2_TIM5: int
+    AF3_TIM10: int
+    AF3_TIM11: int
+    AF3_TIM8: int
+    AF3_TIM9: int
+    AF2_TIM4: int
+    AF1_TIM1: int
+    AF1_TIM2: int
+    AF2_TIM3: int
+    AF8_UART4: int
+    AF6_I2S2: int
+    AF7_USART1: int
+    AF7_USART2: int
+    AF7_USART3: int
+    AF4_I2C1: int
+    AF5_SPI2: int
+    AF4_I2C2: int
+    AF5_I2S2: int
+    AF5_SPI1: int
+    def mode(self, mode: Optional[Any] = None) -> Any:
+        """
+        Get or set the pin mode.
+        See the constructor documentation for details of the ``mode`` argument.
+
+        Availability: cc3200, stm32 ports.
+        """
+        ...
+    def name(self, *args, **kwargs) -> Any: ...
+    def pull(self, pull: Optional[Any] = None) -> Any:
+        """
+        Get or set the pin pull state.
+        See the constructor documentation for details of the ``pull`` argument.
+
+        Availability: cc3200, stm32 ports.
+        """
+        ...
+    def low(self) -> None:
+        """
+        Set pin to "0" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
+        """
+           Configure an interrupt handler to be called when the trigger source of the
+           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
+           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
+           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
+           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
+           state '0' and the external pin value for state '1'.
+
+           The arguments are:
+
+             - ``handler`` is an optional function to be called when the interrupt
+               triggers. The handler must take exactly one argument which is the
+               ``Pin`` instance.
+
+             - ``trigger`` configures the event which can generate an interrupt.
+               Possible values are:
+
+               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
+               - ``Pin.IRQ_RISING`` interrupt on rising edge.
+               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
+               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
+
+               These values can be OR'ed together to trigger on multiple events.
+
+             - ``priority`` sets the priority level of the interrupt.  The values it
+               can take are port-specific, but higher values always represent higher
+               priorities.
+
+             - ``wake`` selects the power mode in which this interrupt can wake up the
+               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
+               These values can also be OR'ed together to make a pin generate interrupts in
+               more than one power mode.
+
+             - ``hard`` if true a hardware interrupt is used. This reduces the delay
+               between the pin change and the handler being called. Hard interrupt
+               handlers may not allocate memory; see :ref:`isr_rules`.
+               Not all ports support this argument.
+
+           This method returns a callback object.
+
+        The following methods are not part of the core Pin API and only implemented on certain ports.
+        """
+        ...
+    def pin(self, *args, **kwargs) -> Any: ...
+    def port(self, *args, **kwargs) -> Any: ...
+    def names(self, *args, **kwargs) -> Any: ...
+    def on(self) -> None:
+        """
+        Set pin to "1" output level.
+        """
+        ...
+    def off(self) -> None:
+        """
+        Set pin to "0" output level.
+        """
+        ...
+    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
+        """
+        Re-initialise the pin using the given parameters.  Only those arguments that
+        are specified will be set.  The rest of the pin peripheral state will remain
+        unchanged.  See the constructor documentation for details of the arguments.
+
+        Returns ``None``.
+        """
+        ...
+    def af_list(self, *args, **kwargs) -> Any: ...
+    def af(self, *args, **kwargs) -> Any: ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the pin, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the digital logic level of
+        the pin, returning 0 or 1 corresponding to low and high voltage signals
+        respectively.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The method returns the actual input value currently present
+            on the pin.
+          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
+          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
+            return value of the method is undefined.  Otherwise, if the pin is in
+            state '1', the method returns the actual input value currently present
+            on the pin.
+
+        If the argument is supplied then this method sets the digital logic level of
+        the pin.  The argument ``x`` can be anything that converts to a boolean.
+        If it converts to ``True``, the pin is set to state '1', otherwise it is set
+        to state '0'.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
+            pin state does not change, it remains in the high-impedance state.  The
+            stored value will become active on the pin as soon as it is changed to
+            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
+          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
+          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
+            state.  Otherwise the pin is set to high-impedance state.
+
+        When setting the value this method returns ``None``.
+        """
+        ...
+    def high(self) -> None:
+        """
+        Set pin to "1" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+    def gpio(self, *args, **kwargs) -> Any: ...
+    @classmethod
+    def dict(cls, *args, **kwargs) -> Any: ...
+    @classmethod
+    def debug(cls, *args, **kwargs) -> Any: ...
+
+    class cpu:
+        B9: Any
+        B8: Any
+        B7: Any
+        C0: Any
+        C1: Any
+        C10: Any
+        B3: Any
+        B2: Any
+        B6: Any
+        B4: Any
+        B5: Any
+        B15: Any
+        C7: Any
+        C6: Any
+        C5: Any
+        C8: Any
+        C9: Any
+        C11: Any
+        C13: Any
+        C12: Any
+        C4: Any
+        C2: Any
+        C3: Any
+        D2: Any
+        A15: Any
+        A14: Any
+        A13: Any
+        A2: Any
+        A3: Any
+        A4: Any
+        A1: Any
+        A0: Any
+        A12: Any
+        A10: Any
+        A11: Any
+        B14: Any
+        B11: Any
+        B10: Any
+        B1: Any
+        B12: Any
+        B13: Any
+        A5: Any
+        A7: Any
+        A6: Any
+        B0: Any
+        A8: Any
+        A9: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    @classmethod
+    def mapper(cls, *args, **kwargs) -> Any: ...
+
+    class board:
+        X5: Any
+        X18: Any
+        X4: Any
+        X8: Any
+        X6: Any
+        X7: Any
+        X2: Any
+        X3: Any
+        X19: Any
+        X22: Any
+        X20: Any
+        X21: Any
+        Y5: Any
+        X9: Any
+        Y4: Any
+        Y8: Any
+        Y6: Any
+        Y7: Any
+        Y10: Any
+        Y3: Any
+        Y1: Any
+        Y2: Any
+        Y11: Any
+        Y12: Any
+        Y9: Any
+        SD_CK: Any
+        X17: Any
+        SD: Any
+        SD_D1: Any
+        SD_CMD: Any
+        SD_D0: Any
+        LED_GREEN: Any
+        MMA_INT: Any
+        LED_BLUE: Any
+        MMA_AVDD: Any
+        LED_RED: Any
+        LED_YELLOW: Any
+        X1: Any
+        SD_D2: Any
+        USB_VBUS: Any
+        X12: Any
+        X10: Any
+        X11: Any
+        SD_SW: Any
+        USB_ID: Any
+        SD_D3: Any
+        USB_DP: Any
+        SW: Any
+        USB_DM: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class I2S:
+    """
+    Construct an I2S object of the given id:
+
+    - ``id`` identifies a particular I2S bus; it is board and port specific
+
+    Keyword-only parameters that are supported on all ports:
+
+      - ``sck`` is a pin object for the serial clock line
+      - ``ws`` is a pin object for the word select line
+      - ``sd`` is a pin object for the serial data line
+      - ``mck`` is a pin object for the master clock line;
+        master clock frequency is sampling rate * 256
+      - ``mode`` specifies receive or transmit
+      - ``bits`` specifies sample size (bits), 16 or 32
+      - ``format`` specifies channel format, STEREO or MONO
+      - ``rate`` specifies audio sampling rate (Hz);
+        this is the frequency of the ``ws`` signal
+      - ``ibuf`` specifies internal buffer length (bytes)
+
+    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
+    sample data is transfered between the internal buffer and the I2S peripheral unit.
+    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
+    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
+    """
+
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
+    @staticmethod
+    def shift(*, buf, bits, shift) -> Any:
+        """
+        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
+        Positive for left shift, negative for right shift.
+        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
+        """
+        ...
+    def init(self, sck, *args, **kwargs) -> Any:
+        """
+        see Constructor for argument descriptions
+        """
+        ...
+    def irq(self, handler) -> Any:
+        """
+        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
+        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
+        ``handler`` is called in the context of the MicroPython scheduler.
+        """
+        ...
+    def readinto(self, buf) -> int:
+        """
+        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the left channel sample data is used.
+        Returns number of bytes read
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        Deinitialize the I2S bus
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the sample data is written to both the right and left channels.
+        Returns number of bytes written
+        """
+        ...
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus, *id*. Values of *id* depend
+    on a particular port and its hardware. Values 0, 1, etc. are commonly used
+    to select hardware SPI block #0, #1, etc.
+
+    With no additional parameters, the SPI object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def init(
+        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
+    ) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``baudrate`` is the SCK clock rate.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
+            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
+            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
+            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
+            (``id`` = -1).
+          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
+            specify them as a tuple of ``pins`` parameter.
+
+        In the case of hardware SPI the actual clock frequency may be lower than the
+        requested baudrate. This is dependant on the platform hardware. The actual
+        rate may be determined by printing the SPI object.
+        """
+        ...
+    def write_readinto(self, write_buf, read_buf) -> int:
+        """
+        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
+        buffers can be the same or different, but both buffers must have the
+        same length.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def read(self, nbytes, write=0x00) -> bytes:
+        """
+        Read a number of bytes specified by ``nbytes`` while continuously writing
+        the single byte given by ``write``.
+        Returns a ``bytes`` object with the data that was read.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes contained in ``buf``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def readinto(self, buf, write=0x00) -> int:
+        """
+        Read into the buffer specified by ``buf`` while continuously writing the
+        single byte given by ``write``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes read.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+mem8: Any
+
+class RTC:
+    """
+    Create an RTC object. See init for parameters of initialization.
+    """
+
+    def info(self, *args, **kwargs) -> Any: ...
+    def init(self, datetime) -> None:
+        """
+        Initialise the RTC. Datetime is a tuple of the form:
+
+           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
+        """
+        ...
+    def wakeup(self, *args, **kwargs) -> Any: ...
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time.
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        The meaning of the ``subseconds`` field is hardware dependent.
+        """
+        ...
+    def calibration(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
+
+class I2C:
+    """
+    Construct and return a new I2C object using the following parameters:
+
+       - *id* identifies a particular I2C peripheral.  Allowed values for
+         depend on the particular port/board
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
+
+    Note that some ports/boards will have default values of *scl* and *sda*
+    that can be changed in this constructor.  Others will have fixed values
+    of *scl* and *sda* that cannot be changed.
+    """
+
+    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.  The number of bytes read is the
+        length of *buf*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_into(self, addr, buf, stop=True, /) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr*.
+        The number of bytes read will be the length of *buf*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr* starting from the memory
+        address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Write *buf* to the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
+        those that respond.  A device responds if it pulls the SDA line low after
+        its address (including a write bit) is sent on the bus.
+        """
+        ...
+    def writeto(self, addr, buf, stop=True, /) -> int:
+        """
+        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
+        NACK is received following the write of a byte from *buf* then the
+        remaining bytes are not sent.  If *stop* is true then a STOP condition is
+        generated at the end of the transfer, even if a NACK is received.
+        The function returns the number of ACKs that were received.
+        """
+        ...
+    def writevto(self, addr, vector, stop=True, /) -> int:
+        """
+        Write the bytes contained in *vector* to the peripheral specified by *addr*.
+        *vector* should be a tuple or list of objects with the buffer protocol.
+        The *addr* is sent once and then the bytes from each object in *vector*
+        are written out sequentially.  The objects in *vector* may be zero bytes
+        in length in which case they don't contribute to the output.
+
+        If a NACK is received following the write of a byte from one of the
+        objects in *vector* then the remaining bytes, and any remaining objects,
+        are not sent.  If *stop* is true then a STOP condition is generated at
+        the end of the transfer, even if a NACK is received.  The function
+        returns the number of ACKs that were received.
+        """
+        ...
+    def start(self) -> None:
+        """
+        Generate a START condition on the bus (SDA transitions to low while SCL is high).
+        """
+        ...
+    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def readinto(self, buf, nack=True, /) -> Any:
+        """
+        Reads bytes from the bus and stores them into *buf*.  The number of bytes
+        read is the length of *buf*.  An ACK will be sent on the bus after
+        receiving all but the last byte.  After the last byte is received, if *nack*
+        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
+        case the peripheral assumes more bytes are going to be read in a later call).
+        """
+        ...
+    def init(self, scl, sda, *, freq=400000) -> None:
+        """
+        Initialise the I2C bus with the given arguments:
+
+           - *scl* is a pin object for the SCL line
+           - *sda* is a pin object for the SDA line
+           - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
+        """
+        ...
+    def stop(self) -> None:
+        """
+        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from *buf* to the bus.  Checks that an ACK is received
+        after each byte and stops transmitting the remaining bytes if a NACK is
+        received.  The function returns the number of ACKs that were received.
+        """
+        ...
+    def __init__(
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
+
+class ADC:
+    """
+    Access the ADC associated with a source identified by *id*.  This
+    *id* may be an integer (usually specifying a channel number), a
+    :ref:`Pin <machine.Pin>` object, or other value supported by the
+    underlying machine.
+
+    If additional keyword-arguments are given then they will configure
+    various aspects of the ADC.  If not given, these settings will take
+    previous or default values.  The settings are:
+
+      - *sample_ns* is the sampling time in nanoseconds.
+
+      - *atten* specifies the input attenuation.
+    """
+
+    VREF: int
+    CORE_VREF: int
+    CORE_VBAT: int
+    CORE_TEMP: int
+    def read_u16(self) -> int:
+        """
+        Take an analog reading and return an integer in the range 0-65535.
+        The return value represents the raw reading taken by the ADC, scaled
+        such that the minimum value is 0 and the maximum value is 65535.
+        """
+        ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
+
+class WDT:
+    """
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
+
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
+    """
+
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
+        ...
+    def __init__(self, id=0, timeout=5000) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
+    virtual timer (if supported by a board).
+    ``id`` shall not be passed as a keyword argument.
+
+    See ``init`` for parameters of initialisation.
+    """
+
+    PERIODIC: int
+    ONE_SHOT: int
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
+        """
+        Initialise the timer. Example::
+
+            def mycallback(t):
+                pass
+
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
+            # periodic with 100ms period
+            tim.init(period=100, callback=mycallback)
+
+            # one shot firing after 1000ms
+            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
+              period of the channel expires.
+            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
+              frequency of the channel.
+
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
+          - ``period`` - The timer period, in milliseconds.
+
+          - ``callback`` - The callable to call upon expiration of the timer period.
+            The callback must take one argument, which is passed the Timer object.
+            The ``callback`` argument shall be specified. Otherwise an exception
+            will occurr upon timer expiration:
+            ``TypeError: 'NoneType' object isn't callable``
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
+
+class SoftSPI:
+    """
+    Construct a new software SPI object.  Additional parameters must be
+    given, usually at least *sck*, *mosi* and *miso*, and these are used
+    to initialise the bus.  See `SPI.init` for a description of the parameters.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
+
+class UART:
+    """
+    Construct a UART object of the given id.
+    """
+
+    IRQ_RXIDLE: int
+    CTS: int
+    RTS: int
+    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - *baudrate* is the clock rate.
+          - *bits* is the number of bits per character, 7, 8 or 9.
+          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
+          - *stop* is the number of stop bits, 1 or 2.
+
+        Additional keyword-only parameters that may be supported by a port are:
+
+          - *tx* specifies the TX pin to use.
+          - *rx* specifies the RX pin to use.
+          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
+          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
+          - *txbuf* specifies the length in characters of the TX buffer.
+          - *rxbuf* specifies the length in characters of the RX buffer.
+          - *timeout* specifies the time to wait for the first character (in ms).
+          - *timeout_char* specifies the time to wait between characters (in ms).
+          - *invert* specifies which lines to invert.
+
+              - ``0`` will not invert lines (idle state of both lines is logic high).
+              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
+              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
+              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
+
+          - *flow* specifies which hardware flow control signals to use. The value
+            is a bitmask.
+
+              - ``0`` will ignore hardware flow control signals.
+              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
+                signal if the receive FIFO has sufficient space to accept more data.
+              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
+                CTS input pin signals that the receiver is running low on buffer space.
+              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
+
+        On the WiPy only the following keyword-only parameter is supported:
+
+          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
+            Any of the pins can be None if one wants the UART to operate with limited functionality.
+            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
+            When no pins are given, then the default set of TX and RX pins is taken, and hardware
+            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
+        """
+        ...
+    def flush(self) -> Any:
+        """
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def irq(self, trigger, priority=1, handler=None, wake=IDLE) -> Any:
+        """
+        Create a callback to be triggered when data is received on the UART.
+
+            - *trigger* can only be ``UART.RX_ANY``
+            - *priority* level of the interrupt. Can take values in the range 1-7.
+              Higher values represent higher priorities.
+            - *handler* an optional function to be called when new characters arrive.
+            - *wake* can only be ``machine.IDLE``.
+
+        .. note::
+
+           The handler will be called whenever any of the following two conditions are met:
+
+               - 8 new characters have been received.
+               - At least 1 new character is waiting in the Rx buffer and the Rx line has been
+                 silent for the duration of 1 complete frame.
+
+           This means that when the handler function is called there will be between 1 to 8
+           characters waiting.
+
+        Returns an irq object.
+
+        Availability: WiPy.
+        """
+        ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
+        """
+        ...
+    def readchar(self, *args, **kwargs) -> Any: ...
+    def writechar(self, *args, **kwargs) -> Any: ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
+        otherwise read as much data as possible. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns an integer counting the number of characters that can be read without
+        blocking.  It will return 0 if there are no characters available and a positive
+        number if there are characters.  The method may return 1 even if there is more
+        than one character available for reading.
+
+        For more sophisticated querying of available characters use select.poll::
+
+         poll = select.poll()
+         poll.register(uart, select.POLLIN)
+         poll.poll(timeout)
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.
+
+        Return value: number of bytes written or ``None`` on timeout.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: the line read or ``None`` on timeout.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+mem32: Any
+mem16: Any
+
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
+
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
+
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
+        ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/micropython.pyi` & `micropython_stm32_stubs-1.20.0.post1/micropython.pyi`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""
-access and control MicroPython internals. See: https://docs.micropython.org/en/v1.19.1/library/micropython.html
-"""
-from typing import Optional, Any, Callable
-
-def opt_level(level: Optional[Any] = None) -> Any:
-    """
-    If *level* is given then this function sets the optimisation level for subsequent
-    compilation of scripts, and returns ``None``.  Otherwise it returns the current
-    optimisation level.
-
-    The optimisation level controls the following compilation features:
-
-    - Assertions: at level 0 assertion statements are enabled and compiled into the
-      bytecode; at levels 1 and higher assertions are not compiled.
-    - Built-in ``__debug__`` variable: at level 0 this variable expands to ``True``;
-      at levels 1 and higher it expands to ``False``.
-    - Source-code line numbers: at levels 0, 1 and 2 source-code line number are
-      stored along with the bytecode so that exceptions can report the line number
-      they occurred at; at levels 3 and higher line numbers are not stored.
-
-    The default optimisation level is usually level 0.
-    """
-    ...
-
-def mem_info(verbose: Optional[Any] = None) -> None:
-    """
-    Print information about currently used memory.  If the *verbose* argument
-    is given then extra information is printed.
-
-    The information that is printed is implementation dependent, but currently
-    includes the amount of stack and heap used.  In verbose mode it prints out
-    the entire heap indicating which blocks are used and which are free.
-    """
-    ...
-
-def stack_use() -> int:
-    """
-    Return an integer representing the current amount of stack that is being
-    used.  The absolute value of this is not particularly useful, rather it
-    should be used to compute differences in stack usage at different points.
-    """
-    ...
-
-def qstr_info(verbose: Optional[Any] = None) -> None:
-    """
-    Print information about currently interned strings.  If the *verbose*
-    argument is given then extra information is printed.
-
-    The information that is printed is implementation dependent, but currently
-    includes the number of interned strings and the amount of RAM they use.  In
-    verbose mode it prints out the names of all RAM-interned strings.
-    """
-    ...
-
-def schedule(func, arg) -> Any:
-    """
-    Schedule the function *func* to be executed "very soon".  The function
-    is passed the value *arg* as its single argument.  "Very soon" means that
-    the MicroPython runtime will do its best to execute the function at the
-    earliest possible time, given that it is also trying to be efficient, and
-    that the following conditions hold:
-
-    - A scheduled function will never preempt another scheduled function.
-    - Scheduled functions are always executed "between opcodes" which means
-      that all fundamental Python operations (such as appending to a list)
-      are guaranteed to be atomic.
-    - A given port may define "critical regions" within which scheduled
-      functions will never be executed.  Functions may be scheduled within
-      a critical region but they will not be executed until that region
-      is exited.  An example of a critical region is a preempting interrupt
-      handler (an IRQ).
-
-    A use for this function is to schedule a callback from a preempting IRQ.
-    Such an IRQ puts restrictions on the code that runs in the IRQ (for example
-    the heap may be locked) and scheduling a function to call later will lift
-    those restrictions.
-
-    Note: If `schedule()` is called from a preempting IRQ, when memory
-    allocation is not allowed and the callback to be passed to `schedule()` is
-    a bound method, passing this directly will fail. This is because creating a
-    reference to a bound method causes memory allocation. A solution is to
-    create a reference to the method in the class constructor and to pass that
-    reference to `schedule()`. This is discussed in detail here
-    :ref:`reference documentation <isr_rules>` under "Creation of Python
-    objects".
-
-    There is a finite queue to hold the scheduled functions and `schedule()`
-    will raise a `RuntimeError` if the queue is full.
-    """
-    ...
-
-def alloc_emergency_exception_buf(size) -> Any:
-    """
-    Allocate *size* bytes of RAM for the emergency exception buffer (a good
-    size is around 100 bytes).  The buffer is used to create exceptions in cases
-    when normal RAM allocation would fail (eg within an interrupt handler) and
-    therefore give useful traceback information in these situations.
-
-    A good way to use this function is to put it at the start of your main script
-    (eg ``boot.py`` or ``main.py``) and then the emergency exception buffer will be active
-    for all the code following it.
-    """
-    ...
-
-def const(expr) -> int:
-    """
-    Used to declare that the expression is a constant so that the compile can
-    optimise it.  The use of this function should be as follows::
-
-     from micropython import const
-
-     CONST_X = const(123)
-     CONST_Y = const(2 * CONST_X + 1)
-
-    Constants declared this way are still accessible as global variables from
-    outside the module they are declared in.  On the other hand, if a constant
-    begins with an underscore then it is hidden, it is not available as a global
-    variable, and does not take up any memory during execution.
-
-    This `const` function is recognised directly by the MicroPython parser and is
-    provided as part of the :mod:`micropython` module mainly so that scripts can be
-    written which run under both CPython and MicroPython, by following the above
-    pattern.
-    """
-    ...
-
-def kbd_intr(chr) -> None:
-    """
-    Set the character that will raise a `KeyboardInterrupt` exception.  By
-    default this is set to 3 during script execution, corresponding to Ctrl-C.
-    Passing -1 to this function will disable capture of Ctrl-C, and passing 3
-    will restore it.
-
-    This function can be used to prevent the capturing of Ctrl-C on the
-    incoming stream of characters that is usually used for the REPL, in case
-    that stream is used for other purposes.
-    """
-    ...
-
-def heap_lock() -> Any: ...
-def heap_unlock() -> Any: ...
-def viper(func: Callable) -> Callable:
-    """
-    The Viper code emitter is not fully compliant. It supports special Viper native data types in pursuit of performance.
-    Integer processing is non-compliant because it uses machine words: arithmetic on 32 bit hardware is performed modulo 2**32.
-    Like the Native emitter Viper produces machine instructions but further optimisations are performed, substantially increasing
-    performance especially for integer arithmetic and bit manipulations.
-    """
-    ...
-
-def native(func: Callable) -> Callable:
-    """
-    This causes the MicroPython compiler to emit native CPU opcodes rather than bytecode.
-    It covers the bulk of the MicroPython functionality, so most functions will require no adaptation.
-    See: https://docs.micropython.org/en/latest/reference/speed_python.html?highlight=viper#the-native-code-emitter
-    """
-    ...
+"""
+access and control MicroPython internals. See: https://docs.micropython.org/en/v1.19.1/library/micropython.html
+"""
+from typing import Optional, Any, Callable
+
+def opt_level(level: Optional[Any] = None) -> Any:
+    """
+    If *level* is given then this function sets the optimisation level for subsequent
+    compilation of scripts, and returns ``None``.  Otherwise it returns the current
+    optimisation level.
+
+    The optimisation level controls the following compilation features:
+
+    - Assertions: at level 0 assertion statements are enabled and compiled into the
+      bytecode; at levels 1 and higher assertions are not compiled.
+    - Built-in ``__debug__`` variable: at level 0 this variable expands to ``True``;
+      at levels 1 and higher it expands to ``False``.
+    - Source-code line numbers: at levels 0, 1 and 2 source-code line number are
+      stored along with the bytecode so that exceptions can report the line number
+      they occurred at; at levels 3 and higher line numbers are not stored.
+
+    The default optimisation level is usually level 0.
+    """
+    ...
+
+def mem_info(verbose: Optional[Any] = None) -> None:
+    """
+    Print information about currently used memory.  If the *verbose* argument
+    is given then extra information is printed.
+
+    The information that is printed is implementation dependent, but currently
+    includes the amount of stack and heap used.  In verbose mode it prints out
+    the entire heap indicating which blocks are used and which are free.
+    """
+    ...
+
+def stack_use() -> int:
+    """
+    Return an integer representing the current amount of stack that is being
+    used.  The absolute value of this is not particularly useful, rather it
+    should be used to compute differences in stack usage at different points.
+    """
+    ...
+
+def qstr_info(verbose: Optional[Any] = None) -> None:
+    """
+    Print information about currently interned strings.  If the *verbose*
+    argument is given then extra information is printed.
+
+    The information that is printed is implementation dependent, but currently
+    includes the number of interned strings and the amount of RAM they use.  In
+    verbose mode it prints out the names of all RAM-interned strings.
+    """
+    ...
+
+def schedule(func, arg) -> Any:
+    """
+    Schedule the function *func* to be executed "very soon".  The function
+    is passed the value *arg* as its single argument.  "Very soon" means that
+    the MicroPython runtime will do its best to execute the function at the
+    earliest possible time, given that it is also trying to be efficient, and
+    that the following conditions hold:
+
+    - A scheduled function will never preempt another scheduled function.
+    - Scheduled functions are always executed "between opcodes" which means
+      that all fundamental Python operations (such as appending to a list)
+      are guaranteed to be atomic.
+    - A given port may define "critical regions" within which scheduled
+      functions will never be executed.  Functions may be scheduled within
+      a critical region but they will not be executed until that region
+      is exited.  An example of a critical region is a preempting interrupt
+      handler (an IRQ).
+
+    A use for this function is to schedule a callback from a preempting IRQ.
+    Such an IRQ puts restrictions on the code that runs in the IRQ (for example
+    the heap may be locked) and scheduling a function to call later will lift
+    those restrictions.
+
+    Note: If `schedule()` is called from a preempting IRQ, when memory
+    allocation is not allowed and the callback to be passed to `schedule()` is
+    a bound method, passing this directly will fail. This is because creating a
+    reference to a bound method causes memory allocation. A solution is to
+    create a reference to the method in the class constructor and to pass that
+    reference to `schedule()`. This is discussed in detail here
+    :ref:`reference documentation <isr_rules>` under "Creation of Python
+    objects".
+
+    There is a finite queue to hold the scheduled functions and `schedule()`
+    will raise a `RuntimeError` if the queue is full.
+    """
+    ...
+
+def alloc_emergency_exception_buf(size) -> Any:
+    """
+    Allocate *size* bytes of RAM for the emergency exception buffer (a good
+    size is around 100 bytes).  The buffer is used to create exceptions in cases
+    when normal RAM allocation would fail (eg within an interrupt handler) and
+    therefore give useful traceback information in these situations.
+
+    A good way to use this function is to put it at the start of your main script
+    (eg ``boot.py`` or ``main.py``) and then the emergency exception buffer will be active
+    for all the code following it.
+    """
+    ...
+
+def const(expr) -> int:
+    """
+    Used to declare that the expression is a constant so that the compile can
+    optimise it.  The use of this function should be as follows::
+
+     from micropython import const
+
+     CONST_X = const(123)
+     CONST_Y = const(2 * CONST_X + 1)
+
+    Constants declared this way are still accessible as global variables from
+    outside the module they are declared in.  On the other hand, if a constant
+    begins with an underscore then it is hidden, it is not available as a global
+    variable, and does not take up any memory during execution.
+
+    This `const` function is recognised directly by the MicroPython parser and is
+    provided as part of the :mod:`micropython` module mainly so that scripts can be
+    written which run under both CPython and MicroPython, by following the above
+    pattern.
+    """
+    ...
+
+def kbd_intr(chr) -> None:
+    """
+    Set the character that will raise a `KeyboardInterrupt` exception.  By
+    default this is set to 3 during script execution, corresponding to Ctrl-C.
+    Passing -1 to this function will disable capture of Ctrl-C, and passing 3
+    will restore it.
+
+    This function can be used to prevent the capturing of Ctrl-C on the
+    incoming stream of characters that is usually used for the REPL, in case
+    that stream is used for other purposes.
+    """
+    ...
+
+def heap_lock() -> Any: ...
+def heap_unlock() -> Any: ...
+def viper(func: Callable) -> Callable:
+    """
+    The Viper code emitter is not fully compliant. It supports special Viper native data types in pursuit of performance.
+    Integer processing is non-compliant because it uses machine words: arithmetic on 32 bit hardware is performed modulo 2**32.
+    Like the Native emitter Viper produces machine instructions but further optimisations are performed, substantially increasing
+    performance especially for integer arithmetic and bit manipulations.
+    """
+    ...
+
+def native(func: Callable) -> Callable:
+    """
+    This causes the MicroPython compiler to emit native CPU opcodes rather than bytecode.
+    It covers the bulk of the MicroPython functionality, so most functions will require no adaptation.
+    See: https://docs.micropython.org/en/latest/reference/speed_python.html?highlight=viper#the-native-code-emitter
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/network.pyi` & `micropython_stm32_stubs-1.20.0.post1/network.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-"""
-network configuration. See: https://docs.micropython.org/en/v1.19.1/library/network.html
-
-This module provides network drivers and routing configuration. To use this
-module, a MicroPython variant/build with network capabilities must be installed.
-Network drivers for specific hardware are available within this module and are
-used to configure hardware network interface(s). Network services provided
-by configured interfaces are then available for use via the :mod:`socket`
-module.
-
-For example::
-
-    # connect/ show IP config a specific network interface
-    # see below for examples of specific drivers
-    import network
-    import time
-    nic = network.Driver(...)
-    if not nic.isconnected():
-        nic.connect()
-        print("Waiting for connection...")
-        while not nic.isconnected():
-            time.sleep(1)
-    print(nic.ifconfig())
-
-    # now use socket as usual
-    import socket
-    addr = socket.getaddrinfo('micropython.org', 80)[0][-1]
-    s = socket.socket()
-    s.connect(addr)
-    s.send(b'GET / HTTP/1.1\r\nHost: micropython.org\r\n\r\n')
-    data = s.recv(1000)
-    s.close()
-"""
-from typing import List, Optional, Tuple, Union, Any
-
-STA_IF: int
-AP_IF: int
-
-def route(*args, **kwargs) -> Any: ...
+"""
+network configuration. See: https://docs.micropython.org/en/v1.20.0/library/network.html
+
+This module provides network drivers and routing configuration. To use this
+module, a MicroPython variant/build with network capabilities must be installed.
+Network drivers for specific hardware are available within this module and are
+used to configure hardware network interface(s). Network services provided
+by configured interfaces are then available for use via the :mod:`socket`
+module.
+
+For example::
+
+    # connect/ show IP config a specific network interface
+    # see below for examples of specific drivers
+    import network
+    import time
+    nic = network.Driver(...)
+    if not nic.isconnected():
+        nic.connect()
+        print("Waiting for connection...")
+        while not nic.isconnected():
+            time.sleep(1)
+    print(nic.ifconfig())
+
+    # now use socket as usual
+    import socket
+    addr = socket.getaddrinfo('micropython.org', 80)[0][-1]
+    s = socket.socket()
+    s.connect(addr)
+    s.send(b'GET / HTTP/1.1\r\nHost: micropython.org\r\n\r\n')
+    data = s.recv(1000)
+    s.close()
+"""
+from typing import List, Optional, Tuple, Union, Any
+
+STA_IF: int
+AP_IF: int
+
+def hostname(*args, **kwargs) -> Any: ...
+def route(*args, **kwargs) -> Any: ...
+def country(*args, **kwargs) -> Any: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/onewire.pyi` & `micropython_stm32_stubs-1.20.0.post1/onewire.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from _typeshed import Incomplete
-
-class OneWireError(Exception): ...
-
-class OneWire:
-    SEARCH_ROM: int
-    MATCH_ROM: int
-    SKIP_ROM: int
-    pin: Incomplete
-    def __init__(self, pin) -> None: ...
-    def reset(self, required: bool = ...): ...
-    def readbit(self): ...
-    def readbyte(self): ...
-    def readinto(self, buf) -> None: ...
-    def writebit(self, value): ...
-    def writebyte(self, value): ...
-    def write(self, buf) -> None: ...
-    def select_rom(self, rom) -> None: ...
-    def scan(self): ...
-    def _search_rom(self, l_rom, diff): ...
-    def crc8(self, data): ...
+from _typeshed import Incomplete
+
+class OneWireError(Exception): ...
+
+class OneWire:
+    SEARCH_ROM: int
+    MATCH_ROM: int
+    SKIP_ROM: int
+    pin: Incomplete
+    def __init__(self, pin) -> None: ...
+    def reset(self, required: bool = ...): ...
+    def readbit(self): ...
+    def readbyte(self): ...
+    def readinto(self, buf) -> None: ...
+    def writebit(self, value): ...
+    def writebyte(self, value): ...
+    def write(self, buf) -> None: ...
+    def select_rom(self, rom) -> None: ...
+    def scan(self): ...
+    def _search_rom(self, l_rom, diff): ...
+    def crc8(self, data): ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/os.pyi` & `micropython_stm32_stubs-1.20.0.post1/os.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-"""
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
-
-|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
-
-The ``os`` module contains functions for filesystem access and mounting,
-terminal redirection and duplication, and the ``uname`` and ``urandom``
-functions.
-"""
-from typing import IO, Iterator, Optional, Tuple, Any
-from stdlib.os import uname_result
-
-sep: str
-
-def statvfs(path) -> Tuple:
-    """
-    Get the status of a fileystem.
-
-    Returns a tuple with the filesystem information in the following order:
-
-         * ``f_bsize`` -- file system block size
-         * ``f_frsize`` -- fragment size
-         * ``f_blocks`` -- size of fs in f_frsize units
-         * ``f_bfree`` -- number of free blocks
-         * ``f_bavail`` -- number of free blocks for unprivileged users
-         * ``f_files`` -- number of inodes
-         * ``f_ffree`` -- number of free inodes
-         * ``f_favail`` -- number of free inodes for unprivileged users
-         * ``f_flag`` -- mount flags
-         * ``f_namemax`` -- maximum filename length
-
-    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
-    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
-    in a port-specific implementation.
-    """
-    ...
-
-def stat(path) -> Any:
-    """
-    Get the status of a file or directory.
-    """
-    ...
-
-def rmdir(path) -> None:
-    """
-    Remove a directory.
-    """
-    ...
-
-def rename(old_path, new_path) -> None:
-    """
-    Rename a file.
-    """
-    ...
-
-def mount(fsobj, mount_point, *, readonly) -> Any:
-    """
-    Mount the filesystem object *fsobj* at the location in the VFS given by the
-    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
-    method, or a block device.  If it's a block device then the filesystem type
-    is automatically detected (an exception is raised if no filesystem was
-    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
-    or ``'/<name>'`` to mount it at a subdirectory under the root.
-
-    If *readonly* is ``True`` then the filesystem is mounted read-only.
-
-    During the mount process the method ``mount()`` is called on the filesystem
-    object.
-
-    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
-    """
-    ...
-
-def sync() -> None:
-    """
-    Sync all filesystems.
-    """
-    ...
-
-def unlink(*args, **kwargs) -> Any: ...
-def uname() -> uname_result:
-    """
-    Return a tuple (possibly a named tuple) containing information about the
-    underlying machine and/or its operating system.  The tuple has five fields
-    in the following order, each of them being a string:
-
-         * ``sysname`` -- the name of the underlying system
-         * ``nodename`` -- the network name (can be the same as ``sysname``)
-         * ``release`` -- the version of the underlying system
-         * ``version`` -- the MicroPython version and build date
-         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
-    """
-    ...
-
-def umount(mount_point) -> Any:
-    """
-    Unmount a filesystem. *mount_point* can be a string naming the mount location,
-    or a previously-mounted filesystem object.  During the unmount process the
-    method ``umount()`` is called on the filesystem object.
-
-    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
-    """
-    ...
-
-def urandom(n) -> bytes:
-    """
-    Return a bytes object with *n* random bytes. Whenever possible, it is
-    generated by the hardware random number generator.
-    """
-    ...
-
-def chdir(path) -> Any:
-    """
-    Change current directory.
-    """
-    ...
-
-def dupterm(stream_object, index=0, /) -> IO:
-    """
-    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
-    object. The *stream_object* argument must be a native stream object, or derive
-    from ``io.IOBase`` and implement the ``readinto()`` and
-    ``write()`` methods.  The stream should be in non-blocking mode and
-    ``readinto()`` should return ``None`` if there is no data available for reading.
-
-    After calling this function all terminal output is repeated on this stream,
-    and any input that is available on the stream is passed on to the terminal input.
-
-    The *index* parameter should be a non-negative integer and specifies which
-    duplication slot is set.  A given port may implement more than one slot (slot 0
-    will always be available) and in that case terminal input and output is
-    duplicated on all the slots that are set.
-
-    If ``None`` is passed as the *stream_object* then duplication is cancelled on
-    the slot given by *index*.
-
-    The function returns the previous stream-like object in the given slot.
-    """
-    ...
-
-def remove(path) -> None:
-    """
-    Remove a file.
-    """
-    ...
-
-def mkdir(path) -> Any:
-    """
-    Create a new directory.
-    """
-    ...
-
-def getcwd() -> Any:
-    """
-    Get the current directory.
-    """
-    ...
-
-def listdir(dir: Optional[Any] = None) -> Any:
-    """
-    With no argument, list the current directory.  Otherwise list the given directory.
-    """
-    ...
-
-def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
-    """
-    This function returns an iterator which then yields tuples corresponding to
-    the entries in the directory that it is listing.  With no argument it lists the
-    current directory, otherwise it lists the directory given by *dir*.
-
-    The tuples have the form *(name, type, inode[, size])*:
-
-     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
-       the entry;
-     - *type* is an integer that specifies the type of the entry, with 0x4000 for
-       directories and 0x8000 for regular files;
-     - *inode* is an integer corresponding to the inode of the file, and may be 0
-       for filesystems that don't have such a notion.
-     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
-       file entries, *size* is an integer representing the size of the file
-       or -1 if unknown.  Its meaning is currently undefined for directory
-       entries.
-    """
-    ...
-
-class VfsLfs2:
-    """
-    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
-    Storage of the littlefs filesystem is provided by *block_dev*, which must
-    support the :ref:`extended interface <block-device-interface>`.
-    Objects created by this constructor can be mounted using :func:`mount`.
-
-    The *mtime* argument enables modification timestamps for files, stored using
-    littlefs attributes.  This option can be disabled or enabled differently each
-    mount time and timestamps will only be added or updated if *mtime* is enabled,
-    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
-    timestamps will work without reformatting and timestamps will be added
-    transparently to existing files once they are opened for writing.  When *mtime*
-    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
-
-    See :ref:`filesystem` for more information.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
-        """
-            Build a Lfs2 filesystem on *block_dev*.
-
-        ``Note:`` There are reports of littlefs v2 failing in certain situations,
-                  for details see `littlefs issue 295`_.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
-
-class VfsFat:
-    """
-    Create a filesystem object that uses the FAT filesystem format.  Storage of
-    the FAT filesystem is provided by *block_dev*.
-    Objects created by this constructor can be mounted using :func:`mount`.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev) -> None:
-        """
-        Build a FAT filesystem on *block_dev*.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev) -> None: ...
+"""
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
+
+|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
+
+The ``os`` module contains functions for filesystem access and mounting,
+terminal redirection and duplication, and the ``uname`` and ``urandom``
+functions.
+"""
+from typing import IO, Iterator, Optional, Tuple, Any
+from stdlib.os import uname_result
+
+sep: str
+
+def statvfs(path) -> Tuple:
+    """
+    Get the status of a fileystem.
+
+    Returns a tuple with the filesystem information in the following order:
+
+         * ``f_bsize`` -- file system block size
+         * ``f_frsize`` -- fragment size
+         * ``f_blocks`` -- size of fs in f_frsize units
+         * ``f_bfree`` -- number of free blocks
+         * ``f_bavail`` -- number of free blocks for unprivileged users
+         * ``f_files`` -- number of inodes
+         * ``f_ffree`` -- number of free inodes
+         * ``f_favail`` -- number of free inodes for unprivileged users
+         * ``f_flag`` -- mount flags
+         * ``f_namemax`` -- maximum filename length
+
+    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
+    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
+    in a port-specific implementation.
+    """
+    ...
+
+def stat(path) -> Any:
+    """
+    Get the status of a file or directory.
+    """
+    ...
+
+def rmdir(path) -> None:
+    """
+    Remove a directory.
+    """
+    ...
+
+def rename(old_path, new_path) -> None:
+    """
+    Rename a file.
+    """
+    ...
+
+def mount(fsobj, mount_point, *, readonly) -> Any:
+    """
+    Mount the filesystem object *fsobj* at the location in the VFS given by the
+    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
+    method, or a block device.  If it's a block device then the filesystem type
+    is automatically detected (an exception is raised if no filesystem was
+    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
+    or ``'/<name>'`` to mount it at a subdirectory under the root.
+
+    If *readonly* is ``True`` then the filesystem is mounted read-only.
+
+    During the mount process the method ``mount()`` is called on the filesystem
+    object.
+
+    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
+    """
+    ...
+
+def sync() -> None:
+    """
+    Sync all filesystems.
+    """
+    ...
+
+def unlink(*args, **kwargs) -> Any: ...
+def uname() -> uname_result:
+    """
+    Return a tuple (possibly a named tuple) containing information about the
+    underlying machine and/or its operating system.  The tuple has five fields
+    in the following order, each of them being a string:
+
+         * ``sysname`` -- the name of the underlying system
+         * ``nodename`` -- the network name (can be the same as ``sysname``)
+         * ``release`` -- the version of the underlying system
+         * ``version`` -- the MicroPython version and build date
+         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
+    """
+    ...
+
+def umount(mount_point) -> Any:
+    """
+    Unmount a filesystem. *mount_point* can be a string naming the mount location,
+    or a previously-mounted filesystem object.  During the unmount process the
+    method ``umount()`` is called on the filesystem object.
+
+    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
+    """
+    ...
+
+def urandom(n) -> bytes:
+    """
+    Return a bytes object with *n* random bytes. Whenever possible, it is
+    generated by the hardware random number generator.
+    """
+    ...
+
+def chdir(path) -> Any:
+    """
+    Change current directory.
+    """
+    ...
+
+def dupterm(stream_object, index=0, /) -> IO:
+    """
+    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
+    object. The *stream_object* argument must be a native stream object, or derive
+    from ``io.IOBase`` and implement the ``readinto()`` and
+    ``write()`` methods.  The stream should be in non-blocking mode and
+    ``readinto()`` should return ``None`` if there is no data available for reading.
+
+    After calling this function all terminal output is repeated on this stream,
+    and any input that is available on the stream is passed on to the terminal input.
+
+    The *index* parameter should be a non-negative integer and specifies which
+    duplication slot is set.  A given port may implement more than one slot (slot 0
+    will always be available) and in that case terminal input and output is
+    duplicated on all the slots that are set.
+
+    If ``None`` is passed as the *stream_object* then duplication is cancelled on
+    the slot given by *index*.
+
+    The function returns the previous stream-like object in the given slot.
+    """
+    ...
+
+def remove(path) -> None:
+    """
+    Remove a file.
+    """
+    ...
+
+def mkdir(path) -> Any:
+    """
+    Create a new directory.
+    """
+    ...
+
+def getcwd() -> Any:
+    """
+    Get the current directory.
+    """
+    ...
+
+def listdir(dir: Optional[Any] = None) -> Any:
+    """
+    With no argument, list the current directory.  Otherwise list the given directory.
+    """
+    ...
+
+def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
+    """
+    This function returns an iterator which then yields tuples corresponding to
+    the entries in the directory that it is listing.  With no argument it lists the
+    current directory, otherwise it lists the directory given by *dir*.
+
+    The tuples have the form *(name, type, inode[, size])*:
+
+     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
+       the entry;
+     - *type* is an integer that specifies the type of the entry, with 0x4000 for
+       directories and 0x8000 for regular files;
+     - *inode* is an integer corresponding to the inode of the file, and may be 0
+       for filesystems that don't have such a notion.
+     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
+       file entries, *size* is an integer representing the size of the file
+       or -1 if unknown.  Its meaning is currently undefined for directory
+       entries.
+    """
+    ...
+
+class VfsLfs2:
+    """
+    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
+    Storage of the littlefs filesystem is provided by *block_dev*, which must
+    support the :ref:`extended interface <block-device-interface>`.
+    Objects created by this constructor can be mounted using :func:`mount`.
+
+    The *mtime* argument enables modification timestamps for files, stored using
+    littlefs attributes.  This option can be disabled or enabled differently each
+    mount time and timestamps will only be added or updated if *mtime* is enabled,
+    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
+    timestamps will work without reformatting and timestamps will be added
+    transparently to existing files once they are opened for writing.  When *mtime*
+    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
+
+    See :ref:`filesystem` for more information.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
+        """
+            Build a Lfs2 filesystem on *block_dev*.
+
+        ``Note:`` There are reports of littlefs v2 failing in certain situations,
+                  for details see `littlefs issue 295`_.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
+
+class VfsFat:
+    """
+    Create a filesystem object that uses the FAT filesystem format.  Storage of
+    the FAT filesystem is provided by *block_dev*.
+    Objects created by this constructor can be mounted using :func:`mount`.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev) -> None:
+        """
+        Build a FAT filesystem on *block_dev*.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/pyb.pyi` & `micropython_stm32_stubs-1.20.0.post1/pyb.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,2200 +1,2236 @@
-"""
-functions related to the board. See: https://docs.micropython.org/en/v1.19.1/library/pyb.html
-
-The ``pyb`` module contains specific functions related to the board.
-"""
-from typing import List, NoReturn, Optional, Tuple, Any
-
-hid_mouse: tuple
-hid_keyboard: tuple
-
-def hard_reset() -> NoReturn:
-    """
-    Resets the pyboard in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-def have_cdc() -> bool:
-    """
-    Return True if USB is connected as a serial device, False otherwise.
-
-    ``Note:`` This function is deprecated.  Use pyb.USB_VCP().isconnected() instead.
-    """
-    ...
-
-def hid(hidtuple: Tuple) -> Any:
-    """
-    Takes a 4-tuple (or list) and sends it to the USB host (the PC) to
-    signal a HID mouse-motion event.
-
-    ``Note:`` This function is deprecated.  Use :meth:`pyb.USB_HID.send()` instead.
-    """
-    ...
-
-def info(dump_alloc_table: Optional[Any] = None) -> None:
-    """
-    Print out lots of information about the board.
-    """
-    ...
-
-def dht_readinto(*args, **kwargs) -> Any: ...
-def elapsed_micros(start) -> int:
-    """
-    Returns the number of microseconds which have elapsed since ``start``.
-
-    This function takes care of counter wrap, and always returns a positive
-    number. This means it can be used to measure periods up to about 17.8 minutes.
-
-    Example::
-
-        start = pyb.micros()
-        while pyb.elapsed_micros(start) < 1000:
-            # Perform some operation
-            pass
-    """
-    ...
-
-def freq(sysclk=0, hclk=0, pclk1=0, pclk2=0) -> Tuple:
-    """
-    If given no arguments, returns a tuple of clock frequencies:
-    (sysclk, hclk, pclk1, pclk2).
-    These correspond to:
-
-     - sysclk: frequency of the CPU
-     - hclk: frequency of the AHB bus, core memory and DMA
-     - pclk1: frequency of the APB1 bus
-     - pclk2: frequency of the APB2 bus
-
-    If given any arguments then the function sets the frequency of the CPU,
-    and the buses if additional arguments are given.  Frequencies are given in
-    Hz.  Eg freq(120000000) sets sysclk (the CPU frequency) to 120MHz.  Note that
-    not all values are supported and the largest supported frequency not greater
-    than the given value will be selected.
-
-    Supported sysclk frequencies are (in MHz): 8, 16, 24, 30, 32, 36, 40, 42, 48,
-    54, 56, 60, 64, 72, 84, 96, 108, 120, 144, 168.
-
-    The maximum frequency of hclk is 168MHz, of pclk1 is 42MHz, and of pclk2 is
-    84MHz.  Be sure not to set frequencies above these values.
-
-    The hclk, pclk1 and pclk2 frequencies are derived from the sysclk frequency
-    using a prescaler (divider).  Supported prescalers for hclk are: 1, 2, 4, 8,
-    16, 64, 128, 256, 512.  Supported prescalers for pclk1 and pclk2 are: 1, 2,
-    4, 8.  A prescaler will be chosen to best match the requested frequency.
-
-    A sysclk frequency of
-    8MHz uses the HSE (external crystal) directly and 16MHz uses the HSI
-    (internal oscillator) directly.  The higher frequencies use the HSE to
-    drive the PLL (phase locked loop), and then use the output of the PLL.
-
-    Note that if you change the frequency while the USB is enabled then
-    the USB may become unreliable.  It is best to change the frequency
-    in boot.py, before the USB peripheral is started.  Also note that sysclk
-    frequencies below 36MHz do not allow the USB to function correctly.
-    """
-    ...
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state: ``False``/``True`` for disabled/enabled IRQs
-    respectively.  This return value can be passed to enable_irq to restore
-    the IRQ to its original state.
-    """
-    ...
-
-def fault_debug(value) -> None:
-    """
-    Enable or disable hard-fault debugging.  A hard-fault is when there is a fatal
-    error in the underlying system, like an invalid memory access.
-
-    If the *value* argument is ``False`` then the board will automatically reset if
-    there is a hard fault.
-
-    If *value* is ``True`` then, when the board has a hard fault, it will print the
-    registers and the stack trace, and then cycle the LEDs indefinitely.
-
-    The default value is disabled, i.e. to automatically reset.
-    """
-    ...
-
-def elapsed_millis(start) -> int:
-    """
-    Returns the number of milliseconds which have elapsed since ``start``.
-
-    This function takes care of counter wrap, and always returns a positive
-    number. This means it can be used to measure periods up to about 12.4 days.
-
-    Example::
-
-        start = pyb.millis()
-        while pyb.elapsed_millis(start) < 1000:
-            # Perform some operation
-    """
-    ...
-
-def enable_irq(state=True) -> None:
-    """
-    Enable interrupt requests.
-    If ``state`` is ``True`` (the default value) then IRQs are enabled.
-    If ``state`` is ``False`` then IRQs are disabled.  The most common use of
-    this function is to pass it the value returned by ``disable_irq`` to
-    exit a critical section.
-    """
-    ...
-
-def sync() -> None:
-    """
-    Sync all file systems.
-    """
-    ...
-
-def servo(*args, **kwargs) -> Any: ...
-def standby() -> Any:
-    """
-    Put the pyboard into a "deep sleep" state.
-
-    This reduces power consumption to less than 50 uA.  To wake from this
-    sleep state requires a real-time-clock event, or an external interrupt
-    on X1 (PA0=WKUP) or X18 (PC13=TAMP1).
-    Upon waking the system undergoes a hard reset.
-
-    See :meth:`rtc.wakeup` to configure a real-time-clock wakeup event.
-    """
-    ...
-
-def usb_mode(modestr: Optional[Any] = None, port=-1, vid=0xF055, pid=-1, msc=(), hid=hid_mouse, high_speed=False) -> str:
-    """
-    If called with no arguments, return the current USB mode as a string.
-
-    If called with *modestr* provided, attempts to configure the USB mode.
-    The following values of *modestr* are understood:
-
-    - ``None``: disables USB
-    - ``'VCP'``: enable with VCP (Virtual COM Port) interface
-    - ``'MSC'``: enable with MSC (mass storage device class) interface
-    - ``'VCP+MSC'``: enable with VCP and MSC
-    - ``'VCP+HID'``: enable with VCP and HID (human interface device)
-    - ``'VCP+MSC+HID'``: enabled with VCP, MSC and HID (only available on PYBD boards)
-
-    For backwards compatibility, ``'CDC'`` is understood to mean
-    ``'VCP'`` (and similarly for ``'CDC+MSC'`` and ``'CDC+HID'``).
-
-    The *port* parameter should be an integer (0, 1, ...) and selects which
-    USB port to use if the board supports multiple ports.  A value of -1 uses
-    the default or automatically selected port.
-
-    The *vid* and *pid* parameters allow you to specify the VID (vendor id)
-    and PID (product id).  A *pid* value of -1 will select a PID based on the
-    value of *modestr*.
-
-    If enabling MSC mode, the *msc* parameter can be used to specify a list
-    of SCSI LUNs to expose on the mass storage interface.  For example
-    ``msc=(pyb.Flash(), pyb.SDCard())``.
-
-    If enabling HID mode, you may also specify the HID details by
-    passing the *hid* keyword parameter.  It takes a tuple of
-    (subclass, protocol, max packet length, polling interval, report
-    descriptor).  By default it will set appropriate values for a USB
-    mouse.  There is also a ``pyb.hid_keyboard`` constant, which is an
-    appropriate tuple for a USB keyboard.
-
-    The *high_speed* parameter, when set to ``True``, enables USB HS mode if
-    it is supported by the hardware.
-    """
-    ...
-
-def udelay(us) -> None:
-    """
-    Delay for the given number of microseconds.
-    """
-    ...
-
-def unique_id() -> str:
-    """
-    Returns a string of 12 bytes (96 bits), which is the unique ID of the MCU.
-    """
-    ...
-
-def micros() -> int:
-    """
-    Returns the number of microseconds since the board was last reset.
-
-    The result is always a MicroPython smallint (31-bit signed number), so
-    after 2^30 microseconds (about 17.8 minutes) this will start to return
-    negative numbers.
-
-    Note that if :meth:`pyb.stop()` is issued the hardware counter supporting this
-    function will pause for the duration of the "sleeping" state. This
-    will affect the outcome of :meth:`pyb.elapsed_micros()`.
-    """
-    ...
-
-def mount(device, mountpoint, *, readonly=False, mkfs=False) -> int:
-    """
-    ``Note:`` This function is deprecated. Mounting and unmounting devices should
-       be performed by :meth:`os.mount` and :meth:`os.umount` instead.
-
-    Mount a block device and make it available as part of the filesystem.
-    ``device`` must be an object that provides the block protocol. (The
-    following is also deprecated. See :class:`os.AbstractBlockDev` for the
-    correct way to create a block device.)
-
-     - ``readblocks(self, blocknum, buf)``
-     - ``writeblocks(self, blocknum, buf)`` (optional)
-     - ``count(self)``
-     - ``sync(self)`` (optional)
-
-    ``readblocks`` and ``writeblocks`` should copy data between ``buf`` and
-    the block device, starting from block number ``blocknum`` on the device.
-    ``buf`` will be a bytearray with length a multiple of 512.  If
-    ``writeblocks`` is not defined then the device is mounted read-only.
-    The return value of these two functions is ignored.
-
-    ``count`` should return the number of blocks available on the device.
-    ``sync``, if implemented, should sync the data on the device.
-
-    The parameter ``mountpoint`` is the location in the root of the filesystem
-    to mount the device.  It must begin with a forward-slash.
-
-    If ``readonly`` is ``True``, then the device is mounted read-only,
-    otherwise it is mounted read-write.
-
-    If ``mkfs`` is ``True``, then a new filesystem is created if one does not
-    already exist.
-    """
-    ...
-
-def rng() -> int:
-    """
-    Return a 30-bit hardware generated random number.
-    """
-    ...
-
-def millis() -> int:
-    """
-    Returns the number of milliseconds since the board was last reset.
-
-    The result is always a MicroPython smallint (31-bit signed number), so
-    after 2^30 milliseconds (about 12.4 days) this will start to return
-    negative numbers.
-
-    Note that if :meth:`pyb.stop()` is issued the hardware counter supporting this
-    function will pause for the duration of the "sleeping" state. This
-    will affect the outcome of :meth:`pyb.elapsed_millis()`.
-    """
-    ...
-
-def repl_uart(uart) -> UART:
-    """
-    Get or set the UART object where the REPL is repeated on.
-    """
-    ...
-
-def pwm(*args, **kwargs) -> Any: ...
-def repl_info(*args, **kwargs) -> Any: ...
-def wfi() -> None:
-    """
-    Wait for an internal or external interrupt.
-
-    This executes a ``wfi`` instruction which reduces power consumption
-    of the MCU until any interrupt occurs (be it internal or external),
-    at which point execution continues.  Note that the system-tick interrupt
-    occurs once every millisecond (1000Hz) so this function will block for
-    at most 1ms.
-    """
-    ...
-
-def stop() -> Any:
-    """
-    Put the pyboard in a "sleeping" state.
-
-    This reduces power consumption to less than 500 uA.  To wake from this
-    sleep state requires an external interrupt or a real-time-clock event.
-    Upon waking execution continues where it left off.
-
-    See :meth:`rtc.wakeup` to configure a real-time-clock wakeup event.
-    """
-    ...
-
-def delay(ms) -> None:
-    """
-    Delay for the given number of milliseconds.
-    """
-    ...
-
-def main(filename) -> None:
-    """
-    Set the filename of the main script to run after boot.py is finished.  If
-    this function is not called then the default file main.py will be executed.
-
-    It only makes sense to call this function from within boot.py.
-    """
-    ...
-
-def bootloader() -> None:
-    """
-    Activate the bootloader without BOOT* pins.
-    """
-    ...
-
-def country(*args, **kwargs) -> Any: ...
-
-class ADCAll:
-    def read_core_vbat(self, *args, **kwargs) -> Any: ...
-    def read_core_vref(self, *args, **kwargs) -> Any: ...
-    def read_vref(self, *args, **kwargs) -> Any: ...
-    def read_core_temp(self, *args, **kwargs) -> Any: ...
-    def read_channel(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
-
-class Accel:
-    """
-    Create and return an accelerometer object.
-    """
-
-    def x(self) -> Any:
-        """
-        Get the x-axis value.
-        """
-        ...
-    def tilt(self) -> Any:
-        """
-        Get the tilt register.
-        """
-        ...
-    def y(self) -> Any:
-        """
-        Get the y-axis value.
-        """
-        ...
-    def z(self) -> Any:
-        """
-        Get the z-axis value.
-        """
-        ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def filtered_xyz(self) -> Tuple:
-        """
-        Get a 3-tuple of filtered x, y and z values.
-
-        Implementation note: this method is currently implemented as taking the
-        sum of 4 samples, sampled from the 3 previous calls to this function along
-        with the sample from the current call.  Returned values are therefore 4
-        times the size of what they would be from the raw x(), y() and z() calls.
-        """
-        ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self) -> None: ...
-
-class CAN:
-    """
-    Construct a CAN object on the given bus.  *bus* can be 1-2, or ``'YA'`` or ``'YB'``.
-    With no additional parameters, the CAN object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See :meth:`CAN.init` for parameters of initialisation.
-
-    The physical pins of the CAN buses are:
-
-      - ``CAN(1)`` is on ``YA``: ``(RX, TX) = (Y3, Y4) = (PB8, PB9)``
-      - ``CAN(2)`` is on ``YB``: ``(RX, TX) = (Y5, Y6) = (PB12, PB13)``
-    """
-
-    MASK16: int
-    MASK32: int
-    LOOPBACK: int
-    LIST32: int
-    SILENT_LOOPBACK: int
-    NORMAL: int
-    SILENT: int
-    STOPPED: int
-    ERROR_ACTIVE: int
-    BUS_OFF: int
-    LIST16: int
-    ERROR_PASSIVE: int
-    ERROR_WARNING: int
-    def restart(self) -> Any:
-        """
-        Force a software restart of the CAN controller without resetting its
-        configuration.
-
-        If the controller enters the bus-off state then it will no longer participate
-        in bus activity.  If the controller is not configured to automatically restart
-        (see :meth:`~CAN.init()`) then this method can be used to trigger a restart,
-        and the controller will follow the CAN protocol to leave the bus-off state and
-        go into the error active state.
-        """
-        ...
-    def recv(self, fifo, list=None, *, timeout=5000) -> Tuple:
-        """
-        Receive data on the bus:
-
-          - *fifo* is an integer, which is the FIFO to receive on
-          - *list* is an optional list object to be used as the return value
-          - *timeout* is the timeout in milliseconds to wait for the receive.
-
-        Return value: A tuple containing five values.
-
-          - The id of the message.
-          - A boolean that indicates if the message ID is standard or extended.
-          - A boolean that indicates if the message is an RTR message.
-          - The FMI (Filter Match Index) value.
-          - An array containing the data.
-
-        If *list* is ``None`` then a new tuple will be allocated, as well as a new
-        bytes object to contain the data (as the fifth element in the tuple).
-
-        If *list* is not ``None`` then it should be a list object with a least five
-        elements.  The fifth element should be a memoryview object which is created
-        from either a bytearray or an array of type 'B' or 'b', and this array must
-        have enough room for at least 8 bytes.  The list object will then be
-        populated with the first four return values above, and the memoryview object
-        will be resized inplace to the size of the data and filled in with that data.
-        The same list and memoryview objects can be reused in subsequent calls to
-        this method, providing a way of receiving data without using the heap.
-        For example::
-
-             buf = bytearray(8)
-             lst = [0, 0, 0, memoryview(buf)]
-             # No heap memory is allocated in the following call
-             can.recv(0, lst)
-        """
-        ...
-    def init(
-        self,
-        mode,
-        prescaler=100,
-        *,
-        sjw=1,
-        bs1=6,
-        bs2=8,
-        auto_restart=False,
-        baudrate=0,
-        sample_point=75,
-        num_filter_banks=14,
-        brs_sjw=1,
-        brs_bs1=8,
-        brs_bs2=3,
-        brs_baudrate=0,
-        brs_sample_point=75,
-    ) -> None:
-        """
-        Initialise the CAN bus with the given parameters:
-
-          - *mode* is one of:  NORMAL, LOOPBACK, SILENT, SILENT_LOOPBACK
-          - *prescaler* is the value by which the CAN input clock is divided to generate the
-            nominal bit time quanta. The prescaler can be a value between 1 and 1024 inclusive
-            for classic CAN, and between 1 and 512 inclusive for CAN FD.
-          - *sjw* is the resynchronisation jump width in units of time quanta for nominal bits;
-            it can be a value between 1 and 4 inclusive for classic CAN, and between 1 and 128 inclusive for CAN FD.
-          - *bs1* defines the location of the sample point in units of the time quanta for nominal bits;
-            it can be a value between 1 and 16 inclusive for classic CAN, and between 2 and 256 inclusive for CAN FD.
-          - *bs2* defines the location of the transmit point in units of the time quanta for nominal bits;
-            it can be a value between 1 and 8 inclusive for classic CAN, and between 2 and 128 inclusive for CAN FD.
-          - *auto_restart* sets whether the controller will automatically try and restart
-            communications after entering the bus-off state; if this is disabled then
-            :meth:`~CAN.restart()` can be used to leave the bus-off state
-          - *baudrate* if a baudrate other than 0 is provided, this function will try to automatically
-            calculate the CAN nominal bit time (overriding *prescaler*, *bs1* and *bs2*) that satisfies
-            both the baudrate and the desired *sample_point*.
-          - *sample_point* given in a percentage of the nominal bit time, the *sample_point* specifies the position
-            of the bit sample with respect to the whole nominal bit time. The default *sample_point* is 75%.
-          - *num_filter_banks* for classic CAN, this is the number of banks that will be assigned to CAN(1),
-            the rest of the 28 are assigned to CAN(2).
-          - *brs_prescaler* is the value by which the CAN FD input clock is divided to generate the
-            data bit time quanta. The prescaler can be a value between 1 and 32 inclusive.
-          - *brs_sjw* is the resynchronisation jump width in units of time quanta for data bits;
-            it can be a value between 1 and 16 inclusive
-          - *brs_bs1* defines the location of the sample point in units of the time quanta for data bits;
-            it can be a value between 1 and 32 inclusive
-          - *brs_bs2* defines the location of the transmit point in units of the time quanta for data bits;
-            it can be a value between 1 and 16 inclusive
-          - *brs_baudrate* if a baudrate other than 0 is provided, this function will try to automatically
-            calculate the CAN data bit time (overriding *brs_prescaler*, *brs_bs1* and *brs_bs2*) that satisfies
-            both the baudrate and the desired *brs_sample_point*.
-          - *brs_sample_point* given in a percentage of the data bit time, the *brs_sample_point* specifies the position
-            of the bit sample with respect to the whole data bit time. The default *brs_sample_point* is 75%.
-
-
-        The time quanta tq is the basic unit of time for the CAN bus.  tq is the CAN
-        prescaler value divided by PCLK1 (the frequency of internal peripheral bus 1);
-        see :meth:`pyb.freq()` to determine PCLK1.
-
-        A single bit is made up of the synchronisation segment, which is always 1 tq.
-        Then follows bit segment 1, then bit segment 2.  The sample point is after bit
-        segment 1 finishes.  The transmit point is after bit segment 2 finishes.
-        The baud rate will be 1/bittime, where the bittime is 1 + BS1 + BS2 multiplied
-        by the time quanta tq.
-
-        For example, with PCLK1=42MHz, prescaler=100, sjw=1, bs1=6, bs2=8, the value of
-        tq is 2.38 microseconds.  The bittime is 35.7 microseconds, and the baudrate
-        is 28kHz.
-
-        See page 680 of the STM32F405 datasheet for more details.
-        """
-        ...
-    def rxcallback(self, fifo, fun) -> None:
-        """
-        Register a function to be called when a message is accepted into a empty fifo:
-
-        - *fifo* is the receiving fifo.
-        - *fun* is the function to be called when the fifo becomes non empty.
-
-        The callback function takes two arguments the first is the can object it self the second is
-        a integer that indicates the reason for the callback.
-
-        +--------+------------------------------------------------+
-        | Reason |                                                |
-        +========+================================================+
-        | 0      | A message has been accepted into a empty FIFO. |
-        +--------+------------------------------------------------+
-        | 1      | The FIFO is full                               |
-        +--------+------------------------------------------------+
-        | 2      | A message has been lost due to a full FIFO     |
-        +--------+------------------------------------------------+
-
-        Example use of rxcallback::
-
-          def cb0(bus, reason):
-            print('cb0')
-            if reason == 0:
-                print('pending')
-            if reason == 1:
-                print('full')
-            if reason == 2:
-                print('overflow')
-
-          can = CAN(1, CAN.LOOPBACK)
-          can.rxcallback(0, cb0)
-        """
-        ...
-    def setfilter(self, bank, mode, fifo, params, *, rtr=None, extframe=False) -> None:
-        """
-        Configure a filter bank:
-
-        - *bank* is the classic CAN controller filter bank, or CAN FD filter index, to configure.
-        - *mode* is the mode the filter should operate in, see the tables below.
-        - *fifo* is which fifo (0 or 1) a message should be stored in, if it is accepted by this filter.
-        - *params* is an array of values the defines the filter. The contents of the array depends on the *mode* argument.
-
-        +-----------+---------------------------------------------------------+
-        |*mode*     |Contents of *params* array for classic CAN controller    |
-        +===========+=========================================================+
-        |CAN.LIST16 |Four 16 bit ids that will be accepted                    |
-        +-----------+---------------------------------------------------------+
-        |CAN.LIST32 |Two 32 bit ids that will be accepted                     |
-        +-----------+---------------------------------------------------------+
-        |CAN.MASK16 |Two 16 bit id/mask pairs. E.g. (1, 3, 4, 4)              |
-        |           | | The first pair, 1 and 3 will accept all ids           |
-        |           | | that have bit 0 = 1 and bit 1 = 0.                    |
-        |           | | The second pair, 4 and 4, will accept all ids         |
-        |           | | that have bit 2 = 1.                                  |
-        +-----------+---------------------------------------------------------+
-        |CAN.MASK32 |As with CAN.MASK16 but with only one 32 bit id/mask pair.|
-        +-----------+---------------------------------------------------------+
-
-        +-----------+---------------------------------------------------------+
-        |*mode*     |Contents of *params* array for CAN FD controller         |
-        +===========+=========================================================+
-        |CAN.RANGE  |Two ids that represent a range of accepted ids.          |
-        +-----------+---------------------------------------------------------+
-        |CAN.DUAL   |Two ids that will be accepted. For example (1, 2)        |
-        +-----------+---------------------------------------------------------+
-        |CAN.MASK   |One filter ID and a mask. For example (0x111, 0x7FF)     |
-        +-----------+---------------------------------------------------------+
-
-        - *rtr* For classic CAN controllers, this is an array of booleans that states if
-          a filter should accept a remote transmission request message. If this argument
-          is not given then it defaults to ``False`` for all entries. The length of the
-          array depends on the *mode* argument. For CAN FD, this argument is ignored.
-
-        +-----------+----------------------+
-        |*mode*     |length of *rtr* array |
-        +===========+======================+
-        |CAN.LIST16 |4                     |
-        +-----------+----------------------+
-        |CAN.LIST32 |2                     |
-        +-----------+----------------------+
-        |CAN.MASK16 |2                     |
-        +-----------+----------------------+
-        |CAN.MASK32 |1                     |
-        +-----------+----------------------+
-
-        - *extframe* If True the frame will have an extended identifier (29 bits),
-          otherwise a standard identifier (11 bits) is used.
-
-        """
-        ...
-    def state(self) -> Any:
-        """
-        Return the state of the controller.  The return value can be one of:
-
-        - ``CAN.STOPPED`` -- the controller is completely off and reset;
-        - ``CAN.ERROR_ACTIVE`` -- the controller is on and in the Error Active state
-          (both TEC and REC are less than 96);
-        - ``CAN.ERROR_WARNING`` -- the controller is on and in the Error Warning state
-          (at least one of TEC or REC is 96 or greater);
-        - ``CAN.ERROR_PASSIVE`` -- the controller is on and in the Error Passive state
-          (at least one of TEC or REC is 128 or greater);
-        - ``CAN.BUS_OFF`` -- the controller is on but not participating in bus activity
-          (TEC overflowed beyond 255).
-        """
-        ...
-    def send(self, data, id, *, timeout=0, rtr=False, extframe=False, fdf=False, brs=False) -> None:
-        """
-        Send a message on the bus:
-
-          - *data* is the data to send (an integer to send, or a buffer object).
-          - *id* is the id of the message to be sent.
-          - *timeout* is the timeout in milliseconds to wait for the send.
-          - *rtr* is a boolean that specifies if the message shall be sent as
-            a remote transmission request.  If *rtr* is True then only the length
-            of *data* is used to fill in the DLC slot of the frame; the actual
-            bytes in *data* are unused.
-          - *extframe* if True the frame will have an extended identifier (29 bits),
-            otherwise a standard identifier (11 bits) is used.
-          - *fdf* for CAN FD controllers, if set to True, the frame will have an FD
-            frame format, which supports data payloads up to 64 bytes.
-          - *brs* for CAN FD controllers, if set to True, the bitrate switching mode
-            is enabled, in which the data phase is transmitted at a differet bitrate.
-            See :meth:`CAN.init` for the data bit timing configuration parameters.
-
-          If timeout is 0 the message is placed in a buffer in one of three hardware
-          buffers and the method returns immediately. If all three buffers are in use
-          an exception is thrown. If timeout is not 0, the method waits until the
-          message is transmitted. If the message can't be transmitted within the
-          specified time an exception is thrown.
-
-        Return value: ``None``.
-        """
-        ...
-    def any(self, fifo) -> bool:
-        """
-        Return ``True`` if any message waiting on the FIFO, else ``False``.
-        """
-        ...
-    def info(self, list: Optional[Any] = None) -> Any:
-        """
-        Get information about the controller's error states and TX and RX buffers.
-        If *list* is provided then it should be a list object with at least 8 entries,
-        which will be filled in with the information.  Otherwise a new list will be
-        created and filled in.  In both cases the return value of the method is the
-        populated list.
-
-        The values in the list are:
-
-        - TEC value
-        - REC value
-        - number of times the controller enterted the Error Warning state (wrapped
-          around to 0 after 65535)
-        - number of times the controller enterted the Error Passive state (wrapped
-          around to 0 after 65535)
-        - number of times the controller enterted the Bus Off state (wrapped
-          around to 0 after 65535)
-        - number of pending TX messages
-        - number of pending RX messages on fifo 0
-        - number of pending RX messages on fifo 1
-        """
-        ...
-    def clearfilter(self, bank, extframe=False) -> None:
-        """
-        Clear and disables a filter bank:
-
-        - *bank* is the classic CAN controller filter bank, or CAN FD filter index, to clear.
-        - *extframe* For CAN FD controllers, if True, clear an extended filter (configured with extframe=True),
-          otherwise the clear a standard identifier (configured with extframe=False).
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Turn off the CAN bus.
-        """
-        ...
-    def __init__(
-        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
-    ) -> None: ...
-
-class ExtInt:
-    """
-    Create an ExtInt object:
-
-      - ``pin`` is the pin on which to enable the interrupt (can be a pin object or any valid pin name).
-      - ``mode`` can be one of:
-        - ``ExtInt.IRQ_RISING`` - trigger on a rising edge;
-        - ``ExtInt.IRQ_FALLING`` - trigger on a falling edge;
-        - ``ExtInt.IRQ_RISING_FALLING`` - trigger on a rising or falling edge.
-      - ``pull`` can be one of:
-        - ``pyb.Pin.PULL_NONE`` - no pull up or down resistors;
-        - ``pyb.Pin.PULL_UP`` - enable the pull-up resistor;
-        - ``pyb.Pin.PULL_DOWN`` - enable the pull-down resistor.
-      - ``callback`` is the function to call when the interrupt triggers.  The
-        callback function must accept exactly 1 argument, which is the line that
-        triggered the interrupt.
-
-    """
-
-    IRQ_FALLING: int
-    IRQ_RISING_FALLING: int
-    IRQ_RISING: int
-    EVT_FALLING: int
-    EVT_RISING_FALLING: int
-    EVT_RISING: int
-    def line(self) -> int:
-        """
-        Return the line number that the pin is mapped to.
-        """
-        ...
-    @classmethod
-    def regs(cls) -> Any:
-        """
-        Dump the values of the EXTI registers.
-
-        """
-        ...
-    def swint(self) -> Any:
-        """
-        Trigger the callback from software.
-
-        """
-        ...
-    def enable(self) -> None:
-        """
-        Enable a disabled interrupt.
-        """
-        ...
-    def disable(self) -> None:
-        """
-        Disable the interrupt associated with the ExtInt object.
-        This could be useful for debouncing.
-        """
-        ...
-    def __init__(self, pin, mode, pull, callback) -> None: ...
-
-class Flash:
-    """
-    Create and return a block device that represents the flash device presented
-    to the USB mass storage interface.
-
-    It includes a virtual partition table at the start, and the actual flash
-    starts at block ``0x100``.
-
-    This constructor is deprecated and will be removed in a future version of MicroPython.
-    """
-
-    def readblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
-    def writeblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
-    def ioctl(self, cmd, arg) -> Any:
-        """
-        These methods implement the simple and :ref:`extended
-        <block-device-interface>` block protocol defined by
-        :class:`os.AbstractBlockDev`.
-        """
-        ...
-    def __init__(self) -> None: ...
-
-class ADC:
-    """
-    Create an ADC object associated with the given pin.
-    This allows you to then read analog values on that pin.
-    """
-
-    def read_timed(self, buf, timer) -> Any:
-        """
-        Read analog values into ``buf`` at a rate set by the ``timer`` object.
-
-        ``buf`` can be bytearray or array.array for example.  The ADC values have
-        12-bit resolution and are stored directly into ``buf`` if its element size is
-        16 bits or greater.  If ``buf`` has only 8-bit elements (eg a bytearray) then
-        the sample resolution will be reduced to 8 bits.
-
-        ``timer`` should be a Timer object, and a sample is read each time the timer
-        triggers.  The timer must already be initialised and running at the desired
-        sampling frequency.
-
-        To support previous behaviour of this function, ``timer`` can also be an
-        integer which specifies the frequency (in Hz) to sample at.  In this case
-        Timer(6) will be automatically configured to run at the given frequency.
-
-        Example using a Timer object (preferred way)::
-
-            adc = pyb.ADC(pyb.Pin.board.X19)    # create an ADC on pin X19
-            tim = pyb.Timer(6, freq=10)         # create a timer running at 10Hz
-            buf = bytearray(100)                # creat a buffer to store the samples
-            adc.read_timed(buf, tim)            # sample 100 values, taking 10s
-
-        Example using an integer for the frequency::
-
-            adc = pyb.ADC(pyb.Pin.board.X19)    # create an ADC on pin X19
-            buf = bytearray(100)                # create a buffer of 100 bytes
-            adc.read_timed(buf, 10)             # read analog values into buf at 10Hz
-                                                #   this will take 10 seconds to finish
-            for val in buf:                     # loop over all values
-                print(val)                      # print the value out
-
-        This function does not allocate any heap memory. It has blocking behaviour:
-        it does not return to the calling program until the buffer is full.
-        """
-        ...
-    def read_timed_multi(self, adcs, bufs, timer) -> bool:
-        """
-        This is a static method. It can be used to extract relative timing or
-        phase data from multiple ADC's.
-
-        It reads analog values from multiple ADC's into buffers at a rate set by
-        the *timer* object. Each time the timer triggers a sample is rapidly
-        read from each ADC in turn.
-
-        ADC and buffer instances are passed in tuples with each ADC having an
-        associated buffer. All buffers must be of the same type and length and
-        the number of buffers must equal the number of ADC's.
-
-        Buffers can be ``bytearray`` or ``array.array`` for example. The ADC values
-        have 12-bit resolution and are stored directly into the buffer if its element
-        size is 16 bits or greater.  If buffers have only 8-bit elements (eg a
-        ``bytearray``) then the sample resolution will be reduced to 8 bits.
-
-        *timer* must be a Timer object. The timer must already be initialised
-        and running at the desired sampling frequency.
-
-        Example reading 3 ADC's::
-
-            adc0 = pyb.ADC(pyb.Pin.board.X1)    # Create ADC's
-            adc1 = pyb.ADC(pyb.Pin.board.X2)
-            adc2 = pyb.ADC(pyb.Pin.board.X3)
-            tim = pyb.Timer(8, freq=100)        # Create timer
-            rx0 = array.array('H', (0 for i in range(100))) # ADC buffers of
-            rx1 = array.array('H', (0 for i in range(100))) # 100 16-bit words
-            rx2 = array.array('H', (0 for i in range(100)))
-            # read analog values into buffers at 100Hz (takes one second)
-            pyb.ADC.read_timed_multi((adc0, adc1, adc2), (rx0, rx1, rx2), tim)
-            for n in range(len(rx0)):
-                print(rx0[n], rx1[n], rx2[n])
-
-        This function does not allocate any heap memory. It has blocking behaviour:
-        it does not return to the calling program until the buffers are full.
-
-        The function returns ``True`` if all samples were acquired with correct
-        timing. At high sample rates the time taken to acquire a set of samples
-        can exceed the timer period. In this case the function returns ``False``,
-        indicating a loss of precision in the sample interval. In extreme cases
-        samples may be missed.
-
-        The maximum rate depends on factors including the data width and the
-        number of ADC's being read. In testing two ADC's were sampled at a timer
-        rate of 210kHz without overrun. Samples were missed at 215kHz.  For three
-        ADC's the limit is around 140kHz, and for four it is around 110kHz.
-        At high sample rates disabling interrupts for the duration can reduce the
-        risk of sporadic data loss.
-        """
-        ...
-    def read(self) -> Any:
-        """
-        Read the value on the analog pin and return it.  The returned value
-        will be between 0 and 4095.
-        """
-        ...
-    def __init__(self, pin) -> None: ...
-
-SD: Any
-
-class DAC:
-    """
-    Construct a new DAC object.
-
-    ``port`` can be a pin object, or an integer (1 or 2).
-    DAC(1) is on pin X5 and DAC(2) is on pin X6.
-
-    ``bits`` is an integer specifying the resolution, and can be 8 or 12.
-    The maximum value for the write and write_timed methods will be
-    2**``bits``-1.
-
-    The *buffering* parameter selects the behaviour of the DAC op-amp output
-    buffer, whose purpose is to reduce the output impedance.  It can be
-    ``None`` to select the default (buffering enabled for :meth:`DAC.noise`,
-    :meth:`DAC.triangle` and :meth:`DAC.write_timed`, and disabled for
-    :meth:`DAC.write`), ``False`` to disable buffering completely, or ``True``
-    to enable output buffering.
-
-    When buffering is enabled the DAC pin can drive loads down to 5KΩ.
-    Otherwise it has an output impedance of 15KΩ maximum: consequently
-    to achieve a 1% accuracy without buffering requires the applied load
-    to be less than 1.5MΩ.  Using the buffer incurs a penalty in accuracy,
-    especially near the extremes of range.
-    """
-
-    CIRCULAR: int
-    NORMAL: int
-    def noise(self, freq) -> None:
-        """
-        Generate a pseudo-random noise signal.  A new random sample is written
-        to the DAC output at the given frequency.
-        """
-        ...
-    def write_timed(self, data, freq, *, mode=NORMAL) -> Any:
-        """
-        Initiates a burst of RAM to DAC using a DMA transfer.
-        The input data is treated as an array of bytes in 8-bit mode, and
-        an array of unsigned half-words (array typecode 'H') in 12-bit mode.
-
-        ``freq`` can be an integer specifying the frequency to write the DAC
-        samples at, using Timer(6).  Or it can be an already-initialised
-        Timer object which is used to trigger the DAC sample.  Valid timers
-        are 2, 4, 5, 6, 7 and 8.
-
-        ``mode`` can be ``DAC.NORMAL`` or ``DAC.CIRCULAR``.
-
-        Example using both DACs at the same time::
-
-          dac1 = DAC(1)
-          dac2 = DAC(2)
-          dac1.write_timed(buf1, pyb.Timer(6, freq=100), mode=DAC.CIRCULAR)
-          dac2.write_timed(buf2, pyb.Timer(7, freq=200), mode=DAC.CIRCULAR)
-        """
-        ...
-    def triangle(self, freq) -> None:
-        """
-        Generate a triangle wave.  The value on the DAC output changes at the given
-        frequency and ramps through the full 12-bit range (up and down). Therefore
-        the frequency of the repeating triangle wave itself is 8192 times smaller.
-        """
-        ...
-    def write(self, value) -> Any:
-        """
-        Direct access to the DAC output.  The minimum value is 0.  The maximum
-        value is 2**``bits``-1, where ``bits`` is set when creating the DAC
-        object or by using the ``init`` method.
-        """
-        ...
-    def init(self, bits=8, *, buffering=None) -> Any:
-        """
-        Reinitialise the DAC.  *bits* can be 8 or 12.  *buffering* can be
-        ``None``, ``False`` or ``True``; see above constructor for the meaning
-        of this parameter.
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        De-initialise the DAC making its pin available for other uses.
-        """
-        ...
-    def __init__(self, port, bits=8, *, buffering=None) -> None: ...
-
-class RTC:
-    """
-    Create an RTC object.
-
-    """
-
-    def info(self) -> Any:
-        """
-        Get information about the startup time and reset source.
-
-         - The lower 0xffff are the number of milliseconds the RTC took to
-           start up.
-         - Bit 0x10000 is set if a power-on reset occurred.
-         - Bit 0x20000 is set if an external reset occurred
-        """
-        ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def wakeup(self, timeout, callback=None) -> None:
-        """
-        Set the RTC wakeup timer to trigger repeatedly at every ``timeout``
-        milliseconds.  This trigger can wake the pyboard from both the sleep
-        states: :meth:`pyb.stop` and :meth:`pyb.standby`.
-
-        If ``timeout`` is ``None`` then the wakeup timer is disabled.
-
-        If ``callback`` is given then it is executed at every trigger of the
-        wakeup timer.  ``callback`` must take exactly one argument.
-        """
-        ...
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time (and ``subseconds`` is reset to 255).
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        ``weekday`` is 1-7 for Monday through Sunday.
-
-        ``subseconds`` counts down from 255 to 0
-        """
-        ...
-    def calibration(self, cal) -> int:
-        """
-        Get or set RTC calibration.
-
-        With no arguments, ``calibration()`` returns the current calibration
-        value, which is an integer in the range [-511 : 512].  With one
-        argument it sets the RTC calibration.
-
-        The RTC Smooth Calibration mechanism adjusts the RTC clock rate by
-        adding or subtracting the given number of ticks from the 32768 Hz
-        clock over a 32 second period (corresponding to 2^20 clock ticks.)
-        Each tick added will speed up the clock by 1 part in 2^20, or 0.954
-        ppm; likewise the RTC clock it slowed by negative values. The
-        usable calibration range is:
-        (-511 * 0.954) ~= -487.5 ppm up to (512 * 0.954) ~= 488.5 ppm
-        """
-        ...
-    def __init__(self) -> None: ...
-
-class USB_VCP:
-    """
-    Create a new USB_VCP object.  The *id* argument specifies which USB VCP port to
-    use.
-
-    """
-
-    RTS: int
-    CTS: int
-    IRQ_RX: int
-    def readlines(self) -> List:
-        """
-        Read as much data as possible from the serial device, breaking it into
-        lines.
-
-        Returns a list of bytes objects, each object being one of the lines.
-        Each line will include the newline character.
-        """
-        ...
-    def recv(self, data, *, timeout=5000) -> int:
-        """
-        Receive data on the bus:
-
-          - ``data`` can be an integer, which is the number of bytes to receive,
-            or a mutable buffer, which will be filled with received bytes.
-          - ``timeout`` is the timeout in milliseconds to wait for the receive.
-
-        Return value: if ``data`` is an integer then a new buffer of the bytes received,
-        otherwise the number of bytes read into ``data`` is returned.
-        """
-        ...
-    def isconnected(self) -> bool:
-        """
-        Return ``True`` if USB is connected as a serial device, else ``False``.
-        """
-        ...
-    def init(self, *, flow=-1) -> None:
-        """
-        Configure the USB VCP port.  If the *flow* argument is not -1 then the value sets
-        the flow control, which can be a bitwise-or of ``USB_VCP.RTS`` and ``USB_VCP.CTS``.
-        RTS is used to control read behaviour and CTS, to control write behaviour.
-        """
-        ...
-    def irq(self, handler=None, trigger=IRQ_RX, hard=False) -> None:
-        """
-        Register *handler* to be called whenever an event specified by *trigger*
-        occurs.  The *handler* function must take exactly one argument, which will
-        be the USB VCP object.  Pass in ``None`` to disable the callback.
-
-        Valid values for *trigger* are:
-
-          - ``USB_VCP.IRQ_RX``: new data is available for reading from the USB VCP object.
-
-        """
-        ...
-    def setinterrupt(self, chr) -> None:
-        """
-        Set the character which interrupts running Python code.  This is set
-        to 3 (CTRL-C) by default, and when a CTRL-C character is received over
-        the USB VCP port, a KeyboardInterrupt exception is raised.
-
-        Set to -1 to disable this interrupt feature.  This is useful when you
-        want to send raw bytes over the USB VCP port.
-        """
-        ...
-    def close(self) -> Any:
-        """
-        This method does nothing.  It exists so the USB_VCP object can act as
-        a file.
-        """
-        ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read at most ``nbytes`` from the serial device and return them as a
-        bytes object.  If ``nbytes`` is not specified then the method reads
-        all available bytes from the serial device.
-        USB_VCP `stream` implicitly works in non-blocking mode,
-        so if no pending data available, this method will return immediately
-        with ``None`` value.
-        """
-        ...
-    def any(self) -> bool:
-        """
-        Return ``True`` if any characters waiting, else ``False``.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from ``buf`` to the serial device.
-
-        Returns the number of bytes written.
-        """
-        ...
-    def send(self, data, *, timeout=5000) -> int:
-        """
-        Send data over the USB VCP:
-
-          - ``data`` is the data to send (an integer to send, or a buffer object).
-          - ``timeout`` is the timeout in milliseconds to wait for the send.
-
-        Return value: number of bytes sent.
-        """
-        ...
-    def readinto(self, buf, maxlen: Optional[Any] = None) -> int:
-        """
-        Read bytes from the serial device and store them into ``buf``, which
-        should be a buffer-like object.  At most ``len(buf)`` bytes are read.
-        If ``maxlen`` is given and then at most ``min(maxlen, len(buf))`` bytes
-        are read.
-
-        Returns the number of bytes read and stored into ``buf`` or ``None``
-        if no pending data available.
-        """
-        ...
-    def readline(self) -> bytes:
-        """
-        Read a whole line from the serial device.
-
-        Returns a bytes object containing the data, including the trailing
-        newline character or ``None`` if no pending data available.
-        """
-        ...
-    def __init__(self, id=0) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given id.  If additional
-    arguments are given, then the timer is initialised by ``init(...)``.
-    ``id`` can be 1 to 14.
-    """
-
-    OC_FORCED_ACTIVE: int
-    OC_FORCED_INACTIVE: int
-    OC_INACTIVE: int
-    OC_ACTIVE: int
-    LOW: int
-    IC: int
-    PWM_INVERTED: int
-    RISING: int
-    OC_TIMING: int
-    PWM: int
-    OC_TOGGLE: int
-    UP: int
-    BRK_LOW: int
-    BRK_OFF: int
-    CENTER: int
-    BRK_HIGH: int
-    BOTH: int
-    HIGH: int
-    ENC_B: int
-    FALLING: int
-    DOWN: int
-    ENC_AB: int
-    ENC_A: int
-    def freq(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the frequency for the timer (changes prescaler and period if set).
-        """
-        ...
-    def init(self, *, freq, prescaler, period, mode=UP, div=1, callback=None, deadtime=0) -> None:
-        """
-        Initialise the timer.  Initialisation must be either by frequency (in Hz)
-        or by prescaler and period::
-
-            tim.init(freq=100)                  # set the timer to trigger at 100Hz
-            tim.init(prescaler=83, period=999)  # set the prescaler and period directly
-
-        Keyword arguments:
-
-          - ``freq`` --- specifies the periodic frequency of the timer. You might also
-            view this as the frequency with which the timer goes through one complete cycle.
-
-          - ``prescaler`` [0-0xffff] - specifies the value to be loaded into the
-            timer's Prescaler Register (PSC). The timer clock source is divided by
-            (``prescaler + 1``) to arrive at the timer clock. Timers 2-7 and 12-14
-            have a clock source of 84 MHz (pyb.freq()[2] * 2), and Timers 1, and 8-11
-            have a clock source of 168 MHz (pyb.freq()[3] * 2).
-
-          - ``period`` [0-0xffff] for timers 1, 3, 4, and 6-15. [0-0x3fffffff] for timers 2 & 5.
-            Specifies the value to be loaded into the timer's AutoReload
-            Register (ARR). This determines the period of the timer (i.e. when the
-            counter cycles). The timer counter will roll-over after ``period + 1``
-            timer clock cycles.
-
-          - ``mode`` can be one of:
-
-            - ``Timer.UP`` - configures the timer to count from 0 to ARR (default)
-            - ``Timer.DOWN`` - configures the timer to count from ARR down to 0.
-            - ``Timer.CENTER`` - configures the timer to count from 0 to ARR and
-              then back down to 0.
-
-          - ``div`` can be one of 1, 2, or 4. Divides the timer clock to determine
-            the sampling clock used by the digital filters.
-
-          - ``callback`` - as per Timer.callback()
-
-          - ``deadtime`` - specifies the amount of "dead" or inactive time between
-            transitions on complimentary channels (both channels will be inactive)
-            for this time). ``deadtime`` may be an integer between 0 and 1008, with
-            the following restrictions: 0-128 in steps of 1. 128-256 in steps of
-            2, 256-512 in steps of 8, and 512-1008 in steps of 16. ``deadtime``
-            measures ticks of ``source_freq`` divided by ``div`` clock ticks.
-            ``deadtime`` is only available on timers 1 and 8.
-
-         You must either specify freq or both of period and prescaler.
-        """
-        ...
-    def period(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the period of the timer.
-        """
-        ...
-    def prescaler(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the prescaler for the timer.
-        """
-        ...
-    def source_freq(self) -> Any:
-        """
-        Get the frequency of the source of the timer.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer.
-
-        Disables the callback (and the associated irq).
-
-        Disables any channel callbacks (and the associated irq).
-        Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def callback(self, fun) -> None:
-        """
-        Set the function to be called when the timer triggers.
-        ``fun`` is passed 1 argument, the timer object.
-        If ``fun`` is ``None`` then the callback will be disabled.
-        """
-        ...
-    def channel(self, channel, mode, pin=None, *args) -> Any:
-        """
-        If only a channel number is passed, then a previously initialized channel
-        object is returned (or ``None`` if there is no previous channel).
-
-        Otherwise, a TimerChannel object is initialized and returned.
-
-        Each channel can be configured to perform pwm, output compare, or
-        input capture. All channels share the same underlying timer, which means
-        that they share the same timer clock.
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.PWM`` --- configure the timer in PWM mode (active high).
-            - ``Timer.PWM_INVERTED`` --- configure the timer in PWM mode (active low).
-            - ``Timer.OC_TIMING`` --- indicates that no pin is driven.
-            - ``Timer.OC_ACTIVE`` --- the pin will be made active when a compare match occurs (active is determined by polarity)
-            - ``Timer.OC_INACTIVE`` --- the pin will be made inactive when a compare match occurs.
-            - ``Timer.OC_TOGGLE`` --- the pin will be toggled when an compare match occurs.
-            - ``Timer.OC_FORCED_ACTIVE`` --- the pin is forced active (compare match is ignored).
-            - ``Timer.OC_FORCED_INACTIVE`` --- the pin is forced inactive (compare match is ignored).
-            - ``Timer.IC`` --- configure the timer in Input Capture mode.
-            - ``Timer.ENC_A`` --- configure the timer in Encoder mode. The counter only changes when CH1 changes.
-            - ``Timer.ENC_B`` --- configure the timer in Encoder mode. The counter only changes when CH2 changes.
-            - ``Timer.ENC_AB`` --- configure the timer in Encoder mode. The counter changes when CH1 or CH2 changes.
-
-          - ``callback`` - as per TimerChannel.callback()
-
-          - ``pin`` None (the default) or a Pin object. If specified (and not None)
-            this will cause the alternate function of the the indicated pin
-            to be configured for this timer channel. An error will be raised if
-            the pin doesn't support any alternate functions for this timer channel.
-
-        Keyword arguments for Timer.PWM modes:
-
-          - ``pulse_width`` - determines the initial pulse width value to use.
-          - ``pulse_width_percent`` - determines the initial pulse width percentage to use.
-
-        Keyword arguments for Timer.OC modes:
-
-          - ``compare`` - determines the initial value of the compare register.
-
-          - ``polarity`` can be one of:
-
-            - ``Timer.HIGH`` - output is active high
-            - ``Timer.LOW`` - output is active low
-
-        Optional keyword arguments for Timer.IC modes:
-
-          - ``polarity`` can be one of:
-
-            - ``Timer.RISING`` - captures on rising edge.
-            - ``Timer.FALLING`` - captures on falling edge.
-            - ``Timer.BOTH`` - captures on both edges.
-
-          Note that capture only works on the primary channel, and not on the
-          complimentary channels.
-
-        Notes for Timer.ENC modes:
-
-          - Requires 2 pins, so one or both pins will need to be configured to use
-            the appropriate timer AF using the Pin API.
-          - Read the encoder value using the timer.counter() method.
-          - Only works on CH1 and CH2 (and not on CH1N or CH2N)
-          - The channel number is ignored when setting the encoder mode.
-
-        PWM Example::
-
-            timer = pyb.Timer(2, freq=1000)
-            ch2 = timer.channel(2, pyb.Timer.PWM, pin=pyb.Pin.board.X2, pulse_width=8000)
-            ch3 = timer.channel(3, pyb.Timer.PWM, pin=pyb.Pin.board.X3, pulse_width=16000)
-        """
-        ...
-    def counter(self, value: Optional[Any] = None) -> Any:
-        """
-        Get or set the timer counter.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class Switch:
-    """
-    Create and return a switch object.
-
-    """
-
-    def callback(self, fun) -> None:
-        """
-        Register the given function to be called when the switch is pressed down.
-        If ``fun`` is ``None``, then it disables the callback.
-        """
-        ...
-    def value(self) -> bool:
-        """
-        Get the switch state.  Returns ``True`` if pressed down, otherwise ``False``.
-        """
-        ...
-    def __init__(self) -> None: ...
-
-class Servo:
-    """
-    Create a servo object.  ``id`` is 1-4, and corresponds to pins X1 through X4.
-
-    """
-
-    def speed(self, speed: Optional[Any] = None, time=0) -> Any:
-        """
-        If no arguments are given, this function returns the current speed.
-
-        If arguments are given, this function sets the speed of the servo:
-
-          - ``speed`` is the speed to change to, between -100 and 100.
-          - ``time`` is the number of milliseconds to take to get to the specified
-            speed.  If omitted, then the servo accelerates as quickly as possible.
-        """
-        ...
-    def pulse_width(self, value: Optional[Any] = None) -> Any:
-        """
-        If no arguments are given, this function returns the current raw pulse-width
-        value.
-
-        If an argument is given, this function sets the raw pulse-width value.
-        """
-        ...
-    def calibration(self, pulse_min, pulse_max, pulse_centre, pulse_angle_90, pulse_speed_100) -> Tuple:
-        """
-        If no arguments are given, this function returns the current calibration
-        data, as a 5-tuple.
-
-        If arguments are given, this function sets the timing calibration:
-
-          - ``pulse_min`` is the minimum allowed pulse width.
-          - ``pulse_max`` is the maximum allowed pulse width.
-          - ``pulse_centre`` is the pulse width corresponding to the centre/zero position.
-          - ``pulse_angle_90`` is the pulse width corresponding to 90 degrees.
-          - ``pulse_speed_100`` is the pulse width corresponding to a speed of 100.
-        """
-        ...
-    def angle(self, angle: Optional[Any] = None, time=0) -> Any:
-        """
-        If no arguments are given, this function returns the current angle.
-
-        If arguments are given, this function sets the angle of the servo:
-
-          - ``angle`` is the angle to move to in degrees.
-          - ``time`` is the number of milliseconds to take to get to the specified
-            angle.  If omitted, then the servo moves as quickly as possible to its
-            new position.
-        """
-        ...
-    def __init__(self, id) -> None: ...
-
-class UART:
-    """
-    Construct a UART object on the given bus.
-    For Pyboard ``bus`` can be 1-4, 6, 'XA', 'XB', 'YA', or 'YB'.
-    For Pyboard Lite ``bus`` can be 1, 2, 6, 'XB', or 'YA'.
-    For Pyboard D ``bus`` can be 1-4, 'XA', 'YA' or 'YB'.
-    With no additional parameters, the UART object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-
-    The physical pins of the UART buses on Pyboard are:
-
-      - ``UART(4)`` is on ``XA``: ``(TX, RX) = (X1, X2) = (PA0, PA1)``
-      - ``UART(1)`` is on ``XB``: ``(TX, RX) = (X9, X10) = (PB6, PB7)``
-      - ``UART(6)`` is on ``YA``: ``(TX, RX) = (Y1, Y2) = (PC6, PC7)``
-      - ``UART(3)`` is on ``YB``: ``(TX, RX) = (Y9, Y10) = (PB10, PB11)``
-      - ``UART(2)`` is on: ``(TX, RX) = (X3, X4) = (PA2, PA3)``
-
-    The Pyboard Lite supports UART(1), UART(2) and UART(6) only, pins are:
-
-      - ``UART(1)`` is on ``XB``: ``(TX, RX) = (X9, X10) = (PB6, PB7)``
-      - ``UART(6)`` is on ``YA``: ``(TX, RX) = (Y1, Y2) = (PC6, PC7)``
-      - ``UART(2)`` is on: ``(TX, RX) = (X1, X2) = (PA2, PA3)``
-
-    The Pyboard D supports UART(1), UART(2), UART(3) and UART(4) only, pins are:
-
-      - ``UART(4)`` is on ``XA``: ``(TX, RX) = (X1, X2) = (PA0, PA1)``
-      - ``UART(1)`` is on ``YA``: ``(TX, RX) = (Y1, Y2) = (PA9, PA10)``
-      - ``UART(3)`` is on ``YB``: ``(TX, RX) = (Y9, Y10) = (PB10, PB11)``
-      - ``UART(2)`` is on: ``(TX, RX) = (X3, X4) = (PA2, PA3)``
-
-    *Note:* Pyboard D has ``UART(1)`` on ``YA``, unlike Pyboard and Pyboard Lite that both
-    have ``UART(1)`` on ``XB`` and ``UART(6)`` on ``YA``.
-    """
-
-    CTS: int
-    RTS: int
-    IRQ_RXIDLE: int
-    def readchar(self) -> int:
-        """
-        Receive a single character on the bus.
-
-        Return value: The character read, as an integer.  Returns -1 on timeout.
-        """
-        ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus.  This drives the bus low for a duration
-        of 13 bits.
-        Return value: ``None``.
-        """
-        ...
-    def irq(self, *args, **kwargs) -> Any: ...
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate, bits=8, parity=None, stop=1, *, timeout=0, flow=0, timeout_char=0, read_buf_len=64) -> Any:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - ``baudrate`` is the clock rate.
-          - ``bits`` is the number of bits per character, 7, 8 or 9.
-          - ``parity`` is the parity, ``None``, 0 (even) or 1 (odd).
-          - ``stop`` is the number of stop bits, 1 or 2.
-          - ``flow`` sets the flow control type. Can be 0, ``UART.RTS``, ``UART.CTS``
-            or ``UART.RTS | UART.CTS``.
-          - ``timeout`` is the timeout in milliseconds to wait for writing/reading the first character.
-          - ``timeout_char`` is the timeout in milliseconds to wait between characters while writing or reading.
-          - ``read_buf_len`` is the character length of the read buffer (0 to disable).
-
-        This method will raise an exception if the baudrate could not be set within
-        5% of the desired value.  The minimum baudrate is dictated by the frequency
-        of the bus that the UART is on; UART(1) and UART(6) are APB2, the rest are on
-        APB1.  The default bus frequencies give a minimum baudrate of 1300 for
-        UART(1) and UART(6) and 650 for the others.  Use :func:`pyb.freq <pyb.freq>`
-        to reduce the bus frequencies to get lower baudrates.
-
-        *Note:* with parity=None, only 8 and 9 bits are supported.  With parity enabled,
-        only 7 and 8 bits are supported.
-        """
-        ...
-    def writechar(self, char) -> None:
-        """
-        Write a single character on the bus.  ``char`` is an integer to write.
-        Return value: ``None``. See note below if CTS flow control is used.
-        """
-        ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes.
-        If ``nbytes`` are available in the buffer, returns immediately, otherwise returns
-        when sufficient characters arrive or the timeout elapses.
-
-        If ``nbytes`` is not given then the method reads as much data as possible.  It
-        returns after the timeout has elapsed.
-
-        *Note:* for 9 bit characters each character takes two bytes, ``nbytes`` must
-        be even, and the number of characters is ``nbytes/2``.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns the number of bytes waiting (may be 0).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.  If characters are 7 or 8 bits wide
-        then each byte is one character.  If characters are 9 bits wide then two
-        bytes are used for each character (little endian), and ``buf`` must contain
-        an even number of bytes.
-
-        Return value: number of bytes written. If a timeout occurs and no bytes
-        were written returns ``None``.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. If such a line exists, return is
-        immediate. If the timeout elapses, all available data is returned regardless
-        of whether a newline exists.
-
-        Return value: the line read or ``None`` on timeout if no data is available.
-        """
-        ...
-    def __init__(
-        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
-    ) -> None: ...
-
-class USB_HID:
-    """
-    Create a new USB_HID object.
-
-    """
-
-    def recv(self, data, *, timeout=5000) -> int:
-        """
-        Receive data on the bus:
-
-          - ``data`` can be an integer, which is the number of bytes to receive,
-            or a mutable buffer, which will be filled with received bytes.
-          - ``timeout`` is the timeout in milliseconds to wait for the receive.
-
-        Return value: if ``data`` is an integer then a new buffer of the bytes received,
-        otherwise the number of bytes read into ``data`` is returned.
-        """
-        ...
-    def send(self, data) -> None:
-        """
-        Send data over the USB HID interface:
-
-          - ``data`` is the data to send (a tuple/list of integers, or a
-            bytearray).
-        """
-        ...
-    def __init__(self) -> None: ...
-
-class I2C:
-    """
-    Construct an I2C object on the given bus.  ``bus`` can be 1 or 2, 'X' or
-    'Y'. With no additional parameters, the I2C object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-
-    The physical pins of the I2C buses on Pyboards V1.0 and V1.1 are:
-
-      - ``I2C(1)`` is on the X position: ``(SCL, SDA) = (X9, X10) = (PB6, PB7)``
-      - ``I2C(2)`` is on the Y position: ``(SCL, SDA) = (Y9, Y10) = (PB10, PB11)``
-
-    On the Pyboard Lite:
-
-      - ``I2C(1)`` is on the X position: ``(SCL, SDA) = (X9, X10) = (PB6, PB7)``
-      - ``I2C(3)`` is on the Y position: ``(SCL, SDA) = (Y9, Y10) = (PA8, PB8)``
-
-    Calling the constructor with 'X' or 'Y' enables portability between Pyboard
-    types.
-    """
-
-    PERIPHERAL: int
-    MASTER: int
-    CONTROLLER: int
-    SLAVE: int
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses from 0x01 to 0x7f and return a list of those that respond.
-        Only valid when in controller mode.
-        """
-        ...
-    def mem_read(self, data, addr, memaddr, *, timeout=5000, addr_size=8) -> Any:
-        """
-        Read from the memory of an I2C device:
-
-          - ``data`` can be an integer (number of bytes to read) or a buffer to read into
-          - ``addr`` is the I2C device address
-          - ``memaddr`` is the memory location within the I2C device
-          - ``timeout`` is the timeout in milliseconds to wait for the read
-          - ``addr_size`` selects width of memaddr: 8 or 16 bits
-
-        Returns the read data.
-        This is only valid in controller mode.
-        """
-        ...
-    def mem_write(self, data, addr, memaddr, *, timeout=5000, addr_size=8) -> None:
-        """
-        Write to the memory of an I2C device:
-
-          - ``data`` can be an integer or a buffer to write from
-          - ``addr`` is the I2C device address
-          - ``memaddr`` is the memory location within the I2C device
-          - ``timeout`` is the timeout in milliseconds to wait for the write
-          - ``addr_size`` selects width of memaddr: 8 or 16 bits
-
-        Returns ``None``.
-        This is only valid in controller mode.
-        """
-        ...
-    def recv(self, recv, addr=0x00, *, timeout=5000) -> bytes:
-        """
-        Receive data on the bus:
-
-          - ``recv`` can be an integer, which is the number of bytes to receive,
-            or a mutable buffer, which will be filled with received bytes
-          - ``addr`` is the address to receive from (only required in controller mode)
-          - ``timeout`` is the timeout in milliseconds to wait for the receive
-
-        Return value: if ``recv`` is an integer then a new buffer of the bytes received,
-        otherwise the same buffer that was passed in to ``recv``.
-        """
-        ...
-    def is_ready(self, addr) -> Any:
-        """
-        Check if an I2C device responds to the given address.  Only valid when in controller mode.
-        """
-        ...
-    def send(self, send, addr=0x00, *, timeout=5000) -> None:
-        """
-        Send data on the bus:
-
-          - ``send`` is the data to send (an integer to send, or a buffer object)
-          - ``addr`` is the address to send to (only required in controller mode)
-          - ``timeout`` is the timeout in milliseconds to wait for the send
-
-        Return value: ``None``.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Turn off the I2C bus.
-        """
-        ...
-    def init(self, mode, *, addr=0x12, baudrate=400000, gencall=False, dma=False) -> None:
-        """
-        Initialise the I2C bus with the given parameters:
-
-           - ``mode`` must be either ``I2C.CONTROLLER`` or ``I2C.PERIPHERAL``
-           - ``addr`` is the 7-bit address (only sensible for a peripheral)
-           - ``baudrate`` is the SCL clock rate (only sensible for a controller)
-           - ``gencall`` is whether to support general call mode
-           - ``dma`` is whether to allow the use of DMA for the I2C transfers (note
-             that DMA transfers have more precise timing but currently do not handle bus
-             errors properly)
-        """
-        ...
-    def __init__(
-        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
-    ) -> None: ...
-
-class LED:
-    """
-    Create an LED object associated with the given LED:
-
-      - ``id`` is the LED number, 1-4.
-
-    """
-
-    def toggle(self) -> Any:
-        """
-        Toggle the LED between on (maximum intensity) and off.  If the LED is at
-        non-zero intensity then it is considered "on" and toggle will turn it off.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Turn the LED on, to maximum intensity.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Turn the LED off.
-        """
-        ...
-    def intensity(self, value: Optional[Any] = None) -> None:
-        """
-        Get or set the LED intensity.  Intensity ranges between 0 (off) and 255 (full on).
-        If no argument is given, return the LED intensity.
-        If an argument is given, set the LED intensity and return ``None``.
-
-        *Note:* Only LED(3) and LED(4) can have a smoothly varying intensity, and
-        they use timer PWM to implement it.  LED(3) uses Timer(2) and LED(4) uses
-        Timer(3).  These timers are only configured for PWM if the intensity of the
-        relevant LED is set to a value between 1 and 254.  Otherwise the timers are
-        free for general purpose use.
-        """
-        ...
-    def __init__(self, id) -> None: ...
-
-class LCD:
-    """
-    Construct an LCD object in the given skin position.  ``skin_position`` can be 'X' or 'Y', and
-    should match the position where the LCD pyskin is plugged in.
-
-    """
-
-    def fill(self, colour) -> None:
-        """
-        Fill the screen with the given colour (0 or 1 for white or black).
-
-        This method writes to the hidden buffer.  Use ``show()`` to show the buffer.
-        """
-        ...
-    def light(self, value) -> None:
-        """
-        Turn the backlight on/off.  True or 1 turns it on, False or 0 turns it off.
-        """
-        ...
-    def pixel(self, x, y, colour) -> None:
-        """
-        Set the pixel at ``(x, y)`` to the given colour (0 or 1).
-
-        This method writes to the hidden buffer.  Use ``show()`` to show the buffer.
-        """
-        ...
-    def show(self) -> None:
-        """
-        Show the hidden buffer on the screen.
-        """
-        ...
-    def text(self, str, x, y, colour) -> None:
-        """
-        Draw the given text to the position ``(x, y)`` using the given colour (0 or 1).
-
-        This method writes to the hidden buffer.  Use ``show()`` to show the buffer.
-        """
-        ...
-    def contrast(self, value) -> None:
-        """
-        Set the contrast of the LCD.  Valid values are between 0 and 47.
-        """
-        ...
-    def get(self, x, y) -> int:
-        """
-        Get the pixel at the position ``(x, y)``.  Returns 0 or 1.
-
-        This method reads from the visible buffer.
-        """
-        ...
-    def write(self, str) -> None:
-        """
-        Write the string ``str`` to the screen.  It will appear immediately.
-        """
-        ...
-    def command(self, instr_data, buf) -> None:
-        """
-        Send an arbitrary command to the LCD.  Pass 0 for ``instr_data`` to send an
-        instruction, otherwise pass 1 to send data.  ``buf`` is a buffer with the
-        instructions/data to send.
-        """
-        ...
-    def __init__(self, skin_position) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus.  ``bus`` can be 1 or 2, or
-    'X' or 'Y'. With no additional parameters, the SPI object is created but
-    not initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-
-    The physical pins of the SPI buses are:
-
-      - ``SPI(1)`` is on the X position: ``(NSS, SCK, MISO, MOSI) = (X5, X6, X7, X8) = (PA4, PA5, PA6, PA7)``
-      - ``SPI(2)`` is on the Y position: ``(NSS, SCK, MISO, MOSI) = (Y5, Y6, Y7, Y8) = (PB12, PB13, PB14, PB15)``
-
-    At the moment, the NSS pin is not used by the SPI driver and is free
-    for other use.
-    """
-
-    MASTER: int
-    LSB: int
-    SLAVE: int
-    MSB: int
-    PERIPHERAL: int
-    CONTROLLER: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def send_recv(self, send, recv=None, *, timeout=5000) -> bytes:
-        """
-        Send and receive data on the bus at the same time:
-
-          - ``send`` is the data to send (an integer to send, or a buffer object).
-          - ``recv`` is a mutable buffer which will be filled with received bytes.
-            It can be the same as ``send``, or omitted.  If omitted, a new buffer will
-            be created.
-          - ``timeout`` is the timeout in milliseconds to wait for the receive.
-
-        Return value: the buffer with the received bytes.
-        """
-        ...
-    def recv(self, recv, *, timeout=5000) -> bytes:
-        """
-        Receive data on the bus:
-
-          - ``recv`` can be an integer, which is the number of bytes to receive,
-            or a mutable buffer, which will be filled with received bytes.
-          - ``timeout`` is the timeout in milliseconds to wait for the receive.
-
-        Return value: if ``recv`` is an integer then a new buffer of the bytes received,
-        otherwise the same buffer that was passed in to ``recv``.
-        """
-        ...
-    def init(self, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``mode`` must be either ``SPI.CONTROLLER`` or ``SPI.PERIPHERAL``.
-          - ``baudrate`` is the SCK clock rate (only sensible for a controller).
-          - ``prescaler`` is the prescaler to use to derive SCK from the APB bus frequency;
-            use of ``prescaler`` overrides ``baudrate``.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` can be 8 or 16, and is the number of bits in each transferred word.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``ti`` True indicates Texas Instruments, as opposed to Motorola, signal conventions.
-          - ``crc`` can be None for no CRC, or a polynomial specifier.
-
-        Note that the SPI clock frequency will not always be the requested baudrate.
-        The hardware only supports baudrates that are the APB bus frequency
-        (see :meth:`pyb.freq`) divided by a prescaler, which can be 2, 4, 8, 16, 32,
-        64, 128 or 256.  SPI(1) is on AHB2, and SPI(2) is on AHB1.  For precise
-        control over the SPI clock frequency, specify ``prescaler`` instead of
-        ``baudrate``.
-
-        Printing the SPI object will show you the computed baudrate and the chosen
-        prescaler.
-        """
-        ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def send(self, send, *, timeout=5000) -> None:
-        """
-        Send data on the bus:
-
-          - ``send`` is the data to send (an integer to send, or a buffer object).
-          - ``timeout`` is the timeout in milliseconds to wait for the send.
-
-        Return value: ``None``.
-        """
-        ...
-    def __init__(
-        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
-    ) -> None: ...
-
-class Pin:
-    """
-    Create a new Pin object associated with the id.  If additional arguments are given,
-    they are used to initialise the pin.  See :meth:`pin.init`.
-    """
-
-    AF_OD: int
-    AF9_TIM14: int
-    ALT_OPEN_DRAIN: int
-    AF_PP: int
-    ALT: int
-    AF9_CAN1: int
-    AF8_USART6: int
-    AF9_TIM13: int
-    AF9_CAN2: int
-    AF9_TIM12: int
-    PULL_UP: int
-    OUT_PP: int
-    OUT_OD: int
-    ANALOG: int
-    PULL_DOWN: int
-    PULL_NONE: int
-    IRQ_FALLING: int
-    IN: int
-    OUT: int
-    IRQ_RISING: int
-    OPEN_DRAIN: int
-    AF2_TIM5: int
-    AF3_TIM10: int
-    AF3_TIM11: int
-    AF3_TIM8: int
-    AF3_TIM9: int
-    AF2_TIM4: int
-    AF1_TIM1: int
-    AF1_TIM2: int
-    AF2_TIM3: int
-    AF8_UART4: int
-    AF6_I2S2: int
-    AF7_USART1: int
-    AF7_USART2: int
-    AF7_USART3: int
-    AF4_I2C1: int
-    AF5_SPI2: int
-    AF4_I2C2: int
-    AF5_I2S2: int
-    AF5_SPI1: int
-    def mode(self) -> Any:
-        """
-        Returns the currently configured mode of the pin. The integer returned
-        will match one of the allowed constants for the mode argument to the init
-        function.
-        """
-        ...
-    def name(self) -> str:
-        """
-        Get the pin name.
-        """
-        ...
-    def pull(self) -> Any:
-        """
-        Returns the currently configured pull of the pin. The integer returned
-        will match one of the allowed constants for the pull argument to the init
-        function.
-        """
-        ...
-    def low(self, *args, **kwargs) -> Any: ...
-    def irq(self, *args, **kwargs) -> Any: ...
-    def pin(self) -> int:
-        """
-        Get the pin number.
-        """
-        ...
-    def port(self) -> Any:
-        """
-        Get the pin port.
-        """
-        ...
-    def names(self) -> str:
-        """
-        Returns the cpu and board names for this pin.
-        """
-        ...
-    def on(self, *args, **kwargs) -> Any: ...
-    def off(self, *args, **kwargs) -> Any: ...
-    def init(self, mode, pull=PULL_NONE, *, value=None, alt=-1) -> None:
-        """
-        Initialise the pin:
-
-          - *mode* can be one of:
-
-             - ``Pin.IN`` - configure the pin for input;
-             - ``Pin.OUT_PP`` - configure the pin for output, with push-pull control;
-             - ``Pin.OUT_OD`` - configure the pin for output, with open-drain control;
-             - ``Pin.AF_PP`` - configure the pin for alternate function, pull-pull;
-             - ``Pin.AF_OD`` - configure the pin for alternate function, open-drain;
-             - ``Pin.ANALOG`` - configure the pin for analog.
-
-          - *pull* can be one of:
-
-             - ``Pin.PULL_NONE`` - no pull up or down resistors;
-             - ``Pin.PULL_UP`` - enable the pull-up resistor;
-             - ``Pin.PULL_DOWN`` - enable the pull-down resistor.
-
-          - *value* if not None will set the port output value before enabling the pin.
-
-          - *alt* can be used when mode is ``Pin.AF_PP`` or ``Pin.AF_OD`` to set the
-            index or name of one of the alternate functions associated with a pin.
-            This arg was previously called *af* which can still be used if needed.
-
-        Returns: ``None``.
-        """
-        ...
-    def af_list(self) -> List:
-        """
-        Returns an array of alternate functions available for this pin.
-        """
-        ...
-    def af(self) -> Any:
-        """
-        Returns the currently configured alternate-function of the pin. The
-        integer returned will match one of the allowed constants for the af
-        argument to the init function.
-        """
-        ...
-    def value(self, value: Optional[Any] = None) -> int:
-        """
-        Get or set the digital logic level of the pin:
-
-          - With no argument, return 0 or 1 depending on the logic level of the pin.
-          - With ``value`` given, set the logic level of the pin.  ``value`` can be
-            anything that converts to a boolean.  If it converts to ``True``, the pin
-            is set high, otherwise it is set low.
-        """
-        ...
-    def high(self, *args, **kwargs) -> Any: ...
-    def gpio(self) -> int:
-        """
-        Returns the base address of the GPIO block associated with this pin.
-        """
-        ...
-    @classmethod
-    def dict(cls, dict: Optional[Any] = None) -> Any:
-        """
-        Get or set the pin mapper dictionary.
-        """
-        ...
-    @classmethod
-    def debug(cls, state: Optional[Any] = None) -> bool:
-        """
-        Get or set the debugging state (``True`` or ``False`` for on or off).
-        """
-        ...
-
-    class cpu:
-        B9: Any
-        B8: Any
-        B7: Any
-        C0: Any
-        C1: Any
-        C10: Any
-        B3: Any
-        B2: Any
-        B6: Any
-        B4: Any
-        B5: Any
-        B15: Any
-        C7: Any
-        C6: Any
-        C5: Any
-        C8: Any
-        C9: Any
-        C11: Any
-        C13: Any
-        C12: Any
-        C4: Any
-        C2: Any
-        C3: Any
-        D2: Any
-        A15: Any
-        A14: Any
-        A13: Any
-        A2: Any
-        A3: Any
-        A4: Any
-        A1: Any
-        A0: Any
-        A12: Any
-        A10: Any
-        A11: Any
-        B14: Any
-        B11: Any
-        B10: Any
-        B1: Any
-        B12: Any
-        B13: Any
-        A5: Any
-        A7: Any
-        A6: Any
-        B0: Any
-        A8: Any
-        A9: Any
-        def __init__(self, *argv, **kwargs) -> None: ...
-
-    @classmethod
-    def mapper(cls, fun: Optional[Any] = None) -> Any:
-        """
-        Get or set the pin mapper function.
-
-        """
-        ...
-
-    class board:
-        X5: Any
-        X18: Any
-        X4: Any
-        X8: Any
-        X6: Any
-        X7: Any
-        X2: Any
-        X3: Any
-        X19: Any
-        X22: Any
-        X20: Any
-        X21: Any
-        Y5: Any
-        X9: Any
-        Y4: Any
-        Y8: Any
-        Y6: Any
-        Y7: Any
-        Y10: Any
-        Y3: Any
-        Y1: Any
-        Y2: Any
-        Y11: Any
-        Y12: Any
-        Y9: Any
-        SD_CK: Any
-        X17: Any
-        SD: Any
-        SD_D1: Any
-        SD_CMD: Any
-        SD_D0: Any
-        LED_GREEN: Any
-        MMA_INT: Any
-        LED_BLUE: Any
-        MMA_AVDD: Any
-        LED_RED: Any
-        LED_YELLOW: Any
-        X1: Any
-        SD_D2: Any
-        USB_VBUS: Any
-        X12: Any
-        X10: Any
-        X11: Any
-        SD_SW: Any
-        USB_ID: Any
-        SD_D3: Any
-        USB_DP: Any
-        SW: Any
-        USB_DM: Any
-        def __init__(self, *argv, **kwargs) -> None: ...
-
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-class SDCard:
-    def writeblocks(self, *args, **kwargs) -> Any: ...
-    def power(self, *args, **kwargs) -> Any: ...
-    def present(self, *args, **kwargs) -> Any: ...
-    def readblocks(self, *args, **kwargs) -> Any: ...
-    def ioctl(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def info(self, *args, **kwargs) -> Any: ...
-    def __init__(self, *argv, **kwargs) -> None: ...
+"""
+functions related to the board. See: https://docs.micropython.org/en/v1.20.0/library/pyb.html
+
+The ``pyb`` module contains specific functions related to the board.
+"""
+from typing import List, NoReturn, Optional, Tuple, Any
+
+hid_mouse: tuple
+hid_keyboard: tuple
+
+def hard_reset() -> NoReturn:
+    """
+    Resets the pyboard in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def have_cdc() -> bool:
+    """
+    Return True if USB is connected as a serial device, False otherwise.
+
+    ``Note:`` This function is deprecated.  Use pyb.USB_VCP().isconnected() instead.
+    """
+    ...
+
+def hid(hidtuple: Tuple) -> Any:
+    """
+    Takes a 4-tuple (or list) and sends it to the USB host (the PC) to
+    signal a HID mouse-motion event.
+
+    ``Note:`` This function is deprecated.  Use :meth:`pyb.USB_HID.send()` instead.
+    """
+    ...
+
+def info(dump_alloc_table: Optional[Any] = None) -> None:
+    """
+    Print out lots of information about the board.
+    """
+    ...
+
+def wfi() -> None:
+    """
+    Wait for an internal or external interrupt.
+
+    This executes a ``wfi`` instruction which reduces power consumption
+    of the MCU until any interrupt occurs (be it internal or external),
+    at which point execution continues.  Note that the system-tick interrupt
+    occurs once every millisecond (1000Hz) so this function will block for
+    at most 1ms.
+    """
+    ...
+
+def elapsed_micros(start) -> int:
+    """
+    Returns the number of microseconds which have elapsed since ``start``.
+
+    This function takes care of counter wrap, and always returns a positive
+    number. This means it can be used to measure periods up to about 17.8 minutes.
+
+    Example::
+
+        start = pyb.micros()
+        while pyb.elapsed_micros(start) < 1000:
+            # Perform some operation
+            pass
+    """
+    ...
+
+def freq(sysclk=0, hclk=0, pclk1=0, pclk2=0) -> Tuple:
+    """
+    If given no arguments, returns a tuple of clock frequencies:
+    (sysclk, hclk, pclk1, pclk2).
+    These correspond to:
+
+     - sysclk: frequency of the CPU
+     - hclk: frequency of the AHB bus, core memory and DMA
+     - pclk1: frequency of the APB1 bus
+     - pclk2: frequency of the APB2 bus
+
+    If given any arguments then the function sets the frequency of the CPU,
+    and the buses if additional arguments are given.  Frequencies are given in
+    Hz.  Eg freq(120000000) sets sysclk (the CPU frequency) to 120MHz.  Note that
+    not all values are supported and the largest supported frequency not greater
+    than the given value will be selected.
+
+    Supported sysclk frequencies are (in MHz): 8, 16, 24, 30, 32, 36, 40, 42, 48,
+    54, 56, 60, 64, 72, 84, 96, 108, 120, 144, 168.
+
+    The maximum frequency of hclk is 168MHz, of pclk1 is 42MHz, and of pclk2 is
+    84MHz.  Be sure not to set frequencies above these values.
+
+    The hclk, pclk1 and pclk2 frequencies are derived from the sysclk frequency
+    using a prescaler (divider).  Supported prescalers for hclk are: 1, 2, 4, 8,
+    16, 64, 128, 256, 512.  Supported prescalers for pclk1 and pclk2 are: 1, 2,
+    4, 8.  A prescaler will be chosen to best match the requested frequency.
+
+    A sysclk frequency of
+    8MHz uses the HSE (external crystal) directly and 16MHz uses the HSI
+    (internal oscillator) directly.  The higher frequencies use the HSE to
+    drive the PLL (phase locked loop), and then use the output of the PLL.
+
+    Note that if you change the frequency while the USB is enabled then
+    the USB may become unreliable.  It is best to change the frequency
+    in boot.py, before the USB peripheral is started.  Also note that sysclk
+    frequencies below 36MHz do not allow the USB to function correctly.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state: ``False``/``True`` for disabled/enabled IRQs
+    respectively.  This return value can be passed to enable_irq to restore
+    the IRQ to its original state.
+    """
+    ...
+
+def fault_debug(value) -> None:
+    """
+    Enable or disable hard-fault debugging.  A hard-fault is when there is a fatal
+    error in the underlying system, like an invalid memory access.
+
+    If the *value* argument is ``False`` then the board will automatically reset if
+    there is a hard fault.
+
+    If *value* is ``True`` then, when the board has a hard fault, it will print the
+    registers and the stack trace, and then cycle the LEDs indefinitely.
+
+    The default value is disabled, i.e. to automatically reset.
+    """
+    ...
+
+def elapsed_millis(start) -> int:
+    """
+    Returns the number of milliseconds which have elapsed since ``start``.
+
+    This function takes care of counter wrap, and always returns a positive
+    number. This means it can be used to measure periods up to about 12.4 days.
+
+    Example::
+
+        start = pyb.millis()
+        while pyb.elapsed_millis(start) < 1000:
+            # Perform some operation
+    """
+    ...
+
+def enable_irq(state=True) -> None:
+    """
+    Enable interrupt requests.
+    If ``state`` is ``True`` (the default value) then IRQs are enabled.
+    If ``state`` is ``False`` then IRQs are disabled.  The most common use of
+    this function is to pass it the value returned by ``disable_irq`` to
+    exit a critical section.
+    """
+    ...
+
+def sync() -> None:
+    """
+    Sync all file systems.
+    """
+    ...
+
+def servo(*args, **kwargs) -> Any: ...
+def standby() -> Any:
+    """
+    Put the pyboard into a "deep sleep" state.
+
+    This reduces power consumption to less than 50 uA.  To wake from this
+    sleep state requires a real-time-clock event, or an external interrupt
+    on X1 (PA0=WKUP) or X18 (PC13=TAMP1).
+    Upon waking the system undergoes a hard reset.
+
+    See :meth:`rtc.wakeup` to configure a real-time-clock wakeup event.
+    """
+    ...
+
+def usb_mode(modestr: Optional[Any] = None, port=-1, vid=0xF055, pid=-1, msc=(), hid=hid_mouse, high_speed=False) -> str:
+    """
+    If called with no arguments, return the current USB mode as a string.
+
+    If called with *modestr* provided, attempts to configure the USB mode.
+    The following values of *modestr* are understood:
+
+    - ``None``: disables USB
+    - ``'VCP'``: enable with VCP (Virtual COM Port) interface
+    - ``'MSC'``: enable with MSC (mass storage device class) interface
+    - ``'VCP+MSC'``: enable with VCP and MSC
+    - ``'VCP+HID'``: enable with VCP and HID (human interface device)
+    - ``'VCP+MSC+HID'``: enabled with VCP, MSC and HID (only available on PYBD boards)
+
+    For backwards compatibility, ``'CDC'`` is understood to mean
+    ``'VCP'`` (and similarly for ``'CDC+MSC'`` and ``'CDC+HID'``).
+
+    The *port* parameter should be an integer (0, 1, ...) and selects which
+    USB port to use if the board supports multiple ports.  A value of -1 uses
+    the default or automatically selected port.
+
+    The *vid* and *pid* parameters allow you to specify the VID (vendor id)
+    and PID (product id).  A *pid* value of -1 will select a PID based on the
+    value of *modestr*.
+
+    If enabling MSC mode, the *msc* parameter can be used to specify a list
+    of SCSI LUNs to expose on the mass storage interface.  For example
+    ``msc=(pyb.Flash(), pyb.SDCard())``.
+
+    If enabling HID mode, you may also specify the HID details by
+    passing the *hid* keyword parameter.  It takes a tuple of
+    (subclass, protocol, max packet length, polling interval, report
+    descriptor).  By default it will set appropriate values for a USB
+    mouse.  There is also a ``pyb.hid_keyboard`` constant, which is an
+    appropriate tuple for a USB keyboard.
+
+    The *high_speed* parameter, when set to ``True``, enables USB HS mode if
+    it is supported by the hardware.
+    """
+    ...
+
+def udelay(us) -> None:
+    """
+    Delay for the given number of microseconds.
+    """
+    ...
+
+def unique_id() -> str:
+    """
+    Returns a string of 12 bytes (96 bits), which is the unique ID of the MCU.
+    """
+    ...
+
+def micros() -> int:
+    """
+    Returns the number of microseconds since the board was last reset.
+
+    The result is always a MicroPython smallint (31-bit signed number), so
+    after 2^30 microseconds (about 17.8 minutes) this will start to return
+    negative numbers.
+
+    Note that if :meth:`pyb.stop()` is issued the hardware counter supporting this
+    function will pause for the duration of the "sleeping" state. This
+    will affect the outcome of :meth:`pyb.elapsed_micros()`.
+    """
+    ...
+
+def mount(device, mountpoint, *, readonly=False, mkfs=False) -> int:
+    """
+    ``Note:`` This function is deprecated. Mounting and unmounting devices should
+       be performed by :meth:`os.mount` and :meth:`os.umount` instead.
+
+    Mount a block device and make it available as part of the filesystem.
+    ``device`` must be an object that provides the block protocol. (The
+    following is also deprecated. See :class:`os.AbstractBlockDev` for the
+    correct way to create a block device.)
+
+     - ``readblocks(self, blocknum, buf)``
+     - ``writeblocks(self, blocknum, buf)`` (optional)
+     - ``count(self)``
+     - ``sync(self)`` (optional)
+
+    ``readblocks`` and ``writeblocks`` should copy data between ``buf`` and
+    the block device, starting from block number ``blocknum`` on the device.
+    ``buf`` will be a bytearray with length a multiple of 512.  If
+    ``writeblocks`` is not defined then the device is mounted read-only.
+    The return value of these two functions is ignored.
+
+    ``count`` should return the number of blocks available on the device.
+    ``sync``, if implemented, should sync the data on the device.
+
+    The parameter ``mountpoint`` is the location in the root of the filesystem
+    to mount the device.  It must begin with a forward-slash.
+
+    If ``readonly`` is ``True``, then the device is mounted read-only,
+    otherwise it is mounted read-write.
+
+    If ``mkfs`` is ``True``, then a new filesystem is created if one does not
+    already exist.
+    """
+    ...
+
+def rng() -> int:
+    """
+    Return a 30-bit hardware generated random number.
+    """
+    ...
+
+def millis() -> int:
+    """
+    Returns the number of milliseconds since the board was last reset.
+
+    The result is always a MicroPython smallint (31-bit signed number), so
+    after 2^30 milliseconds (about 12.4 days) this will start to return
+    negative numbers.
+
+    Note that if :meth:`pyb.stop()` is issued the hardware counter supporting this
+    function will pause for the duration of the "sleeping" state. This
+    will affect the outcome of :meth:`pyb.elapsed_millis()`.
+    """
+    ...
+
+def repl_uart(uart) -> UART:
+    """
+    Get or set the UART object where the REPL is repeated on.
+    """
+    ...
+
+def pwm(*args, **kwargs) -> Any: ...
+def repl_info(*args, **kwargs) -> Any: ...
+def stop() -> Any:
+    """
+    Put the pyboard in a "sleeping" state.
+
+    This reduces power consumption to less than 500 uA.  To wake from this
+    sleep state requires an external interrupt or a real-time-clock event.
+    Upon waking execution continues where it left off.
+
+    See :meth:`rtc.wakeup` to configure a real-time-clock wakeup event.
+    """
+    ...
+
+def delay(ms) -> None:
+    """
+    Delay for the given number of milliseconds.
+    """
+    ...
+
+def main(filename) -> None:
+    """
+    Set the filename of the main script to run after boot.py is finished.  If
+    this function is not called then the default file main.py will be executed.
+
+    It only makes sense to call this function from within boot.py.
+    """
+    ...
+
+def bootloader() -> None:
+    """
+    Activate the bootloader without BOOT* pins.
+    """
+    ...
+
+def country(*args, **kwargs) -> Any: ...
+
+class ADCAll:
+    def read_core_vbat(self, *args, **kwargs) -> Any: ...
+    def read_core_vref(self, *args, **kwargs) -> Any: ...
+    def read_vref(self, *args, **kwargs) -> Any: ...
+    def read_core_temp(self, *args, **kwargs) -> Any: ...
+    def read_channel(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
+
+class Accel:
+    """
+    Create and return an accelerometer object.
+    """
+
+    def x(self) -> Any:
+        """
+        Get the x-axis value.
+        """
+        ...
+    def tilt(self) -> Any:
+        """
+        Get the tilt register.
+        """
+        ...
+    def y(self) -> Any:
+        """
+        Get the y-axis value.
+        """
+        ...
+    def z(self) -> Any:
+        """
+        Get the z-axis value.
+        """
+        ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def filtered_xyz(self) -> Tuple:
+        """
+        Get a 3-tuple of filtered x, y and z values.
+
+        Implementation note: this method is currently implemented as taking the
+        sum of 4 samples, sampled from the 3 previous calls to this function along
+        with the sample from the current call.  Returned values are therefore 4
+        times the size of what they would be from the raw x(), y() and z() calls.
+        """
+        ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self) -> None: ...
+
+class CAN:
+    """
+    Construct a CAN object on the given bus.  *bus* can be 1-2, or ``'YA'`` or ``'YB'``.
+    With no additional parameters, the CAN object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See :meth:`CAN.init` for parameters of initialisation.
+
+    The physical pins of the CAN buses are:
+
+      - ``CAN(1)`` is on ``YA``: ``(RX, TX) = (Y3, Y4) = (PB8, PB9)``
+      - ``CAN(2)`` is on ``YB``: ``(RX, TX) = (Y5, Y6) = (PB12, PB13)``
+    """
+
+    MASK16: int
+    MASK32: int
+    LOOPBACK: int
+    LIST32: int
+    SILENT_LOOPBACK: int
+    NORMAL: int
+    SILENT: int
+    STOPPED: int
+    ERROR_ACTIVE: int
+    BUS_OFF: int
+    LIST16: int
+    ERROR_PASSIVE: int
+    ERROR_WARNING: int
+    def restart(self) -> Any:
+        """
+        Force a software restart of the CAN controller without resetting its
+        configuration.
+
+        If the controller enters the bus-off state then it will no longer participate
+        in bus activity.  If the controller is not configured to automatically restart
+        (see :meth:`~CAN.init()`) then this method can be used to trigger a restart,
+        and the controller will follow the CAN protocol to leave the bus-off state and
+        go into the error active state.
+        """
+        ...
+    def recv(self, fifo, list=None, *, timeout=5000) -> Tuple:
+        """
+        Receive data on the bus:
+
+          - *fifo* is an integer, which is the FIFO to receive on
+          - *list* is an optional list object to be used as the return value
+          - *timeout* is the timeout in milliseconds to wait for the receive.
+
+        Return value: A tuple containing five values.
+
+          - The id of the message.
+          - A boolean that indicates if the message ID is standard or extended.
+          - A boolean that indicates if the message is an RTR message.
+          - The FMI (Filter Match Index) value.
+          - An array containing the data.
+
+        If *list* is ``None`` then a new tuple will be allocated, as well as a new
+        bytes object to contain the data (as the fifth element in the tuple).
+
+        If *list* is not ``None`` then it should be a list object with a least five
+        elements.  The fifth element should be a memoryview object which is created
+        from either a bytearray or an array of type 'B' or 'b', and this array must
+        have enough room for at least 8 bytes.  The list object will then be
+        populated with the first four return values above, and the memoryview object
+        will be resized inplace to the size of the data and filled in with that data.
+        The same list and memoryview objects can be reused in subsequent calls to
+        this method, providing a way of receiving data without using the heap.
+        For example::
+
+             buf = bytearray(8)
+             lst = [0, 0, 0, 0, memoryview(buf)]
+             # No heap memory is allocated in the following call
+             can.recv(0, lst)
+        """
+        ...
+    def init(
+        self,
+        mode,
+        prescaler=100,
+        *,
+        sjw=1,
+        bs1=6,
+        bs2=8,
+        auto_restart=False,
+        baudrate=0,
+        sample_point=75,
+        num_filter_banks=14,
+        brs_sjw=1,
+        brs_bs1=8,
+        brs_bs2=3,
+        brs_baudrate=0,
+        brs_sample_point=75,
+    ) -> None:
+        """
+        Initialise the CAN bus with the given parameters:
+
+          - *mode* is one of:  NORMAL, LOOPBACK, SILENT, SILENT_LOOPBACK
+          - *prescaler* is the value by which the CAN input clock is divided to generate the
+            nominal bit time quanta. The prescaler can be a value between 1 and 1024 inclusive
+            for classic CAN, and between 1 and 512 inclusive for CAN FD.
+          - *sjw* is the resynchronisation jump width in units of time quanta for nominal bits;
+            it can be a value between 1 and 4 inclusive for classic CAN, and between 1 and 128 inclusive for CAN FD.
+          - *bs1* defines the location of the sample point in units of the time quanta for nominal bits;
+            it can be a value between 1 and 16 inclusive for classic CAN, and between 2 and 256 inclusive for CAN FD.
+          - *bs2* defines the location of the transmit point in units of the time quanta for nominal bits;
+            it can be a value between 1 and 8 inclusive for classic CAN, and between 2 and 128 inclusive for CAN FD.
+          - *auto_restart* sets whether the controller will automatically try and restart
+            communications after entering the bus-off state; if this is disabled then
+            :meth:`~CAN.restart()` can be used to leave the bus-off state
+          - *baudrate* if a baudrate other than 0 is provided, this function will try to automatically
+            calculate the CAN nominal bit time (overriding *prescaler*, *bs1* and *bs2*) that satisfies
+            both the baudrate and the desired *sample_point*.
+          - *sample_point* given in a percentage of the nominal bit time, the *sample_point* specifies the position
+            of the bit sample with respect to the whole nominal bit time. The default *sample_point* is 75%.
+          - *num_filter_banks* for classic CAN, this is the number of banks that will be assigned to CAN(1),
+            the rest of the 28 are assigned to CAN(2).
+          - *brs_prescaler* is the value by which the CAN FD input clock is divided to generate the
+            data bit time quanta. The prescaler can be a value between 1 and 32 inclusive.
+          - *brs_sjw* is the resynchronisation jump width in units of time quanta for data bits;
+            it can be a value between 1 and 16 inclusive
+          - *brs_bs1* defines the location of the sample point in units of the time quanta for data bits;
+            it can be a value between 1 and 32 inclusive
+          - *brs_bs2* defines the location of the transmit point in units of the time quanta for data bits;
+            it can be a value between 1 and 16 inclusive
+          - *brs_baudrate* if a baudrate other than 0 is provided, this function will try to automatically
+            calculate the CAN data bit time (overriding *brs_prescaler*, *brs_bs1* and *brs_bs2*) that satisfies
+            both the baudrate and the desired *brs_sample_point*.
+          - *brs_sample_point* given in a percentage of the data bit time, the *brs_sample_point* specifies the position
+            of the bit sample with respect to the whole data bit time. The default *brs_sample_point* is 75%.
+
+
+        The time quanta tq is the basic unit of time for the CAN bus.  tq is the CAN
+        prescaler value divided by PCLK1 (the frequency of internal peripheral bus 1);
+        see :meth:`pyb.freq()` to determine PCLK1.
+
+        A single bit is made up of the synchronisation segment, which is always 1 tq.
+        Then follows bit segment 1, then bit segment 2.  The sample point is after bit
+        segment 1 finishes.  The transmit point is after bit segment 2 finishes.
+        The baud rate will be 1/bittime, where the bittime is 1 + BS1 + BS2 multiplied
+        by the time quanta tq.
+
+        For example, with PCLK1=42MHz, prescaler=100, sjw=1, bs1=6, bs2=8, the value of
+        tq is 2.38 microseconds.  The bittime is 35.7 microseconds, and the baudrate
+        is 28kHz.
+
+        See page 680 of the STM32F405 datasheet for more details.
+        """
+        ...
+    def rxcallback(self, fifo, fun) -> None:
+        """
+        Register a function to be called when a message is accepted into a empty fifo:
+
+        - *fifo* is the receiving fifo.
+        - *fun* is the function to be called when the fifo becomes non empty.
+
+        The callback function takes two arguments the first is the can object it self the second is
+        a integer that indicates the reason for the callback.
+
+        +--------+------------------------------------------------+
+        | Reason |                                                |
+        +========+================================================+
+        | 0      | A message has been accepted into a empty FIFO. |
+        +--------+------------------------------------------------+
+        | 1      | The FIFO is full                               |
+        +--------+------------------------------------------------+
+        | 2      | A message has been lost due to a full FIFO     |
+        +--------+------------------------------------------------+
+
+        Example use of rxcallback::
+
+          def cb0(bus, reason):
+            print('cb0')
+            if reason == 0:
+                print('pending')
+            if reason == 1:
+                print('full')
+            if reason == 2:
+                print('overflow')
+
+          can = CAN(1, CAN.LOOPBACK)
+          can.rxcallback(0, cb0)
+        """
+        ...
+    def setfilter(self, bank, mode, fifo, params, *, rtr=None, extframe=False) -> None:
+        """
+        Configure a filter bank:
+
+        - *bank* is the classic CAN controller filter bank, or CAN FD filter index, to configure.
+        - *mode* is the mode the filter should operate in, see the tables below.
+        - *fifo* is which fifo (0 or 1) a message should be stored in, if it is accepted by this filter.
+        - *params* is an array of values the defines the filter. The contents of the array depends on the *mode* argument.
+
+        +-----------+---------------------------------------------------------+
+        |*mode*     |Contents of *params* array for classic CAN controller    |
+        +===========+=========================================================+
+        |CAN.LIST16 |Four 16 bit ids that will be accepted                    |
+        +-----------+---------------------------------------------------------+
+        |CAN.LIST32 |Two 32 bit ids that will be accepted                     |
+        +-----------+---------------------------------------------------------+
+        |CAN.MASK16 |Two 16 bit id/mask pairs. E.g. (1, 3, 4, 4)              |
+        |           | | The first pair, 1 and 3 will accept all ids           |
+        |           | | that have bit 0 = 1 and bit 1 = 0.                    |
+        |           | | The second pair, 4 and 4, will accept all ids         |
+        |           | | that have bit 2 = 1.                                  |
+        +-----------+---------------------------------------------------------+
+        |CAN.MASK32 |As with CAN.MASK16 but with only one 32 bit id/mask pair.|
+        +-----------+---------------------------------------------------------+
+
+        +-----------+---------------------------------------------------------+
+        |*mode*     |Contents of *params* array for CAN FD controller         |
+        +===========+=========================================================+
+        |CAN.RANGE  |Two ids that represent a range of accepted ids.          |
+        +-----------+---------------------------------------------------------+
+        |CAN.DUAL   |Two ids that will be accepted. For example (1, 2)        |
+        +-----------+---------------------------------------------------------+
+        |CAN.MASK   |One filter ID and a mask. For example (0x111, 0x7FF)     |
+        +-----------+---------------------------------------------------------+
+
+        - *rtr* For classic CAN controllers, this is an array of booleans that states if
+          a filter should accept a remote transmission request message. If this argument
+          is not given then it defaults to ``False`` for all entries. The length of the
+          array depends on the *mode* argument. For CAN FD, this argument is ignored.
+
+        +-----------+----------------------+
+        |*mode*     |length of *rtr* array |
+        +===========+======================+
+        |CAN.LIST16 |4                     |
+        +-----------+----------------------+
+        |CAN.LIST32 |2                     |
+        +-----------+----------------------+
+        |CAN.MASK16 |2                     |
+        +-----------+----------------------+
+        |CAN.MASK32 |1                     |
+        +-----------+----------------------+
+
+        - *extframe* If True the frame will have an extended identifier (29 bits),
+          otherwise a standard identifier (11 bits) is used.
+
+        """
+        ...
+    def state(self) -> Any:
+        """
+        Return the state of the controller.  The return value can be one of:
+
+        - ``CAN.STOPPED`` -- the controller is completely off and reset;
+        - ``CAN.ERROR_ACTIVE`` -- the controller is on and in the Error Active state
+          (both TEC and REC are less than 96);
+        - ``CAN.ERROR_WARNING`` -- the controller is on and in the Error Warning state
+          (at least one of TEC or REC is 96 or greater);
+        - ``CAN.ERROR_PASSIVE`` -- the controller is on and in the Error Passive state
+          (at least one of TEC or REC is 128 or greater);
+        - ``CAN.BUS_OFF`` -- the controller is on but not participating in bus activity
+          (TEC overflowed beyond 255).
+        """
+        ...
+    def send(self, data, id, *, timeout=0, rtr=False, extframe=False, fdf=False, brs=False) -> None:
+        """
+        Send a message on the bus:
+
+          - *data* is the data to send (an integer to send, or a buffer object).
+          - *id* is the id of the message to be sent.
+          - *timeout* is the timeout in milliseconds to wait for the send.
+          - *rtr* is a boolean that specifies if the message shall be sent as
+            a remote transmission request.  If *rtr* is True then only the length
+            of *data* is used to fill in the DLC slot of the frame; the actual
+            bytes in *data* are unused.
+          - *extframe* if True the frame will have an extended identifier (29 bits),
+            otherwise a standard identifier (11 bits) is used.
+          - *fdf* for CAN FD controllers, if set to True, the frame will have an FD
+            frame format, which supports data payloads up to 64 bytes.
+          - *brs* for CAN FD controllers, if set to True, the bitrate switching mode
+            is enabled, in which the data phase is transmitted at a differet bitrate.
+            See :meth:`CAN.init` for the data bit timing configuration parameters.
+
+          If timeout is 0 the message is placed in a buffer in one of three hardware
+          buffers and the method returns immediately. If all three buffers are in use
+          an exception is thrown. If timeout is not 0, the method waits until the
+          message is transmitted. If the message can't be transmitted within the
+          specified time an exception is thrown.
+
+        Return value: ``None``.
+        """
+        ...
+    def any(self, fifo) -> bool:
+        """
+        Return ``True`` if any message waiting on the FIFO, else ``False``.
+        """
+        ...
+    def info(self, list: Optional[Any] = None) -> Any:
+        """
+        Get information about the controller's error states and TX and RX buffers.
+        If *list* is provided then it should be a list object with at least 8 entries,
+        which will be filled in with the information.  Otherwise a new list will be
+        created and filled in.  In both cases the return value of the method is the
+        populated list.
+
+        The values in the list are:
+
+        - TEC value
+        - REC value
+        - number of times the controller enterted the Error Warning state (wrapped
+          around to 0 after 65535)
+        - number of times the controller enterted the Error Passive state (wrapped
+          around to 0 after 65535)
+        - number of times the controller enterted the Bus Off state (wrapped
+          around to 0 after 65535)
+        - number of pending TX messages
+        - number of pending RX messages on fifo 0
+        - number of pending RX messages on fifo 1
+        """
+        ...
+    def clearfilter(self, bank, extframe=False) -> None:
+        """
+        Clear and disables a filter bank:
+
+        - *bank* is the classic CAN controller filter bank, or CAN FD filter index, to clear.
+        - *extframe* For CAN FD controllers, if True, clear an extended filter (configured with extframe=True),
+          otherwise the clear a standard identifier (configured with extframe=False).
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Turn off the CAN bus.
+        """
+        ...
+    def __init__(
+        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
+    ) -> None: ...
+
+class ExtInt:
+    """
+    Create an ExtInt object:
+
+      - ``pin`` is the pin on which to enable the interrupt (can be a pin object or any valid pin name).
+      - ``mode`` can be one of:
+        - ``ExtInt.IRQ_RISING`` - trigger on a rising edge;
+        - ``ExtInt.IRQ_FALLING`` - trigger on a falling edge;
+        - ``ExtInt.IRQ_RISING_FALLING`` - trigger on a rising or falling edge.
+      - ``pull`` can be one of:
+        - ``pyb.Pin.PULL_NONE`` - no pull up or down resistors;
+        - ``pyb.Pin.PULL_UP`` - enable the pull-up resistor;
+        - ``pyb.Pin.PULL_DOWN`` - enable the pull-down resistor.
+      - ``callback`` is the function to call when the interrupt triggers.  The
+        callback function must accept exactly 1 argument, which is the line that
+        triggered the interrupt.
+
+    """
+
+    IRQ_FALLING: int
+    IRQ_RISING_FALLING: int
+    IRQ_RISING: int
+    EVT_FALLING: int
+    EVT_RISING_FALLING: int
+    EVT_RISING: int
+    def line(self) -> int:
+        """
+        Return the line number that the pin is mapped to.
+        """
+        ...
+    @classmethod
+    def regs(cls) -> Any:
+        """
+        Dump the values of the EXTI registers.
+
+        """
+        ...
+    def swint(self) -> Any:
+        """
+        Trigger the callback from software.
+
+        """
+        ...
+    def enable(self) -> None:
+        """
+        Enable a disabled interrupt.
+        """
+        ...
+    def disable(self) -> None:
+        """
+        Disable the interrupt associated with the ExtInt object.
+        This could be useful for debouncing.
+        """
+        ...
+    def __init__(self, pin, mode, pull, callback) -> None: ...
+
+class Flash:
+    """
+    Create and return a block device that represents the flash device presented
+    to the USB mass storage interface.
+
+    It includes a virtual partition table at the start, and the actual flash
+    starts at block ``0x100``.
+
+    This constructor is deprecated and will be removed in a future version of MicroPython.
+    """
+
+    def readblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
+    def writeblocks(self, block_num, buf, offset: Optional[int] = 0) -> Any: ...
+    def ioctl(self, cmd, arg) -> Any:
+        """
+        These methods implement the simple and :ref:`extended
+        <block-device-interface>` block protocol defined by
+        :class:`os.AbstractBlockDev`.
+        """
+        ...
+    def __init__(self) -> None: ...
+
+class ADC:
+    """
+    Create an ADC object associated with the given pin.
+    This allows you to then read analog values on that pin.
+    """
+
+    def read_timed(self, buf, timer) -> Any:
+        """
+        Read analog values into ``buf`` at a rate set by the ``timer`` object.
+
+        ``buf`` can be bytearray or array.array for example.  The ADC values have
+        12-bit resolution and are stored directly into ``buf`` if its element size is
+        16 bits or greater.  If ``buf`` has only 8-bit elements (eg a bytearray) then
+        the sample resolution will be reduced to 8 bits.
+
+        ``timer`` should be a Timer object, and a sample is read each time the timer
+        triggers.  The timer must already be initialised and running at the desired
+        sampling frequency.
+
+        To support previous behaviour of this function, ``timer`` can also be an
+        integer which specifies the frequency (in Hz) to sample at.  In this case
+        Timer(6) will be automatically configured to run at the given frequency.
+
+        Example using a Timer object (preferred way)::
+
+            adc = pyb.ADC(pyb.Pin.board.X19)    # create an ADC on pin X19
+            tim = pyb.Timer(6, freq=10)         # create a timer running at 10Hz
+            buf = bytearray(100)                # creat a buffer to store the samples
+            adc.read_timed(buf, tim)            # sample 100 values, taking 10s
+
+        Example using an integer for the frequency::
+
+            adc = pyb.ADC(pyb.Pin.board.X19)    # create an ADC on pin X19
+            buf = bytearray(100)                # create a buffer of 100 bytes
+            adc.read_timed(buf, 10)             # read analog values into buf at 10Hz
+                                                #   this will take 10 seconds to finish
+            for val in buf:                     # loop over all values
+                print(val)                      # print the value out
+
+        This function does not allocate any heap memory. It has blocking behaviour:
+        it does not return to the calling program until the buffer is full.
+        """
+        ...
+    def read_timed_multi(self, adcs, bufs, timer) -> bool:
+        """
+        This is a static method. It can be used to extract relative timing or
+        phase data from multiple ADC's.
+
+        It reads analog values from multiple ADC's into buffers at a rate set by
+        the *timer* object. Each time the timer triggers a sample is rapidly
+        read from each ADC in turn.
+
+        ADC and buffer instances are passed in tuples with each ADC having an
+        associated buffer. All buffers must be of the same type and length and
+        the number of buffers must equal the number of ADC's.
+
+        Buffers can be ``bytearray`` or ``array.array`` for example. The ADC values
+        have 12-bit resolution and are stored directly into the buffer if its element
+        size is 16 bits or greater.  If buffers have only 8-bit elements (eg a
+        ``bytearray``) then the sample resolution will be reduced to 8 bits.
+
+        *timer* must be a Timer object. The timer must already be initialised
+        and running at the desired sampling frequency.
+
+        Example reading 3 ADC's::
+
+            adc0 = pyb.ADC(pyb.Pin.board.X1)    # Create ADC's
+            adc1 = pyb.ADC(pyb.Pin.board.X2)
+            adc2 = pyb.ADC(pyb.Pin.board.X3)
+            tim = pyb.Timer(8, freq=100)        # Create timer
+            rx0 = array.array('H', (0 for i in range(100))) # ADC buffers of
+            rx1 = array.array('H', (0 for i in range(100))) # 100 16-bit words
+            rx2 = array.array('H', (0 for i in range(100)))
+            # read analog values into buffers at 100Hz (takes one second)
+            pyb.ADC.read_timed_multi((adc0, adc1, adc2), (rx0, rx1, rx2), tim)
+            for n in range(len(rx0)):
+                print(rx0[n], rx1[n], rx2[n])
+
+        This function does not allocate any heap memory. It has blocking behaviour:
+        it does not return to the calling program until the buffers are full.
+
+        The function returns ``True`` if all samples were acquired with correct
+        timing. At high sample rates the time taken to acquire a set of samples
+        can exceed the timer period. In this case the function returns ``False``,
+        indicating a loss of precision in the sample interval. In extreme cases
+        samples may be missed.
+
+        The maximum rate depends on factors including the data width and the
+        number of ADC's being read. In testing two ADC's were sampled at a timer
+        rate of 210kHz without overrun. Samples were missed at 215kHz.  For three
+        ADC's the limit is around 140kHz, and for four it is around 110kHz.
+        At high sample rates disabling interrupts for the duration can reduce the
+        risk of sporadic data loss.
+        """
+        ...
+    def read(self) -> Any:
+        """
+        Read the value on the analog pin and return it.  The returned value
+        will be between 0 and 4095.
+        """
+        ...
+    def __init__(self, pin) -> None: ...
+
+SD: Any
+
+class DAC:
+    """
+    Construct a new DAC object.
+
+    ``port`` can be a pin object, or an integer (1 or 2).
+    DAC(1) is on pin X5 and DAC(2) is on pin X6.
+
+    ``bits`` is an integer specifying the resolution, and can be 8 or 12.
+    The maximum value for the write and write_timed methods will be
+    2**``bits``-1.
+
+    The *buffering* parameter selects the behaviour of the DAC op-amp output
+    buffer, whose purpose is to reduce the output impedance.  It can be
+    ``None`` to select the default (buffering enabled for :meth:`DAC.noise`,
+    :meth:`DAC.triangle` and :meth:`DAC.write_timed`, and disabled for
+    :meth:`DAC.write`), ``False`` to disable buffering completely, or ``True``
+    to enable output buffering.
+
+    When buffering is enabled the DAC pin can drive loads down to 5KΩ.
+    Otherwise it has an output impedance of 15KΩ maximum: consequently
+    to achieve a 1% accuracy without buffering requires the applied load
+    to be less than 1.5MΩ.  Using the buffer incurs a penalty in accuracy,
+    especially near the extremes of range.
+    """
+
+    CIRCULAR: int
+    NORMAL: int
+    def noise(self, freq) -> None:
+        """
+        Generate a pseudo-random noise signal.  A new random sample is written
+        to the DAC output at the given frequency.
+        """
+        ...
+    def write_timed(self, data, freq, *, mode=NORMAL) -> Any:
+        """
+        Initiates a burst of RAM to DAC using a DMA transfer.
+        The input data is treated as an array of bytes in 8-bit mode, and
+        an array of unsigned half-words (array typecode 'H') in 12-bit mode.
+
+        ``freq`` can be an integer specifying the frequency to write the DAC
+        samples at, using Timer(6).  Or it can be an already-initialised
+        Timer object which is used to trigger the DAC sample.  Valid timers
+        are 2, 4, 5, 6, 7 and 8.
+
+        ``mode`` can be ``DAC.NORMAL`` or ``DAC.CIRCULAR``.
+
+        Example using both DACs at the same time::
+
+          dac1 = DAC(1)
+          dac2 = DAC(2)
+          dac1.write_timed(buf1, pyb.Timer(6, freq=100), mode=DAC.CIRCULAR)
+          dac2.write_timed(buf2, pyb.Timer(7, freq=200), mode=DAC.CIRCULAR)
+        """
+        ...
+    def triangle(self, freq) -> None:
+        """
+        Generate a triangle wave.  The value on the DAC output changes at the given
+        frequency and ramps through the full 12-bit range (up and down). Therefore
+        the frequency of the repeating triangle wave itself is 8192 times smaller.
+        """
+        ...
+    def write(self, value) -> Any:
+        """
+        Direct access to the DAC output.  The minimum value is 0.  The maximum
+        value is 2**``bits``-1, where ``bits`` is set when creating the DAC
+        object or by using the ``init`` method.
+        """
+        ...
+    def init(self, bits=8, *, buffering=None) -> Any:
+        """
+        Reinitialise the DAC.  *bits* can be 8 or 12.  *buffering* can be
+        ``None``, ``False`` or ``True``; see above constructor for the meaning
+        of this parameter.
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        De-initialise the DAC making its pin available for other uses.
+        """
+        ...
+    def __init__(self, port, bits=8, *, buffering=None) -> None: ...
+
+class RTC:
+    """
+    Create an RTC object.
+
+    """
+
+    def info(self) -> Any:
+        """
+        Get information about the startup time and reset source.
+
+         - The lower 0xffff are the number of milliseconds the RTC took to
+           start up.
+         - Bit 0x10000 is set if a power-on reset occurred.
+         - Bit 0x20000 is set if an external reset occurred
+        """
+        ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def wakeup(self, timeout, callback=None) -> None:
+        """
+        Set the RTC wakeup timer to trigger repeatedly at every ``timeout``
+        milliseconds.  This trigger can wake the pyboard from both the sleep
+        states: :meth:`pyb.stop` and :meth:`pyb.standby`.
+
+        If ``timeout`` is ``None`` then the wakeup timer is disabled.
+
+        If ``callback`` is given then it is executed at every trigger of the
+        wakeup timer.  ``callback`` must take exactly one argument.
+        """
+        ...
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time (and ``subseconds`` is reset to 255).
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        ``weekday`` is 1-7 for Monday through Sunday.
+
+        ``subseconds`` counts down from 255 to 0
+        """
+        ...
+    def calibration(self, cal) -> int:
+        """
+        Get or set RTC calibration.
+
+        With no arguments, ``calibration()`` returns the current calibration
+        value, which is an integer in the range [-511 : 512].  With one
+        argument it sets the RTC calibration.
+
+        The RTC Smooth Calibration mechanism adjusts the RTC clock rate by
+        adding or subtracting the given number of ticks from the 32768 Hz
+        clock over a 32 second period (corresponding to 2^20 clock ticks.)
+        Each tick added will speed up the clock by 1 part in 2^20, or 0.954
+        ppm; likewise the RTC clock it slowed by negative values. The
+        usable calibration range is:
+        (-511 * 0.954) ~= -487.5 ppm up to (512 * 0.954) ~= 488.5 ppm
+        """
+        ...
+    def __init__(self) -> None: ...
+
+class USB_VCP:
+    """
+    Create a new USB_VCP object.  The *id* argument specifies which USB VCP port to
+    use.
+
+    """
+
+    RTS: int
+    CTS: int
+    IRQ_RX: int
+    def readlines(self) -> List:
+        """
+        Read as much data as possible from the serial device, breaking it into
+        lines.
+
+        Returns a list of bytes objects, each object being one of the lines.
+        Each line will include the newline character.
+        """
+        ...
+    def recv(self, data, *, timeout=5000) -> int:
+        """
+        Receive data on the bus:
+
+          - ``data`` can be an integer, which is the number of bytes to receive,
+            or a mutable buffer, which will be filled with received bytes.
+          - ``timeout`` is the timeout in milliseconds to wait for the receive.
+
+        Return value: if ``data`` is an integer then a new buffer of the bytes received,
+        otherwise the number of bytes read into ``data`` is returned.
+        """
+        ...
+    def isconnected(self) -> bool:
+        """
+        Return ``True`` if USB is connected as a serial device, else ``False``.
+        """
+        ...
+    def init(self, *, flow=-1) -> None:
+        """
+        Configure the USB VCP port.  If the *flow* argument is not -1 then the value sets
+        the flow control, which can be a bitwise-or of ``USB_VCP.RTS`` and ``USB_VCP.CTS``.
+        RTS is used to control read behaviour and CTS, to control write behaviour.
+        """
+        ...
+    def irq(self, handler=None, trigger=IRQ_RX, hard=False) -> None:
+        """
+        Register *handler* to be called whenever an event specified by *trigger*
+        occurs.  The *handler* function must take exactly one argument, which will
+        be the USB VCP object.  Pass in ``None`` to disable the callback.
+
+        Valid values for *trigger* are:
+
+          - ``USB_VCP.IRQ_RX``: new data is available for reading from the USB VCP object.
+
+        """
+        ...
+    def setinterrupt(self, chr) -> None:
+        """
+        Set the character which interrupts running Python code.  This is set
+        to 3 (CTRL-C) by default, and when a CTRL-C character is received over
+        the USB VCP port, a KeyboardInterrupt exception is raised.
+
+        Set to -1 to disable this interrupt feature.  This is useful when you
+        want to send raw bytes over the USB VCP port.
+        """
+        ...
+    def close(self) -> Any:
+        """
+        This method does nothing.  It exists so the USB_VCP object can act as
+        a file.
+        """
+        ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read at most ``nbytes`` from the serial device and return them as a
+        bytes object.  If ``nbytes`` is not specified then the method reads
+        all available bytes from the serial device.
+        USB_VCP `stream` implicitly works in non-blocking mode,
+        so if no pending data available, this method will return immediately
+        with ``None`` value.
+        """
+        ...
+    def any(self) -> bool:
+        """
+        Return ``True`` if any characters waiting, else ``False``.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from ``buf`` to the serial device.
+
+        Returns the number of bytes written.
+        """
+        ...
+    def send(self, data, *, timeout=5000) -> int:
+        """
+        Send data over the USB VCP:
+
+          - ``data`` is the data to send (an integer to send, or a buffer object).
+          - ``timeout`` is the timeout in milliseconds to wait for the send.
+
+        Return value: number of bytes sent.
+        """
+        ...
+    def readinto(self, buf, maxlen: Optional[Any] = None) -> int:
+        """
+        Read bytes from the serial device and store them into ``buf``, which
+        should be a buffer-like object.  At most ``len(buf)`` bytes are read.
+        If ``maxlen`` is given and then at most ``min(maxlen, len(buf))`` bytes
+        are read.
+
+        Returns the number of bytes read and stored into ``buf`` or ``None``
+        if no pending data available.
+        """
+        ...
+    def readline(self) -> bytes:
+        """
+        Read a whole line from the serial device.
+
+        Returns a bytes object containing the data, including the trailing
+        newline character or ``None`` if no pending data available.
+        """
+        ...
+    def __init__(self, id=0) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given id.  If additional
+    arguments are given, then the timer is initialised by ``init(...)``.
+    ``id`` can be 1 to 14.
+    """
+
+    OC_FORCED_ACTIVE: int
+    OC_FORCED_INACTIVE: int
+    OC_INACTIVE: int
+    OC_ACTIVE: int
+    LOW: int
+    IC: int
+    PWM_INVERTED: int
+    RISING: int
+    OC_TIMING: int
+    PWM: int
+    OC_TOGGLE: int
+    UP: int
+    BRK_LOW: int
+    BRK_OFF: int
+    CENTER: int
+    BRK_HIGH: int
+    BOTH: int
+    HIGH: int
+    ENC_B: int
+    FALLING: int
+    DOWN: int
+    ENC_AB: int
+    ENC_A: int
+    def freq(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the frequency for the timer (changes prescaler and period if set).
+        """
+        ...
+    def init(self, *, freq, prescaler, period, mode=UP, div=1, callback=None, deadtime=0, brk=BRK_OFF) -> None:
+        """
+        Initialise the timer.  Initialisation must be either by frequency (in Hz)
+        or by prescaler and period::
+
+            tim.init(freq=100)                  # set the timer to trigger at 100Hz
+            tim.init(prescaler=83, period=999)  # set the prescaler and period directly
+
+        Keyword arguments:
+
+          - ``freq`` --- specifies the periodic frequency of the timer. You might also
+            view this as the frequency with which the timer goes through one complete cycle.
+
+          - ``prescaler`` [0-0xffff] - specifies the value to be loaded into the
+            timer's Prescaler Register (PSC). The timer clock source is divided by
+            (``prescaler + 1``) to arrive at the timer clock. Timers 2-7 and 12-14
+            have a clock source of 84 MHz (pyb.freq()[2] * 2), and Timers 1, and 8-11
+            have a clock source of 168 MHz (pyb.freq()[3] * 2).
+
+          - ``period`` [0-0xffff] for timers 1, 3, 4, and 6-15. [0-0x3fffffff] for timers 2 & 5.
+            Specifies the value to be loaded into the timer's AutoReload
+            Register (ARR). This determines the period of the timer (i.e. when the
+            counter cycles). The timer counter will roll-over after ``period + 1``
+            timer clock cycles.
+
+          - ``mode`` can be one of:
+
+            - ``Timer.UP`` - configures the timer to count from 0 to ARR (default)
+            - ``Timer.DOWN`` - configures the timer to count from ARR down to 0.
+            - ``Timer.CENTER`` - configures the timer to count from 0 to ARR and
+              then back down to 0.
+
+          - ``div`` can be one of 1, 2, or 4. Divides the timer clock to determine
+            the sampling clock used by the digital filters.
+
+          - ``callback`` - as per Timer.callback()
+
+          - ``deadtime`` - specifies the amount of "dead" or inactive time between
+            transitions on complimentary channels (both channels will be inactive)
+            for this time). ``deadtime`` may be an integer between 0 and 1008, with
+            the following restrictions: 0-128 in steps of 1. 128-256 in steps of
+            2, 256-512 in steps of 8, and 512-1008 in steps of 16. ``deadtime``
+            measures ticks of ``source_freq`` divided by ``div`` clock ticks.
+            ``deadtime`` is only available on timers 1 and 8.
+
+          - ``brk`` - specifies if the break mode is used to kill the output of
+            the PWM when the ``BRK_IN`` input is asserted. The value of this
+            argument determines if break is enabled and what the polarity is, and
+            can be one of ``Timer.BRK_OFF``, ``Timer.BRK_LOW`` or
+            ``Timer.BRK_HIGH``. To select the ``BRK_IN`` pin construct a Pin object with
+            ``mode=Pin.ALT, alt=Pin.AFn_TIMx``. The pin's GPIO input features are
+            available in alt mode - ``pull=`` , ``value()`` and ``irq()``.
+
+         You must either specify freq or both of period and prescaler.
+        """
+        ...
+    def period(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the period of the timer.
+        """
+        ...
+    def prescaler(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the prescaler for the timer.
+        """
+        ...
+    def source_freq(self) -> Any:
+        """
+        Get the frequency of the source of the timer.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer.
+
+        Disables the callback (and the associated irq).
+
+        Disables any channel callbacks (and the associated irq).
+        Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def callback(self, fun) -> None:
+        """
+        Set the function to be called when the timer triggers.
+        ``fun`` is passed 1 argument, the timer object.
+        If ``fun`` is ``None`` then the callback will be disabled.
+        """
+        ...
+    def channel(self, channel, mode, pin=None, *args) -> Any:
+        """
+        If only a channel number is passed, then a previously initialized channel
+        object is returned (or ``None`` if there is no previous channel).
+
+        Otherwise, a TimerChannel object is initialized and returned.
+
+        Each channel can be configured to perform pwm, output compare, or
+        input capture. All channels share the same underlying timer, which means
+        that they share the same timer clock.
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.PWM`` --- configure the timer in PWM mode (active high).
+            - ``Timer.PWM_INVERTED`` --- configure the timer in PWM mode (active low).
+            - ``Timer.OC_TIMING`` --- indicates that no pin is driven.
+            - ``Timer.OC_ACTIVE`` --- the pin will be made active when a compare match occurs (active is determined by polarity)
+            - ``Timer.OC_INACTIVE`` --- the pin will be made inactive when a compare match occurs.
+            - ``Timer.OC_TOGGLE`` --- the pin will be toggled when an compare match occurs.
+            - ``Timer.OC_FORCED_ACTIVE`` --- the pin is forced active (compare match is ignored).
+            - ``Timer.OC_FORCED_INACTIVE`` --- the pin is forced inactive (compare match is ignored).
+            - ``Timer.IC`` --- configure the timer in Input Capture mode.
+            - ``Timer.ENC_A`` --- configure the timer in Encoder mode. The counter only changes when CH1 changes.
+            - ``Timer.ENC_B`` --- configure the timer in Encoder mode. The counter only changes when CH2 changes.
+            - ``Timer.ENC_AB`` --- configure the timer in Encoder mode. The counter changes when CH1 or CH2 changes.
+
+          - ``callback`` - as per TimerChannel.callback()
+
+          - ``pin`` None (the default) or a Pin object. If specified (and not None)
+            this will cause the alternate function of the the indicated pin
+            to be configured for this timer channel. An error will be raised if
+            the pin doesn't support any alternate functions for this timer channel.
+
+        Keyword arguments for Timer.PWM modes:
+
+          - ``pulse_width`` - determines the initial pulse width value to use.
+          - ``pulse_width_percent`` - determines the initial pulse width percentage to use.
+
+        Keyword arguments for Timer.OC modes:
+
+          - ``compare`` - determines the initial value of the compare register.
+
+          - ``polarity`` can be one of:
+
+            - ``Timer.HIGH`` - output is active high
+            - ``Timer.LOW`` - output is active low
+
+        Optional keyword arguments for Timer.IC modes:
+
+          - ``polarity`` can be one of:
+
+            - ``Timer.RISING`` - captures on rising edge.
+            - ``Timer.FALLING`` - captures on falling edge.
+            - ``Timer.BOTH`` - captures on both edges.
+
+          Note that capture only works on the primary channel, and not on the
+          complimentary channels.
+
+        Notes for Timer.ENC modes:
+
+          - Requires 2 pins, so one or both pins will need to be configured to use
+            the appropriate timer AF using the Pin API.
+          - Read the encoder value using the timer.counter() method.
+          - Only works on CH1 and CH2 (and not on CH1N or CH2N)
+          - The channel number is ignored when setting the encoder mode.
+
+        PWM Example::
+
+            timer = pyb.Timer(2, freq=1000)
+            ch2 = timer.channel(2, pyb.Timer.PWM, pin=pyb.Pin.board.X2, pulse_width=8000)
+            ch3 = timer.channel(3, pyb.Timer.PWM, pin=pyb.Pin.board.X3, pulse_width=16000)
+
+        PWM Motor Example with complementary outputs, dead time, break input and break callback::
+
+            from pyb import Timer
+            from machine import Pin # machine.Pin supports alt mode and irq on the same pin.
+            pin_t8_1 = Pin(Pin.board.Y1, mode=Pin.ALT, af=Pin.AF3_TIM8)   # Pin PC6, TIM8_CH1
+            pin_t8_1n = Pin(Pin.board.X8, mode=Pin.ALT, af=Pin.AF3_TIM8)  # Pin PA7, TIM8_CH1N
+            pin_bkin = Pin(Pin.board.X7, mode=Pin.ALT, af=Pin.AF3_TIM8)   # Pin PA6, TIM8_BKIN
+            pin_bkin.irq(handler=break_callabck, trigger=Pin.IRQ_FALLING)
+            timer = pyb.Timer(8, freq=1000, deadtime=1008, brk=Timer.BRK_LOW)
+            ch1 = timer.channel(1, pyb.Timer.PWM, pulse_width_percent=30)
+        """
+        ...
+    def counter(self, value: Optional[Any] = None) -> Any:
+        """
+        Get or set the timer counter.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+class Switch(Pin):
+    """
+    Create and return a switch object.
+
+    """
+
+    def callback(self, fun) -> None:
+        """
+        Register the given function to be called when the switch is pressed down.
+        If ``fun`` is ``None``, then it disables the callback.
+        """
+        ...
+    def value(self) -> bool:
+        """
+        Get the switch state.  Returns ``True`` if pressed down, otherwise ``False``.
+        """
+        ...
+    def __init__(self) -> None: ...
+
+class Servo:
+    """
+    Create a servo object.  ``id`` is 1-4, and corresponds to pins X1 through X4.
+
+    """
+
+    def speed(self, speed: Optional[Any] = None, time=0) -> Any:
+        """
+        If no arguments are given, this function returns the current speed.
+
+        If arguments are given, this function sets the speed of the servo:
+
+          - ``speed`` is the speed to change to, between -100 and 100.
+          - ``time`` is the number of milliseconds to take to get to the specified
+            speed.  If omitted, then the servo accelerates as quickly as possible.
+        """
+        ...
+    def pulse_width(self, value: Optional[Any] = None) -> Any:
+        """
+        If no arguments are given, this function returns the current raw pulse-width
+        value.
+
+        If an argument is given, this function sets the raw pulse-width value.
+        """
+        ...
+    def calibration(self, pulse_min, pulse_max, pulse_centre, pulse_angle_90, pulse_speed_100) -> Tuple:
+        """
+        If no arguments are given, this function returns the current calibration
+        data, as a 5-tuple.
+
+        If arguments are given, this function sets the timing calibration:
+
+          - ``pulse_min`` is the minimum allowed pulse width.
+          - ``pulse_max`` is the maximum allowed pulse width.
+          - ``pulse_centre`` is the pulse width corresponding to the centre/zero position.
+          - ``pulse_angle_90`` is the pulse width corresponding to 90 degrees.
+          - ``pulse_speed_100`` is the pulse width corresponding to a speed of 100.
+        """
+        ...
+    def angle(self, angle: Optional[Any] = None, time=0) -> Any:
+        """
+        If no arguments are given, this function returns the current angle.
+
+        If arguments are given, this function sets the angle of the servo:
+
+          - ``angle`` is the angle to move to in degrees.
+          - ``time`` is the number of milliseconds to take to get to the specified
+            angle.  If omitted, then the servo moves as quickly as possible to its
+            new position.
+        """
+        ...
+    def __init__(self, id) -> None: ...
+
+class UART:
+    """
+    Construct a UART object on the given bus.
+    For Pyboard ``bus`` can be 1-4, 6, 'XA', 'XB', 'YA', or 'YB'.
+    For Pyboard Lite ``bus`` can be 1, 2, 6, 'XB', or 'YA'.
+    For Pyboard D ``bus`` can be 1-4, 'XA', 'YA' or 'YB'.
+    With no additional parameters, the UART object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+
+    The physical pins of the UART buses on Pyboard are:
+
+      - ``UART(4)`` is on ``XA``: ``(TX, RX) = (X1, X2) = (PA0, PA1)``
+      - ``UART(1)`` is on ``XB``: ``(TX, RX) = (X9, X10) = (PB6, PB7)``
+      - ``UART(6)`` is on ``YA``: ``(TX, RX) = (Y1, Y2) = (PC6, PC7)``
+      - ``UART(3)`` is on ``YB``: ``(TX, RX) = (Y9, Y10) = (PB10, PB11)``
+      - ``UART(2)`` is on: ``(TX, RX) = (X3, X4) = (PA2, PA3)``
+
+    The Pyboard Lite supports UART(1), UART(2) and UART(6) only, pins are:
+
+      - ``UART(1)`` is on ``XB``: ``(TX, RX) = (X9, X10) = (PB6, PB7)``
+      - ``UART(6)`` is on ``YA``: ``(TX, RX) = (Y1, Y2) = (PC6, PC7)``
+      - ``UART(2)`` is on: ``(TX, RX) = (X1, X2) = (PA2, PA3)``
+
+    The Pyboard D supports UART(1), UART(2), UART(3) and UART(4) only, pins are:
+
+      - ``UART(4)`` is on ``XA``: ``(TX, RX) = (X1, X2) = (PA0, PA1)``
+      - ``UART(1)`` is on ``YA``: ``(TX, RX) = (Y1, Y2) = (PA9, PA10)``
+      - ``UART(3)`` is on ``YB``: ``(TX, RX) = (Y9, Y10) = (PB10, PB11)``
+      - ``UART(2)`` is on: ``(TX, RX) = (X3, X4) = (PA2, PA3)``
+
+    *Note:* Pyboard D has ``UART(1)`` on ``YA``, unlike Pyboard and Pyboard Lite that both
+    have ``UART(1)`` on ``XB`` and ``UART(6)`` on ``YA``.
+    """
+
+    IRQ_RXIDLE: int
+    CTS: int
+    RTS: int
+    def init(self, baudrate, bits=8, parity=None, stop=1, *, timeout=0, flow=0, timeout_char=0, read_buf_len=64) -> Any:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - ``baudrate`` is the clock rate.
+          - ``bits`` is the number of bits per character, 7, 8 or 9.
+          - ``parity`` is the parity, ``None``, 0 (even) or 1 (odd).
+          - ``stop`` is the number of stop bits, 1 or 2.
+          - ``flow`` sets the flow control type. Can be 0, ``UART.RTS``, ``UART.CTS``
+            or ``UART.RTS | UART.CTS``.
+          - ``timeout`` is the timeout in milliseconds to wait for writing/reading the first character.
+          - ``timeout_char`` is the timeout in milliseconds to wait between characters while writing or reading.
+          - ``read_buf_len`` is the character length of the read buffer (0 to disable).
+
+        This method will raise an exception if the baudrate could not be set within
+        5% of the desired value.  The minimum baudrate is dictated by the frequency
+        of the bus that the UART is on; UART(1) and UART(6) are APB2, the rest are on
+        APB1.  The default bus frequencies give a minimum baudrate of 1300 for
+        UART(1) and UART(6) and 650 for the others.  Use :func:`pyb.freq <pyb.freq>`
+        to reduce the bus frequencies to get lower baudrates.
+
+        *Note:* with parity=None, only 8 and 9 bits are supported.  With parity enabled,
+        only 7 and 8 bits are supported.
+        """
+        ...
+    def flush(self, *args, **kwargs) -> Any: ...
+    def irq(self, *args, **kwargs) -> Any: ...
+    def txdone(self, *args, **kwargs) -> Any: ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus.  This drives the bus low for a duration
+        of 13 bits.
+        Return value: ``None``.
+        """
+        ...
+    def readchar(self) -> int:
+        """
+        Receive a single character on the bus.
+
+        Return value: The character read, as an integer.  Returns -1 on timeout.
+        """
+        ...
+    def writechar(self, char) -> None:
+        """
+        Write a single character on the bus.  ``char`` is an integer to write.
+        Return value: ``None``. See note below if CTS flow control is used.
+        """
+        ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes.
+        If ``nbytes`` are available in the buffer, returns immediately, otherwise returns
+        when sufficient characters arrive or the timeout elapses.
+
+        If ``nbytes`` is not given then the method reads as much data as possible.  It
+        returns after the timeout has elapsed.
+
+        *Note:* for 9 bit characters each character takes two bytes, ``nbytes`` must
+        be even, and the number of characters is ``nbytes/2``.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns the number of bytes waiting (may be 0).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.  If characters are 7 or 8 bits wide
+        then each byte is one character.  If characters are 9 bits wide then two
+        bytes are used for each character (little endian), and ``buf`` must contain
+        an even number of bytes.
+
+        Return value: number of bytes written. If a timeout occurs and no bytes
+        were written returns ``None``.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. If such a line exists, return is
+        immediate. If the timeout elapses, all available data is returned regardless
+        of whether a newline exists.
+
+        Return value: the line read or ``None`` on timeout if no data is available.
+        """
+        ...
+    def __init__(
+        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
+    ) -> None: ...
+
+class USB_HID:
+    """
+    Create a new USB_HID object.
+
+    """
+
+    def recv(self, data, *, timeout=5000) -> int:
+        """
+        Receive data on the bus:
+
+          - ``data`` can be an integer, which is the number of bytes to receive,
+            or a mutable buffer, which will be filled with received bytes.
+          - ``timeout`` is the timeout in milliseconds to wait for the receive.
+
+        Return value: if ``data`` is an integer then a new buffer of the bytes received,
+        otherwise the number of bytes read into ``data`` is returned.
+        """
+        ...
+    def send(self, data) -> None:
+        """
+        Send data over the USB HID interface:
+
+          - ``data`` is the data to send (a tuple/list of integers, or a
+            bytearray).
+        """
+        ...
+    def __init__(self) -> None: ...
+
+class I2C:
+    """
+    Construct an I2C object on the given bus.  ``bus`` can be 1 or 2, 'X' or
+    'Y'. With no additional parameters, the I2C object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+
+    The physical pins of the I2C buses on Pyboards V1.0 and V1.1 are:
+
+      - ``I2C(1)`` is on the X position: ``(SCL, SDA) = (X9, X10) = (PB6, PB7)``
+      - ``I2C(2)`` is on the Y position: ``(SCL, SDA) = (Y9, Y10) = (PB10, PB11)``
+
+    On the Pyboard Lite:
+
+      - ``I2C(1)`` is on the X position: ``(SCL, SDA) = (X9, X10) = (PB6, PB7)``
+      - ``I2C(3)`` is on the Y position: ``(SCL, SDA) = (Y9, Y10) = (PA8, PB8)``
+
+    Calling the constructor with 'X' or 'Y' enables portability between Pyboard
+    types.
+    """
+
+    PERIPHERAL: int
+    MASTER: int
+    CONTROLLER: int
+    SLAVE: int
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses from 0x01 to 0x7f and return a list of those that respond.
+        Only valid when in controller mode.
+        """
+        ...
+    def mem_read(self, data, addr, memaddr, *, timeout=5000, addr_size=8) -> Any:
+        """
+        Read from the memory of an I2C device:
+
+          - ``data`` can be an integer (number of bytes to read) or a buffer to read into
+          - ``addr`` is the I2C device address
+          - ``memaddr`` is the memory location within the I2C device
+          - ``timeout`` is the timeout in milliseconds to wait for the read
+          - ``addr_size`` selects width of memaddr: 8 or 16 bits
+
+        Returns the read data.
+        This is only valid in controller mode.
+        """
+        ...
+    def mem_write(self, data, addr, memaddr, *, timeout=5000, addr_size=8) -> None:
+        """
+        Write to the memory of an I2C device:
+
+          - ``data`` can be an integer or a buffer to write from
+          - ``addr`` is the I2C device address
+          - ``memaddr`` is the memory location within the I2C device
+          - ``timeout`` is the timeout in milliseconds to wait for the write
+          - ``addr_size`` selects width of memaddr: 8 or 16 bits
+
+        Returns ``None``.
+        This is only valid in controller mode.
+        """
+        ...
+    def recv(self, recv, addr=0x00, *, timeout=5000) -> bytes:
+        """
+        Receive data on the bus:
+
+          - ``recv`` can be an integer, which is the number of bytes to receive,
+            or a mutable buffer, which will be filled with received bytes
+          - ``addr`` is the address to receive from (only required in controller mode)
+          - ``timeout`` is the timeout in milliseconds to wait for the receive
+
+        Return value: if ``recv`` is an integer then a new buffer of the bytes received,
+        otherwise the same buffer that was passed in to ``recv``.
+        """
+        ...
+    def is_ready(self, addr) -> Any:
+        """
+        Check if an I2C device responds to the given address.  Only valid when in controller mode.
+        """
+        ...
+    def send(self, send, addr=0x00, *, timeout=5000) -> None:
+        """
+        Send data on the bus:
+
+          - ``send`` is the data to send (an integer to send, or a buffer object)
+          - ``addr`` is the address to send to (only required in controller mode)
+          - ``timeout`` is the timeout in milliseconds to wait for the send
+
+        Return value: ``None``.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Turn off the I2C bus.
+        """
+        ...
+    def init(self, mode, *, addr=0x12, baudrate=400000, gencall=False, dma=False) -> None:
+        """
+        Initialise the I2C bus with the given parameters:
+
+           - ``mode`` must be either ``I2C.CONTROLLER`` or ``I2C.PERIPHERAL``
+           - ``addr`` is the 7-bit address (only sensible for a peripheral)
+           - ``baudrate`` is the SCL clock rate (only sensible for a controller)
+           - ``gencall`` is whether to support general call mode
+           - ``dma`` is whether to allow the use of DMA for the I2C transfers (note
+             that DMA transfers have more precise timing but currently do not handle bus
+             errors properly)
+
+         The actual clock frequency may be lower than the requested frequency.
+         This is dependant on the platform hardware. The actual rate may be determined
+         by printing the I2C object.
+        """
+        ...
+    def __init__(
+        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
+    ) -> None: ...
+
+class LED:
+    """
+    Create an LED object associated with the given LED:
+
+      - ``id`` is the LED number, 1-4.
+
+    """
+
+    def toggle(self) -> Any:
+        """
+        Toggle the LED between on (maximum intensity) and off.  If the LED is at
+        non-zero intensity then it is considered "on" and toggle will turn it off.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Turn the LED on, to maximum intensity.
+        """
+        ...
+    def off(self) -> None:
+        """
+        Turn the LED off.
+        """
+        ...
+    def intensity(self, value: Optional[Any] = None) -> None:
+        """
+        Get or set the LED intensity.  Intensity ranges between 0 (off) and 255 (full on).
+        If no argument is given, return the LED intensity.
+        If an argument is given, set the LED intensity and return ``None``.
+
+        *Note:* Only LED(3) and LED(4) can have a smoothly varying intensity, and
+        they use timer PWM to implement it.  LED(3) uses Timer(2) and LED(4) uses
+        Timer(3).  These timers are only configured for PWM if the intensity of the
+        relevant LED is set to a value between 1 and 254.  Otherwise the timers are
+        free for general purpose use.
+        """
+        ...
+    def __init__(self, id) -> None: ...
+
+class LCD:
+    """
+    Construct an LCD object in the given skin position.  ``skin_position`` can be 'X' or 'Y', and
+    should match the position where the LCD pyskin is plugged in.
+
+    """
+
+    def fill(self, colour) -> None:
+        """
+        Fill the screen with the given colour (0 or 1 for white or black).
+
+        This method writes to the hidden buffer.  Use ``show()`` to show the buffer.
+        """
+        ...
+    def light(self, value) -> None:
+        """
+        Turn the backlight on/off.  True or 1 turns it on, False or 0 turns it off.
+        """
+        ...
+    def pixel(self, x, y, colour) -> None:
+        """
+        Set the pixel at ``(x, y)`` to the given colour (0 or 1).
+
+        This method writes to the hidden buffer.  Use ``show()`` to show the buffer.
+        """
+        ...
+    def show(self) -> None:
+        """
+        Show the hidden buffer on the screen.
+        """
+        ...
+    def text(self, str, x, y, colour) -> None:
+        """
+        Draw the given text to the position ``(x, y)`` using the given colour (0 or 1).
+
+        This method writes to the hidden buffer.  Use ``show()`` to show the buffer.
+        """
+        ...
+    def contrast(self, value) -> None:
+        """
+        Set the contrast of the LCD.  Valid values are between 0 and 47.
+        """
+        ...
+    def get(self, x, y) -> int:
+        """
+        Get the pixel at the position ``(x, y)``.  Returns 0 or 1.
+
+        This method reads from the visible buffer.
+        """
+        ...
+    def write(self, str) -> None:
+        """
+        Write the string ``str`` to the screen.  It will appear immediately.
+        """
+        ...
+    def command(self, instr_data, buf) -> None:
+        """
+        Send an arbitrary command to the LCD.  Pass 0 for ``instr_data`` to send an
+        instruction, otherwise pass 1 to send data.  ``buf`` is a buffer with the
+        instructions/data to send.
+        """
+        ...
+    def __init__(self, skin_position) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus.  ``bus`` can be 1 or 2, or
+    'X' or 'Y'. With no additional parameters, the SPI object is created but
+    not initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+
+    The physical pins of the SPI buses are:
+
+      - ``SPI(1)`` is on the X position: ``(NSS, SCK, MISO, MOSI) = (X5, X6, X7, X8) = (PA4, PA5, PA6, PA7)``
+      - ``SPI(2)`` is on the Y position: ``(NSS, SCK, MISO, MOSI) = (Y5, Y6, Y7, Y8) = (PB12, PB13, PB14, PB15)``
+
+    At the moment, the NSS pin is not used by the SPI driver and is free
+    for other use.
+    """
+
+    MASTER: int
+    LSB: int
+    SLAVE: int
+    MSB: int
+    PERIPHERAL: int
+    CONTROLLER: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def send_recv(self, send, recv=None, *, timeout=5000) -> bytes:
+        """
+        Send and receive data on the bus at the same time:
+
+          - ``send`` is the data to send (an integer to send, or a buffer object).
+          - ``recv`` is a mutable buffer which will be filled with received bytes.
+            It can be the same as ``send``, or omitted.  If omitted, a new buffer will
+            be created.
+          - ``timeout`` is the timeout in milliseconds to wait for the receive.
+
+        Return value: the buffer with the received bytes.
+        """
+        ...
+    def recv(self, recv, *, timeout=5000) -> bytes:
+        """
+        Receive data on the bus:
+
+          - ``recv`` can be an integer, which is the number of bytes to receive,
+            or a mutable buffer, which will be filled with received bytes.
+          - ``timeout`` is the timeout in milliseconds to wait for the receive.
+
+        Return value: if ``recv`` is an integer then a new buffer of the bytes received,
+        otherwise the same buffer that was passed in to ``recv``.
+        """
+        ...
+    def init(self, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``mode`` must be either ``SPI.CONTROLLER`` or ``SPI.PERIPHERAL``.
+          - ``baudrate`` is the SCK clock rate (only sensible for a controller).
+          - ``prescaler`` is the prescaler to use to derive SCK from the APB bus frequency;
+            use of ``prescaler`` overrides ``baudrate``.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` can be 8 or 16, and is the number of bits in each transferred word.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``ti`` True indicates Texas Instruments, as opposed to Motorola, signal conventions.
+          - ``crc`` can be None for no CRC, or a polynomial specifier.
+
+        Note that the SPI clock frequency will not always be the requested baudrate.
+        The hardware only supports baudrates that are the APB bus frequency
+        (see :meth:`pyb.freq`) divided by a prescaler, which can be 2, 4, 8, 16, 32,
+        64, 128 or 256.  SPI(1) is on AHB2, and SPI(2) is on AHB1.  For precise
+        control over the SPI clock frequency, specify ``prescaler`` instead of
+        ``baudrate``.
+
+        Printing the SPI object will show you the computed baudrate and the chosen
+        prescaler.
+        """
+        ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def send(self, send, *, timeout=5000) -> None:
+        """
+        Send data on the bus:
+
+          - ``send`` is the data to send (an integer to send, or a buffer object).
+          - ``timeout`` is the timeout in milliseconds to wait for the send.
+
+        Return value: ``None``.
+        """
+        ...
+    def __init__(
+        self, bus, mode, baudrate=328125, *, prescaler=-1, polarity=1, phase=0, bits=8, firstbit=MSB, ti=False, crc=None
+    ) -> None: ...
+
+class Pin:
+    """
+    Create a new Pin object associated with the id.  If additional arguments are given,
+    they are used to initialise the pin.  See :meth:`pin.init`.
+    """
+
+    AF_OD: int
+    AF9_TIM14: int
+    ALT_OPEN_DRAIN: int
+    AF_PP: int
+    ALT: int
+    AF9_CAN1: int
+    AF8_USART6: int
+    AF9_TIM13: int
+    AF9_CAN2: int
+    AF9_TIM12: int
+    PULL_UP: int
+    OUT_PP: int
+    OUT_OD: int
+    ANALOG: int
+    PULL_DOWN: int
+    PULL_NONE: int
+    IRQ_FALLING: int
+    IN: int
+    OUT: int
+    IRQ_RISING: int
+    OPEN_DRAIN: int
+    AF2_TIM5: int
+    AF3_TIM10: int
+    AF3_TIM11: int
+    AF3_TIM8: int
+    AF3_TIM9: int
+    AF2_TIM4: int
+    AF1_TIM1: int
+    AF1_TIM2: int
+    AF2_TIM3: int
+    AF8_UART4: int
+    AF6_I2S2: int
+    AF7_USART1: int
+    AF7_USART2: int
+    AF7_USART3: int
+    AF4_I2C1: int
+    AF5_SPI2: int
+    AF4_I2C2: int
+    AF5_I2S2: int
+    AF5_SPI1: int
+    def mode(self) -> Any:
+        """
+        Returns the currently configured mode of the pin. The integer returned
+        will match one of the allowed constants for the mode argument to the init
+        function.
+        """
+        ...
+    def name(self) -> str:
+        """
+        Get the pin name.
+        """
+        ...
+    def pull(self) -> Any:
+        """
+        Returns the currently configured pull of the pin. The integer returned
+        will match one of the allowed constants for the pull argument to the init
+        function.
+        """
+        ...
+    def low(self, *args, **kwargs) -> Any: ...
+    def irq(self, *args, **kwargs) -> Any: ...
+    def pin(self) -> int:
+        """
+        Get the pin number.
+        """
+        ...
+    def port(self) -> Any:
+        """
+        Get the pin port.
+        """
+        ...
+    def names(self) -> str:
+        """
+        Returns the cpu and board names for this pin.
+        """
+        ...
+    def on(self, *args, **kwargs) -> Any: ...
+    def off(self, *args, **kwargs) -> Any: ...
+    def init(self, mode, pull=PULL_NONE, *, value=None, alt=-1) -> None:
+        """
+        Initialise the pin:
+
+          - *mode* can be one of:
+
+             - ``Pin.IN`` - configure the pin for input;
+             - ``Pin.OUT_PP`` - configure the pin for output, with push-pull control;
+             - ``Pin.OUT_OD`` - configure the pin for output, with open-drain control;
+             - ``Pin.ALT`` - configure the pin for alternate function, input or output;
+             - ``Pin.AF_PP`` - configure the pin for alternate function, push-pull;
+             - ``Pin.AF_OD`` - configure the pin for alternate function, open-drain;
+             - ``Pin.ANALOG`` - configure the pin for analog.
+
+          - *pull* can be one of:
+
+             - ``Pin.PULL_NONE`` - no pull up or down resistors;
+             - ``Pin.PULL_UP`` - enable the pull-up resistor;
+             - ``Pin.PULL_DOWN`` - enable the pull-down resistor.
+
+            When a pin has the ``Pin.PULL_UP`` or ``Pin.PULL_DOWN`` pull-mode enabled,
+            that pin has an effective 40k Ohm resistor pulling it to 3V3 or GND
+            respectively (except pin Y5 which has 11k Ohm resistors).
+
+          - *value* if not None will set the port output value before enabling the pin.
+
+          - *alt* can be used when mode is ``Pin.ALT`` , ``Pin.AF_PP`` or ``Pin.AF_OD`` to
+            set the index or name of one of the alternate functions associated with a pin.
+            This arg was previously called *af* which can still be used if needed.
+
+        Returns: ``None``.
+        """
+        ...
+    def af_list(self) -> List:
+        """
+        Returns an array of alternate functions available for this pin.
+        """
+        ...
+    def af(self) -> Any:
+        """
+        Returns the currently configured alternate-function of the pin. The
+        integer returned will match one of the allowed constants for the af
+        argument to the init function.
+        """
+        ...
+    def value(self, value: Optional[Any] = None) -> int:
+        """
+        Get or set the digital logic level of the pin:
+
+          - With no argument, return 0 or 1 depending on the logic level of the pin.
+          - With ``value`` given, set the logic level of the pin.  ``value`` can be
+            anything that converts to a boolean.  If it converts to ``True``, the pin
+            is set high, otherwise it is set low.
+        """
+        ...
+    def high(self, *args, **kwargs) -> Any: ...
+    def gpio(self) -> int:
+        """
+        Returns the base address of the GPIO block associated with this pin.
+        """
+        ...
+    @classmethod
+    def dict(cls, dict: Optional[Any] = None) -> Any:
+        """
+        Get or set the pin mapper dictionary.
+        """
+        ...
+    @classmethod
+    def debug(cls, state: Optional[Any] = None) -> bool:
+        """
+        Get or set the debugging state (``True`` or ``False`` for on or off).
+        """
+        ...
+
+    class cpu:
+        B9: Any
+        B8: Any
+        B7: Any
+        C0: Any
+        C1: Any
+        C10: Any
+        B3: Any
+        B2: Any
+        B6: Any
+        B4: Any
+        B5: Any
+        B15: Any
+        C7: Any
+        C6: Any
+        C5: Any
+        C8: Any
+        C9: Any
+        C11: Any
+        C13: Any
+        C12: Any
+        C4: Any
+        C2: Any
+        C3: Any
+        D2: Any
+        A15: Any
+        A14: Any
+        A13: Any
+        A2: Any
+        A3: Any
+        A4: Any
+        A1: Any
+        A0: Any
+        A12: Any
+        A10: Any
+        A11: Any
+        B14: Any
+        B11: Any
+        B10: Any
+        B1: Any
+        B12: Any
+        B13: Any
+        A5: Any
+        A7: Any
+        A6: Any
+        B0: Any
+        A8: Any
+        A9: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    @classmethod
+    def mapper(cls, fun: Optional[Any] = None) -> Any:
+        """
+        Get or set the pin mapper function.
+
+        """
+        ...
+
+    class board:
+        X5: Any
+        X18: Any
+        X4: Any
+        X8: Any
+        X6: Any
+        X7: Any
+        X2: Any
+        X3: Any
+        X19: Any
+        X22: Any
+        X20: Any
+        X21: Any
+        Y5: Any
+        X9: Any
+        Y4: Any
+        Y8: Any
+        Y6: Any
+        Y7: Any
+        Y10: Any
+        Y3: Any
+        Y1: Any
+        Y2: Any
+        Y11: Any
+        Y12: Any
+        Y9: Any
+        SD_CK: Any
+        X17: Any
+        SD: Any
+        SD_D1: Any
+        SD_CMD: Any
+        SD_D0: Any
+        LED_GREEN: Any
+        MMA_INT: Any
+        LED_BLUE: Any
+        MMA_AVDD: Any
+        LED_RED: Any
+        LED_YELLOW: Any
+        X1: Any
+        SD_D2: Any
+        USB_VBUS: Any
+        X12: Any
+        X10: Any
+        X11: Any
+        SD_SW: Any
+        USB_ID: Any
+        SD_D3: Any
+        USB_DP: Any
+        SW: Any
+        USB_DM: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    def __init__(self, id, *args, **kwargs) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class SDCard:
+    def writeblocks(self, *args, **kwargs) -> Any: ...
+    def power(self, *args, **kwargs) -> Any: ...
+    def present(self, *args, **kwargs) -> Any: ...
+    def readblocks(self, *args, **kwargs) -> Any: ...
+    def ioctl(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def info(self, *args, **kwargs) -> Any: ...
+    def __init__(self, *argv, **kwargs) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/pyproject.toml` & `micropython_stm32_stubs-1.20.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropython-stm32-stubs"
-version = "1.19.1.post9"
+version = "1.20.0.post1"
 description = "MicroPython stubs"
 authors = [
     "josverl <josverl@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/josverl/micropython-stubs#micropython-stubs"
@@ -29,27 +29,29 @@
     "Programming Language :: Python :: Implementation :: MicroPython",
     "Operating System :: OS Independent",
     "Topic :: Text Editors :: Integrated Development Environments (IDE)",
     "Topic :: Software Development :: Build Tools",
 ]
 packages = [
     { include = "_onewire.pyi" },
+    { include = "_thread.pyi" },
     { include = "_uasyncio.pyi" },
     { include = "array.pyi" },
     { include = "binascii.pyi" },
     { include = "cmath.pyi" },
+    { include = "collections.pyi" },
     { include = "dht.pyi" },
     { include = "errno.pyi" },
     { include = "framebuf.pyi" },
     { include = "gc.pyi" },
     { include = "hashlib.pyi" },
     { include = "heapq.pyi" },
+    { include = "io.pyi" },
     { include = "json.pyi" },
     { include = "lcd160cr.pyi" },
-    { include = "lcd160cr_test.pyi" },
     { include = "machine.pyi" },
     { include = "math.pyi" },
     { include = "micropython.pyi" },
     { include = "network.pyi" },
     { include = "onewire.pyi" },
     { include = "os.pyi" },
     { include = "platform.pyi" },
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/select.pyi` & `micropython_stm32_stubs-1.20.0.post1/select.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
-
-|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
-
-This module provides functions to efficiently wait for events on multiple
-`streams <stream>` (select streams which are ready for operations).
-"""
-from typing import Iterator, List, Optional, Tuple, Any
-
-POLLOUT: int
-POLLIN: int
-POLLHUP: int
-POLLERR: int
-
-class select:
-    """
-    Wait for activity on a set of objects.
-
-    This function is provided by some MicroPython ports for compatibility
-    and is not efficient. Usage of :class:`Poll` is recommended instead.
-    """
-
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
-
-class poll:
-    """
-    Create an instance of the Poll class.
-    """
-
-    def __init__(self) -> None: ...
-    def register(self, obj, eventmask: Optional[Any] = None) -> None:
-        """
-        Register `stream` *obj* for polling. *eventmask* is logical OR of:
-
-        * ``select.POLLIN``  - data available for reading
-        * ``select.POLLOUT`` - more data can be written
-
-        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
-        *not* valid as input eventmask (these are unsolicited events which
-        will be returned from `poll()` regardless of whether they are asked
-        for). This semantics is per POSIX.
-
-        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
-
-        It is OK to call this function multiple times for the same *obj*.
-        Successive calls will update *obj*'s eventmask to the value of
-        *eventmask* (i.e. will behave as `modify()`).
-        """
-        ...
-    def unregister(self, obj) -> Any:
-        """
-        Unregister *obj* from polling.
-        """
-        ...
-    def modify(self, obj, eventmask) -> None:
-        """
-        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
-        is raised with error of ENOENT.
-        """
-        ...
-    def poll(self, timeout=-1, /) -> List:
-        """
-        Wait for at least one of the registered objects to become ready or have an
-        exceptional condition, with optional timeout in milliseconds (if *timeout*
-        arg is not specified or -1, there is no timeout).
-
-        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
-        tuple, depending on a platform and version, so don't assume that its size is 2.
-        The ``event`` element specifies which events happened with a stream and
-        is a combination of ``select.POLL*`` constants described above. Note that
-        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
-        (even if were not asked for), and must be acted on accordingly (the
-        corresponding stream unregistered from poll and likely closed), because
-        otherwise all further invocations of `poll()` may return immediately with
-        these flags set for this stream again.
-
-        In case of timeout, an empty list is returned.
-        """
-        ...
-    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
-        """
-        Like :meth:`poll.poll`, but instead returns an iterator which yields a
-        `callee-owned tuple`. This function provides an efficient, allocation-free
-        way to poll on streams.
-
-        If *flags* is 1, one-shot behaviour for events is employed: streams for
-        which events happened will have their event masks automatically reset
-        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
-        won't be processed until new mask is set with `poll.modify()`. This
-        behaviour is useful for asynchronous I/O schedulers.
-        """
-        ...
+"""
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
+
+|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
+
+This module provides functions to efficiently wait for events on multiple
+`streams <stream>` (select streams which are ready for operations).
+"""
+from typing import Iterator, List, Optional, Tuple, Any
+
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
+
+class select:
+    """
+    Wait for activity on a set of objects.
+
+    This function is provided by some MicroPython ports for compatibility
+    and is not efficient. Usage of :class:`Poll` is recommended instead.
+    """
+
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
+
+class poll:
+    """
+    Create an instance of the Poll class.
+    """
+
+    def __init__(self) -> None: ...
+    def register(self, obj, eventmask: Optional[Any] = None) -> None:
+        """
+        Register `stream` *obj* for polling. *eventmask* is logical OR of:
+
+        * ``select.POLLIN``  - data available for reading
+        * ``select.POLLOUT`` - more data can be written
+
+        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
+        *not* valid as input eventmask (these are unsolicited events which
+        will be returned from `poll()` regardless of whether they are asked
+        for). This semantics is per POSIX.
+
+        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
+
+        It is OK to call this function multiple times for the same *obj*.
+        Successive calls will update *obj*'s eventmask to the value of
+        *eventmask* (i.e. will behave as `modify()`).
+        """
+        ...
+    def unregister(self, obj) -> Any:
+        """
+        Unregister *obj* from polling.
+        """
+        ...
+    def modify(self, obj, eventmask) -> None:
+        """
+        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
+        is raised with error of ENOENT.
+        """
+        ...
+    def poll(self, timeout=-1, /) -> List:
+        """
+        Wait for at least one of the registered objects to become ready or have an
+        exceptional condition, with optional timeout in milliseconds (if *timeout*
+        arg is not specified or -1, there is no timeout).
+
+        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
+        tuple, depending on a platform and version, so don't assume that its size is 2.
+        The ``event`` element specifies which events happened with a stream and
+        is a combination of ``select.POLL*`` constants described above. Note that
+        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
+        (even if were not asked for), and must be acted on accordingly (the
+        corresponding stream unregistered from poll and likely closed), because
+        otherwise all further invocations of `poll()` may return immediately with
+        these flags set for this stream again.
+
+        In case of timeout, an empty list is returned.
+        """
+        ...
+    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
+        """
+        Like :meth:`poll.poll`, but instead returns an iterator which yields a
+        `callee-owned tuple`. This function provides an efficient, allocation-free
+        way to poll on streams.
+
+        If *flags* is 1, one-shot behaviour for events is employed: streams for
+        which events happened will have their event masks automatically reset
+        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
+        won't be processed until new mask is set with `poll.modify()`. This
+        behaviour is useful for asynchronous I/O schedulers.
+        """
+        ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/socket.pyi` & `micropython_stm32_stubs-1.20.0.post1/socket.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-"""
-socket module. See: https://docs.micropython.org/en/v1.19.1/library/socket.html
-
-|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
-
-This module provides access to the BSD socket interface.
-"""
-from typing import IO, Optional, Tuple, Any
-
-SO_KEEPALIVE: int
-SOL_SOCKET: int
-SO_SNDTIMEO: int
-SO_RCVTIMEO: int
-SO_REUSEADDR: int
-AF_INET6: int
-AF_INET: int
-SOCK_STREAM: int
-SOCK_DGRAM: int
-SOCK_RAW: int
-
-def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
-    """
-    Translate the host/port argument into a sequence of 5-tuples that contain all the
-    necessary arguments for creating a socket connected to that service. Arguments
-    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
-    can be used to filter which kind of addresses are returned. If a parameter is not
-    specified or zero, all combinations of addresses can be returned (requiring
-    filtering on the user side).
-
-    The resulting list of 5-tuples has the following structure::
-
-       (family, type, proto, canonname, sockaddr)
-
-    The following example shows how to connect to a given url::
-
-       s = socket.socket()
-       # This assumes that if "type" is not specified, an address for
-       # SOCK_STREAM will be returned, which may be not true
-       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
-
-    Recommended use of filtering params::
-
-       s = socket.socket()
-       # Guaranteed to return an address which can be connect'ed to for
-       # stream operation.
-       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
-    """
-    ...
-
-class socket:
-    """
-    Create a new socket using the given address family, socket type and
-    protocol number. Note that specifying *proto* in most cases is not
-    required (and not recommended, as some MicroPython ports may omit
-    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
-    protocol automatically::
-
-         # Create STREAM TCP socket
-         socket(AF_INET, SOCK_STREAM)
-         # Create DGRAM UDP socket
-         socket(AF_INET, SOCK_DGRAM)
-    """
-
-    def recvfrom(self, bufsize) -> Tuple:
-        """
-        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
-        bytes object representing the data received and *address* is the address of the socket sending
-        the data.
-        """
-        ...
-    def recv(self, bufsize) -> bytes:
-        """
-        Receive data from the socket. The return value is a bytes object representing the data
-        received. The maximum amount of data to be received at once is specified by bufsize.
-        """
-        ...
-    def makefile(self, mode="rb", buffering=0, /) -> IO:
-        """
-        Return a file object associated with the socket. The exact returned type depends on the arguments
-        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
-        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
-        """
-        ...
-    def listen(self, backlog: Optional[Any] = None) -> None:
-        """
-        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
-        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
-        that the system will allow before refusing new connections. If not specified, a default
-        reasonable value is chosen.
-        """
-        ...
-    def settimeout(self, value) -> Any:
-        """
-        **Note**: Not every port supports this method, see below.
-
-        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
-        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
-        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
-        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
-        is put in blocking mode.
-
-        Not every :term:`MicroPython port` supports this method. A more portable and
-        generic solution is to use `select.poll` object. This allows to wait on
-        multiple objects at the same time (and not just on sockets, but on generic
-        `stream` objects which support polling). Example::
-
-             # Instead of:
-             s.settimeout(1.0)  # time in seconds
-             s.read(10)  # may timeout
-
-             # Use:
-             poller = select.poll()
-             poller.register(s, select.POLLIN)
-             res = poller.poll(1000)  # time in milliseconds
-             if not res:
-                 # s is still not ready for input, i.e. operation timed out
-        """
-        ...
-    def sendall(self, bytes) -> int:
-        """
-        Send all data to the socket. The socket must be connected to a remote socket.
-        Unlike `send()`, this method will try to send all of data, by sending data
-        chunk by chunk consecutively.
-
-        The behaviour of this method on non-blocking sockets is undefined. Due to this,
-        on MicroPython, it's recommended to use `write()` method instead, which
-        has the same "no short writes" policy for blocking sockets, and will return
-        number of bytes sent on non-blocking sockets.
-        """
-        ...
-    def setsockopt(self, level, optname, value) -> None:
-        """
-        Set the value of the given socket option. The needed symbolic constants are defined in the
-        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
-        a buffer.
-        """
-        ...
-    def setblocking(self, flag) -> Any:
-        """
-        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
-        else to blocking mode.
-
-        This method is a shorthand for certain `settimeout()` calls:
-
-        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
-        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
-        """
-        ...
-    def sendto(self, bytes, address) -> None:
-        """
-        Send data to the socket. The socket should not be connected to a remote socket, since the
-        destination socket is specified by *address*.
-        """
-        ...
-    def readline(self) -> Any:
-        """
-        Read a line, ending in a newline character.
-
-        Return value: the line read.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the *buf*.  If *nbytes* is specified then read at most
-        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
-        `read()`, this method follows "no short reads" policy.
-
-        Return value: number of bytes read and stored into *buf*.
-        """
-        ...
-    def read(self, size: Optional[Any] = None) -> bytes:
-        """
-        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
-        reads all data available from the socket until EOF; as such the method will not return until
-        the socket is closed. This function tries to read as much data as
-        requested (no "short reads"). This may be not possible with
-        non-blocking socket though, and then less data will be returned.
-        """
-        ...
-    def close(self) -> Any:
-        """
-        Mark the socket closed and release all resources. Once that happens, all future operations
-        on the socket object will fail. The remote end will receive EOF indication if
-        supported by protocol.
-
-        Sockets are automatically closed when they are garbage-collected, but it is recommended
-        to `close()` them explicitly as soon you finished working with them.
-        """
-        ...
-    def connect(self, address) -> None:
-        """
-        Connect to a remote socket at *address*.
-        """
-        ...
-    def send(self, bytes) -> int:
-        """
-        Send data to the socket. The socket must be connected to a remote socket.
-        Returns number of bytes sent, which may be smaller than the length of data
-        ("short write").
-        """
-        ...
-    def bind(self, address) -> Any:
-        """
-        Bind the socket to *address*. The socket must not already be bound.
-        """
-        ...
-    def accept(self) -> Tuple:
-        """
-        Accept a connection. The socket must be bound to an address and listening for connections.
-        The return value is a pair (conn, address) where conn is a new socket object usable to send
-        and receive data on the connection, and address is the address bound to the socket on the
-        other end of the connection.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the socket. This function will try to
-        write all data to a socket (no "short writes"). This may be not possible
-        with a non-blocking socket though, and returned value will be less than
-        the length of *buf*.
-
-        Return value: number of bytes written.
-        """
-        ...
-    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
+"""
+socket module. See: https://docs.micropython.org/en/v1.20.0/library/socket.html
+
+|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
+
+This module provides access to the BSD socket interface.
+"""
+from typing import IO, Optional, Tuple, Any
+
+SO_KEEPALIVE: int
+SOL_SOCKET: int
+SO_SNDTIMEO: int
+SO_RCVTIMEO: int
+SO_REUSEADDR: int
+AF_INET6: int
+AF_INET: int
+SOCK_STREAM: int
+SOCK_DGRAM: int
+SOCK_RAW: int
+
+def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
+    """
+    Translate the host/port argument into a sequence of 5-tuples that contain all the
+    necessary arguments for creating a socket connected to that service. Arguments
+    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
+    can be used to filter which kind of addresses are returned. If a parameter is not
+    specified or zero, all combinations of addresses can be returned (requiring
+    filtering on the user side).
+
+    The resulting list of 5-tuples has the following structure::
+
+       (family, type, proto, canonname, sockaddr)
+
+    The following example shows how to connect to a given url::
+
+       s = socket.socket()
+       # This assumes that if "type" is not specified, an address for
+       # SOCK_STREAM will be returned, which may be not true
+       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
+
+    Recommended use of filtering params::
+
+       s = socket.socket()
+       # Guaranteed to return an address which can be connect'ed to for
+       # stream operation.
+       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
+    """
+    ...
+
+class socket:
+    """
+    Create a new socket using the given address family, socket type and
+    protocol number. Note that specifying *proto* in most cases is not
+    required (and not recommended, as some MicroPython ports may omit
+    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
+    protocol automatically::
+
+         # Create STREAM TCP socket
+         socket(AF_INET, SOCK_STREAM)
+         # Create DGRAM UDP socket
+         socket(AF_INET, SOCK_DGRAM)
+    """
+
+    def recvfrom(self, bufsize) -> Tuple:
+        """
+        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
+        bytes object representing the data received and *address* is the address of the socket sending
+        the data.
+        """
+        ...
+    def recv(self, bufsize) -> bytes:
+        """
+        Receive data from the socket. The return value is a bytes object representing the data
+        received. The maximum amount of data to be received at once is specified by bufsize.
+        """
+        ...
+    def makefile(self, mode="rb", buffering=0, /) -> IO:
+        """
+        Return a file object associated with the socket. The exact returned type depends on the arguments
+        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
+        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
+        """
+        ...
+    def listen(self, backlog: Optional[Any] = None) -> None:
+        """
+        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
+        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
+        that the system will allow before refusing new connections. If not specified, a default
+        reasonable value is chosen.
+        """
+        ...
+    def settimeout(self, value) -> Any:
+        """
+        **Note**: Not every port supports this method, see below.
+
+        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
+        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
+        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
+        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
+        is put in blocking mode.
+
+        Not every :term:`MicroPython port` supports this method. A more portable and
+        generic solution is to use `select.poll` object. This allows to wait on
+        multiple objects at the same time (and not just on sockets, but on generic
+        `stream` objects which support polling). Example::
+
+             # Instead of:
+             s.settimeout(1.0)  # time in seconds
+             s.read(10)  # may timeout
+
+             # Use:
+             poller = select.poll()
+             poller.register(s, select.POLLIN)
+             res = poller.poll(1000)  # time in milliseconds
+             if not res:
+                 # s is still not ready for input, i.e. operation timed out
+        """
+        ...
+    def sendall(self, bytes) -> int:
+        """
+        Send all data to the socket. The socket must be connected to a remote socket.
+        Unlike `send()`, this method will try to send all of data, by sending data
+        chunk by chunk consecutively.
+
+        The behaviour of this method on non-blocking sockets is undefined. Due to this,
+        on MicroPython, it's recommended to use `write()` method instead, which
+        has the same "no short writes" policy for blocking sockets, and will return
+        number of bytes sent on non-blocking sockets.
+        """
+        ...
+    def setsockopt(self, level, optname, value) -> None:
+        """
+        Set the value of the given socket option. The needed symbolic constants are defined in the
+        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
+        a buffer.
+        """
+        ...
+    def setblocking(self, flag) -> Any:
+        """
+        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
+        else to blocking mode.
+
+        This method is a shorthand for certain `settimeout()` calls:
+
+        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
+        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
+        """
+        ...
+    def sendto(self, bytes, address) -> None:
+        """
+        Send data to the socket. The socket should not be connected to a remote socket, since the
+        destination socket is specified by *address*.
+        """
+        ...
+    def readline(self) -> Any:
+        """
+        Read a line, ending in a newline character.
+
+        Return value: the line read.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the *buf*.  If *nbytes* is specified then read at most
+        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
+        `read()`, this method follows "no short reads" policy.
+
+        Return value: number of bytes read and stored into *buf*.
+        """
+        ...
+    def read(self, size: Optional[Any] = None) -> bytes:
+        """
+        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
+        reads all data available from the socket until EOF; as such the method will not return until
+        the socket is closed. This function tries to read as much data as
+        requested (no "short reads"). This may be not possible with
+        non-blocking socket though, and then less data will be returned.
+        """
+        ...
+    def close(self) -> Any:
+        """
+        Mark the socket closed and release all resources. Once that happens, all future operations
+        on the socket object will fail. The remote end will receive EOF indication if
+        supported by protocol.
+
+        Sockets are automatically closed when they are garbage-collected, but it is recommended
+        to `close()` them explicitly as soon you finished working with them.
+        """
+        ...
+    def connect(self, address) -> None:
+        """
+        Connect to a remote socket at *address*.
+        """
+        ...
+    def send(self, bytes) -> int:
+        """
+        Send data to the socket. The socket must be connected to a remote socket.
+        Returns number of bytes sent, which may be smaller than the length of data
+        ("short write").
+        """
+        ...
+    def bind(self, address) -> Any:
+        """
+        Bind the socket to *address*. The socket must not already be bound.
+        """
+        ...
+    def accept(self) -> Tuple:
+        """
+        Accept a connection. The socket must be bound to an address and listening for connections.
+        The return value is a pair (conn, address) where conn is a new socket object usable to send
+        and receive data on the connection, and address is the address bound to the socket on the
+        other end of the connection.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the socket. This function will try to
+        write all data to a socket (no "short writes"). This may be not possible
+        with a non-blocking socket though, and returned value will be less than
+        the length of *buf*.
+
+        Return value: number of bytes written.
+        """
+        ...
+    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/sys.pyi` & `micropython_stm32_stubs-1.20.0.post1/sys.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-system specific functions. See: https://docs.micropython.org/en/v1.19.1/library/sys.html
-
-|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
-"""
-from typing import Dict, List, Tuple, Any
-
-platform: str
-version_info: tuple
-path: list
-version: str
-ps1: str
-ps2: str
-byteorder: str
-modules: dict
-argv: list
-implementation: tuple
-maxsize: int
-
-def print_exception(exc, file=stdout, /) -> None:
-    """
-    Print exception with a traceback to a file-like object *file* (or
-    `sys.stdout` by default).
-    """
-    ...
-
-def exit(retval=0, /) -> Any:
-    """
-    Terminate current program with a given exit code. Underlyingly, this
-    function raise as `SystemExit` exception. If an argument is given, its
-    value given as an argument to `SystemExit`.
-    """
-    ...
-
-stderr: Any
-stdout: Any
-stdin: Any
+"""
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
+
+|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
+"""
+from typing import Dict, List, Tuple, Any
+
+platform: str
+version_info: tuple
+path: list
+version: str
+ps1: str
+ps2: str
+byteorder: str
+modules: dict
+argv: list
+implementation: tuple
+maxsize: int
+
+def print_exception(exc, file=stdout, /) -> None:
+    """
+    Print exception with a traceback to a file-like object *file* (or
+    `sys.stdout` by default).
+    """
+    ...
+
+def exit(retval=0, /) -> Any:
+    """
+    Terminate current program with a given exit code. Underlyingly, this
+    function raise as `SystemExit` exception. If an argument is given, its
+    value given as an argument to `SystemExit`.
+    """
+    ...
+
+stderr: Any
+stdout: Any
+stdin: Any
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/time.pyi` & `micropython_stm32_stubs-1.20.0.post1/time.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
-
-|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
-
-The ``time`` module provides functions for getting the current time and date,
-measuring time intervals, and for delays.
-
-**Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
-
-**Maintaining actual calendar date/time**: This requires a
-Real Time Clock (RTC). On systems with underlying OS (including some
-RTOS), an RTC may be implicit. Setting and maintaining actual calendar
-time is responsibility of OS/RTOS and is done outside of MicroPython,
-it just uses OS API to query date/time. On baremetal ports however
-system time depends on ``machine.RTC()`` object. The current calendar time
-may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
-by following means:
-
-* By a backup battery (which may be an additional, optional component for
-  a particular board).
-* Using networked time protocol (requires setup by a port/user).
-* Set manually by a user on each power-up (many boards then maintain
-  RTC time across hard resets, though some may require setting it again
-  in such case).
-
-If actual calendar time is not maintained with a system/MicroPython RTC,
-functions below which require reference to current absolute time may
-behave not as expected.
-"""
-from typing import Optional, Tuple, Any
-
-def ticks_diff(ticks1, ticks2) -> int:
-    """
-    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
-    or `ticks_cpu()` functions, as a signed value which may wrap around.
-
-    The argument order is the same as for subtraction
-    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
-    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
-    directly using subtraction on them will produce incorrect result. That is why
-    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
-    arithmetics to produce correct result even for wrap-around values (as long as they not
-    too distant inbetween, see below). The function returns **signed** value in the range
-    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
-    two's-complement signed binary integers). If the result is negative, it means that
-    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
-    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
-    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
-    not hold, incorrect result will be returned. Specifically, if two tick values are
-    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
-    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
-    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
-    to the negative range of possible values.
-
-    Informal rationale of the constraints above: Suppose you are locked in a room with no
-    means to monitor passing of time except a standard 12-notch clock. Then if you look at
-    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
-    long sleep), then once you finally look again, it may seem to you that only 1 hour
-    has passed. To avoid this mistake, just look at the clock regularly. Your application
-    should do the same. "Too long sleep" metaphor also maps directly to application
-    behaviour: don't let your application run any single task for too long. Run tasks
-    in steps, and do time-keeping inbetween.
-
-    `ticks_diff()` is designed to accommodate various usage patterns, among them:
-
-    * Polling with timeout. In this case, the order of events is known, and you will deal
-      only with positive results of `ticks_diff()`::
-
-         # Wait for GPIO pin to be asserted, but at most 500us
-         start = time.ticks_us()
-         while pin.value() == 0:
-             if time.ticks_diff(time.ticks_us(), start) > 500:
-                 raise TimeoutError
-
-    * Scheduling events. In this case, `ticks_diff()` result may be negative
-      if an event is overdue::
-
-         # This code snippet is not optimized
-         now = time.ticks_ms()
-         scheduled_time = task.scheduled_time()
-         if ticks_diff(scheduled_time, now) > 0:
-             print("Too early, let's nap")
-             sleep_ms(ticks_diff(scheduled_time, now))
-             task.run()
-         elif ticks_diff(scheduled_time, now) == 0:
-             print("Right at time!")
-             task.run()
-         elif ticks_diff(scheduled_time, now) < 0:
-             print("Oops, running late, tell task to run faster!")
-             task.run(run_faster=true)
-
-    Note: Do not pass `time()` values to `ticks_diff()`, you should use
-    normal mathematical operations on them. But note that `time()` may (and will)
-    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
-
-    """
-    ...
-
-def ticks_add(ticks, delta) -> Any:
-    """
-    Offset ticks value by a given number, which can be either positive or negative.
-    Given a *ticks* value, this function allows to calculate ticks value *delta*
-    ticks before or after it, following modular-arithmetic definition of tick values
-    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
-    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
-    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
-    or numeric expression. `ticks_add()` is useful for calculating deadlines for
-    events/tasks. (Note: you must use `ticks_diff()` function to work with
-    deadlines.)
-
-    Examples::
-
-         # Find out what ticks value there was 100ms ago
-         print(ticks_add(time.ticks_ms(), -100))
-
-         # Calculate deadline for operation and test for it
-         deadline = ticks_add(time.ticks_ms(), 200)
-         while ticks_diff(deadline, time.ticks_ms()) > 0:
-             do_a_little_of_something()
-
-         # Find out TICKS_MAX used by this port
-         print(ticks_add(0, -1))
-
-    """
-    ...
-
-def ticks_cpu() -> Any:
-    """
-    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
-    in the system. This is usually CPU clocks, and that's why the function is named that
-    way. But it doesn't have to be a CPU clock, some other timing source available in a
-    system (e.g. high-resolution timer) can be used instead. The exact timing unit
-    (resolution) of this function is not specified on ``time`` module level, but
-    documentation for a specific port may provide more specific information. This
-    function is intended for very fine benchmarking or very tight real-time loops.
-    Avoid using it in portable code.
-
-    Availability: Not every port implements this function.
-
-    """
-    ...
-
-class time:
-    """
-    Returns the number of seconds, as an integer, since the Epoch, assuming that
-    underlying RTC is set and maintained as described above. If an RTC is not set, this
-    function returns number of seconds since a port-specific reference point in time (for
-    embedded boards without a battery-backed RTC, usually since power up or reset). If you
-    want to develop portable MicroPython application, you should not rely on this function
-    to provide higher than second precision.  If you need higher precision, absolute
-    timestamps, use `time_ns()`.  If relative times are acceptable then use the
-    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
-    `localtime()` without an argument is a better choice.
-    """
-
-    def __init__(self) -> None: ...
-
-def ticks_ms() -> int:
-    """
-    Returns an increasing millisecond counter with an arbitrary reference point, that
-    wraps around after some value.
-
-    The wrap-around value is not explicitly exposed, but we will
-    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
-    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
-    two, but otherwise may differ from port to port. The same period value is used
-    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
-    simplicity). Thus, these functions will return a value in range [*0* ..
-    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
-    non-negative values are used. For the most part, you should treat values returned
-    by these functions as opaque. The only operations available for them are
-    `ticks_diff()` and `ticks_add()` functions described below.
-
-    Note: Performing standard mathematical operations (+, -) or relational
-    operators (<, <=, >, >=) directly on these value will lead to invalid
-    result. Performing mathematical operations and then passing their results
-    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
-    invalid results from the latter functions.
-    """
-    ...
-
-def ticks_us() -> Any:
-    """
-    Just like `ticks_ms()` above, but in microseconds.
-    """
-    ...
-
-def time_ns() -> int:
-    """
-    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
-    a big integer, so will allocate on the heap).
-    """
-    ...
-
-def localtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_us(us) -> None:
-    """
-    Delay for given number of microseconds, should be positive or 0.
-
-    This function attempts to provide an accurate delay of at least *us*
-    microseconds, but it may take longer if the system has other higher priority
-    processing to perform.
-    """
-    ...
-
-def gmtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_ms(ms) -> None:
-    """
-    Delay for given number of milliseconds, should be positive or 0.
-
-    This function will delay for at least the given number of milliseconds, but
-    may take longer than that if other processing must take place, for example
-    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
-    this other processing to occur.  Use `sleep_us()` for more precise delays.
-    """
-    ...
-
-def mktime() -> int:
-    """
-    This is inverse function of localtime. It's argument is a full 8-tuple
-    which expresses a time as per localtime. It returns an integer which is
-    the number of seconds since Jan 1, 2000.
-    """
-    ...
-
-def sleep(seconds) -> Any:
-    """
-    Sleep for the given number of seconds. Some boards may accept *seconds* as a
-    floating-point number to sleep for a fractional number of seconds. Note that
-    other boards may not accept a floating-point argument, for compatibility with
-    them use `sleep_ms()` and `sleep_us()` functions.
-    """
-    ...
+"""
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
+
+|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
+
+The ``time`` module provides functions for getting the current time and date,
+measuring time intervals, and for delays.
+
+**Time Epoch**: Unix port uses standard for POSIX systems epoch of
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
+
+**Maintaining actual calendar date/time**: This requires a
+Real Time Clock (RTC). On systems with underlying OS (including some
+RTOS), an RTC may be implicit. Setting and maintaining actual calendar
+time is responsibility of OS/RTOS and is done outside of MicroPython,
+it just uses OS API to query date/time. On baremetal ports however
+system time depends on ``machine.RTC()`` object. The current calendar time
+may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
+by following means:
+
+* By a backup battery (which may be an additional, optional component for
+  a particular board).
+* Using networked time protocol (requires setup by a port/user).
+* Set manually by a user on each power-up (many boards then maintain
+  RTC time across hard resets, though some may require setting it again
+  in such case).
+
+If actual calendar time is not maintained with a system/MicroPython RTC,
+functions below which require reference to current absolute time may
+behave not as expected.
+"""
+from typing import Optional, Tuple, Any
+
+def ticks_diff(ticks1, ticks2) -> int:
+    """
+    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
+    or `ticks_cpu()` functions, as a signed value which may wrap around.
+
+    The argument order is the same as for subtraction
+    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
+    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
+    directly using subtraction on them will produce incorrect result. That is why
+    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
+    arithmetics to produce correct result even for wrap-around values (as long as they not
+    too distant inbetween, see below). The function returns **signed** value in the range
+    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
+    two's-complement signed binary integers). If the result is negative, it means that
+    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
+    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
+    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
+    not hold, incorrect result will be returned. Specifically, if two tick values are
+    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
+    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
+    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
+    to the negative range of possible values.
+
+    Informal rationale of the constraints above: Suppose you are locked in a room with no
+    means to monitor passing of time except a standard 12-notch clock. Then if you look at
+    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
+    long sleep), then once you finally look again, it may seem to you that only 1 hour
+    has passed. To avoid this mistake, just look at the clock regularly. Your application
+    should do the same. "Too long sleep" metaphor also maps directly to application
+    behaviour: don't let your application run any single task for too long. Run tasks
+    in steps, and do time-keeping inbetween.
+
+    `ticks_diff()` is designed to accommodate various usage patterns, among them:
+
+    * Polling with timeout. In this case, the order of events is known, and you will deal
+      only with positive results of `ticks_diff()`::
+
+         # Wait for GPIO pin to be asserted, but at most 500us
+         start = time.ticks_us()
+         while pin.value() == 0:
+             if time.ticks_diff(time.ticks_us(), start) > 500:
+                 raise TimeoutError
+
+    * Scheduling events. In this case, `ticks_diff()` result may be negative
+      if an event is overdue::
+
+         # This code snippet is not optimized
+         now = time.ticks_ms()
+         scheduled_time = task.scheduled_time()
+         if ticks_diff(scheduled_time, now) > 0:
+             print("Too early, let's nap")
+             sleep_ms(ticks_diff(scheduled_time, now))
+             task.run()
+         elif ticks_diff(scheduled_time, now) == 0:
+             print("Right at time!")
+             task.run()
+         elif ticks_diff(scheduled_time, now) < 0:
+             print("Oops, running late, tell task to run faster!")
+             task.run(run_faster=true)
+
+    Note: Do not pass `time()` values to `ticks_diff()`, you should use
+    normal mathematical operations on them. But note that `time()` may (and will)
+    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
+
+    """
+    ...
+
+def ticks_add(ticks, delta) -> Any:
+    """
+    Offset ticks value by a given number, which can be either positive or negative.
+    Given a *ticks* value, this function allows to calculate ticks value *delta*
+    ticks before or after it, following modular-arithmetic definition of tick values
+    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
+    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
+    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
+    or numeric expression. `ticks_add()` is useful for calculating deadlines for
+    events/tasks. (Note: you must use `ticks_diff()` function to work with
+    deadlines.)
+
+    Examples::
+
+         # Find out what ticks value there was 100ms ago
+         print(ticks_add(time.ticks_ms(), -100))
+
+         # Calculate deadline for operation and test for it
+         deadline = ticks_add(time.ticks_ms(), 200)
+         while ticks_diff(deadline, time.ticks_ms()) > 0:
+             do_a_little_of_something()
+
+         # Find out TICKS_MAX used by this port
+         print(ticks_add(0, -1))
+
+    """
+    ...
+
+def ticks_cpu() -> Any:
+    """
+    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
+    in the system. This is usually CPU clocks, and that's why the function is named that
+    way. But it doesn't have to be a CPU clock, some other timing source available in a
+    system (e.g. high-resolution timer) can be used instead. The exact timing unit
+    (resolution) of this function is not specified on ``time`` module level, but
+    documentation for a specific port may provide more specific information. This
+    function is intended for very fine benchmarking or very tight real-time loops.
+    Avoid using it in portable code.
+
+    Availability: Not every port implements this function.
+
+    """
+    ...
+
+class time:
+    """
+    Returns the number of seconds, as an integer, since the Epoch, assuming that
+    underlying RTC is set and maintained as described above. If an RTC is not set, this
+    function returns number of seconds since a port-specific reference point in time (for
+    embedded boards without a battery-backed RTC, usually since power up or reset). If you
+    want to develop portable MicroPython application, you should not rely on this function
+    to provide higher than second precision.  If you need higher precision, absolute
+    timestamps, use `time_ns()`.  If relative times are acceptable then use the
+    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
+    `localtime()` without an argument is a better choice.
+    """
+
+    def __init__(self) -> None: ...
+
+def ticks_ms() -> int:
+    """
+    Returns an increasing millisecond counter with an arbitrary reference point, that
+    wraps around after some value.
+
+    The wrap-around value is not explicitly exposed, but we will
+    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
+    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
+    two, but otherwise may differ from port to port. The same period value is used
+    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
+    simplicity). Thus, these functions will return a value in range [*0* ..
+    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
+    non-negative values are used. For the most part, you should treat values returned
+    by these functions as opaque. The only operations available for them are
+    `ticks_diff()` and `ticks_add()` functions described below.
+
+    Note: Performing standard mathematical operations (+, -) or relational
+    operators (<, <=, >, >=) directly on these value will lead to invalid
+    result. Performing mathematical operations and then passing their results
+    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
+    invalid results from the latter functions.
+    """
+    ...
+
+def ticks_us() -> Any:
+    """
+    Just like `ticks_ms()` above, but in microseconds.
+    """
+    ...
+
+def time_ns() -> int:
+    """
+    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
+    a big integer, so will allocate on the heap).
+    """
+    ...
+
+def localtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_us(us) -> None:
+    """
+    Delay for given number of microseconds, should be positive or 0.
+
+    This function attempts to provide an accurate delay of at least *us*
+    microseconds, but it may take longer if the system has other higher priority
+    processing to perform.
+    """
+    ...
+
+def gmtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_ms(ms) -> None:
+    """
+    Delay for given number of milliseconds, should be positive or 0.
+
+    This function will delay for at least the given number of milliseconds, but
+    may take longer than that if other processing must take place, for example
+    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
+    this other processing to occur.  Use `sleep_us()` for more precise delays.
+    """
+    ...
+
+def mktime() -> int:
+    """
+    This is inverse function of localtime. It's argument is a full 8-tuple
+    which expresses a time as per localtime. It returns an integer which is
+    the number of seconds since Jan 1, 2000.
+    """
+    ...
+
+def sleep(seconds) -> Any:
+    """
+    Sleep for the given number of seconds. Some boards may accept *seconds* as a
+    floating-point number to sleep for a fractional number of seconds. Note that
+    other boards may not accept a floating-point argument, for compatibility with
+    them use `sleep_ms()` and `sleep_us()` functions.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uarray.pyi` & `micropython_stm32_stubs-1.20.0.post1/uarray.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""
-efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.19.1/library/array.html
-
-|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
-
-Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
-``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
-floating-point support).
-"""
-from typing import Optional, Any
-
-class array:
-    """
-    Create array with elements of given type. Initial contents of the
-    array are given by *iterable*. If it is not provided, an empty
-    array is created.
-    """
-
-    def extend(self, iterable) -> Any:
-        """
-        Append new elements as contained in *iterable* to the end of
-        array, growing it.
-        """
-        ...
-    def decode(self, *args, **kwargs) -> Any: ...
-    def append(self, val) -> Any:
-        """
-        Append new element *val* to the end of array, growing it.
-        """
-        ...
-    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
+"""
+efficient arrays of numeric data. See: https://docs.micropython.org/en/v1.20.0/library/array.html
+
+|see_cpython_module| :mod:`python:array` https://docs.python.org/3/library/array.html .
+
+Supported format codes: ``b``, ``B``, ``h``, ``H``, ``i``, ``I``, ``l``,
+``L``, ``q``, ``Q``, ``f``, ``d`` (the latter 2 depending on the
+floating-point support).
+"""
+from typing import List, Optional, Any
+
+class array:
+    """
+    Create array with elements of given type. Initial contents of the
+    array are given by *iterable*. If it is not provided, an empty
+    array is created.
+    """
+
+    def extend(self, iterable) -> Any:
+        """
+        Append new elements as contained in *iterable* to the end of
+        array, growing it.
+        """
+        ...
+    def append(self, val) -> Any:
+        """
+        Append new element *val* to the end of array, growing it.
+        """
+        ...
+    def __init__(self, typecode, iterable: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uasyncio/core.pyi` & `micropython_stm32_stubs-1.20.0.post1/uasyncio/core.pyi`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from .task import Task as Task, TaskQueue as TaskQueue
-from _typeshed import Incomplete
-
-class CancelledError(BaseException): ...
-class TimeoutError(Exception): ...
-
-_exc_context: Incomplete
-
-class SingletonGenerator:
-    state: Incomplete
-    exc: Incomplete
-    def __init__(self) -> None: ...
-    def __iter__(self): ...
-    def __next__(self) -> None: ...
-
-def sleep_ms(t, sgen=...): ...
-def sleep(t): ...
-
-class IOQueue:
-    poller: Incomplete
-    map: Incomplete
-    def __init__(self) -> None: ...
-    def _enqueue(self, s, idx) -> None: ...
-    def _dequeue(self, s) -> None: ...
-    def queue_read(self, s) -> None: ...
-    def queue_write(self, s) -> None: ...
-    def remove(self, task) -> None: ...
-    def wait_io_event(self, dt) -> None: ...
-
-def _promote_to_task(aw): ...
-def create_task(coro): ...
-def run_until_complete(main_task: Incomplete | None = ...): ...
-def run(coro): ...
-async def _stopper() -> None: ...
-
-_stop_task: Incomplete
-
-class Loop:
-    _exc_handler: Incomplete
-    def create_task(coro): ...
-    def run_forever() -> None: ...
-    def run_until_complete(aw): ...
-    def stop() -> None: ...
-    def close() -> None: ...
-    def set_exception_handler(handler) -> None: ...
-    def get_exception_handler(): ...
-    def default_exception_handler(loop, context) -> None: ...
-    def call_exception_handler(context) -> None: ...
-
-def get_event_loop(runq_len: int = ..., waitq_len: int = ...): ...
-def current_task(): ...
-def new_event_loop(): ...
+from .task import Task as Task, TaskQueue as TaskQueue
+from _typeshed import Incomplete
+
+class CancelledError(BaseException): ...
+class TimeoutError(Exception): ...
+
+_exc_context: Incomplete
+
+class SingletonGenerator:
+    state: Incomplete
+    exc: Incomplete
+    def __init__(self) -> None: ...
+    def __iter__(self): ...
+    def __next__(self) -> None: ...
+
+def sleep_ms(t, sgen=...): ...
+def sleep(t): ...
+
+class IOQueue:
+    poller: Incomplete
+    map: Incomplete
+    def __init__(self) -> None: ...
+    def _enqueue(self, s, idx) -> None: ...
+    def _dequeue(self, s) -> None: ...
+    def queue_read(self, s) -> None: ...
+    def queue_write(self, s) -> None: ...
+    def remove(self, task) -> None: ...
+    def wait_io_event(self, dt) -> None: ...
+
+def _promote_to_task(aw): ...
+def create_task(coro): ...
+def run_until_complete(main_task: Incomplete | None = ...): ...
+def run(coro): ...
+async def _stopper() -> None: ...
+
+_stop_task: Incomplete
+
+class Loop:
+    _exc_handler: Incomplete
+    def create_task(coro): ...
+    def run_forever() -> None: ...
+    def run_until_complete(aw): ...
+    def stop() -> None: ...
+    def close() -> None: ...
+    def set_exception_handler(handler) -> None: ...
+    def get_exception_handler(): ...
+    def default_exception_handler(loop, context) -> None: ...
+    def call_exception_handler(context) -> None: ...
+
+def get_event_loop(runq_len: int = ..., waitq_len: int = ...): ...
+def current_task(): ...
+def new_event_loop(): ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uasyncio/event.pyi` & `micropython_stm32_stubs-1.20.0.post1/uasyncio/event.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import uio
-from . import core as core
-from _typeshed import Incomplete
-from collections.abc import Generator
-
-class Event:
-    state: bool
-    waiting: Incomplete
-    def __init__(self) -> None: ...
-    def is_set(self): ...
-    def set(self) -> None: ...
-    def clear(self) -> None: ...
-    async def wait(self) -> Generator[None, None, Incomplete]: ...
-
-class ThreadSafeFlag(uio.IOBase):
-    _flag: int
-    def __init__(self) -> None: ...
-    def ioctl(self, req, flags): ...
-    def set(self) -> None: ...
-    async def wait(self) -> Generator[Incomplete, None, None]: ...
+import uio
+from . import core as core
+from _typeshed import Incomplete
+from collections.abc import Generator
+
+class Event:
+    state: bool
+    waiting: Incomplete
+    def __init__(self) -> None: ...
+    def is_set(self): ...
+    def set(self) -> None: ...
+    def clear(self) -> None: ...
+    def wait(self) -> Generator[None, None, Incomplete]: ...
+
+class ThreadSafeFlag(uio.IOBase):
+    state: int
+    def __init__(self) -> None: ...
+    def ioctl(self, req, flags): ...
+    def set(self) -> None: ...
+    def clear(self) -> None: ...
+    async def wait(self) -> Generator[Incomplete, None, None]: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uasyncio/stream.pyi` & `micropython_stm32_stubs-1.20.0.post1/uasyncio/stream.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from . import core as core
-from _typeshed import Incomplete
-from collections.abc import Generator
-
-class Stream:
-    s: Incomplete
-    e: Incomplete
-    out_buf: bytes
-    def __init__(self, s, e=...) -> None: ...
-    def get_extra_info(self, v): ...
-    async def __aenter__(self): ...
-    async def __aexit__(self, exc_type, exc, tb) -> None: ...
-    def close(self) -> None: ...
-    async def wait_closed(self) -> None: ...
-    async def read(self, n) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readinto(self, buf) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readexactly(self, n) -> Generator[Incomplete, None, Incomplete]: ...
-    async def readline(self) -> Generator[Incomplete, None, Incomplete]: ...
-    def write(self, buf) -> None: ...
-    async def drain(self) -> Generator[Incomplete, None, None]: ...
-
-StreamReader = Stream
-StreamWriter = Stream
-
-async def open_connection(host, port) -> Generator[Incomplete, None, Incomplete]: ...
-
-class Server:
-    async def __aenter__(self): ...
-    async def __aexit__(self, exc_type, exc, tb) -> None: ...
-    def close(self) -> None: ...
-    async def wait_closed(self) -> None: ...
-    async def _serve(self, s, cb) -> Generator[Incomplete, None, None]: ...
-
-async def start_server(cb, host, port, backlog: int = ...): ...
-async def stream_awrite(self, buf, off: int = ..., sz: int = ...) -> None: ...
+from . import core as core
+from _typeshed import Incomplete
+from collections.abc import Generator
+
+class Stream:
+    s: Incomplete
+    e: Incomplete
+    out_buf: bytes
+    def __init__(self, s, e=...) -> None: ...
+    def get_extra_info(self, v): ...
+    async def __aenter__(self): ...
+    async def __aexit__(self, exc_type, exc, tb) -> None: ...
+    def close(self) -> None: ...
+    async def wait_closed(self) -> None: ...
+    def read(self, n: int = ...) -> Generator[Incomplete, None, Incomplete]: ...
+    def readinto(self, buf) -> Generator[Incomplete, None, Incomplete]: ...
+    def readexactly(self, n) -> Generator[Incomplete, None, Incomplete]: ...
+    def readline(self) -> Generator[Incomplete, None, Incomplete]: ...
+    def write(self, buf) -> None: ...
+    def drain(self) -> Generator[Incomplete, None, Incomplete]: ...
+
+StreamReader = Stream
+StreamWriter = Stream
+
+def open_connection(host, port) -> Generator[Incomplete, None, Incomplete]: ...
+
+class Server:
+    async def __aenter__(self): ...
+    async def __aexit__(self, exc_type, exc, tb) -> None: ...
+    def close(self) -> None: ...
+    async def wait_closed(self) -> None: ...
+    async def _serve(self, s, cb) -> Generator[Incomplete, None, None]: ...
+
+async def start_server(cb, host, port, backlog: int = ...): ...
+async def stream_awrite(self, buf, off: int = ..., sz: int = ...) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/ubinascii.pyi` & `micropython_stm32_stubs-1.20.0.post1/ubinascii.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-binary/ASCII conversions. See: https://docs.micropython.org/en/v1.19.1/library/binascii.html
-
-|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
-
-This module implements conversions between binary data and various
-encodings of it in ASCII form (in both directions).
-"""
-from typing import Optional, Any
-
-def crc32(*args, **kwargs) -> Any: ...
-def hexlify(data, sep: Optional[Any] = None) -> bytes:
-    """
-    Convert the bytes in the *data* object to a hexadecimal representation.
-    Returns a bytes object.
-
-    If the additional argument *sep* is supplied it is used as a separator
-    between hexadecimal values.
-    """
-    ...
-
-def unhexlify(data) -> bytes:
-    """
-    Convert hexadecimal data to binary representation. Returns bytes string.
-    (i.e. inverse of hexlify)
-    """
-    ...
-
-def b2a_base64(data, *, newline=True) -> bytes:
-    """
-    Encode binary data in base64 format, as in `RFC 3548
-    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
-    followed by a newline character if newline is true, as a bytes object.
-    """
-    ...
-
-def a2b_base64(data) -> bytes:
-    """
-    Decode base64-encoded data, ignoring invalid characters in the input.
-    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
-    Returns a bytes object.
-    """
-    ...
+"""
+binary/ASCII conversions. See: https://docs.micropython.org/en/v1.20.0/library/binascii.html
+
+|see_cpython_module| :mod:`python:binascii` https://docs.python.org/3/library/binascii.html .
+
+This module implements conversions between binary data and various
+encodings of it in ASCII form (in both directions).
+"""
+from typing import Optional, Any
+
+def crc32(*args, **kwargs) -> Any: ...
+def hexlify(data, sep: Optional[Any] = None) -> bytes:
+    """
+    Convert the bytes in the *data* object to a hexadecimal representation.
+    Returns a bytes object.
+
+    If the additional argument *sep* is supplied it is used as a separator
+    between hexadecimal values.
+    """
+    ...
+
+def unhexlify(data) -> bytes:
+    """
+    Convert hexadecimal data to binary representation. Returns bytes string.
+    (i.e. inverse of hexlify)
+    """
+    ...
+
+def b2a_base64(data, *, newline=True) -> bytes:
+    """
+    Encode binary data in base64 format, as in `RFC 3548
+    <https://tools.ietf.org/html/rfc3548.html>`_. Returns the encoded data
+    followed by a newline character if newline is true, as a bytes object.
+    """
+    ...
+
+def a2b_base64(data) -> bytes:
+    """
+    Decode base64-encoded data, ignoring invalid characters in the input.
+    Conforms to `RFC 2045 s.6.8 <https://tools.ietf.org/html/rfc2045#section-6.8>`_.
+    Returns a bytes object.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/ucollections.pyi` & `micropython_stm32_stubs-1.20.0.post1/collections.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""
-collection and container types. See: https://docs.micropython.org/en/v1.19.1/library/collections.html
-
-|see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
-
-This module implements advanced collection and container types to
-hold/accumulate various objects.
-"""
-from typing import Optional, Any
-from queue import Queue
-
-def namedtuple(name, fields) -> Any:
-    """
-    This is factory function to create a new namedtuple type with a specific
-    name and set of fields. A namedtuple is a subclass of tuple which allows
-    to access its fields not just by numeric index, but also with an attribute
-    access syntax using symbolic field names. Fields is a sequence of strings
-    specifying field names. For compatibility with CPython it can also be a
-    a string with space-separated field named (but this is less efficient).
-    Example of use::
-
-        from collections import namedtuple
-
-        MyTuple = namedtuple("MyTuple", ("id", "name"))
-        t1 = MyTuple(1, "foo")
-        t2 = MyTuple(2, "bar")
-        print(t1.name)
-        assert t2.name == t2[1]
-    """
-    ...
-
-class OrderedDict:
-    """
-    ``dict`` type subclass which remembers and preserves the order of keys
-    added. When ordered dict is iterated over, keys/items are returned in
-    the order they were added::
-
-        from collections import OrderedDict
-
-        # To make benefit of ordered keys, OrderedDict should be initialized
-        # from sequence of (key, value) pairs.
-        d = OrderedDict([("z", 1), ("a", 2)])
-        # More items can be added as usual
-        d["w"] = 5
-        d["b"] = 3
-        for k, v in d.items():
-            print(k, v)
-
-    Output::
-
-        z 1
-        a 2
-        w 5
-        b 3
-    """
-
-    def popitem(self, *args, **kwargs) -> Any: ...
-    def pop(self, *args, **kwargs) -> Any: ...
-    def values(self, *args, **kwargs) -> Any: ...
-    def setdefault(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def copy(self, *args, **kwargs) -> Any: ...
-    def clear(self, *args, **kwargs) -> Any: ...
-    def keys(self, *args, **kwargs) -> Any: ...
-    def get(self, *args, **kwargs) -> Any: ...
-    def items(self, *args, **kwargs) -> Any: ...
-    @classmethod
-    def fromkeys(cls, *args, **kwargs) -> Any: ...
-    def __init__(self, *args, **kwargs) -> None: ...
-
-class deque:
-    """
-    Deques (double-ended queues) are a list-like container that support O(1)
-    appends and pops from either side of the deque.  New deques are created
-    using the following arguments:
-
-        - *iterable* must be the empty tuple, and the new deque is created empty.
-
-        - *maxlen* must be specified and the deque will be bounded to this
-          maximum length.  Once the deque is full, any new items added will
-          discard items from the opposite end.
-
-        - The optional *flags* can be 1 to check for overflow when adding items.
-
-    As well as supporting `bool` and `len`, deque objects have the following
-    methods:
-    """
-
-    def popleft(self) -> Any:
-        """
-        Remove and return an item from the left side of the deque.
-        Raises IndexError if no items are present.
-        """
-        ...
-    def append(self, x) -> Any:
-        """
-        Add *x* to the right side of the deque.
-        Raises IndexError if overflow checking is enabled and there is no more room left.
-        """
-        ...
-    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
+"""
+collection and container types. See: https://docs.micropython.org/en/v1.20.0/library/collections.html
+
+|see_cpython_module| :mod:`python:collections` https://docs.python.org/3/library/collections.html .
+
+This module implements advanced collection and container types to
+hold/accumulate various objects.
+"""
+from typing import Optional, Any
+from queue import Queue
+
+def namedtuple(name, fields) -> Any:
+    """
+    This is factory function to create a new namedtuple type with a specific
+    name and set of fields. A namedtuple is a subclass of tuple which allows
+    to access its fields not just by numeric index, but also with an attribute
+    access syntax using symbolic field names. Fields is a sequence of strings
+    specifying field names. For compatibility with CPython it can also be a
+    a string with space-separated field named (but this is less efficient).
+    Example of use::
+
+        from collections import namedtuple
+
+        MyTuple = namedtuple("MyTuple", ("id", "name"))
+        t1 = MyTuple(1, "foo")
+        t2 = MyTuple(2, "bar")
+        print(t1.name)
+        assert t2.name == t2[1]
+    """
+    ...
+
+class OrderedDict(dict):
+    """
+    ``dict`` type subclass which remembers and preserves the order of keys
+    added. When ordered dict is iterated over, keys/items are returned in
+    the order they were added::
+
+        from collections import OrderedDict
+
+        # To make benefit of ordered keys, OrderedDict should be initialized
+        # from sequence of (key, value) pairs.
+        d = OrderedDict([("z", 1), ("a", 2)])
+        # More items can be added as usual
+        d["w"] = 5
+        d["b"] = 3
+        for k, v in d.items():
+            print(k, v)
+
+    Output::
+
+        z 1
+        a 2
+        w 5
+        b 3
+    """
+
+    def popitem(self, *args, **kwargs) -> Any: ...
+    def pop(self, *args, **kwargs) -> Any: ...
+    def values(self, *args, **kwargs) -> Any: ...
+    def setdefault(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def copy(self, *args, **kwargs) -> Any: ...
+    def clear(self, *args, **kwargs) -> Any: ...
+    def keys(self, *args, **kwargs) -> Any: ...
+    def get(self, *args, **kwargs) -> Any: ...
+    def items(self, *args, **kwargs) -> Any: ...
+    @classmethod
+    def fromkeys(cls, *args, **kwargs) -> Any: ...
+    def __init__(self, *args, **kwargs) -> None: ...
+
+class deque(Queue):
+    """
+    Deques (double-ended queues) are a list-like container that support O(1)
+    appends and pops from either side of the deque.  New deques are created
+    using the following arguments:
+
+        - *iterable* must be the empty tuple, and the new deque is created empty.
+
+        - *maxlen* must be specified and the deque will be bounded to this
+          maximum length.  Once the deque is full, any new items added will
+          discard items from the opposite end.
+
+        - The optional *flags* can be 1 to check for overflow when adding items.
+
+    As well as supporting `bool` and `len`, deque objects have the following
+    methods:
+    """
+
+    def popleft(self) -> Any:
+        """
+        Remove and return an item from the left side of the deque.
+        Raises IndexError if no items are present.
+        """
+        ...
+    def append(self, x) -> Any:
+        """
+        Add *x* to the right side of the deque.
+        Raises IndexError if overflow checking is enabled and there is no more room left.
+        """
+        ...
+    def __init__(self, iterable, maxlen, flags: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uctypes.pyi` & `micropython_stm32_stubs-1.20.0.post1/uctypes.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-access binary data in a structured way. See: https://docs.micropython.org/en/v1.19.1/library/uctypes.html
-
-This module implements "foreign data interface" for MicroPython. The idea
-behind it is similar to CPython's ``ctypes`` modules, but the actual API is
-different, streamlined and optimized for small size. The basic idea of the
-module is to define data structure layout with about the same power as the
-C language allows, and then access it using familiar dot-syntax to reference
-sub-fields.
-"""
-from typing import Any
-
-VOID: int
-NATIVE: int
-PTR: int
-SHORT: int
-LONGLONG: int
-INT8: int
-LITTLE_ENDIAN: int
-LONG: int
-UINT: int
-ULONG: int
-ULONGLONG: int
-USHORT: int
-UINT8: int
-UINT16: int
-UINT32: int
-UINT64: int
-INT64: int
-BFUINT16: int
-BFUINT32: int
-BFUINT8: int
-BFINT8: int
-ARRAY: int
-BFINT16: int
-BFINT32: int
-BF_LEN: int
-INT: int
-INT16: int
-INT32: int
-FLOAT64: int
-BF_POS: int
-BIG_ENDIAN: int
-FLOAT32: int
-
-def sizeof(struct, layout_type=NATIVE, /) -> int:
-    """
-    Return size of data structure in bytes. The *struct* argument can be
-    either a structure class or a specific instantiated structure object
-    (or its aggregate field).
-    """
-    ...
-
-def bytes_at(addr, size) -> bytes:
-    """
-    Capture memory at the given address and size as bytes object. As bytes
-    object is immutable, memory is actually duplicated and copied into
-    bytes object, so if memory contents change later, created object
-    retains original value.
-    """
-    ...
-
-def bytearray_at(addr, size) -> bytearray:
-    """
-    Capture memory at the given address and size as bytearray object.
-    Unlike bytes_at() function above, memory is captured by reference,
-    so it can be both written too, and you will access current value
-    at the given memory address.
-    """
-    ...
-
-def addressof(obj) -> int:
-    """
-    Return address of an object. Argument should be bytes, bytearray or
-    other object supporting buffer protocol (and address of this buffer
-    is what actually returned).
-    """
-    ...
-
-class struct:
-    """
-    Instantiate a "foreign data structure" object based on structure address in
-    memory, descriptor (encoded as a dictionary), and layout type (see below).
-    """
-
-    def __init__(self, addr, descriptor, layout_type=NATIVE, /) -> None: ...
+"""
+access binary data in a structured way. See: https://docs.micropython.org/en/v1.20.0/library/uctypes.html
+
+This module implements "foreign data interface" for MicroPython. The idea
+behind it is similar to CPython's ``ctypes`` modules, but the actual API is
+different, streamlined and optimized for small size. The basic idea of the
+module is to define data structure layout with about the same power as the
+C language allows, and then access it using familiar dot-syntax to reference
+sub-fields.
+"""
+from typing import Any
+
+VOID: int
+NATIVE: int
+PTR: int
+SHORT: int
+LONGLONG: int
+INT8: int
+LITTLE_ENDIAN: int
+LONG: int
+UINT: int
+ULONG: int
+ULONGLONG: int
+USHORT: int
+UINT8: int
+UINT16: int
+UINT32: int
+UINT64: int
+INT64: int
+BFUINT16: int
+BFUINT32: int
+BFUINT8: int
+BFINT8: int
+ARRAY: int
+BFINT16: int
+BFINT32: int
+BF_LEN: int
+INT: int
+INT16: int
+INT32: int
+FLOAT64: int
+BF_POS: int
+BIG_ENDIAN: int
+FLOAT32: int
+
+def sizeof(struct, layout_type=NATIVE, /) -> int:
+    """
+    Return size of data structure in bytes. The *struct* argument can be
+    either a structure class or a specific instantiated structure object
+    (or its aggregate field).
+    """
+    ...
+
+def bytes_at(addr, size) -> bytes:
+    """
+    Capture memory at the given address and size as bytes object. As bytes
+    object is immutable, memory is actually duplicated and copied into
+    bytes object, so if memory contents change later, created object
+    retains original value.
+    """
+    ...
+
+def bytearray_at(addr, size) -> bytearray:
+    """
+    Capture memory at the given address and size as bytearray object.
+    Unlike bytes_at() function above, memory is captured by reference,
+    so it can be both written too, and you will access current value
+    at the given memory address.
+    """
+    ...
+
+def addressof(obj) -> int:
+    """
+    Return address of an object. Argument should be bytes, bytearray or
+    other object supporting buffer protocol (and address of this buffer
+    is what actually returned).
+    """
+    ...
+
+class struct:
+    """
+    Instantiate a "foreign data structure" object based on structure address in
+    memory, descriptor (encoded as a dictionary), and layout type (see below).
+    """
+
+    def __init__(self, addr, descriptor, layout_type=NATIVE, /) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uhashlib.pyi` & `micropython_stm32_stubs-1.20.0.post1/uhashlib.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-hashing algorithms. See: https://docs.micropython.org/en/v1.19.1/library/hashlib.html
-
-|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
-
-This module implements binary data hashing algorithms. The exact inventory
-of available algorithms depends on a board. Among the algorithms which may
-be implemented:
-
-* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
-  It is suitable for cryptographically-secure purposes. Included in the
-  MicroPython core and any board is recommended to provide this, unless
-  it has particular code size constraints.
-
-* SHA1 - A previous generation algorithm. Not recommended for new usages,
-  but SHA1 is a part of number of Internet standards and existing
-  applications, so boards targeting network connectivity and
-  interoperability will try to provide this.
-
-* MD5 - A legacy algorithm, not considered cryptographically secure. Only
-  selected boards, targeting interoperability with legacy applications,
-  will offer this.
-"""
-from typing import Optional, Any
-
-class sha256:
-    """
-    Create an SHA256 hasher object and optionally feed ``data`` into it.
-    """
-
-    def digest(self, *args, **kwargs) -> Any: ...
-    def update(self, *args, **kwargs) -> Any: ...
-    def __init__(self, data: Optional[Any] = None) -> None: ...
+"""
+hashing algorithms. See: https://docs.micropython.org/en/v1.20.0/library/hashlib.html
+
+|see_cpython_module| :mod:`python:hashlib` https://docs.python.org/3/library/hashlib.html .
+
+This module implements binary data hashing algorithms. The exact inventory
+of available algorithms depends on a board. Among the algorithms which may
+be implemented:
+
+* SHA256 - The current generation, modern hashing algorithm (of SHA2 series).
+  It is suitable for cryptographically-secure purposes. Included in the
+  MicroPython core and any board is recommended to provide this, unless
+  it has particular code size constraints.
+
+* SHA1 - A previous generation algorithm. Not recommended for new usages,
+  but SHA1 is a part of number of Internet standards and existing
+  applications, so boards targeting network connectivity and
+  interoperability will try to provide this.
+
+* MD5 - A legacy algorithm, not considered cryptographically secure. Only
+  selected boards, targeting interoperability with legacy applications,
+  will offer this.
+"""
+from typing import Optional, Any
+
+class sha256:
+    """
+    Create an SHA256 hasher object and optionally feed ``data`` into it.
+    """
+
+    def digest(self, *args, **kwargs) -> Any: ...
+    def update(self, *args, **kwargs) -> Any: ...
+    def __init__(self, data: Optional[Any] = None) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uheapq.pyi` & `micropython_stm32_stubs-1.20.0.post1/uheapq.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-heap queue algorithm. See: https://docs.micropython.org/en/v1.19.1/library/heapq.html
-
-|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
-
-This module implements the
-`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
-
-A heap queue is essentially a list that has its elements stored in such a way
-that the first item of the list is always the smallest.
-"""
-from typing import Any
-
-def heappop(heap) -> Any:
-    """
-    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
-    ``heap`` is empty.
-
-    The returned item will be the smallest item in the ``heap``.
-    """
-    ...
-
-def heappush(heap, item) -> Any:
-    """
-    Push the ``item`` onto the ``heap``.
-    """
-    ...
-
-def heapify(x) -> Any:
-    """
-    Convert the list ``x`` into a heap.  This is an in-place operation.
-    """
-    ...
+"""
+heap queue algorithm. See: https://docs.micropython.org/en/v1.20.0/library/heapq.html
+
+|see_cpython_module| :mod:`python:heapq` https://docs.python.org/3/library/heapq.html .
+
+This module implements the
+`min heap queue algorithm <https://en.wikipedia.org/wiki/Heap_%28data_structure%29>`_.
+
+A heap queue is essentially a list that has its elements stored in such a way
+that the first item of the list is always the smallest.
+"""
+from typing import Any
+
+def heappop(heap) -> Any:
+    """
+    Pop the first item from the ``heap``, and return it.  Raise ``IndexError`` if
+    ``heap`` is empty.
+
+    The returned item will be the smallest item in the ``heap``.
+    """
+    ...
+
+def heappush(heap, item) -> Any:
+    """
+    Push the ``item`` onto the ``heap``.
+    """
+    ...
+
+def heapify(x) -> Any:
+    """
+    Convert the list ``x`` into a heap.  This is an in-place operation.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/umachine.pyi` & `micropython_stm32_stubs-1.20.0.post1/umachine.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,1204 +1,1273 @@
-"""
-functions related to the hardware. See: https://docs.micropython.org/en/v1.19.1/library/machine.html
-
-The ``machine`` module contains specific functions related to the hardware
-on a particular board. Most functions in this module allow to achieve direct
-and unrestricted access to and control of hardware blocks on a system
-(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
-malfunction, lockups, crashes of your board, and in extreme cases, hardware
-damage.
-"""
-from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
-
-HARD_RESET: int
-PWRON_RESET: int
-SOFT_RESET: int
-DEEPSLEEP_RESET: int
-WDT_RESET: int
-
-def idle() -> Any:
-    """
-    Gates the clock to the CPU, useful to reduce power consumption at any time during
-    short or long periods. Peripherals continue working and execution resumes as soon
-    as any interrupt is triggered (on many ports this includes system timer
-    interrupt occurring at regular intervals on the order of millisecond).
-    """
-    ...
-
-def freq(hz: Optional[Any] = None) -> Any:
-    """
-    Returns the CPU frequency in hertz.
-
-    On some ports this can also be used to set the CPU frequency by passing in *hz*.
-    """
-    ...
-
-def info(*args, **kwargs) -> Any: ...
-def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def enable_irq(state) -> Any:
-    """
-    Re-enable interrupt requests.
-    The *state* parameter should be the value that was returned from the most
-    recent call to the `disable_irq()` function.
-    """
-    ...
-
-def disable_irq() -> Any:
-    """
-    Disable interrupt requests.
-    Returns the previous IRQ state which should be considered an opaque value.
-    This return value should be passed to the `enable_irq()` function to restore
-    interrupts to their original state, before `disable_irq()` was called.
-    """
-    ...
-
-def unique_id() -> bytes:
-    """
-    Returns a byte string with a unique identifier of a board/SoC. It will vary
-    from a board/SoC instance to another, if underlying hardware allows. Length
-    varies by hardware (so use substring of a full value if you expect a short
-    ID). In some MicroPython ports, ID corresponds to the network MAC address.
-    """
-    ...
-
-def soft_reset() -> NoReturn:
-    """
-    Performs a soft reset of the interpreter, deleting all Python objects and
-    resetting the Python heap.  It tries to retain the method by which the user
-    is connected to the MicroPython REPL (eg serial, USB, Wifi).
-    """
-    ...
-
-def sleep() -> Any:
-    """
-    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
-    """
-    ...
-
-def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
-    """
-    Time a pulse on the given *pin*, and return the duration of the pulse in
-    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
-    or 1 to time a high pulse.
-
-    If the current input value of the pin is different to *pulse_level*,
-    the function first (*) waits until the pin input becomes equal to *pulse_level*,
-    then (**) times the duration that the pin is equal to *pulse_level*.
-    If the pin is already equal to *pulse_level* then timing starts straight away.
-
-    The function will return -2 if there was timeout waiting for condition marked
-    (*) above, and -1 if there was timeout during the main measurement, marked (**)
-    above. The timeout is the same for both cases and given by *timeout_us* (which
-    is in microseconds).
-    """
-    ...
-
-def lightsleep(time_ms: Optional[Any] = None) -> Any:
-    """
-    Stops execution in an attempt to enter a low power state.
-
-    If *time_ms* is specified then this will be the maximum time in milliseconds that
-    the sleep will last for.  Otherwise the sleep can last indefinitely.
-
-    With or without a timeout, execution may resume at any time if there are events
-    that require processing.  Such events, or wake sources, should be configured before
-    sleeping, like `Pin` change or `RTC` timeout.
-
-    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
-    highly dependent on the underlying hardware, but the general properties are:
-
-    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
-      from the point where the sleep was requested, with all subsystems operational.
-
-    * A deepsleep may not retain RAM or any other state of the system (for example
-      peripherals or network interfaces).  Upon wake execution is resumed from the main
-      script, similar to a hard or power-on reset. The `reset_cause()` function will
-      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
-      from other resets.
-    """
-    ...
-
-def reset() -> NoReturn:
-    """
-    Resets the device in a manner similar to pushing the external RESET
-    button.
-    """
-    ...
-
-def rng() -> int:
-    """
-    Return a 24-bit software generated random number.
-
-    Availability: WiPy.
-    """
-    ...
-
-def reset_cause() -> int:
-    """
-    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
-    """
-    ...
-
-def bootloader(value: Optional[Any] = None) -> None:
-    """
-    Reset the device and enter its bootloader.  This is typically used to put the
-    device into a state where it can be programmed with new firmware.
-
-    Some ports support passing in an optional *value* argument which can control
-    which bootloader to enter, what to pass to it, or other things.
-    """
-    ...
-
-def bitstream(pin, encoding, timing, data, /) -> Any:
-    """
-    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
-    specifies how the bits are encoded, and *timing* is an encoding-specific timing
-    specification.
-
-    The supported encodings are:
-
-      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
-        1 bits as timed pulses, starting with the most significant bit.
-        The *timing* must be a four-tuple of nanoseconds in the format
-        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
-        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
-        at 800kHz.
-
-    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
-    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
-    will be closer to +/-30ns.
-
-    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
-       module for a higher-level API.
-    """
-    ...
-
-class Pin:
-    """
-    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
-    additional arguments are given in the constructor then they are used to initialise
-    the pin.  Any settings that are not specified will remain in their previous state.
-
-    The arguments are:
-
-      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
-        types are: int (an internal Pin identifier), str (a Pin name), and tuple
-        (pair of [port, pin]).
-
-      - ``mode`` specifies the pin mode, which can be one of:
-
-        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
-          is in high-impedance state.
-
-        - ``Pin.OUT`` - Pin is configured for (normal) output.
-
-        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
-          output works in the following way: if the output value is set to 0 the pin
-          is active at a low level; if the output value is 1 the pin is in a high-impedance
-          state.  Not all ports implement this mode, or some might only on certain pins.
-
-        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
-          port specific.  For a pin configured in such a way any other Pin methods
-          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
-          or a hardware-specific, result).  Not all ports implement this mode.
-
-        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
-          open-drain.  Not all ports implement this mode.
-
-        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
-
-      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
-        one of:
-
-        - ``None`` - No pull up or down resistor.
-        - ``Pin.PULL_UP`` - Pull up resistor enabled.
-        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
-
-      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
-        output pin value if given, otherwise the state of the pin peripheral remains
-        unchanged.
-
-      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
-        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
-        capabilities are port dependent.  Not all ports implement this argument.
-
-      - ``alt`` specifies an alternate function for the pin and the values it can take are
-        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
-        modes.  It may be used when a pin supports more than one alternate function.  If only
-        one pin alternate function is supported the this argument is not required.  Not all
-        ports implement this argument.
-
-    As specified above, the Pin class allows to set an alternate function for a particular
-    pin, but it does not specify any further operations on such a pin.  Pins configured in
-    alternate-function mode are usually not used as GPIO but are instead driven by other
-    hardware peripherals.  The only operation supported on such a pin is re-initialising,
-    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
-    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
-    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
-    """
-
-    AF_OD: int
-    AF9_TIM14: int
-    ALT_OPEN_DRAIN: int
-    AF_PP: int
-    ALT: int
-    AF9_CAN1: int
-    AF8_USART6: int
-    AF9_TIM13: int
-    AF9_CAN2: int
-    AF9_TIM12: int
-    PULL_UP: int
-    OUT_PP: int
-    OUT_OD: int
-    ANALOG: int
-    PULL_DOWN: int
-    PULL_NONE: int
-    IRQ_FALLING: int
-    IN: int
-    OUT: int
-    IRQ_RISING: int
-    OPEN_DRAIN: int
-    AF2_TIM5: int
-    AF3_TIM10: int
-    AF3_TIM11: int
-    AF3_TIM8: int
-    AF3_TIM9: int
-    AF2_TIM4: int
-    AF1_TIM1: int
-    AF1_TIM2: int
-    AF2_TIM3: int
-    AF8_UART4: int
-    AF6_I2S2: int
-    AF7_USART1: int
-    AF7_USART2: int
-    AF7_USART3: int
-    AF4_I2C1: int
-    AF5_SPI2: int
-    AF4_I2C2: int
-    AF5_I2S2: int
-    AF5_SPI1: int
-    def mode(self, mode: Optional[Any] = None) -> Any:
-        """
-        Get or set the pin mode.
-        See the constructor documentation for details of the ``mode`` argument.
-
-        Availability: cc3200, stm32 ports.
-        """
-        ...
-    def name(self, *args, **kwargs) -> Any: ...
-    def pull(self, pull: Optional[Any] = None) -> Any:
-        """
-        Get or set the pin pull state.
-        See the constructor documentation for details of the ``pull`` argument.
-
-        Availability: cc3200, stm32 ports.
-        """
-        ...
-    def low(self) -> None:
-        """
-        Set pin to "0" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
-        """
-           Configure an interrupt handler to be called when the trigger source of the
-           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
-           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
-           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
-           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
-           state '0' and the external pin value for state '1'.
-
-           The arguments are:
-
-             - ``handler`` is an optional function to be called when the interrupt
-               triggers. The handler must take exactly one argument which is the
-               ``Pin`` instance.
-
-             - ``trigger`` configures the event which can generate an interrupt.
-               Possible values are:
-
-               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
-               - ``Pin.IRQ_RISING`` interrupt on rising edge.
-               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
-               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
-
-               These values can be OR'ed together to trigger on multiple events.
-
-             - ``priority`` sets the priority level of the interrupt.  The values it
-               can take are port-specific, but higher values always represent higher
-               priorities.
-
-             - ``wake`` selects the power mode in which this interrupt can wake up the
-               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
-               These values can also be OR'ed together to make a pin generate interrupts in
-               more than one power mode.
-
-             - ``hard`` if true a hardware interrupt is used. This reduces the delay
-               between the pin change and the handler being called. Hard interrupt
-               handlers may not allocate memory; see :ref:`isr_rules`.
-               Not all ports support this argument.
-
-           This method returns a callback object.
-
-        The following methods are not part of the core Pin API and only implemented on certain ports.
-        """
-        ...
-    def pin(self, *args, **kwargs) -> Any: ...
-    def port(self, *args, **kwargs) -> Any: ...
-    def names(self, *args, **kwargs) -> Any: ...
-    def on(self) -> None:
-        """
-        Set pin to "1" output level.
-        """
-        ...
-    def off(self) -> None:
-        """
-        Set pin to "0" output level.
-        """
-        ...
-    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
-        """
-        Re-initialise the pin using the given parameters.  Only those arguments that
-        are specified will be set.  The rest of the pin peripheral state will remain
-        unchanged.  See the constructor documentation for details of the arguments.
-
-        Returns ``None``.
-        """
-        ...
-    def af_list(self, *args, **kwargs) -> Any: ...
-    def af(self, *args, **kwargs) -> Any: ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the pin, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the digital logic level of
-        the pin, returning 0 or 1 corresponding to low and high voltage signals
-        respectively.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The method returns the actual input value currently present
-            on the pin.
-          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
-          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
-            return value of the method is undefined.  Otherwise, if the pin is in
-            state '1', the method returns the actual input value currently present
-            on the pin.
-
-        If the argument is supplied then this method sets the digital logic level of
-        the pin.  The argument ``x`` can be anything that converts to a boolean.
-        If it converts to ``True``, the pin is set to state '1', otherwise it is set
-        to state '0'.  The behaviour of this method depends on the mode of the pin:
-
-          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
-            pin state does not change, it remains in the high-impedance state.  The
-            stored value will become active on the pin as soon as it is changed to
-            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
-          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
-          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
-            state.  Otherwise the pin is set to high-impedance state.
-
-        When setting the value this method returns ``None``.
-        """
-        ...
-    def high(self) -> None:
-        """
-        Set pin to "1" output level.
-
-        Availability: nrf, rp2, stm32 ports.
-        """
-        ...
-    def gpio(self, *args, **kwargs) -> Any: ...
-    @classmethod
-    def dict(cls, *args, **kwargs) -> Any: ...
-    @classmethod
-    def debug(cls, *args, **kwargs) -> Any: ...
-
-    class cpu:
-        B9: Any
-        B8: Any
-        B7: Any
-        C0: Any
-        C1: Any
-        C10: Any
-        B3: Any
-        B2: Any
-        B6: Any
-        B4: Any
-        B5: Any
-        B15: Any
-        C7: Any
-        C6: Any
-        C5: Any
-        C8: Any
-        C9: Any
-        C11: Any
-        C13: Any
-        C12: Any
-        C4: Any
-        C2: Any
-        C3: Any
-        D2: Any
-        A15: Any
-        A14: Any
-        A13: Any
-        A2: Any
-        A3: Any
-        A4: Any
-        A1: Any
-        A0: Any
-        A12: Any
-        A10: Any
-        A11: Any
-        B14: Any
-        B11: Any
-        B10: Any
-        B1: Any
-        B12: Any
-        B13: Any
-        A5: Any
-        A7: Any
-        A6: Any
-        B0: Any
-        A8: Any
-        A9: Any
-        def __init__(self, *argv, **kwargs) -> None: ...
-
-    @classmethod
-    def mapper(cls, *args, **kwargs) -> Any: ...
-
-    class board:
-        X5: Any
-        X18: Any
-        X4: Any
-        X8: Any
-        X6: Any
-        X7: Any
-        X2: Any
-        X3: Any
-        X19: Any
-        X22: Any
-        X20: Any
-        X21: Any
-        Y5: Any
-        X9: Any
-        Y4: Any
-        Y8: Any
-        Y6: Any
-        Y7: Any
-        Y10: Any
-        Y3: Any
-        Y1: Any
-        Y2: Any
-        Y11: Any
-        Y12: Any
-        Y9: Any
-        SD_CK: Any
-        X17: Any
-        SD: Any
-        SD_D1: Any
-        SD_CMD: Any
-        SD_D0: Any
-        LED_GREEN: Any
-        MMA_INT: Any
-        LED_BLUE: Any
-        MMA_AVDD: Any
-        LED_RED: Any
-        LED_YELLOW: Any
-        X1: Any
-        SD_D2: Any
-        USB_VBUS: Any
-        X12: Any
-        X10: Any
-        X11: Any
-        SD_SW: Any
-        USB_ID: Any
-        SD_D3: Any
-        USB_DP: Any
-        SW: Any
-        USB_DM: Any
-        def __init__(self, *argv, **kwargs) -> None: ...
-
-    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
-
-class I2S:
-    """
-    Construct an I2S object of the given id:
-
-    - ``id`` identifies a particular I2S bus; it is board and port specific
-
-    Keyword-only parameters that are supported on all ports:
-
-      - ``sck`` is a pin object for the serial clock line
-      - ``ws`` is a pin object for the word select line
-      - ``sd`` is a pin object for the serial data line
-      - ``mck`` is a pin object for the master clock line;
-        master clock frequency is sampling rate * 256
-      - ``mode`` specifies receive or transmit
-      - ``bits`` specifies sample size (bits), 16 or 32
-      - ``format`` specifies channel format, STEREO or MONO
-      - ``rate`` specifies audio sampling rate (Hz);
-        this is the frequency of the ``ws`` signal
-      - ``ibuf`` specifies internal buffer length (bytes)
-
-    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
-    sample data is transfered between the internal buffer and the I2S peripheral unit.
-    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
-    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
-    """
-
-    RX: int
-    MONO: int
-    STEREO: int
-    TX: int
-    @staticmethod
-    def shift(*, buf, bits, shift) -> Any:
-        """
-        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
-        Positive for left shift, negative for right shift.
-        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
-        """
-        ...
-    def init(self, sck, *args, **kwargs) -> Any:
-        """
-        see Constructor for argument descriptions
-        """
-        ...
-    def irq(self, handler) -> Any:
-        """
-        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
-        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
-        ``handler`` is called in the context of the MicroPython scheduler.
-        """
-        ...
-    def readinto(self, buf) -> int:
-        """
-        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the left channel sample data is used.
-        Returns number of bytes read
-        """
-        ...
-    def deinit(self) -> Any:
-        """
-        Deinitialize the I2S bus
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
-        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
-        the sample data is written to both the right and left channels.
-        Returns number of bytes written
-        """
-        ...
-    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
-
-class SPI:
-    """
-    Construct an SPI object on the given bus, *id*. Values of *id* depend
-    on a particular port and its hardware. Values 0, 1, etc. are commonly used
-    to select hardware SPI block #0, #1, etc.
-
-    With no additional parameters, the SPI object is created but not
-    initialised (it has the settings from the last initialisation of
-    the bus, if any).  If extra arguments are given, the bus is initialised.
-    See ``init`` for parameters of initialisation.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self) -> None:
-        """
-        Turn off the SPI bus.
-        """
-        ...
-    def init(
-        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
-    ) -> None:
-        """
-        Initialise the SPI bus with the given parameters:
-
-          - ``baudrate`` is the SCK clock rate.
-          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
-          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
-            respectively.
-          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
-          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
-          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
-            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
-            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
-            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
-            (``id`` = -1).
-          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
-            specify them as a tuple of ``pins`` parameter.
-
-        In the case of hardware SPI the actual clock frequency may be lower than the
-        requested baudrate. This is dependant on the platform hardware. The actual
-        rate may be determined by printing the SPI object.
-        """
-        ...
-    def write_readinto(self, write_buf, read_buf) -> int:
-        """
-        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
-        buffers can be the same or different, but both buffers must have the
-        same length.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def read(self, nbytes, write=0x00) -> bytes:
-        """
-        Read a number of bytes specified by ``nbytes`` while continuously writing
-        the single byte given by ``write``.
-        Returns a ``bytes`` object with the data that was read.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes contained in ``buf``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes written.
-        """
-        ...
-    def readinto(self, buf, write=0x00) -> int:
-        """
-        Read into the buffer specified by ``buf`` while continuously writing the
-        single byte given by ``write``.
-        Returns ``None``.
-
-        Note: on WiPy this function returns the number of bytes read.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-mem8: Any
-
-class RTC:
-    """
-    Create an RTC object. See init for parameters of initialization.
-    """
-
-    def info(self, *args, **kwargs) -> Any: ...
-    def init(self, datetime) -> None:
-        """
-        Initialise the RTC. Datetime is a tuple of the form:
-
-           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
-        """
-        ...
-    def wakeup(self, *args, **kwargs) -> Any: ...
-    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
-        """
-        Get or set the date and time of the RTC.
-
-        With no arguments, this method returns an 8-tuple with the current
-        date and time.  With 1 argument (being an 8-tuple) it sets the date
-        and time.
-
-        The 8-tuple has the following format:
-
-            (year, month, day, weekday, hours, minutes, seconds, subseconds)
-
-        The meaning of the ``subseconds`` field is hardware dependent.
-        """
-        ...
-    def calibration(self, *args, **kwargs) -> Any: ...
-    def __init__(self, id=0, *args, **kwargs) -> None: ...
-
-class I2C:
-    """
-    Construct and return a new I2C object using the following parameters:
-
-       - *id* identifies a particular I2C peripheral.  Allowed values for
-         depend on the particular port/board
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-
-    Note that some ports/boards will have default values of *scl* and *sda*
-    that can be changed in this constructor.  Others will have fixed values
-    of *scl* and *sda* that cannot be changed.
-    """
-
-    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.  The number of bytes read is the
-        length of *buf*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_into(self, addr, buf, stop=True, /) -> None:
-        """
-        Read into *buf* from the peripheral specified by *addr*.
-        The number of bytes read will be the length of *buf*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-
-        The method returns ``None``.
-        """
-        ...
-    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr* starting from the memory
-        address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
-        """
-        Write *buf* to the peripheral specified by *addr* starting from the
-        memory address specified by *memaddr*.
-        The argument *addrsize* specifies the address size in bits (on ESP8266
-        this argument is not recognised and the address size is always 8 bits).
-
-        The method returns ``None``.
-        """
-        ...
-    def scan(self) -> List:
-        """
-        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
-        those that respond.  A device responds if it pulls the SDA line low after
-        its address (including a write bit) is sent on the bus.
-        """
-        ...
-    def writeto(self, addr, buf, stop=True, /) -> int:
-        """
-        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
-        NACK is received following the write of a byte from *buf* then the
-        remaining bytes are not sent.  If *stop* is true then a STOP condition is
-        generated at the end of the transfer, even if a NACK is received.
-        The function returns the number of ACKs that were received.
-        """
-        ...
-    def writevto(self, addr, vector, stop=True, /) -> int:
-        """
-        Write the bytes contained in *vector* to the peripheral specified by *addr*.
-        *vector* should be a tuple or list of objects with the buffer protocol.
-        The *addr* is sent once and then the bytes from each object in *vector*
-        are written out sequentially.  The objects in *vector* may be zero bytes
-        in length in which case they don't contribute to the output.
-
-        If a NACK is received following the write of a byte from one of the
-        objects in *vector* then the remaining bytes, and any remaining objects,
-        are not sent.  If *stop* is true then a STOP condition is generated at
-        the end of the transfer, even if a NACK is received.  The function
-        returns the number of ACKs that were received.
-        """
-        ...
-    def start(self) -> None:
-        """
-        Generate a START condition on the bus (SDA transitions to low while SCL is high).
-        """
-        ...
-    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
-        """
-        Read *nbytes* from the peripheral specified by *addr*.
-        If *stop* is true then a STOP condition is generated at the end of the transfer.
-        Returns a `bytes` object with the data read.
-        """
-        ...
-    def readinto(self, buf, nack=True, /) -> Any:
-        """
-        Reads bytes from the bus and stores them into *buf*.  The number of bytes
-        read is the length of *buf*.  An ACK will be sent on the bus after
-        receiving all but the last byte.  After the last byte is received, if *nack*
-        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
-        case the peripheral assumes more bytes are going to be read in a later call).
-        """
-        ...
-    def init(self, scl, sda, *, freq=400000) -> None:
-        """
-        Initialise the I2C bus with the given arguments:
-
-           - *scl* is a pin object for the SCL line
-           - *sda* is a pin object for the SDA line
-           - *freq* is the SCL clock rate
-        """
-        ...
-    def stop(self) -> None:
-        """
-        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the bytes from *buf* to the bus.  Checks that an ACK is received
-        after each byte and stops transmitting the remaining bytes if a NACK is
-        received.  The function returns the number of ACKs that were received.
-        """
-        ...
-    def __init__(
-        self, id: Union[int, str] = -1, *, scl: Optional[Union[Pin, str]] = None, sda: Optional[Union[Pin, str]] = None, freq=400_000
-    ) -> None: ...
-
-class ADC:
-    """
-    Access the ADC associated with a source identified by *id*.  This
-    *id* may be an integer (usually specifying a channel number), a
-    :ref:`Pin <machine.Pin>` object, or other value supported by the
-    underlying machine.
-
-    If additional keyword-arguments are given then they will configure
-    various aspects of the ADC.  If not given, these settings will take
-    previous or default values.  The settings are:
-
-      - *sample_ns* is the sampling time in nanoseconds.
-
-      - *atten* specifies the input attenuation.
-    """
-
-    VREF: int
-    CORE_VREF: int
-    CORE_VBAT: int
-    CORE_TEMP: int
-    def read_u16(self) -> int:
-        """
-        Take an analog reading and return an integer in the range 0-65535.
-        The return value represents the raw reading taken by the ADC, scaled
-        such that the minimum value is 0 and the maximum value is 65535.
-        """
-        ...
-    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
-
-class WDT:
-    """
-    Create a WDT object and start it. The timeout must be given in milliseconds.
-    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
-
-    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
-    cannot be specified, it is determined by the underlying system.
-    """
-
-    def feed(self) -> None:
-        """
-        Feed the WDT to prevent it from resetting the system. The application
-        should place this call in a sensible place ensuring that the WDT is
-        only fed after verifying that everything is functioning correctly.
-        """
-        ...
-    def __init__(self, id=0, timeout=5000) -> None: ...
-
-class Timer:
-    """
-    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
-    virtual timer (if supported by a board).
-    ``id`` shall not be passed as a keyword argument.
-
-    See ``init`` for parameters of initialisation.
-    """
-
-    PERIODIC: int
-    ONE_SHOT: int
-    def init(self, *, mode=PERIODIC, period=-1, callback=None) -> None:
-        """
-        Initialise the timer. Example::
-
-            def mycallback(t):
-                pass
-
-            # periodic with 100ms period
-            tim.init(period=100, callback=mycallback)
-
-            # one shot firing after 1000ms
-            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
-
-        Keyword arguments:
-
-          - ``mode`` can be one of:
-
-            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
-              period of the channel expires.
-            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
-              frequency of the channel.
-
-          - ``period`` - The timer period, in milliseconds.
-
-          - ``callback`` - The callable to call upon expiration of the timer period.
-            The callback must take one argument, which is passed the Timer object.
-            The ``callback`` argument shall be specified. Otherwise an exception
-            will occurr upon timer expiration:
-            ``TypeError: 'NoneType' object isn't callable``
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
-        """
-        ...
-    def __init__(self, id=-1, *args, **kwargs) -> None: ...
-
-class SoftSPI:
-    """
-    Construct a new software SPI object.  Additional parameters must be
-    given, usually at least *sck*, *mosi* and *miso*, and these are used
-    to initialise the bus.  See `SPI.init` for a description of the parameters.
-    """
-
-    LSB: int
-    MSB: int
-    def deinit(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def write_readinto(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
-
-class UART:
-    """
-    Construct a UART object of the given id.
-    """
-
-    CTS: int
-    RTS: int
-    IRQ_RXIDLE: int
-    def readchar(self, *args, **kwargs) -> Any: ...
-    def sendbreak(self) -> None:
-        """
-        Send a break condition on the bus. This drives the bus low for a duration
-        longer than required for a normal transmission of a character.
-        """
-        ...
-    def irq(self, trigger, priority=1, handler=None, wake=IDLE) -> Any:
-        """
-        Create a callback to be triggered when data is received on the UART.
-
-            - *trigger* can only be ``UART.RX_ANY``
-            - *priority* level of the interrupt. Can take values in the range 1-7.
-              Higher values represent higher priorities.
-            - *handler* an optional function to be called when new characters arrive.
-            - *wake* can only be ``machine.IDLE``.
-
-        .. note::
-
-           The handler will be called whenever any of the following two conditions are met:
-
-               - 8 new characters have been received.
-               - At least 1 new character is waiting in the Rx buffer and the Rx line has been
-                 silent for the duration of 1 complete frame.
-
-           This means that when the handler function is called there will be between 1 to 8
-           characters waiting.
-
-        Returns an irq object.
-
-        Availability: WiPy.
-        """
-        ...
-    def deinit(self) -> None:
-        """
-        Turn off the UART bus.
-        """
-        ...
-    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
-        """
-        Initialise the UART bus with the given parameters:
-
-          - *baudrate* is the clock rate.
-          - *bits* is the number of bits per character, 7, 8 or 9.
-          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
-          - *stop* is the number of stop bits, 1 or 2.
-
-        Additional keyword-only parameters that may be supported by a port are:
-
-          - *tx* specifies the TX pin to use.
-          - *rx* specifies the RX pin to use.
-          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
-          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
-          - *txbuf* specifies the length in characters of the TX buffer.
-          - *rxbuf* specifies the length in characters of the RX buffer.
-          - *timeout* specifies the time to wait for the first character (in ms).
-          - *timeout_char* specifies the time to wait between characters (in ms).
-          - *invert* specifies which lines to invert.
-
-              - ``0`` will not invert lines (idle state of both lines is logic high).
-              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
-              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
-              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
-
-          - *flow* specifies which hardware flow control signals to use. The value
-            is a bitmask.
-
-              - ``0`` will ignore hardware flow control signals.
-              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
-                signal if the receive FIFO has sufficient space to accept more data.
-              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
-                CTS input pin signals that the receiver is running low on buffer space.
-              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
-
-        On the WiPy only the following keyword-only parameter is supported:
-
-          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
-            Any of the pins can be None if one wants the UART to operate with limited functionality.
-            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
-            When no pins are given, then the default set of TX and RX pins is taken, and hardware
-            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
-        """
-        ...
-    def writechar(self, *args, **kwargs) -> Any: ...
-    def read(self, nbytes: Optional[Any] = None) -> bytes:
-        """
-        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
-        otherwise read as much data as possible. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: a bytes object containing the bytes read in.  Returns ``None``
-        on timeout.
-        """
-        ...
-    def any(self) -> int:
-        """
-        Returns an integer counting the number of characters that can be read without
-        blocking.  It will return 0 if there are no characters available and a positive
-        number if there are characters.  The method may return 1 even if there is more
-        than one character available for reading.
-
-        For more sophisticated querying of available characters use select.poll::
-
-         poll = select.poll()
-         poll.register(uart, select.POLLIN)
-         poll.poll(timeout)
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the bus.
-
-        Return value: number of bytes written or ``None`` on timeout.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: number of bytes read and stored into ``buf`` or ``None`` on
-        timeout.
-        """
-        ...
-    def readline(self) -> None:
-        """
-        Read a line, ending in a newline character. It may return sooner if a timeout
-        is reached. The timeout is configurable in the constructor.
-
-        Return value: the line read or ``None`` on timeout.
-        """
-        ...
-    def __init__(self, id, *args, **kwargs) -> None: ...
-
-mem32: Any
-mem16: Any
-
-class SoftI2C:
-    """
-    Construct a new software I2C object.  The parameters are:
-
-       - *scl* should be a pin object specifying the pin to use for SCL.
-       - *sda* should be a pin object specifying the pin to use for SDA.
-       - *freq* should be an integer which sets the maximum frequency
-         for SCL.
-       - *timeout* is the maximum time in microseconds to wait for clock
-         stretching (SCL held low by another device on the bus), after
-         which an ``OSError(ETIMEDOUT)`` exception is raised.
-    """
-
-    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_into(self, *args, **kwargs) -> Any: ...
-    def readfrom_mem(self, *args, **kwargs) -> Any: ...
-    def writeto_mem(self, *args, **kwargs) -> Any: ...
-    def scan(self, *args, **kwargs) -> Any: ...
-    def writeto(self, *args, **kwargs) -> Any: ...
-    def writevto(self, *args, **kwargs) -> Any: ...
-    def start(self, *args, **kwargs) -> Any: ...
-    def readfrom(self, *args, **kwargs) -> Any: ...
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def init(self, *args, **kwargs) -> Any: ...
-    def stop(self, *args, **kwargs) -> Any: ...
-    def write(self, *args, **kwargs) -> Any: ...
-    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
-
-class Signal:
-    """
-            Signal(pin_arguments..., *, invert=False)
-
-    Create a Signal object. There're two ways to create it:
-
-    * By wrapping existing Pin object - universal method which works for
-      any board.
-    * By passing required Pin parameters directly to Signal constructor,
-      skipping the need to create intermediate Pin object. Available on
-      many, but not all boards.
-
-    The arguments are:
-
-      - ``pin_obj`` is existing Pin object.
-
-      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
-
-      - ``invert`` - if True, the signal will be inverted (active low).
-    """
-
-    def off(self) -> None:
-        """
-        Deactivate signal.
-        """
-        ...
-    def on(self) -> None:
-        """
-        Activate signal.
-        """
-        ...
-    def value(self, x: Optional[Any] = None) -> int:
-        """
-        This method allows to set and get the value of the signal, depending on whether
-        the argument ``x`` is supplied or not.
-
-        If the argument is omitted then this method gets the signal level, 1 meaning
-        signal is asserted (active) and 0 - signal inactive.
-
-        If the argument is supplied then this method sets the signal level. The
-        argument ``x`` can be anything that converts to a boolean. If it converts
-        to ``True``, the signal is active, otherwise it is inactive.
-
-        Correspondence between signal being active and actual logic level on the
-        underlying pin depends on whether signal is inverted (active-low) or not.
-        For non-inverted signal, active status corresponds to logical 1, inactive -
-        to logical 0. For inverted/active-low signal, active status corresponds
-        to logical 0, while inactive - to logical 1.
-        """
-        ...
-    def __init__(self, pin_obj, *args, invert=False) -> None: ...
+"""
+functions related to the hardware. See: https://docs.micropython.org/en/v1.20.0/library/machine.html
+
+The ``machine`` module contains specific functions related to the hardware
+on a particular board. Most functions in this module allow to achieve direct
+and unrestricted access to and control of hardware blocks on a system
+(like CPU, timers, buses, etc.). Used incorrectly, this can lead to
+malfunction, lockups, crashes of your board, and in extreme cases, hardware
+damage.
+"""
+from typing import Callable, List, NoReturn, Optional, Tuple, Union, Any
+
+HARD_RESET: int
+PWRON_RESET: int
+SOFT_RESET: int
+DEEPSLEEP_RESET: int
+WDT_RESET: int
+
+def idle() -> Any:
+    """
+    Gates the clock to the CPU, useful to reduce power consumption at any time during
+    short or long periods. Peripherals continue working and execution resumes as soon
+    as any interrupt is triggered (on many ports this includes system timer
+    interrupt occurring at regular intervals on the order of millisecond).
+    """
+    ...
+
+def freq(hz: Optional[Any] = None) -> Any:
+    """
+    Returns the CPU frequency in hertz.
+
+    On some ports this can also be used to set the CPU frequency by passing in *hz*.
+    """
+    ...
+
+def info(*args, **kwargs) -> Any: ...
+def dht_readinto(*args, **kwargs) -> Any: ...
+def enable_irq(state) -> Any:
+    """
+    Re-enable interrupt requests.
+    The *state* parameter should be the value that was returned from the most
+    recent call to the `disable_irq()` function.
+    """
+    ...
+
+def disable_irq() -> Any:
+    """
+    Disable interrupt requests.
+    Returns the previous IRQ state which should be considered an opaque value.
+    This return value should be passed to the `enable_irq()` function to restore
+    interrupts to their original state, before `disable_irq()` was called.
+    """
+    ...
+
+def deepsleep(time_ms: Optional[Any] = None) -> NoReturn:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def soft_reset() -> NoReturn:
+    """
+    Performs a soft reset of the interpreter, deleting all Python objects and
+    resetting the Python heap.  It tries to retain the method by which the user
+    is connected to the MicroPython REPL (eg serial, USB, Wifi).
+    """
+    ...
+
+def sleep() -> Any:
+    """
+    ``Note:`` This function is deprecated, use `lightsleep()` instead with no arguments.
+    """
+    ...
+
+def time_pulse_us(pin, pulse_level, timeout_us=1000000, /) -> int:
+    """
+    Time a pulse on the given *pin*, and return the duration of the pulse in
+    microseconds.  The *pulse_level* argument should be 0 to time a low pulse
+    or 1 to time a high pulse.
+
+    If the current input value of the pin is different to *pulse_level*,
+    the function first (*) waits until the pin input becomes equal to *pulse_level*,
+    then (**) times the duration that the pin is equal to *pulse_level*.
+    If the pin is already equal to *pulse_level* then timing starts straight away.
+
+    The function will return -2 if there was timeout waiting for condition marked
+    (*) above, and -1 if there was timeout during the main measurement, marked (**)
+    above. The timeout is the same for both cases and given by *timeout_us* (which
+    is in microseconds).
+    """
+    ...
+
+def lightsleep(time_ms: Optional[Any] = None) -> Any:
+    """
+    Stops execution in an attempt to enter a low power state.
+
+    If *time_ms* is specified then this will be the maximum time in milliseconds that
+    the sleep will last for.  Otherwise the sleep can last indefinitely.
+
+    With or without a timeout, execution may resume at any time if there are events
+    that require processing.  Such events, or wake sources, should be configured before
+    sleeping, like `Pin` change or `RTC` timeout.
+
+    The precise behaviour and power-saving capabilities of lightsleep and deepsleep is
+    highly dependent on the underlying hardware, but the general properties are:
+
+    * A lightsleep has full RAM and state retention.  Upon wake execution is resumed
+      from the point where the sleep was requested, with all subsystems operational.
+
+    * A deepsleep may not retain RAM or any other state of the system (for example
+      peripherals or network interfaces).  Upon wake execution is resumed from the main
+      script, similar to a hard or power-on reset. The `reset_cause()` function will
+      return `machine.DEEPSLEEP` and this can be used to distinguish a deepsleep wake
+      from other resets.
+    """
+    ...
+
+def reset() -> NoReturn:
+    """
+    Resets the device in a manner similar to pushing the external RESET
+    button.
+    """
+    ...
+
+def rng() -> int:
+    """
+    Return a 24-bit software generated random number.
+
+    Availability: WiPy.
+    """
+    ...
+
+def reset_cause() -> int:
+    """
+    Get the reset cause. See :ref:`constants <machine_constants>` for the possible return values.
+    """
+    ...
+
+def unique_id() -> bytes:
+    """
+    Returns a byte string with a unique identifier of a board/SoC. It will vary
+    from a board/SoC instance to another, if underlying hardware allows. Length
+    varies by hardware (so use substring of a full value if you expect a short
+    ID). In some MicroPython ports, ID corresponds to the network MAC address.
+    """
+    ...
+
+def bootloader(value: Optional[Any] = None) -> None:
+    """
+    Reset the device and enter its bootloader.  This is typically used to put the
+    device into a state where it can be programmed with new firmware.
+
+    Some ports support passing in an optional *value* argument which can control
+    which bootloader to enter, what to pass to it, or other things.
+    """
+    ...
+
+def bitstream(pin, encoding, timing, data, /) -> Any:
+    """
+    Transmits *data* by bit-banging the specified *pin*. The *encoding* argument
+    specifies how the bits are encoded, and *timing* is an encoding-specific timing
+    specification.
+
+    The supported encodings are:
+
+      - ``0`` for "high low" pulse duration modulation. This will transmit 0 and
+        1 bits as timed pulses, starting with the most significant bit.
+        The *timing* must be a four-tuple of nanoseconds in the format
+        ``(high_time_0, low_time_0, high_time_1, low_time_1)``. For example,
+        ``(400, 850, 800, 450)`` is the timing specification for WS2812 RGB LEDs
+        at 800kHz.
+
+    The accuracy of the timing varies between ports. On Cortex M0 at 48MHz, it is
+    at best +/- 120ns, however on faster MCUs (ESP8266, ESP32, STM32, Pyboard), it
+    will be closer to +/-30ns.
+
+    ``Note:`` For controlling WS2812 / NeoPixel strips, see the :mod:`neopixel`
+       module for a higher-level API.
+    """
+    ...
+
+class Pin:
+    """
+    Access the pin peripheral (GPIO pin) associated with the given ``id``.  If
+    additional arguments are given in the constructor then they are used to initialise
+    the pin.  Any settings that are not specified will remain in their previous state.
+
+    The arguments are:
+
+      - ``id`` is mandatory and can be an arbitrary object.  Among possible value
+        types are: int (an internal Pin identifier), str (a Pin name), and tuple
+        (pair of [port, pin]).
+
+      - ``mode`` specifies the pin mode, which can be one of:
+
+        - ``Pin.IN`` - Pin is configured for input.  If viewed as an output the pin
+          is in high-impedance state.
+
+        - ``Pin.OUT`` - Pin is configured for (normal) output.
+
+        - ``Pin.OPEN_DRAIN`` - Pin is configured for open-drain output. Open-drain
+          output works in the following way: if the output value is set to 0 the pin
+          is active at a low level; if the output value is 1 the pin is in a high-impedance
+          state.  Not all ports implement this mode, or some might only on certain pins.
+
+        - ``Pin.ALT`` - Pin is configured to perform an alternative function, which is
+          port specific.  For a pin configured in such a way any other Pin methods
+          (except :meth:`Pin.init`) are not applicable (calling them will lead to undefined,
+          or a hardware-specific, result).  Not all ports implement this mode.
+
+        - ``Pin.ALT_OPEN_DRAIN`` - The Same as ``Pin.ALT``, but the pin is configured as
+          open-drain.  Not all ports implement this mode.
+
+        - ``Pin.ANALOG`` - Pin is configured for analog input, see the :class:`ADC` class.
+
+      - ``pull`` specifies if the pin has a (weak) pull resistor attached, and can be
+        one of:
+
+        - ``None`` - No pull up or down resistor.
+        - ``Pin.PULL_UP`` - Pull up resistor enabled.
+        - ``Pin.PULL_DOWN`` - Pull down resistor enabled.
+
+      - ``value`` is valid only for Pin.OUT and Pin.OPEN_DRAIN modes and specifies initial
+        output pin value if given, otherwise the state of the pin peripheral remains
+        unchanged.
+
+      - ``drive`` specifies the output power of the pin and can be one of: ``Pin.DRIVE_0``,
+        ``Pin.DRIVE_1``, etc., increasing in drive strength.  The actual current driving
+        capabilities are port dependent.  Not all ports implement this argument.
+
+      - ``alt`` specifies an alternate function for the pin and the values it can take are
+        port dependent.  This argument is valid only for ``Pin.ALT`` and ``Pin.ALT_OPEN_DRAIN``
+        modes.  It may be used when a pin supports more than one alternate function.  If only
+        one pin alternate function is supported the this argument is not required.  Not all
+        ports implement this argument.
+
+    As specified above, the Pin class allows to set an alternate function for a particular
+    pin, but it does not specify any further operations on such a pin.  Pins configured in
+    alternate-function mode are usually not used as GPIO but are instead driven by other
+    hardware peripherals.  The only operation supported on such a pin is re-initialising,
+    by calling the constructor or :meth:`Pin.init` method.  If a pin that is configured in
+    alternate-function mode is re-initialised with ``Pin.IN``, ``Pin.OUT``, or
+    ``Pin.OPEN_DRAIN``, the alternate function will be removed from the pin.
+    """
+
+    AF_OD: int
+    AF9_TIM14: int
+    ALT_OPEN_DRAIN: int
+    AF_PP: int
+    ALT: int
+    AF9_CAN1: int
+    AF8_USART6: int
+    AF9_TIM13: int
+    AF9_CAN2: int
+    AF9_TIM12: int
+    PULL_UP: int
+    OUT_PP: int
+    OUT_OD: int
+    ANALOG: int
+    PULL_DOWN: int
+    PULL_NONE: int
+    IRQ_FALLING: int
+    IN: int
+    OUT: int
+    IRQ_RISING: int
+    OPEN_DRAIN: int
+    AF2_TIM5: int
+    AF3_TIM10: int
+    AF3_TIM11: int
+    AF3_TIM8: int
+    AF3_TIM9: int
+    AF2_TIM4: int
+    AF1_TIM1: int
+    AF1_TIM2: int
+    AF2_TIM3: int
+    AF8_UART4: int
+    AF6_I2S2: int
+    AF7_USART1: int
+    AF7_USART2: int
+    AF7_USART3: int
+    AF4_I2C1: int
+    AF5_SPI2: int
+    AF4_I2C2: int
+    AF5_I2S2: int
+    AF5_SPI1: int
+    def mode(self, mode: Optional[Any] = None) -> Any:
+        """
+        Get or set the pin mode.
+        See the constructor documentation for details of the ``mode`` argument.
+
+        Availability: cc3200, stm32 ports.
+        """
+        ...
+    def name(self, *args, **kwargs) -> Any: ...
+    def pull(self, pull: Optional[Any] = None) -> Any:
+        """
+        Get or set the pin pull state.
+        See the constructor documentation for details of the ``pull`` argument.
+
+        Availability: cc3200, stm32 ports.
+        """
+        ...
+    def low(self) -> None:
+        """
+        Set pin to "0" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+    def irq(self, handler=None, trigger=IRQ_FALLING, *, priority=1, wake=None, hard=False) -> Callable[..., Any]:
+        """
+           Configure an interrupt handler to be called when the trigger source of the
+           pin is active.  If the pin mode is ``Pin.IN`` then the trigger source is
+           the external value on the pin.  If the pin mode is ``Pin.OUT`` then the
+           trigger source is the output buffer of the pin.  Otherwise, if the pin mode
+           is ``Pin.OPEN_DRAIN`` then the trigger source is the output buffer for
+           state '0' and the external pin value for state '1'.
+
+           The arguments are:
+
+             - ``handler`` is an optional function to be called when the interrupt
+               triggers. The handler must take exactly one argument which is the
+               ``Pin`` instance.
+
+             - ``trigger`` configures the event which can generate an interrupt.
+               Possible values are:
+
+               - ``Pin.IRQ_FALLING`` interrupt on falling edge.
+               - ``Pin.IRQ_RISING`` interrupt on rising edge.
+               - ``Pin.IRQ_LOW_LEVEL`` interrupt on low level.
+               - ``Pin.IRQ_HIGH_LEVEL`` interrupt on high level.
+
+               These values can be OR'ed together to trigger on multiple events.
+
+             - ``priority`` sets the priority level of the interrupt.  The values it
+               can take are port-specific, but higher values always represent higher
+               priorities.
+
+             - ``wake`` selects the power mode in which this interrupt can wake up the
+               system.  It can be ``machine.IDLE``, ``machine.SLEEP`` or ``machine.DEEPSLEEP``.
+               These values can also be OR'ed together to make a pin generate interrupts in
+               more than one power mode.
+
+             - ``hard`` if true a hardware interrupt is used. This reduces the delay
+               between the pin change and the handler being called. Hard interrupt
+               handlers may not allocate memory; see :ref:`isr_rules`.
+               Not all ports support this argument.
+
+           This method returns a callback object.
+
+        The following methods are not part of the core Pin API and only implemented on certain ports.
+        """
+        ...
+    def pin(self, *args, **kwargs) -> Any: ...
+    def port(self, *args, **kwargs) -> Any: ...
+    def names(self, *args, **kwargs) -> Any: ...
+    def on(self) -> None:
+        """
+        Set pin to "1" output level.
+        """
+        ...
+    def off(self) -> None:
+        """
+        Set pin to "0" output level.
+        """
+        ...
+    def init(self, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None:
+        """
+        Re-initialise the pin using the given parameters.  Only those arguments that
+        are specified will be set.  The rest of the pin peripheral state will remain
+        unchanged.  See the constructor documentation for details of the arguments.
+
+        Returns ``None``.
+        """
+        ...
+    def af_list(self, *args, **kwargs) -> Any: ...
+    def af(self, *args, **kwargs) -> Any: ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the pin, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the digital logic level of
+        the pin, returning 0 or 1 corresponding to low and high voltage signals
+        respectively.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The method returns the actual input value currently present
+            on the pin.
+          - ``Pin.OUT`` - The behaviour and return value of the method is undefined.
+          - ``Pin.OPEN_DRAIN`` - If the pin is in state '0' then the behaviour and
+            return value of the method is undefined.  Otherwise, if the pin is in
+            state '1', the method returns the actual input value currently present
+            on the pin.
+
+        If the argument is supplied then this method sets the digital logic level of
+        the pin.  The argument ``x`` can be anything that converts to a boolean.
+        If it converts to ``True``, the pin is set to state '1', otherwise it is set
+        to state '0'.  The behaviour of this method depends on the mode of the pin:
+
+          - ``Pin.IN`` - The value is stored in the output buffer for the pin.  The
+            pin state does not change, it remains in the high-impedance state.  The
+            stored value will become active on the pin as soon as it is changed to
+            ``Pin.OUT`` or ``Pin.OPEN_DRAIN`` mode.
+          - ``Pin.OUT`` - The output buffer is set to the given value immediately.
+          - ``Pin.OPEN_DRAIN`` - If the value is '0' the pin is set to a low voltage
+            state.  Otherwise the pin is set to high-impedance state.
+
+        When setting the value this method returns ``None``.
+        """
+        ...
+    def high(self) -> None:
+        """
+        Set pin to "1" output level.
+
+        Availability: nrf, rp2, stm32 ports.
+        """
+        ...
+    def gpio(self, *args, **kwargs) -> Any: ...
+    @classmethod
+    def dict(cls, *args, **kwargs) -> Any: ...
+    @classmethod
+    def debug(cls, *args, **kwargs) -> Any: ...
+
+    class cpu:
+        B9: Any
+        B8: Any
+        B7: Any
+        C0: Any
+        C1: Any
+        C10: Any
+        B3: Any
+        B2: Any
+        B6: Any
+        B4: Any
+        B5: Any
+        B15: Any
+        C7: Any
+        C6: Any
+        C5: Any
+        C8: Any
+        C9: Any
+        C11: Any
+        C13: Any
+        C12: Any
+        C4: Any
+        C2: Any
+        C3: Any
+        D2: Any
+        A15: Any
+        A14: Any
+        A13: Any
+        A2: Any
+        A3: Any
+        A4: Any
+        A1: Any
+        A0: Any
+        A12: Any
+        A10: Any
+        A11: Any
+        B14: Any
+        B11: Any
+        B10: Any
+        B1: Any
+        B12: Any
+        B13: Any
+        A5: Any
+        A7: Any
+        A6: Any
+        B0: Any
+        A8: Any
+        A9: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    @classmethod
+    def mapper(cls, *args, **kwargs) -> Any: ...
+
+    class board:
+        X5: Any
+        X18: Any
+        X4: Any
+        X8: Any
+        X6: Any
+        X7: Any
+        X2: Any
+        X3: Any
+        X19: Any
+        X22: Any
+        X20: Any
+        X21: Any
+        Y5: Any
+        X9: Any
+        Y4: Any
+        Y8: Any
+        Y6: Any
+        Y7: Any
+        Y10: Any
+        Y3: Any
+        Y1: Any
+        Y2: Any
+        Y11: Any
+        Y12: Any
+        Y9: Any
+        SD_CK: Any
+        X17: Any
+        SD: Any
+        SD_D1: Any
+        SD_CMD: Any
+        SD_D0: Any
+        LED_GREEN: Any
+        MMA_INT: Any
+        LED_BLUE: Any
+        MMA_AVDD: Any
+        LED_RED: Any
+        LED_YELLOW: Any
+        X1: Any
+        SD_D2: Any
+        USB_VBUS: Any
+        X12: Any
+        X10: Any
+        X11: Any
+        SD_SW: Any
+        USB_ID: Any
+        SD_D3: Any
+        USB_DP: Any
+        SW: Any
+        USB_DM: Any
+        def __init__(self, *argv, **kwargs) -> None: ...
+
+    def __init__(self, id, mode=-1, pull=-1, *, value=None, drive=0, alt=-1) -> None: ...
+    def __call__(self, x: Optional[Any] = None) -> Any:
+        """
+        Pin objects are callable.  The call method provides a (fast) shortcut to set
+        and get the value of the pin.  It is equivalent to Pin.value([x]).
+        See :meth:`Pin.value` for more details.
+        """
+        ...
+
+class I2S:
+    """
+    Construct an I2S object of the given id:
+
+    - ``id`` identifies a particular I2S bus; it is board and port specific
+
+    Keyword-only parameters that are supported on all ports:
+
+      - ``sck`` is a pin object for the serial clock line
+      - ``ws`` is a pin object for the word select line
+      - ``sd`` is a pin object for the serial data line
+      - ``mck`` is a pin object for the master clock line;
+        master clock frequency is sampling rate * 256
+      - ``mode`` specifies receive or transmit
+      - ``bits`` specifies sample size (bits), 16 or 32
+      - ``format`` specifies channel format, STEREO or MONO
+      - ``rate`` specifies audio sampling rate (Hz);
+        this is the frequency of the ``ws`` signal
+      - ``ibuf`` specifies internal buffer length (bytes)
+
+    For all ports, DMA runs continuously in the background and allows user applications to perform other operations while
+    sample data is transfered between the internal buffer and the I2S peripheral unit.
+    Increasing the size of the internal buffer has the potential to increase the time that user applications can perform non-I2S operations
+    before underflow (e.g. ``write`` method) or overflow (e.g. ``readinto`` method).
+    """
+
+    RX: int
+    MONO: int
+    STEREO: int
+    TX: int
+    @staticmethod
+    def shift(*, buf, bits, shift) -> Any:
+        """
+        bitwise shift of all samples contained in ``buf``. ``bits`` specifies sample size in bits. ``shift`` specifies the number of bits to shift each sample.
+        Positive for left shift, negative for right shift.
+        Typically used for volume control.  Each bit shift changes sample volume by 6dB.
+        """
+        ...
+    def init(self, sck, *args, **kwargs) -> Any:
+        """
+        see Constructor for argument descriptions
+        """
+        ...
+    def irq(self, handler) -> Any:
+        """
+        Set a callback. ``handler`` is called when ``buf`` is emptied (``write`` method) or becomes full (``readinto`` method).
+        Setting a callback changes the ``write`` and ``readinto`` methods to non-blocking operation.
+        ``handler`` is called in the context of the MicroPython scheduler.
+        """
+        ...
+    def readinto(self, buf) -> int:
+        """
+        Read audio samples into the buffer specified by ``buf``.  ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the left channel sample data is used.
+        Returns number of bytes read
+        """
+        ...
+    def deinit(self) -> Any:
+        """
+        Deinitialize the I2S bus
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write audio samples contained in ``buf``. ``buf`` must support the buffer protocol, such as bytearray or array.
+        "buf" byte ordering is little-endian.  For Stereo format, left channel sample precedes right channel sample. For Mono format,
+        the sample data is written to both the right and left channels.
+        Returns number of bytes written
+        """
+        ...
+    def __init__(self, id, *, sck, ws, sd, mck=None, mode, bits, format, rate, ibuf) -> None: ...
+
+class SPI:
+    """
+    Construct an SPI object on the given bus, *id*. Values of *id* depend
+    on a particular port and its hardware. Values 0, 1, etc. are commonly used
+    to select hardware SPI block #0, #1, etc.
+
+    With no additional parameters, the SPI object is created but not
+    initialised (it has the settings from the last initialisation of
+    the bus, if any).  If extra arguments are given, the bus is initialised.
+    See ``init`` for parameters of initialisation.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self) -> None:
+        """
+        Turn off the SPI bus.
+        """
+        ...
+    def init(
+        self, baudrate=1000000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None, pins: Optional[Tuple]
+    ) -> None:
+        """
+        Initialise the SPI bus with the given parameters:
+
+          - ``baudrate`` is the SCK clock rate.
+          - ``polarity`` can be 0 or 1, and is the level the idle clock line sits at.
+          - ``phase`` can be 0 or 1 to sample data on the first or second clock edge
+            respectively.
+          - ``bits`` is the width in bits of each transfer. Only 8 is guaranteed to be supported by all hardware.
+          - ``firstbit`` can be ``SPI.MSB`` or ``SPI.LSB``.
+          - ``sck``, ``mosi``, ``miso`` are pins (machine.Pin) objects to use for bus signals. For most
+            hardware SPI blocks (as selected by ``id`` parameter to the constructor), pins are fixed
+            and cannot be changed. In some cases, hardware blocks allow 2-3 alternative pin sets for
+            a hardware SPI block. Arbitrary pin assignments are possible only for a bitbanging SPI driver
+            (``id`` = -1).
+          - ``pins`` - WiPy port doesn't ``sck``, ``mosi``, ``miso`` arguments, and instead allows to
+            specify them as a tuple of ``pins`` parameter.
+
+        In the case of hardware SPI the actual clock frequency may be lower than the
+        requested baudrate. This is dependant on the platform hardware. The actual
+        rate may be determined by printing the SPI object.
+        """
+        ...
+    def write_readinto(self, write_buf, read_buf) -> int:
+        """
+        Write the bytes from ``write_buf`` while reading into ``read_buf``.  The
+        buffers can be the same or different, but both buffers must have the
+        same length.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def read(self, nbytes, write=0x00) -> bytes:
+        """
+        Read a number of bytes specified by ``nbytes`` while continuously writing
+        the single byte given by ``write``.
+        Returns a ``bytes`` object with the data that was read.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes contained in ``buf``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes written.
+        """
+        ...
+    def readinto(self, buf, write=0x00) -> int:
+        """
+        Read into the buffer specified by ``buf`` while continuously writing the
+        single byte given by ``write``.
+        Returns ``None``.
+
+        Note: on WiPy this function returns the number of bytes read.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+mem8: Any
+
+class RTC:
+    """
+    Create an RTC object. See init for parameters of initialization.
+    """
+
+    def info(self, *args, **kwargs) -> Any: ...
+    def init(self, datetime) -> None:
+        """
+        Initialise the RTC. Datetime is a tuple of the form:
+
+           ``(year, month, day[, hour[, minute[, second[, microsecond[, tzinfo]]]]])``
+        """
+        ...
+    def wakeup(self, *args, **kwargs) -> Any: ...
+    def datetime(self, datetimetuple: Optional[Any] = None) -> Tuple:
+        """
+        Get or set the date and time of the RTC.
+
+        With no arguments, this method returns an 8-tuple with the current
+        date and time.  With 1 argument (being an 8-tuple) it sets the date
+        and time.
+
+        The 8-tuple has the following format:
+
+            (year, month, day, weekday, hours, minutes, seconds, subseconds)
+
+        The meaning of the ``subseconds`` field is hardware dependent.
+        """
+        ...
+    def calibration(self, *args, **kwargs) -> Any: ...
+    def __init__(self, id=0, *args, **kwargs) -> None: ...
+
+class I2C:
+    """
+    Construct and return a new I2C object using the following parameters:
+
+       - *id* identifies a particular I2C peripheral.  Allowed values for
+         depend on the particular port/board
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to allow for I2C
+         transactions.  This parameter is not allowed on some ports.
+
+    Note that some ports/boards will have default values of *scl* and *sda*
+    that can be changed in this constructor.  Others will have fixed values
+    of *scl* and *sda* that cannot be changed.
+    """
+
+    def readfrom_mem_into(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.  The number of bytes read is the
+        length of *buf*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_into(self, addr, buf, stop=True, /) -> None:
+        """
+        Read into *buf* from the peripheral specified by *addr*.
+        The number of bytes read will be the length of *buf*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+
+        The method returns ``None``.
+        """
+        ...
+    def readfrom_mem(self, addr, memaddr, nbytes, *, addrsize=8) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr* starting from the memory
+        address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def writeto_mem(self, addr, memaddr, buf, *, addrsize=8) -> None:
+        """
+        Write *buf* to the peripheral specified by *addr* starting from the
+        memory address specified by *memaddr*.
+        The argument *addrsize* specifies the address size in bits (on ESP8266
+        this argument is not recognised and the address size is always 8 bits).
+
+        The method returns ``None``.
+        """
+        ...
+    def scan(self) -> List:
+        """
+        Scan all I2C addresses between 0x08 and 0x77 inclusive and return a list of
+        those that respond.  A device responds if it pulls the SDA line low after
+        its address (including a write bit) is sent on the bus.
+        """
+        ...
+    def writeto(self, addr, buf, stop=True, /) -> int:
+        """
+        Write the bytes from *buf* to the peripheral specified by *addr*.  If a
+        NACK is received following the write of a byte from *buf* then the
+        remaining bytes are not sent.  If *stop* is true then a STOP condition is
+        generated at the end of the transfer, even if a NACK is received.
+        The function returns the number of ACKs that were received.
+        """
+        ...
+    def writevto(self, addr, vector, stop=True, /) -> int:
+        """
+        Write the bytes contained in *vector* to the peripheral specified by *addr*.
+        *vector* should be a tuple or list of objects with the buffer protocol.
+        The *addr* is sent once and then the bytes from each object in *vector*
+        are written out sequentially.  The objects in *vector* may be zero bytes
+        in length in which case they don't contribute to the output.
+
+        If a NACK is received following the write of a byte from one of the
+        objects in *vector* then the remaining bytes, and any remaining objects,
+        are not sent.  If *stop* is true then a STOP condition is generated at
+        the end of the transfer, even if a NACK is received.  The function
+        returns the number of ACKs that were received.
+        """
+        ...
+    def start(self) -> None:
+        """
+        Generate a START condition on the bus (SDA transitions to low while SCL is high).
+        """
+        ...
+    def readfrom(self, addr, nbytes, stop=True, /) -> bytes:
+        """
+        Read *nbytes* from the peripheral specified by *addr*.
+        If *stop* is true then a STOP condition is generated at the end of the transfer.
+        Returns a `bytes` object with the data read.
+        """
+        ...
+    def readinto(self, buf, nack=True, /) -> Any:
+        """
+        Reads bytes from the bus and stores them into *buf*.  The number of bytes
+        read is the length of *buf*.  An ACK will be sent on the bus after
+        receiving all but the last byte.  After the last byte is received, if *nack*
+        is true then a NACK will be sent, otherwise an ACK will be sent (and in this
+        case the peripheral assumes more bytes are going to be read in a later call).
+        """
+        ...
+    def init(self, scl, sda, *, freq=400000) -> None:
+        """
+        Initialise the I2C bus with the given arguments:
+
+           - *scl* is a pin object for the SCL line
+           - *sda* is a pin object for the SDA line
+           - *freq* is the SCL clock rate
+
+         In the case of hardware I2C the actual clock frequency may be lower than the
+         requested frequency. This is dependant on the platform hardware. The actual
+         rate may be determined by printing the I2C object.
+        """
+        ...
+    def stop(self) -> None:
+        """
+        Generate a STOP condition on the bus (SDA transitions to high while SCL is high).
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the bytes from *buf* to the bus.  Checks that an ACK is received
+        after each byte and stops transmitting the remaining bytes if a NACK is
+        received.  The function returns the number of ACKs that were received.
+        """
+        ...
+    def __init__(
+        self,
+        id: Union[int, str] = -1,
+        *,
+        scl: Optional[Union[Pin, str]] = None,
+        sda: Optional[Union[Pin, str]] = None,
+        freq=400_000,
+        timeout=50000,
+    ) -> None: ...
+
+class ADC:
+    """
+    Access the ADC associated with a source identified by *id*.  This
+    *id* may be an integer (usually specifying a channel number), a
+    :ref:`Pin <machine.Pin>` object, or other value supported by the
+    underlying machine.
+
+    If additional keyword-arguments are given then they will configure
+    various aspects of the ADC.  If not given, these settings will take
+    previous or default values.  The settings are:
+
+      - *sample_ns* is the sampling time in nanoseconds.
+
+      - *atten* specifies the input attenuation.
+    """
+
+    VREF: int
+    CORE_VREF: int
+    CORE_VBAT: int
+    CORE_TEMP: int
+    def read_u16(self) -> int:
+        """
+        Take an analog reading and return an integer in the range 0-65535.
+        The return value represents the raw reading taken by the ADC, scaled
+        such that the minimum value is 0 and the maximum value is 65535.
+        """
+        ...
+    def __init__(self, id, *, sample_ns: Optional[int] = 0, atten: Optional[int] = ATTN_0DB) -> None: ...
+
+class WDT:
+    """
+    Create a WDT object and start it. The timeout must be given in milliseconds.
+    Once it is running the timeout cannot be changed and the WDT cannot be stopped either.
+
+    Notes: On the esp32 the minimum timeout is 1 second. On the esp8266 a timeout
+    cannot be specified, it is determined by the underlying system. On rp2040 devices,
+    the maximum timeout is 8388 ms.
+    """
+
+    def feed(self) -> None:
+        """
+        Feed the WDT to prevent it from resetting the system. The application
+        should place this call in a sensible place ensuring that the WDT is
+        only fed after verifying that everything is functioning correctly.
+        """
+        ...
+    def __init__(self, id=0, timeout=5000) -> None: ...
+
+class Timer:
+    """
+    Construct a new timer object of the given ``id``. ``id`` of -1 constructs a
+    virtual timer (if supported by a board).
+    ``id`` shall not be passed as a keyword argument.
+
+    See ``init`` for parameters of initialisation.
+    """
+
+    PERIODIC: int
+    ONE_SHOT: int
+    def init(self, *, mode=PERIODIC, freq=-1, period=-1, callback=None) -> None:
+        """
+        Initialise the timer. Example::
+
+            def mycallback(t):
+                pass
+
+            # periodic at 1kHz
+            tim.init(mode=Timer.PERIODIC, freq=1000, callback=mycallback)
+
+            # periodic with 100ms period
+            tim.init(period=100, callback=mycallback)
+
+            # one shot firing after 1000ms
+            tim.init(mode=Timer.ONE_SHOT, period=1000, callback=mycallback)
+
+        Keyword arguments:
+
+          - ``mode`` can be one of:
+
+            - ``Timer.ONE_SHOT`` - The timer runs once until the configured
+              period of the channel expires.
+            - ``Timer.PERIODIC`` - The timer runs periodically at the configured
+              frequency of the channel.
+
+          - ``freq`` - The timer frequency, in units of Hz.  The upper bound of
+            the frequency is dependent on the port.  When both the ``freq`` and
+            ``period`` arguments are given, ``freq`` has a higher priority and
+            ``period`` is ignored.
+
+          - ``period`` - The timer period, in milliseconds.
+
+          - ``callback`` - The callable to call upon expiration of the timer period.
+            The callback must take one argument, which is passed the Timer object.
+            The ``callback`` argument shall be specified. Otherwise an exception
+            will occurr upon timer expiration:
+            ``TypeError: 'NoneType' object isn't callable``
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Deinitialises the timer. Stops the timer, and disables the timer peripheral.
+        """
+        ...
+    def __init__(self, id=-1, *args, **kwargs) -> None: ...
+
+class SoftSPI:
+    """
+    Construct a new software SPI object.  Additional parameters must be
+    given, usually at least *sck*, *mosi* and *miso*, and these are used
+    to initialise the bus.  See `SPI.init` for a description of the parameters.
+    """
+
+    LSB: int
+    MSB: int
+    def deinit(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def write_readinto(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def __init__(self, baudrate=500000, *, polarity=0, phase=0, bits=8, firstbit=MSB, sck=None, mosi=None, miso=None) -> None: ...
+
+class UART:
+    """
+    Construct a UART object of the given id.
+    """
+
+    IRQ_RXIDLE: int
+    CTS: int
+    RTS: int
+    def init(self, baudrate=9600, bits=8, parity=None, stop=1, *args, **kwargs) -> None:
+        """
+        Initialise the UART bus with the given parameters:
+
+          - *baudrate* is the clock rate.
+          - *bits* is the number of bits per character, 7, 8 or 9.
+          - *parity* is the parity, ``None``, 0 (even) or 1 (odd).
+          - *stop* is the number of stop bits, 1 or 2.
+
+        Additional keyword-only parameters that may be supported by a port are:
+
+          - *tx* specifies the TX pin to use.
+          - *rx* specifies the RX pin to use.
+          - *rts* specifies the RTS (output) pin to use for hardware receive flow control.
+          - *cts* specifies the CTS (input) pin to use for hardware transmit flow control.
+          - *txbuf* specifies the length in characters of the TX buffer.
+          - *rxbuf* specifies the length in characters of the RX buffer.
+          - *timeout* specifies the time to wait for the first character (in ms).
+          - *timeout_char* specifies the time to wait between characters (in ms).
+          - *invert* specifies which lines to invert.
+
+              - ``0`` will not invert lines (idle state of both lines is logic high).
+              - ``UART.INV_TX`` will invert TX line (idle state of TX line now logic low).
+              - ``UART.INV_RX`` will invert RX line (idle state of RX line now logic low).
+              - ``UART.INV_TX | UART.INV_RX`` will invert both lines (idle state at logic low).
+
+          - *flow* specifies which hardware flow control signals to use. The value
+            is a bitmask.
+
+              - ``0`` will ignore hardware flow control signals.
+              - ``UART.RTS`` will enable receive flow control by using the RTS output pin to
+                signal if the receive FIFO has sufficient space to accept more data.
+              - ``UART.CTS`` will enable transmit flow control by pausing transmission when the
+                CTS input pin signals that the receiver is running low on buffer space.
+              - ``UART.RTS | UART.CTS`` will enable both, for full hardware flow control.
+
+        On the WiPy only the following keyword-only parameter is supported:
+
+          - *pins* is a 4 or 2 item list indicating the TX, RX, RTS and CTS pins (in that order).
+            Any of the pins can be None if one wants the UART to operate with limited functionality.
+            If the RTS pin is given the the RX pin must be given as well. The same applies to CTS.
+            When no pins are given, then the default set of TX and RX pins is taken, and hardware
+            flow control will be disabled. If *pins* is ``None``, no pin assignment will be made.
+
+        .. note::
+          It is possible to call ``init()`` multiple times on the same object in
+          order to reconfigure  UART on the fly. That allows using single UART
+          peripheral to serve different devices attached to different GPIO pins.
+          Only one device can be served at a time in that case.
+          Also do not call ``deinit()`` as it will prevent calling ``init()``
+          again.
+        """
+        ...
+    def flush(self) -> Any:
+        """
+        Waits until all data has been sent. In case of a timeout, an exception is raised. The timeout
+        duration depends on the tx buffer size and the baud rate. Unless flow control is enabled, a timeout
+        should not occur.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call returns while the last byte is sent.
+            If required, a one character wait time has to be added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def irq(self, trigger, priority=1, handler=None, wake=IDLE) -> Any:
+        """
+        Create a callback to be triggered when data is received on the UART.
+
+            - *trigger* can only be ``UART.RX_ANY``
+            - *priority* level of the interrupt. Can take values in the range 1-7.
+              Higher values represent higher priorities.
+            - *handler* an optional function to be called when new characters arrive.
+            - *wake* can only be ``machine.IDLE``.
+
+        .. note::
+
+           The handler will be called whenever any of the following two conditions are met:
+
+               - 8 new characters have been received.
+               - At least 1 new character is waiting in the Rx buffer and the Rx line has been
+                 silent for the duration of 1 complete frame.
+
+           This means that when the handler function is called there will be between 1 to 8
+           characters waiting.
+
+        Returns an irq object.
+
+        Availability: WiPy.
+        """
+        ...
+    def txdone(self) -> bool:
+        """
+        Tells whether all data has been sent or no data transfer is happening. In this case,
+        it returns ``True``. If a data transmission is ongoing it returns ``False``.
+
+        .. note::
+
+            For the rp2, esp8266 and nrf ports the call may return ``True`` even if the last byte
+            of a transfer is still being sent. If required, a one character wait time has to be
+            added in the calling script.
+
+        Availability: rp2, esp32, esp8266, mimxrt, cc3200, stm32, nrf ports, renesas-ra
+        """
+        ...
+    def sendbreak(self) -> None:
+        """
+        Send a break condition on the bus. This drives the bus low for a duration
+        longer than required for a normal transmission of a character.
+        """
+        ...
+    def readchar(self, *args, **kwargs) -> Any: ...
+    def writechar(self, *args, **kwargs) -> Any: ...
+    def read(self, nbytes: Optional[Any] = None) -> bytes:
+        """
+        Read characters.  If ``nbytes`` is specified then read at most that many bytes,
+        otherwise read as much data as possible. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: a bytes object containing the bytes read in.  Returns ``None``
+        on timeout.
+        """
+        ...
+    def deinit(self) -> None:
+        """
+        Turn off the UART bus.
+
+        .. note::
+          You will not be able to call ``init()`` on the object after ``deinit()``.
+          A new instance needs to be created in that case.
+        """
+        ...
+    def any(self) -> int:
+        """
+        Returns an integer counting the number of characters that can be read without
+        blocking.  It will return 0 if there are no characters available and a positive
+        number if there are characters.  The method may return 1 even if there is more
+        than one character available for reading.
+
+        For more sophisticated querying of available characters use select.poll::
+
+         poll = select.poll()
+         poll.register(uart, select.POLLIN)
+         poll.poll(timeout)
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the bus.
+
+        Return value: number of bytes written or ``None`` on timeout.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
+        that many bytes.  Otherwise, read at most ``len(buf)`` bytes. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: number of bytes read and stored into ``buf`` or ``None`` on
+        timeout.
+        """
+        ...
+    def readline(self) -> None:
+        """
+        Read a line, ending in a newline character. It may return sooner if a timeout
+        is reached. The timeout is configurable in the constructor.
+
+        Return value: the line read or ``None`` on timeout.
+        """
+        ...
+    def __init__(self, id, *args, **kwargs) -> None: ...
+
+mem32: Any
+mem16: Any
+
+class SoftI2C(I2C):
+    """
+    Construct a new software I2C object.  The parameters are:
+
+       - *scl* should be a pin object specifying the pin to use for SCL.
+       - *sda* should be a pin object specifying the pin to use for SDA.
+       - *freq* should be an integer which sets the maximum frequency
+         for SCL.
+       - *timeout* is the maximum time in microseconds to wait for clock
+         stretching (SCL held low by another device on the bus), after
+         which an ``OSError(ETIMEDOUT)`` exception is raised.
+    """
+
+    def readfrom_mem_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_into(self, *args, **kwargs) -> Any: ...
+    def readfrom_mem(self, *args, **kwargs) -> Any: ...
+    def writeto_mem(self, *args, **kwargs) -> Any: ...
+    def scan(self, *args, **kwargs) -> Any: ...
+    def writeto(self, *args, **kwargs) -> Any: ...
+    def writevto(self, *args, **kwargs) -> Any: ...
+    def start(self, *args, **kwargs) -> Any: ...
+    def readfrom(self, *args, **kwargs) -> Any: ...
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def init(self, *args, **kwargs) -> Any: ...
+    def stop(self, *args, **kwargs) -> Any: ...
+    def write(self, *args, **kwargs) -> Any: ...
+    def __init__(self, scl, sda, *, freq=400000, timeout=50000) -> None: ...
+
+class Signal(Pin):
+    """
+            Signal(pin_arguments..., *, invert=False)
+
+    Create a Signal object. There're two ways to create it:
+
+    * By wrapping existing Pin object - universal method which works for
+      any board.
+    * By passing required Pin parameters directly to Signal constructor,
+      skipping the need to create intermediate Pin object. Available on
+      many, but not all boards.
+
+    The arguments are:
+
+      - ``pin_obj`` is existing Pin object.
+
+      - ``pin_arguments`` are the same arguments as can be passed to Pin constructor.
+
+      - ``invert`` - if True, the signal will be inverted (active low).
+    """
+
+    def off(self) -> None:
+        """
+        Deactivate signal.
+        """
+        ...
+    def on(self) -> None:
+        """
+        Activate signal.
+        """
+        ...
+    def value(self, x: Optional[Any] = None) -> int:
+        """
+        This method allows to set and get the value of the signal, depending on whether
+        the argument ``x`` is supplied or not.
+
+        If the argument is omitted then this method gets the signal level, 1 meaning
+        signal is asserted (active) and 0 - signal inactive.
+
+        If the argument is supplied then this method sets the signal level. The
+        argument ``x`` can be anything that converts to a boolean. If it converts
+        to ``True``, the signal is active, otherwise it is inactive.
+
+        Correspondence between signal being active and actual logic level on the
+        underlying pin depends on whether signal is inverted (active-low) or not.
+        For non-inverted signal, active status corresponds to logical 1, inactive -
+        to logical 0. For inverted/active-low signal, active status corresponds
+        to logical 0, while inactive - to logical 1.
+        """
+        ...
+    def __init__(self, pin_obj, *args, invert=False) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uos.pyi` & `micropython_stm32_stubs-1.20.0.post1/uos.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-"""
-basic "operating system" services. See: https://docs.micropython.org/en/v1.19.1/library/os.html
-
-|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
-
-The ``os`` module contains functions for filesystem access and mounting,
-terminal redirection and duplication, and the ``uname`` and ``urandom``
-functions.
-"""
-from typing import IO, Iterator, Optional, Tuple, Any
-from stdlib.os import uname_result
-
-sep: str
-
-def statvfs(path) -> Tuple:
-    """
-    Get the status of a fileystem.
-
-    Returns a tuple with the filesystem information in the following order:
-
-         * ``f_bsize`` -- file system block size
-         * ``f_frsize`` -- fragment size
-         * ``f_blocks`` -- size of fs in f_frsize units
-         * ``f_bfree`` -- number of free blocks
-         * ``f_bavail`` -- number of free blocks for unprivileged users
-         * ``f_files`` -- number of inodes
-         * ``f_ffree`` -- number of free inodes
-         * ``f_favail`` -- number of free inodes for unprivileged users
-         * ``f_flag`` -- mount flags
-         * ``f_namemax`` -- maximum filename length
-
-    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
-    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
-    in a port-specific implementation.
-    """
-    ...
-
-def stat(path) -> Any:
-    """
-    Get the status of a file or directory.
-    """
-    ...
-
-def rmdir(path) -> None:
-    """
-    Remove a directory.
-    """
-    ...
-
-def rename(old_path, new_path) -> None:
-    """
-    Rename a file.
-    """
-    ...
-
-def mount(fsobj, mount_point, *, readonly) -> Any:
-    """
-    Mount the filesystem object *fsobj* at the location in the VFS given by the
-    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
-    method, or a block device.  If it's a block device then the filesystem type
-    is automatically detected (an exception is raised if no filesystem was
-    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
-    or ``'/<name>'`` to mount it at a subdirectory under the root.
-
-    If *readonly* is ``True`` then the filesystem is mounted read-only.
-
-    During the mount process the method ``mount()`` is called on the filesystem
-    object.
-
-    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
-    """
-    ...
-
-def sync() -> None:
-    """
-    Sync all filesystems.
-    """
-    ...
-
-def unlink(*args, **kwargs) -> Any: ...
-def uname() -> uname_result:
-    """
-    Return a tuple (possibly a named tuple) containing information about the
-    underlying machine and/or its operating system.  The tuple has five fields
-    in the following order, each of them being a string:
-
-         * ``sysname`` -- the name of the underlying system
-         * ``nodename`` -- the network name (can be the same as ``sysname``)
-         * ``release`` -- the version of the underlying system
-         * ``version`` -- the MicroPython version and build date
-         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
-    """
-    ...
-
-def umount(mount_point) -> Any:
-    """
-    Unmount a filesystem. *mount_point* can be a string naming the mount location,
-    or a previously-mounted filesystem object.  During the unmount process the
-    method ``umount()`` is called on the filesystem object.
-
-    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
-    """
-    ...
-
-def urandom(n) -> bytes:
-    """
-    Return a bytes object with *n* random bytes. Whenever possible, it is
-    generated by the hardware random number generator.
-    """
-    ...
-
-def chdir(path) -> Any:
-    """
-    Change current directory.
-    """
-    ...
-
-def dupterm(stream_object, index=0, /) -> IO:
-    """
-    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
-    object. The *stream_object* argument must be a native stream object, or derive
-    from ``io.IOBase`` and implement the ``readinto()`` and
-    ``write()`` methods.  The stream should be in non-blocking mode and
-    ``readinto()`` should return ``None`` if there is no data available for reading.
-
-    After calling this function all terminal output is repeated on this stream,
-    and any input that is available on the stream is passed on to the terminal input.
-
-    The *index* parameter should be a non-negative integer and specifies which
-    duplication slot is set.  A given port may implement more than one slot (slot 0
-    will always be available) and in that case terminal input and output is
-    duplicated on all the slots that are set.
-
-    If ``None`` is passed as the *stream_object* then duplication is cancelled on
-    the slot given by *index*.
-
-    The function returns the previous stream-like object in the given slot.
-    """
-    ...
-
-def remove(path) -> None:
-    """
-    Remove a file.
-    """
-    ...
-
-def mkdir(path) -> Any:
-    """
-    Create a new directory.
-    """
-    ...
-
-def getcwd() -> Any:
-    """
-    Get the current directory.
-    """
-    ...
-
-def listdir(dir: Optional[Any] = None) -> Any:
-    """
-    With no argument, list the current directory.  Otherwise list the given directory.
-    """
-    ...
-
-def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
-    """
-    This function returns an iterator which then yields tuples corresponding to
-    the entries in the directory that it is listing.  With no argument it lists the
-    current directory, otherwise it lists the directory given by *dir*.
-
-    The tuples have the form *(name, type, inode[, size])*:
-
-     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
-       the entry;
-     - *type* is an integer that specifies the type of the entry, with 0x4000 for
-       directories and 0x8000 for regular files;
-     - *inode* is an integer corresponding to the inode of the file, and may be 0
-       for filesystems that don't have such a notion.
-     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
-       file entries, *size* is an integer representing the size of the file
-       or -1 if unknown.  Its meaning is currently undefined for directory
-       entries.
-    """
-    ...
-
-class VfsLfs2:
-    """
-    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
-    Storage of the littlefs filesystem is provided by *block_dev*, which must
-    support the :ref:`extended interface <block-device-interface>`.
-    Objects created by this constructor can be mounted using :func:`mount`.
-
-    The *mtime* argument enables modification timestamps for files, stored using
-    littlefs attributes.  This option can be disabled or enabled differently each
-    mount time and timestamps will only be added or updated if *mtime* is enabled,
-    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
-    timestamps will work without reformatting and timestamps will be added
-    transparently to existing files once they are opened for writing.  When *mtime*
-    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
-
-    See :ref:`filesystem` for more information.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
-        """
-            Build a Lfs2 filesystem on *block_dev*.
-
-        ``Note:`` There are reports of littlefs v2 failing in certain situations,
-                  for details see `littlefs issue 295`_.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
-
-class VfsFat:
-    """
-    Create a filesystem object that uses the FAT filesystem format.  Storage of
-    the FAT filesystem is provided by *block_dev*.
-    Objects created by this constructor can be mounted using :func:`mount`.
-    """
-
-    def rename(self, *args, **kwargs) -> Any: ...
-    @staticmethod
-    def mkfs(block_dev) -> None:
-        """
-        Build a FAT filesystem on *block_dev*.
-        """
-        ...
-    def mount(self, *args, **kwargs) -> Any: ...
-    def statvfs(self, *args, **kwargs) -> Any: ...
-    def rmdir(self, *args, **kwargs) -> Any: ...
-    def stat(self, *args, **kwargs) -> Any: ...
-    def umount(self, *args, **kwargs) -> Any: ...
-    def remove(self, *args, **kwargs) -> Any: ...
-    def mkdir(self, *args, **kwargs) -> Any: ...
-    def open(self, *args, **kwargs) -> Any: ...
-    def ilistdir(self, *args, **kwargs) -> Any: ...
-    def chdir(self, *args, **kwargs) -> Any: ...
-    def getcwd(self, *args, **kwargs) -> Any: ...
-    def __init__(self, block_dev) -> None: ...
+"""
+basic "operating system" services. See: https://docs.micropython.org/en/v1.20.0/library/os.html
+
+|see_cpython_module| :mod:`python:os` https://docs.python.org/3/library/os.html .
+
+The ``os`` module contains functions for filesystem access and mounting,
+terminal redirection and duplication, and the ``uname`` and ``urandom``
+functions.
+"""
+from typing import IO, Iterator, Optional, Tuple, Any
+from stdlib.os import uname_result
+
+sep: str
+
+def statvfs(path) -> Tuple:
+    """
+    Get the status of a fileystem.
+
+    Returns a tuple with the filesystem information in the following order:
+
+         * ``f_bsize`` -- file system block size
+         * ``f_frsize`` -- fragment size
+         * ``f_blocks`` -- size of fs in f_frsize units
+         * ``f_bfree`` -- number of free blocks
+         * ``f_bavail`` -- number of free blocks for unprivileged users
+         * ``f_files`` -- number of inodes
+         * ``f_ffree`` -- number of free inodes
+         * ``f_favail`` -- number of free inodes for unprivileged users
+         * ``f_flag`` -- mount flags
+         * ``f_namemax`` -- maximum filename length
+
+    Parameters related to inodes: ``f_files``, ``f_ffree``, ``f_avail``
+    and the ``f_flags`` parameter may return ``0`` as they can be unavailable
+    in a port-specific implementation.
+    """
+    ...
+
+def stat(path) -> Any:
+    """
+    Get the status of a file or directory.
+    """
+    ...
+
+def rmdir(path) -> None:
+    """
+    Remove a directory.
+    """
+    ...
+
+def rename(old_path, new_path) -> None:
+    """
+    Rename a file.
+    """
+    ...
+
+def mount(fsobj, mount_point, *, readonly) -> Any:
+    """
+    Mount the filesystem object *fsobj* at the location in the VFS given by the
+    *mount_point* string.  *fsobj* can be a a VFS object that has a ``mount()``
+    method, or a block device.  If it's a block device then the filesystem type
+    is automatically detected (an exception is raised if no filesystem was
+    recognised).  *mount_point* may be ``'/'`` to mount *fsobj* at the root,
+    or ``'/<name>'`` to mount it at a subdirectory under the root.
+
+    If *readonly* is ``True`` then the filesystem is mounted read-only.
+
+    During the mount process the method ``mount()`` is called on the filesystem
+    object.
+
+    Will raise ``OSError(EPERM)`` if *mount_point* is already mounted.
+    """
+    ...
+
+def sync() -> None:
+    """
+    Sync all filesystems.
+    """
+    ...
+
+def unlink(*args, **kwargs) -> Any: ...
+def uname() -> uname_result:
+    """
+    Return a tuple (possibly a named tuple) containing information about the
+    underlying machine and/or its operating system.  The tuple has five fields
+    in the following order, each of them being a string:
+
+         * ``sysname`` -- the name of the underlying system
+         * ``nodename`` -- the network name (can be the same as ``sysname``)
+         * ``release`` -- the version of the underlying system
+         * ``version`` -- the MicroPython version and build date
+         * ``machine`` -- an identifier for the underlying hardware (eg board, CPU)
+    """
+    ...
+
+def umount(mount_point) -> Any:
+    """
+    Unmount a filesystem. *mount_point* can be a string naming the mount location,
+    or a previously-mounted filesystem object.  During the unmount process the
+    method ``umount()`` is called on the filesystem object.
+
+    Will raise ``OSError(EINVAL)`` if *mount_point* is not found.
+    """
+    ...
+
+def urandom(n) -> bytes:
+    """
+    Return a bytes object with *n* random bytes. Whenever possible, it is
+    generated by the hardware random number generator.
+    """
+    ...
+
+def chdir(path) -> Any:
+    """
+    Change current directory.
+    """
+    ...
+
+def dupterm(stream_object, index=0, /) -> IO:
+    """
+    Duplicate or switch the MicroPython terminal (the REPL) on the given `stream`-like
+    object. The *stream_object* argument must be a native stream object, or derive
+    from ``io.IOBase`` and implement the ``readinto()`` and
+    ``write()`` methods.  The stream should be in non-blocking mode and
+    ``readinto()`` should return ``None`` if there is no data available for reading.
+
+    After calling this function all terminal output is repeated on this stream,
+    and any input that is available on the stream is passed on to the terminal input.
+
+    The *index* parameter should be a non-negative integer and specifies which
+    duplication slot is set.  A given port may implement more than one slot (slot 0
+    will always be available) and in that case terminal input and output is
+    duplicated on all the slots that are set.
+
+    If ``None`` is passed as the *stream_object* then duplication is cancelled on
+    the slot given by *index*.
+
+    The function returns the previous stream-like object in the given slot.
+    """
+    ...
+
+def remove(path) -> None:
+    """
+    Remove a file.
+    """
+    ...
+
+def mkdir(path) -> Any:
+    """
+    Create a new directory.
+    """
+    ...
+
+def getcwd() -> Any:
+    """
+    Get the current directory.
+    """
+    ...
+
+def listdir(dir: Optional[Any] = None) -> Any:
+    """
+    With no argument, list the current directory.  Otherwise list the given directory.
+    """
+    ...
+
+def ilistdir(dir: Optional[Any] = None) -> Iterator[Tuple]:
+    """
+    This function returns an iterator which then yields tuples corresponding to
+    the entries in the directory that it is listing.  With no argument it lists the
+    current directory, otherwise it lists the directory given by *dir*.
+
+    The tuples have the form *(name, type, inode[, size])*:
+
+     - *name* is a string (or bytes if *dir* is a bytes object) and is the name of
+       the entry;
+     - *type* is an integer that specifies the type of the entry, with 0x4000 for
+       directories and 0x8000 for regular files;
+     - *inode* is an integer corresponding to the inode of the file, and may be 0
+       for filesystems that don't have such a notion.
+     - Some platforms may return a 4-tuple that includes the entry's *size*.  For
+       file entries, *size* is an integer representing the size of the file
+       or -1 if unknown.  Its meaning is currently undefined for directory
+       entries.
+    """
+    ...
+
+class VfsLfs2:
+    """
+    Create a filesystem object that uses the `littlefs v2 filesystem format`_.
+    Storage of the littlefs filesystem is provided by *block_dev*, which must
+    support the :ref:`extended interface <block-device-interface>`.
+    Objects created by this constructor can be mounted using :func:`mount`.
+
+    The *mtime* argument enables modification timestamps for files, stored using
+    littlefs attributes.  This option can be disabled or enabled differently each
+    mount time and timestamps will only be added or updated if *mtime* is enabled,
+    otherwise the timestamps will remain untouched.  Littlefs v2 filesystems without
+    timestamps will work without reformatting and timestamps will be added
+    transparently to existing files once they are opened for writing.  When *mtime*
+    is enabled `os.stat` on files without timestamps will return 0 for the timestamp.
+
+    See :ref:`filesystem` for more information.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev, readsize=32, progsize=32, lookahead=32) -> None:
+        """
+            Build a Lfs2 filesystem on *block_dev*.
+
+        ``Note:`` There are reports of littlefs v2 failing in certain situations,
+                  for details see `littlefs issue 295`_.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev, readsize=32, progsize=32, lookahead=32, mtime=True) -> None: ...
+
+class VfsFat:
+    """
+    Create a filesystem object that uses the FAT filesystem format.  Storage of
+    the FAT filesystem is provided by *block_dev*.
+    Objects created by this constructor can be mounted using :func:`mount`.
+    """
+
+    def rename(self, *args, **kwargs) -> Any: ...
+    @staticmethod
+    def mkfs(block_dev) -> None:
+        """
+        Build a FAT filesystem on *block_dev*.
+        """
+        ...
+    def mount(self, *args, **kwargs) -> Any: ...
+    def statvfs(self, *args, **kwargs) -> Any: ...
+    def rmdir(self, *args, **kwargs) -> Any: ...
+    def stat(self, *args, **kwargs) -> Any: ...
+    def umount(self, *args, **kwargs) -> Any: ...
+    def remove(self, *args, **kwargs) -> Any: ...
+    def mkdir(self, *args, **kwargs) -> Any: ...
+    def open(self, *args, **kwargs) -> Any: ...
+    def ilistdir(self, *args, **kwargs) -> Any: ...
+    def chdir(self, *args, **kwargs) -> Any: ...
+    def getcwd(self, *args, **kwargs) -> Any: ...
+    def __init__(self, block_dev) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uselect.pyi` & `micropython_stm32_stubs-1.20.0.post1/uselect.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-"""
-wait for events on a set of streams. See: https://docs.micropython.org/en/v1.19.1/library/select.html
-
-|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
-
-This module provides functions to efficiently wait for events on multiple
-`streams <stream>` (select streams which are ready for operations).
-"""
-from typing import Iterator, List, Optional, Tuple, Any
-
-POLLOUT: int
-POLLIN: int
-POLLHUP: int
-POLLERR: int
-
-class select:
-    """
-    Wait for activity on a set of objects.
-
-    This function is provided by some MicroPython ports for compatibility
-    and is not efficient. Usage of :class:`Poll` is recommended instead.
-    """
-
-    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
-
-class poll:
-    """
-    Create an instance of the Poll class.
-    """
-
-    def __init__(self) -> None: ...
-    def register(self, obj, eventmask: Optional[Any] = None) -> None:
-        """
-        Register `stream` *obj* for polling. *eventmask* is logical OR of:
-
-        * ``select.POLLIN``  - data available for reading
-        * ``select.POLLOUT`` - more data can be written
-
-        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
-        *not* valid as input eventmask (these are unsolicited events which
-        will be returned from `poll()` regardless of whether they are asked
-        for). This semantics is per POSIX.
-
-        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
-
-        It is OK to call this function multiple times for the same *obj*.
-        Successive calls will update *obj*'s eventmask to the value of
-        *eventmask* (i.e. will behave as `modify()`).
-        """
-        ...
-    def unregister(self, obj) -> Any:
-        """
-        Unregister *obj* from polling.
-        """
-        ...
-    def modify(self, obj, eventmask) -> None:
-        """
-        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
-        is raised with error of ENOENT.
-        """
-        ...
-    def poll(self, timeout=-1, /) -> List:
-        """
-        Wait for at least one of the registered objects to become ready or have an
-        exceptional condition, with optional timeout in milliseconds (if *timeout*
-        arg is not specified or -1, there is no timeout).
-
-        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
-        tuple, depending on a platform and version, so don't assume that its size is 2.
-        The ``event`` element specifies which events happened with a stream and
-        is a combination of ``select.POLL*`` constants described above. Note that
-        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
-        (even if were not asked for), and must be acted on accordingly (the
-        corresponding stream unregistered from poll and likely closed), because
-        otherwise all further invocations of `poll()` may return immediately with
-        these flags set for this stream again.
-
-        In case of timeout, an empty list is returned.
-        """
-        ...
-    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
-        """
-        Like :meth:`poll.poll`, but instead returns an iterator which yields a
-        `callee-owned tuple`. This function provides an efficient, allocation-free
-        way to poll on streams.
-
-        If *flags* is 1, one-shot behaviour for events is employed: streams for
-        which events happened will have their event masks automatically reset
-        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
-        won't be processed until new mask is set with `poll.modify()`. This
-        behaviour is useful for asynchronous I/O schedulers.
-        """
-        ...
+"""
+wait for events on a set of streams. See: https://docs.micropython.org/en/v1.20.0/library/select.html
+
+|see_cpython_module| :mod:`python:select` https://docs.python.org/3/library/select.html .
+
+This module provides functions to efficiently wait for events on multiple
+`streams <stream>` (select streams which are ready for operations).
+"""
+from typing import Iterator, List, Optional, Tuple, Any
+
+POLLOUT: int
+POLLIN: int
+POLLHUP: int
+POLLERR: int
+
+class select:
+    """
+    Wait for activity on a set of objects.
+
+    This function is provided by some MicroPython ports for compatibility
+    and is not efficient. Usage of :class:`Poll` is recommended instead.
+    """
+
+    def __init__(self, rlist, wlist, xlist, timeout: Optional[Any] = None) -> None: ...
+
+class poll:
+    """
+    Create an instance of the Poll class.
+    """
+
+    def __init__(self) -> None: ...
+    def register(self, obj, eventmask: Optional[Any] = None) -> None:
+        """
+        Register `stream` *obj* for polling. *eventmask* is logical OR of:
+
+        * ``select.POLLIN``  - data available for reading
+        * ``select.POLLOUT`` - more data can be written
+
+        Note that flags like ``select.POLLHUP`` and ``select.POLLERR`` are
+        *not* valid as input eventmask (these are unsolicited events which
+        will be returned from `poll()` regardless of whether they are asked
+        for). This semantics is per POSIX.
+
+        *eventmask* defaults to ``select.POLLIN | select.POLLOUT``.
+
+        It is OK to call this function multiple times for the same *obj*.
+        Successive calls will update *obj*'s eventmask to the value of
+        *eventmask* (i.e. will behave as `modify()`).
+        """
+        ...
+    def unregister(self, obj) -> Any:
+        """
+        Unregister *obj* from polling.
+        """
+        ...
+    def modify(self, obj, eventmask) -> None:
+        """
+        Modify the *eventmask* for *obj*. If *obj* is not registered, `OSError`
+        is raised with error of ENOENT.
+        """
+        ...
+    def poll(self, timeout=-1, /) -> List:
+        """
+        Wait for at least one of the registered objects to become ready or have an
+        exceptional condition, with optional timeout in milliseconds (if *timeout*
+        arg is not specified or -1, there is no timeout).
+
+        Returns list of (``obj``, ``event``, ...) tuples. There may be other elements in
+        tuple, depending on a platform and version, so don't assume that its size is 2.
+        The ``event`` element specifies which events happened with a stream and
+        is a combination of ``select.POLL*`` constants described above. Note that
+        flags ``select.POLLHUP`` and ``select.POLLERR`` can be returned at any time
+        (even if were not asked for), and must be acted on accordingly (the
+        corresponding stream unregistered from poll and likely closed), because
+        otherwise all further invocations of `poll()` may return immediately with
+        these flags set for this stream again.
+
+        In case of timeout, an empty list is returned.
+        """
+        ...
+    def ipoll(self, timeout=-1, flags=0, /) -> Iterator[Tuple]:
+        """
+        Like :meth:`poll.poll`, but instead returns an iterator which yields a
+        `callee-owned tuple`. This function provides an efficient, allocation-free
+        way to poll on streams.
+
+        If *flags* is 1, one-shot behaviour for events is employed: streams for
+        which events happened will have their event masks automatically reset
+        (equivalent to ``poll.modify(obj, 0)``), so new events for such a stream
+        won't be processed until new mask is set with `poll.modify()`. This
+        behaviour is useful for asynchronous I/O schedulers.
+        """
+        ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/usocket.pyi` & `micropython_stm32_stubs-1.20.0.post1/usocket.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-"""
-socket module. See: https://docs.micropython.org/en/v1.19.1/library/socket.html
-
-|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
-
-This module provides access to the BSD socket interface.
-"""
-from typing import IO, Optional, Tuple, Any
-
-SO_KEEPALIVE: int
-SOL_SOCKET: int
-SO_SNDTIMEO: int
-SO_RCVTIMEO: int
-SO_REUSEADDR: int
-AF_INET6: int
-AF_INET: int
-SOCK_STREAM: int
-SOCK_DGRAM: int
-SOCK_RAW: int
-
-def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
-    """
-    Translate the host/port argument into a sequence of 5-tuples that contain all the
-    necessary arguments for creating a socket connected to that service. Arguments
-    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
-    can be used to filter which kind of addresses are returned. If a parameter is not
-    specified or zero, all combinations of addresses can be returned (requiring
-    filtering on the user side).
-
-    The resulting list of 5-tuples has the following structure::
-
-       (family, type, proto, canonname, sockaddr)
-
-    The following example shows how to connect to a given url::
-
-       s = socket.socket()
-       # This assumes that if "type" is not specified, an address for
-       # SOCK_STREAM will be returned, which may be not true
-       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
-
-    Recommended use of filtering params::
-
-       s = socket.socket()
-       # Guaranteed to return an address which can be connect'ed to for
-       # stream operation.
-       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
-    """
-    ...
-
-class socket:
-    """
-    Create a new socket using the given address family, socket type and
-    protocol number. Note that specifying *proto* in most cases is not
-    required (and not recommended, as some MicroPython ports may omit
-    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
-    protocol automatically::
-
-         # Create STREAM TCP socket
-         socket(AF_INET, SOCK_STREAM)
-         # Create DGRAM UDP socket
-         socket(AF_INET, SOCK_DGRAM)
-    """
-
-    def recvfrom(self, bufsize) -> Tuple:
-        """
-        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
-        bytes object representing the data received and *address* is the address of the socket sending
-        the data.
-        """
-        ...
-    def recv(self, bufsize) -> bytes:
-        """
-        Receive data from the socket. The return value is a bytes object representing the data
-        received. The maximum amount of data to be received at once is specified by bufsize.
-        """
-        ...
-    def makefile(self, mode="rb", buffering=0, /) -> IO:
-        """
-        Return a file object associated with the socket. The exact returned type depends on the arguments
-        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
-        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
-        """
-        ...
-    def listen(self, backlog: Optional[Any] = None) -> None:
-        """
-        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
-        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
-        that the system will allow before refusing new connections. If not specified, a default
-        reasonable value is chosen.
-        """
-        ...
-    def settimeout(self, value) -> Any:
-        """
-        **Note**: Not every port supports this method, see below.
-
-        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
-        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
-        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
-        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
-        is put in blocking mode.
-
-        Not every :term:`MicroPython port` supports this method. A more portable and
-        generic solution is to use `select.poll` object. This allows to wait on
-        multiple objects at the same time (and not just on sockets, but on generic
-        `stream` objects which support polling). Example::
-
-             # Instead of:
-             s.settimeout(1.0)  # time in seconds
-             s.read(10)  # may timeout
-
-             # Use:
-             poller = select.poll()
-             poller.register(s, select.POLLIN)
-             res = poller.poll(1000)  # time in milliseconds
-             if not res:
-                 # s is still not ready for input, i.e. operation timed out
-        """
-        ...
-    def sendall(self, bytes) -> int:
-        """
-        Send all data to the socket. The socket must be connected to a remote socket.
-        Unlike `send()`, this method will try to send all of data, by sending data
-        chunk by chunk consecutively.
-
-        The behaviour of this method on non-blocking sockets is undefined. Due to this,
-        on MicroPython, it's recommended to use `write()` method instead, which
-        has the same "no short writes" policy for blocking sockets, and will return
-        number of bytes sent on non-blocking sockets.
-        """
-        ...
-    def setsockopt(self, level, optname, value) -> None:
-        """
-        Set the value of the given socket option. The needed symbolic constants are defined in the
-        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
-        a buffer.
-        """
-        ...
-    def setblocking(self, flag) -> Any:
-        """
-        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
-        else to blocking mode.
-
-        This method is a shorthand for certain `settimeout()` calls:
-
-        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
-        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
-        """
-        ...
-    def sendto(self, bytes, address) -> None:
-        """
-        Send data to the socket. The socket should not be connected to a remote socket, since the
-        destination socket is specified by *address*.
-        """
-        ...
-    def readline(self) -> Any:
-        """
-        Read a line, ending in a newline character.
-
-        Return value: the line read.
-        """
-        ...
-    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
-        """
-        Read bytes into the *buf*.  If *nbytes* is specified then read at most
-        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
-        `read()`, this method follows "no short reads" policy.
-
-        Return value: number of bytes read and stored into *buf*.
-        """
-        ...
-    def read(self, size: Optional[Any] = None) -> bytes:
-        """
-        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
-        reads all data available from the socket until EOF; as such the method will not return until
-        the socket is closed. This function tries to read as much data as
-        requested (no "short reads"). This may be not possible with
-        non-blocking socket though, and then less data will be returned.
-        """
-        ...
-    def close(self) -> Any:
-        """
-        Mark the socket closed and release all resources. Once that happens, all future operations
-        on the socket object will fail. The remote end will receive EOF indication if
-        supported by protocol.
-
-        Sockets are automatically closed when they are garbage-collected, but it is recommended
-        to `close()` them explicitly as soon you finished working with them.
-        """
-        ...
-    def connect(self, address) -> None:
-        """
-        Connect to a remote socket at *address*.
-        """
-        ...
-    def send(self, bytes) -> int:
-        """
-        Send data to the socket. The socket must be connected to a remote socket.
-        Returns number of bytes sent, which may be smaller than the length of data
-        ("short write").
-        """
-        ...
-    def bind(self, address) -> Any:
-        """
-        Bind the socket to *address*. The socket must not already be bound.
-        """
-        ...
-    def accept(self) -> Tuple:
-        """
-        Accept a connection. The socket must be bound to an address and listening for connections.
-        The return value is a pair (conn, address) where conn is a new socket object usable to send
-        and receive data on the connection, and address is the address bound to the socket on the
-        other end of the connection.
-        """
-        ...
-    def write(self, buf) -> int:
-        """
-        Write the buffer of bytes to the socket. This function will try to
-        write all data to a socket (no "short writes"). This may be not possible
-        with a non-blocking socket though, and returned value will be less than
-        the length of *buf*.
-
-        Return value: number of bytes written.
-        """
-        ...
-    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
+"""
+socket module. See: https://docs.micropython.org/en/v1.20.0/library/socket.html
+
+|see_cpython_module| :mod:`python:socket` https://docs.python.org/3/library/socket.html .
+
+This module provides access to the BSD socket interface.
+"""
+from typing import IO, Optional, Tuple, Any
+
+SO_KEEPALIVE: int
+SOL_SOCKET: int
+SO_SNDTIMEO: int
+SO_RCVTIMEO: int
+SO_REUSEADDR: int
+AF_INET6: int
+AF_INET: int
+SOCK_STREAM: int
+SOCK_DGRAM: int
+SOCK_RAW: int
+
+def getaddrinfo(host, port, af=0, type=0, proto=0, flags=0, /) -> Any:
+    """
+    Translate the host/port argument into a sequence of 5-tuples that contain all the
+    necessary arguments for creating a socket connected to that service. Arguments
+    *af*, *type*, and *proto* (which have the same meaning as for the `socket()` function)
+    can be used to filter which kind of addresses are returned. If a parameter is not
+    specified or zero, all combinations of addresses can be returned (requiring
+    filtering on the user side).
+
+    The resulting list of 5-tuples has the following structure::
+
+       (family, type, proto, canonname, sockaddr)
+
+    The following example shows how to connect to a given url::
+
+       s = socket.socket()
+       # This assumes that if "type" is not specified, an address for
+       # SOCK_STREAM will be returned, which may be not true
+       s.connect(socket.getaddrinfo('www.micropython.org', 80)[0][-1])
+
+    Recommended use of filtering params::
+
+       s = socket.socket()
+       # Guaranteed to return an address which can be connect'ed to for
+       # stream operation.
+       s.connect(socket.getaddrinfo('www.micropython.org', 80, 0, SOCK_STREAM)[0][-1])
+    """
+    ...
+
+class socket:
+    """
+    Create a new socket using the given address family, socket type and
+    protocol number. Note that specifying *proto* in most cases is not
+    required (and not recommended, as some MicroPython ports may omit
+    ``IPPROTO_*`` constants). Instead, *type* argument will select needed
+    protocol automatically::
+
+         # Create STREAM TCP socket
+         socket(AF_INET, SOCK_STREAM)
+         # Create DGRAM UDP socket
+         socket(AF_INET, SOCK_DGRAM)
+    """
+
+    def recvfrom(self, bufsize) -> Tuple:
+        """
+        Receive data from the socket. The return value is a pair *(bytes, address)* where *bytes* is a
+        bytes object representing the data received and *address* is the address of the socket sending
+        the data.
+        """
+        ...
+    def recv(self, bufsize) -> bytes:
+        """
+        Receive data from the socket. The return value is a bytes object representing the data
+        received. The maximum amount of data to be received at once is specified by bufsize.
+        """
+        ...
+    def makefile(self, mode="rb", buffering=0, /) -> IO:
+        """
+        Return a file object associated with the socket. The exact returned type depends on the arguments
+        given to makefile(). The support is limited to binary modes only ('rb', 'wb', and 'rwb').
+        CPython's arguments: *encoding*, *errors* and *newline* are not supported.
+        """
+        ...
+    def listen(self, backlog: Optional[Any] = None) -> None:
+        """
+        Enable a server to accept connections. If *backlog* is specified, it must be at least 0
+        (if it's lower, it will be set to 0); and specifies the number of unaccepted connections
+        that the system will allow before refusing new connections. If not specified, a default
+        reasonable value is chosen.
+        """
+        ...
+    def settimeout(self, value) -> Any:
+        """
+        **Note**: Not every port supports this method, see below.
+
+        Set a timeout on blocking socket operations. The value argument can be a nonnegative floating
+        point number expressing seconds, or None. If a non-zero value is given, subsequent socket operations
+        will raise an `OSError` exception if the timeout period value has elapsed before the operation has
+        completed. If zero is given, the socket is put in non-blocking mode. If None is given, the socket
+        is put in blocking mode.
+
+        Not every :term:`MicroPython port` supports this method. A more portable and
+        generic solution is to use `select.poll` object. This allows to wait on
+        multiple objects at the same time (and not just on sockets, but on generic
+        `stream` objects which support polling). Example::
+
+             # Instead of:
+             s.settimeout(1.0)  # time in seconds
+             s.read(10)  # may timeout
+
+             # Use:
+             poller = select.poll()
+             poller.register(s, select.POLLIN)
+             res = poller.poll(1000)  # time in milliseconds
+             if not res:
+                 # s is still not ready for input, i.e. operation timed out
+        """
+        ...
+    def sendall(self, bytes) -> int:
+        """
+        Send all data to the socket. The socket must be connected to a remote socket.
+        Unlike `send()`, this method will try to send all of data, by sending data
+        chunk by chunk consecutively.
+
+        The behaviour of this method on non-blocking sockets is undefined. Due to this,
+        on MicroPython, it's recommended to use `write()` method instead, which
+        has the same "no short writes" policy for blocking sockets, and will return
+        number of bytes sent on non-blocking sockets.
+        """
+        ...
+    def setsockopt(self, level, optname, value) -> None:
+        """
+        Set the value of the given socket option. The needed symbolic constants are defined in the
+        socket module (SO_* etc.). The *value* can be an integer or a bytes-like object representing
+        a buffer.
+        """
+        ...
+    def setblocking(self, flag) -> Any:
+        """
+        Set blocking or non-blocking mode of the socket: if flag is false, the socket is set to non-blocking,
+        else to blocking mode.
+
+        This method is a shorthand for certain `settimeout()` calls:
+
+        * ``sock.setblocking(True)`` is equivalent to ``sock.settimeout(None)``
+        * ``sock.setblocking(False)`` is equivalent to ``sock.settimeout(0)``
+        """
+        ...
+    def sendto(self, bytes, address) -> None:
+        """
+        Send data to the socket. The socket should not be connected to a remote socket, since the
+        destination socket is specified by *address*.
+        """
+        ...
+    def readline(self) -> Any:
+        """
+        Read a line, ending in a newline character.
+
+        Return value: the line read.
+        """
+        ...
+    def readinto(self, buf, nbytes: Optional[Any] = None) -> int:
+        """
+        Read bytes into the *buf*.  If *nbytes* is specified then read at most
+        that many bytes.  Otherwise, read at most *len(buf)* bytes. Just as
+        `read()`, this method follows "no short reads" policy.
+
+        Return value: number of bytes read and stored into *buf*.
+        """
+        ...
+    def read(self, size: Optional[Any] = None) -> bytes:
+        """
+        Read up to size bytes from the socket. Return a bytes object. If *size* is not given, it
+        reads all data available from the socket until EOF; as such the method will not return until
+        the socket is closed. This function tries to read as much data as
+        requested (no "short reads"). This may be not possible with
+        non-blocking socket though, and then less data will be returned.
+        """
+        ...
+    def close(self) -> Any:
+        """
+        Mark the socket closed and release all resources. Once that happens, all future operations
+        on the socket object will fail. The remote end will receive EOF indication if
+        supported by protocol.
+
+        Sockets are automatically closed when they are garbage-collected, but it is recommended
+        to `close()` them explicitly as soon you finished working with them.
+        """
+        ...
+    def connect(self, address) -> None:
+        """
+        Connect to a remote socket at *address*.
+        """
+        ...
+    def send(self, bytes) -> int:
+        """
+        Send data to the socket. The socket must be connected to a remote socket.
+        Returns number of bytes sent, which may be smaller than the length of data
+        ("short write").
+        """
+        ...
+    def bind(self, address) -> Any:
+        """
+        Bind the socket to *address*. The socket must not already be bound.
+        """
+        ...
+    def accept(self) -> Tuple:
+        """
+        Accept a connection. The socket must be bound to an address and listening for connections.
+        The return value is a pair (conn, address) where conn is a new socket object usable to send
+        and receive data on the connection, and address is the address bound to the socket on the
+        other end of the connection.
+        """
+        ...
+    def write(self, buf) -> int:
+        """
+        Write the buffer of bytes to the socket. This function will try to
+        write all data to a socket (no "short writes"). This may be not possible
+        with a non-blocking socket though, and returned value will be less than
+        the length of *buf*.
+
+        Return value: number of bytes written.
+        """
+        ...
+    def __init__(self, af=AF_INET, type=SOCK_STREAM, proto=IPPROTO_TCP, /) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/usys.pyi` & `micropython_stm32_stubs-1.20.0.post1/usys.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-system specific functions. See: https://docs.micropython.org/en/v1.19.1/library/sys.html
-
-|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
-"""
-from typing import Dict, List, Tuple, Any
-
-platform: str
-version_info: tuple
-path: list
-version: str
-ps1: str
-ps2: str
-byteorder: str
-modules: dict
-argv: list
-implementation: tuple
-maxsize: int
-
-def print_exception(exc, file=stdout, /) -> None:
-    """
-    Print exception with a traceback to a file-like object *file* (or
-    `sys.stdout` by default).
-    """
-    ...
-
-def exit(retval=0, /) -> Any:
-    """
-    Terminate current program with a given exit code. Underlyingly, this
-    function raise as `SystemExit` exception. If an argument is given, its
-    value given as an argument to `SystemExit`.
-    """
-    ...
-
-stderr: Any
-stdout: Any
-stdin: Any
+"""
+system specific functions. See: https://docs.micropython.org/en/v1.20.0/library/sys.html
+
+|see_cpython_module| :mod:`python:sys` https://docs.python.org/3/library/sys.html .
+"""
+from typing import Dict, List, Tuple, Any
+
+platform: str
+version_info: tuple
+path: list
+version: str
+ps1: str
+ps2: str
+byteorder: str
+modules: dict
+argv: list
+implementation: tuple
+maxsize: int
+
+def print_exception(exc, file=stdout, /) -> None:
+    """
+    Print exception with a traceback to a file-like object *file* (or
+    `sys.stdout` by default).
+    """
+    ...
+
+def exit(retval=0, /) -> Any:
+    """
+    Terminate current program with a given exit code. Underlyingly, this
+    function raise as `SystemExit` exception. If an argument is given, its
+    value given as an argument to `SystemExit`.
+    """
+    ...
+
+stderr: Any
+stdout: Any
+stdin: Any
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/utime.pyi` & `micropython_stm32_stubs-1.20.0.post1/utime.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-time related functions. See: https://docs.micropython.org/en/v1.19.1/library/time.html
-
-|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
-
-The ``time`` module provides functions for getting the current time and date,
-measuring time intervals, and for delays.
-
-**Time Epoch**: Unix port uses standard for POSIX systems epoch of
-1970-01-01 00:00:00 UTC. However, embedded ports use epoch of
-2000-01-01 00:00:00 UTC.
-
-**Maintaining actual calendar date/time**: This requires a
-Real Time Clock (RTC). On systems with underlying OS (including some
-RTOS), an RTC may be implicit. Setting and maintaining actual calendar
-time is responsibility of OS/RTOS and is done outside of MicroPython,
-it just uses OS API to query date/time. On baremetal ports however
-system time depends on ``machine.RTC()`` object. The current calendar time
-may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
-by following means:
-
-* By a backup battery (which may be an additional, optional component for
-  a particular board).
-* Using networked time protocol (requires setup by a port/user).
-* Set manually by a user on each power-up (many boards then maintain
-  RTC time across hard resets, though some may require setting it again
-  in such case).
-
-If actual calendar time is not maintained with a system/MicroPython RTC,
-functions below which require reference to current absolute time may
-behave not as expected.
-"""
-from typing import Optional, Tuple, Any
-
-def ticks_diff(ticks1, ticks2) -> int:
-    """
-    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
-    or `ticks_cpu()` functions, as a signed value which may wrap around.
-
-    The argument order is the same as for subtraction
-    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
-    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
-    directly using subtraction on them will produce incorrect result. That is why
-    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
-    arithmetics to produce correct result even for wrap-around values (as long as they not
-    too distant inbetween, see below). The function returns **signed** value in the range
-    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
-    two's-complement signed binary integers). If the result is negative, it means that
-    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
-    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
-    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
-    not hold, incorrect result will be returned. Specifically, if two tick values are
-    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
-    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
-    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
-    to the negative range of possible values.
-
-    Informal rationale of the constraints above: Suppose you are locked in a room with no
-    means to monitor passing of time except a standard 12-notch clock. Then if you look at
-    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
-    long sleep), then once you finally look again, it may seem to you that only 1 hour
-    has passed. To avoid this mistake, just look at the clock regularly. Your application
-    should do the same. "Too long sleep" metaphor also maps directly to application
-    behaviour: don't let your application run any single task for too long. Run tasks
-    in steps, and do time-keeping inbetween.
-
-    `ticks_diff()` is designed to accommodate various usage patterns, among them:
-
-    * Polling with timeout. In this case, the order of events is known, and you will deal
-      only with positive results of `ticks_diff()`::
-
-         # Wait for GPIO pin to be asserted, but at most 500us
-         start = time.ticks_us()
-         while pin.value() == 0:
-             if time.ticks_diff(time.ticks_us(), start) > 500:
-                 raise TimeoutError
-
-    * Scheduling events. In this case, `ticks_diff()` result may be negative
-      if an event is overdue::
-
-         # This code snippet is not optimized
-         now = time.ticks_ms()
-         scheduled_time = task.scheduled_time()
-         if ticks_diff(scheduled_time, now) > 0:
-             print("Too early, let's nap")
-             sleep_ms(ticks_diff(scheduled_time, now))
-             task.run()
-         elif ticks_diff(scheduled_time, now) == 0:
-             print("Right at time!")
-             task.run()
-         elif ticks_diff(scheduled_time, now) < 0:
-             print("Oops, running late, tell task to run faster!")
-             task.run(run_faster=true)
-
-    Note: Do not pass `time()` values to `ticks_diff()`, you should use
-    normal mathematical operations on them. But note that `time()` may (and will)
-    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
-
-    """
-    ...
-
-def ticks_add(ticks, delta) -> Any:
-    """
-    Offset ticks value by a given number, which can be either positive or negative.
-    Given a *ticks* value, this function allows to calculate ticks value *delta*
-    ticks before or after it, following modular-arithmetic definition of tick values
-    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
-    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
-    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
-    or numeric expression. `ticks_add()` is useful for calculating deadlines for
-    events/tasks. (Note: you must use `ticks_diff()` function to work with
-    deadlines.)
-
-    Examples::
-
-         # Find out what ticks value there was 100ms ago
-         print(ticks_add(time.ticks_ms(), -100))
-
-         # Calculate deadline for operation and test for it
-         deadline = ticks_add(time.ticks_ms(), 200)
-         while ticks_diff(deadline, time.ticks_ms()) > 0:
-             do_a_little_of_something()
-
-         # Find out TICKS_MAX used by this port
-         print(ticks_add(0, -1))
-
-    """
-    ...
-
-def ticks_cpu() -> Any:
-    """
-    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
-    in the system. This is usually CPU clocks, and that's why the function is named that
-    way. But it doesn't have to be a CPU clock, some other timing source available in a
-    system (e.g. high-resolution timer) can be used instead. The exact timing unit
-    (resolution) of this function is not specified on ``time`` module level, but
-    documentation for a specific port may provide more specific information. This
-    function is intended for very fine benchmarking or very tight real-time loops.
-    Avoid using it in portable code.
-
-    Availability: Not every port implements this function.
-
-    """
-    ...
-
-class time:
-    """
-    Returns the number of seconds, as an integer, since the Epoch, assuming that
-    underlying RTC is set and maintained as described above. If an RTC is not set, this
-    function returns number of seconds since a port-specific reference point in time (for
-    embedded boards without a battery-backed RTC, usually since power up or reset). If you
-    want to develop portable MicroPython application, you should not rely on this function
-    to provide higher than second precision.  If you need higher precision, absolute
-    timestamps, use `time_ns()`.  If relative times are acceptable then use the
-    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
-    `localtime()` without an argument is a better choice.
-    """
-
-    def __init__(self) -> None: ...
-
-def ticks_ms() -> int:
-    """
-    Returns an increasing millisecond counter with an arbitrary reference point, that
-    wraps around after some value.
-
-    The wrap-around value is not explicitly exposed, but we will
-    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
-    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
-    two, but otherwise may differ from port to port. The same period value is used
-    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
-    simplicity). Thus, these functions will return a value in range [*0* ..
-    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
-    non-negative values are used. For the most part, you should treat values returned
-    by these functions as opaque. The only operations available for them are
-    `ticks_diff()` and `ticks_add()` functions described below.
-
-    Note: Performing standard mathematical operations (+, -) or relational
-    operators (<, <=, >, >=) directly on these value will lead to invalid
-    result. Performing mathematical operations and then passing their results
-    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
-    invalid results from the latter functions.
-    """
-    ...
-
-def ticks_us() -> Any:
-    """
-    Just like `ticks_ms()` above, but in microseconds.
-    """
-    ...
-
-def time_ns() -> int:
-    """
-    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
-    a big integer, so will allocate on the heap).
-    """
-    ...
-
-def localtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_us(us) -> None:
-    """
-    Delay for given number of microseconds, should be positive or 0.
-
-    This function attempts to provide an accurate delay of at least *us*
-    microseconds, but it may take longer if the system has other higher priority
-    processing to perform.
-    """
-    ...
-
-def gmtime(secs: Optional[Any] = None) -> Tuple:
-    """
-    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
-    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
-    If *secs* is not provided or None, then the current time from the RTC is used.
-
-    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
-    date-time tuple in local time.
-
-    The format of the entries in the 8-tuple are:
-
-    * year includes the century (for example 2014).
-    * month   is 1-12
-    * mday    is 1-31
-    * hour    is 0-23
-    * minute  is 0-59
-    * second  is 0-59
-    * weekday is 0-6 for Mon-Sun
-    * yearday is 1-366
-    """
-    ...
-
-def sleep_ms(ms) -> None:
-    """
-    Delay for given number of milliseconds, should be positive or 0.
-
-    This function will delay for at least the given number of milliseconds, but
-    may take longer than that if other processing must take place, for example
-    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
-    this other processing to occur.  Use `sleep_us()` for more precise delays.
-    """
-    ...
-
-def mktime() -> int:
-    """
-    This is inverse function of localtime. It's argument is a full 8-tuple
-    which expresses a time as per localtime. It returns an integer which is
-    the number of seconds since Jan 1, 2000.
-    """
-    ...
-
-def sleep(seconds) -> Any:
-    """
-    Sleep for the given number of seconds. Some boards may accept *seconds* as a
-    floating-point number to sleep for a fractional number of seconds. Note that
-    other boards may not accept a floating-point argument, for compatibility with
-    them use `sleep_ms()` and `sleep_us()` functions.
-    """
-    ...
+"""
+time related functions. See: https://docs.micropython.org/en/v1.20.0/library/time.html
+
+|see_cpython_module| :mod:`python:time` https://docs.python.org/3/library/time.html .
+
+The ``time`` module provides functions for getting the current time and date,
+measuring time intervals, and for delays.
+
+**Time Epoch**: Unix port uses standard for POSIX systems epoch of
+1970-01-01 00:00:00 UTC. However, some embedded ports use epoch of
+2000-01-01 00:00:00 UTC. Epoch year may be determined with ``gmtime(0)[0]``.
+
+**Maintaining actual calendar date/time**: This requires a
+Real Time Clock (RTC). On systems with underlying OS (including some
+RTOS), an RTC may be implicit. Setting and maintaining actual calendar
+time is responsibility of OS/RTOS and is done outside of MicroPython,
+it just uses OS API to query date/time. On baremetal ports however
+system time depends on ``machine.RTC()`` object. The current calendar time
+may be set using ``machine.RTC().datetime(tuple)`` function, and maintained
+by following means:
+
+* By a backup battery (which may be an additional, optional component for
+  a particular board).
+* Using networked time protocol (requires setup by a port/user).
+* Set manually by a user on each power-up (many boards then maintain
+  RTC time across hard resets, though some may require setting it again
+  in such case).
+
+If actual calendar time is not maintained with a system/MicroPython RTC,
+functions below which require reference to current absolute time may
+behave not as expected.
+"""
+from typing import Optional, Tuple, Any
+
+def ticks_diff(ticks1, ticks2) -> int:
+    """
+    Measure ticks difference between values returned from `ticks_ms()`, `ticks_us()`,
+    or `ticks_cpu()` functions, as a signed value which may wrap around.
+
+    The argument order is the same as for subtraction
+    operator, ``ticks_diff(ticks1, ticks2)`` has the same meaning as ``ticks1 - ticks2``.
+    However, values returned by `ticks_ms()`, etc. functions may wrap around, so
+    directly using subtraction on them will produce incorrect result. That is why
+    `ticks_diff()` is needed, it implements modular (or more specifically, ring)
+    arithmetics to produce correct result even for wrap-around values (as long as they not
+    too distant inbetween, see below). The function returns **signed** value in the range
+    [*-TICKS_PERIOD/2* .. *TICKS_PERIOD/2-1*] (that's a typical range definition for
+    two's-complement signed binary integers). If the result is negative, it means that
+    *ticks1* occurred earlier in time than *ticks2*. Otherwise, it means that
+    *ticks1* occurred after *ticks2*. This holds **only** if *ticks1* and *ticks2*
+    are apart from each other for no more than *TICKS_PERIOD/2-1* ticks. If that does
+    not hold, incorrect result will be returned. Specifically, if two tick values are
+    apart for *TICKS_PERIOD/2-1* ticks, that value will be returned by the function.
+    However, if *TICKS_PERIOD/2* of real-time ticks has passed between them, the
+    function will return *-TICKS_PERIOD/2* instead, i.e. result value will wrap around
+    to the negative range of possible values.
+
+    Informal rationale of the constraints above: Suppose you are locked in a room with no
+    means to monitor passing of time except a standard 12-notch clock. Then if you look at
+    dial-plate now, and don't look again for another 13 hours (e.g., if you fall for a
+    long sleep), then once you finally look again, it may seem to you that only 1 hour
+    has passed. To avoid this mistake, just look at the clock regularly. Your application
+    should do the same. "Too long sleep" metaphor also maps directly to application
+    behaviour: don't let your application run any single task for too long. Run tasks
+    in steps, and do time-keeping inbetween.
+
+    `ticks_diff()` is designed to accommodate various usage patterns, among them:
+
+    * Polling with timeout. In this case, the order of events is known, and you will deal
+      only with positive results of `ticks_diff()`::
+
+         # Wait for GPIO pin to be asserted, but at most 500us
+         start = time.ticks_us()
+         while pin.value() == 0:
+             if time.ticks_diff(time.ticks_us(), start) > 500:
+                 raise TimeoutError
+
+    * Scheduling events. In this case, `ticks_diff()` result may be negative
+      if an event is overdue::
+
+         # This code snippet is not optimized
+         now = time.ticks_ms()
+         scheduled_time = task.scheduled_time()
+         if ticks_diff(scheduled_time, now) > 0:
+             print("Too early, let's nap")
+             sleep_ms(ticks_diff(scheduled_time, now))
+             task.run()
+         elif ticks_diff(scheduled_time, now) == 0:
+             print("Right at time!")
+             task.run()
+         elif ticks_diff(scheduled_time, now) < 0:
+             print("Oops, running late, tell task to run faster!")
+             task.run(run_faster=true)
+
+    Note: Do not pass `time()` values to `ticks_diff()`, you should use
+    normal mathematical operations on them. But note that `time()` may (and will)
+    also overflow. This is known as https://en.wikipedia.org/wiki/Year_2038_problem .
+
+    """
+    ...
+
+def ticks_add(ticks, delta) -> Any:
+    """
+    Offset ticks value by a given number, which can be either positive or negative.
+    Given a *ticks* value, this function allows to calculate ticks value *delta*
+    ticks before or after it, following modular-arithmetic definition of tick values
+    (see `ticks_ms()` above). *ticks* parameter must be a direct result of call
+    to `ticks_ms()`, `ticks_us()`, or `ticks_cpu()` functions (or from previous
+    call to `ticks_add()`). However, *delta* can be an arbitrary integer number
+    or numeric expression. `ticks_add()` is useful for calculating deadlines for
+    events/tasks. (Note: you must use `ticks_diff()` function to work with
+    deadlines.)
+
+    Examples::
+
+         # Find out what ticks value there was 100ms ago
+         print(ticks_add(time.ticks_ms(), -100))
+
+         # Calculate deadline for operation and test for it
+         deadline = ticks_add(time.ticks_ms(), 200)
+         while ticks_diff(deadline, time.ticks_ms()) > 0:
+             do_a_little_of_something()
+
+         # Find out TICKS_MAX used by this port
+         print(ticks_add(0, -1))
+
+    """
+    ...
+
+def ticks_cpu() -> Any:
+    """
+    Similar to `ticks_ms()` and `ticks_us()`, but with the highest possible resolution
+    in the system. This is usually CPU clocks, and that's why the function is named that
+    way. But it doesn't have to be a CPU clock, some other timing source available in a
+    system (e.g. high-resolution timer) can be used instead. The exact timing unit
+    (resolution) of this function is not specified on ``time`` module level, but
+    documentation for a specific port may provide more specific information. This
+    function is intended for very fine benchmarking or very tight real-time loops.
+    Avoid using it in portable code.
+
+    Availability: Not every port implements this function.
+
+    """
+    ...
+
+class time:
+    """
+    Returns the number of seconds, as an integer, since the Epoch, assuming that
+    underlying RTC is set and maintained as described above. If an RTC is not set, this
+    function returns number of seconds since a port-specific reference point in time (for
+    embedded boards without a battery-backed RTC, usually since power up or reset). If you
+    want to develop portable MicroPython application, you should not rely on this function
+    to provide higher than second precision.  If you need higher precision, absolute
+    timestamps, use `time_ns()`.  If relative times are acceptable then use the
+    `ticks_ms()` and `ticks_us()` functions.  If you need calendar time, `gmtime()` or
+    `localtime()` without an argument is a better choice.
+    """
+
+    def __init__(self) -> None: ...
+
+def ticks_ms() -> int:
+    """
+    Returns an increasing millisecond counter with an arbitrary reference point, that
+    wraps around after some value.
+
+    The wrap-around value is not explicitly exposed, but we will
+    refer to it as *TICKS_MAX* to simplify discussion. Period of the values is
+    *TICKS_PERIOD = TICKS_MAX + 1*. *TICKS_PERIOD* is guaranteed to be a power of
+    two, but otherwise may differ from port to port. The same period value is used
+    for all of `ticks_ms()`, `ticks_us()`, `ticks_cpu()` functions (for
+    simplicity). Thus, these functions will return a value in range [*0* ..
+    *TICKS_MAX*], inclusive, total *TICKS_PERIOD* values. Note that only
+    non-negative values are used. For the most part, you should treat values returned
+    by these functions as opaque. The only operations available for them are
+    `ticks_diff()` and `ticks_add()` functions described below.
+
+    Note: Performing standard mathematical operations (+, -) or relational
+    operators (<, <=, >, >=) directly on these value will lead to invalid
+    result. Performing mathematical operations and then passing their results
+    as arguments to `ticks_diff()` or `ticks_add()` will also lead to
+    invalid results from the latter functions.
+    """
+    ...
+
+def ticks_us() -> Any:
+    """
+    Just like `ticks_ms()` above, but in microseconds.
+    """
+    ...
+
+def time_ns() -> int:
+    """
+    Similar to `time()` but returns nanoseconds since the Epoch, as an integer (usually
+    a big integer, so will allocate on the heap).
+    """
+    ...
+
+def localtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_us(us) -> None:
+    """
+    Delay for given number of microseconds, should be positive or 0.
+
+    This function attempts to provide an accurate delay of at least *us*
+    microseconds, but it may take longer if the system has other higher priority
+    processing to perform.
+    """
+    ...
+
+def gmtime(secs: Optional[Any] = None) -> Tuple:
+    """
+    Convert the time *secs* expressed in seconds since the Epoch (see above) into an
+    8-tuple which contains: ``(year, month, mday, hour, minute, second, weekday, yearday)``
+    If *secs* is not provided or None, then the current time from the RTC is used.
+
+    The `gmtime()` function returns a date-time tuple in UTC, and `localtime()` returns a
+    date-time tuple in local time.
+
+    The format of the entries in the 8-tuple are:
+
+    * year includes the century (for example 2014).
+    * month   is 1-12
+    * mday    is 1-31
+    * hour    is 0-23
+    * minute  is 0-59
+    * second  is 0-59
+    * weekday is 0-6 for Mon-Sun
+    * yearday is 1-366
+    """
+    ...
+
+def sleep_ms(ms) -> None:
+    """
+    Delay for given number of milliseconds, should be positive or 0.
+
+    This function will delay for at least the given number of milliseconds, but
+    may take longer than that if other processing must take place, for example
+    interrupt handlers or other threads.  Passing in 0 for *ms* will still allow
+    this other processing to occur.  Use `sleep_us()` for more precise delays.
+    """
+    ...
+
+def mktime() -> int:
+    """
+    This is inverse function of localtime. It's argument is a full 8-tuple
+    which expresses a time as per localtime. It returns an integer which is
+    the number of seconds since Jan 1, 2000.
+    """
+    ...
+
+def sleep(seconds) -> Any:
+    """
+    Sleep for the given number of seconds. Some boards may accept *seconds* as a
+    floating-point number to sleep for a fractional number of seconds. Note that
+    other boards may not accept a floating-point argument, for compatibility with
+    them use `sleep_ms()` and `sleep_us()` functions.
+    """
+    ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/uzlib.pyi` & `micropython_stm32_stubs-1.20.0.post1/uzlib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-zlib decompression. See: https://docs.micropython.org/en/v1.19.1/library/zlib.html
-
-|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
-
-This module allows to decompress binary data compressed with
-`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
-(commonly used in zlib library and gzip archiver). Compression
-is not yet implemented.
-"""
-from typing import IO, Any
-
-def decompress(data, wbits=0, bufsize=0, /) -> bytes:
-    """
-    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
-    size used during compression (8-15, the dictionary size is power of 2 of
-    that value). Additionally, if value is positive, *data* is assumed to be
-    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
-    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
-    CPython and is ignored.
-    """
-    ...
-
-class DecompIO:
-    """
-    Create a `stream` wrapper which allows transparent decompression of
-    compressed data in another *stream*. This allows to process compressed
-    streams with data larger than available heap size. In addition to
-    values described in :func:`decompress`, *wbits* may take values
-    24..31 (16 + 8..15), meaning that input stream has gzip header.
-    """
-
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def readline(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, stream, wbits=0, /) -> None: ...
+"""
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
+
+|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
+
+This module allows to decompress binary data compressed with
+`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
+(commonly used in zlib library and gzip archiver). Compression
+is not yet implemented.
+"""
+from typing import Any
+
+def decompress(data, wbits=0, bufsize=0, /) -> bytes:
+    """
+    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
+    size used during compression (8-15, the dictionary size is power of 2 of
+    that value). Additionally, if value is positive, *data* is assumed to be
+    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
+    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
+    CPython and is ignored.
+    """
+    ...
+
+class DecompIO:
+    """
+    Create a `stream` wrapper which allows transparent decompression of
+    compressed data in another *stream*. This allows to process compressed
+    streams with data larger than available heap size. In addition to
+    values described in :func:`decompress`, *wbits* may take values
+    24..31 (16 + 8..15), meaning that input stream has gzip header.
+    """
+
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def readline(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, stream, wbits=0, /) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/zlib.pyi` & `micropython_stm32_stubs-1.20.0.post1/zlib.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-zlib decompression. See: https://docs.micropython.org/en/v1.19.1/library/zlib.html
-
-|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
-
-This module allows to decompress binary data compressed with
-`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
-(commonly used in zlib library and gzip archiver). Compression
-is not yet implemented.
-"""
-from typing import IO, Any
-
-def decompress(data, wbits=0, bufsize=0, /) -> bytes:
-    """
-    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
-    size used during compression (8-15, the dictionary size is power of 2 of
-    that value). Additionally, if value is positive, *data* is assumed to be
-    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
-    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
-    CPython and is ignored.
-    """
-    ...
-
-class DecompIO:
-    """
-    Create a `stream` wrapper which allows transparent decompression of
-    compressed data in another *stream*. This allows to process compressed
-    streams with data larger than available heap size. In addition to
-    values described in :func:`decompress`, *wbits* may take values
-    24..31 (16 + 8..15), meaning that input stream has gzip header.
-    """
-
-    def readinto(self, *args, **kwargs) -> Any: ...
-    def readline(self, *args, **kwargs) -> Any: ...
-    def read(self, *args, **kwargs) -> Any: ...
-    def __init__(self, stream, wbits=0, /) -> None: ...
+"""
+zlib decompression. See: https://docs.micropython.org/en/v1.20.0/library/zlib.html
+
+|see_cpython_module| :mod:`python:zlib` https://docs.python.org/3/library/zlib.html .
+
+This module allows to decompress binary data compressed with
+`DEFLATE algorithm <https://en.wikipedia.org/wiki/DEFLATE>`_
+(commonly used in zlib library and gzip archiver). Compression
+is not yet implemented.
+"""
+from typing import Any
+
+def decompress(data, wbits=0, bufsize=0, /) -> bytes:
+    """
+    Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
+    size used during compression (8-15, the dictionary size is power of 2 of
+    that value). Additionally, if value is positive, *data* is assumed to be
+    zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
+    to be raw DEFLATE stream. *bufsize* parameter is for compatibility with
+    CPython and is ignored.
+    """
+    ...
+
+class DecompIO:
+    """
+    Create a `stream` wrapper which allows transparent decompression of
+    compressed data in another *stream*. This allows to process compressed
+    streams with data larger than available heap size. In addition to
+    values described in :func:`decompress`, *wbits* may take values
+    24..31 (16 + 8..15), meaning that input stream has gzip header.
+    """
+
+    def readinto(self, *args, **kwargs) -> Any: ...
+    def readline(self, *args, **kwargs) -> Any: ...
+    def read(self, *args, **kwargs) -> Any: ...
+    def __init__(self, stream, wbits=0, /) -> None: ...
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/setup.py` & `micropython_stm32_stubs-1.20.0.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['_onewire',
+ '_thread',
  '_uasyncio',
  'array',
  'binascii',
  'cmath',
+ 'collections',
  'dht',
  'errno',
  'framebuf',
  'gc',
  'hashlib',
  'heapq',
+ 'io',
  'json',
  'lcd160cr',
- 'lcd160cr_test',
  'machine',
  'math',
  'micropython',
  'network',
  'onewire',
  'os',
  'platform',
@@ -61,17 +63,17 @@
  'uzlib',
  'zlib']
 install_requires = \
 ['micropython-stdlib-stubs>=0.9.0']
 
 setup_kwargs = {
     'name': 'micropython-stm32-stubs',
-    'version': '1.19.1.post9',
+    'version': '1.20.0.post1',
     'description': 'MicroPython stubs',
-    'long_description': '# micropython-stm32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* Merged stubs from `stubs/micropython-v1_19_1-stm32-merged`\n* Frozen stubs from `stubs/micropython-v1_19_1-frozen/stm32/GENERIC`\n* Core Stubs from `stubs/cpython_core-pycopy`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nFirmware | micropython | stm32 | PYBv1.1 with STM32F405RG | v1.19.1 \nDocumentation | micropython | - | - | v1.19.1 \nCore | micropython | stm32 | - | v1.19.1 \n',
+    'long_description': '# micropython-stm32-stubs\n\n\nThis is a stub-only package for MicroPython.\nIt is intended to be installed in a projects virtual environment to allow static type checkers and intellisense features to be used while writing Micropython code.\n\nThe version of this package is alligned the the version of the MicroPython firmware.\n - Major, Minor and Patch levels are alligned to the same version as the firmware.  \n - The post release level is used to publish new releases of the stubs.\n\nFor `Micropython 1.17` the stubs are published as `1.17.post1` ... `1.17.post2`  \nfor `Micropython 1.18` the stubs are published as `1.18.post1` ... `1.18.post2`  \n\nTo install the latest stubs:  \n`pip install -I  micropython-<port>-stubs` where port is the port of the MicroPython firmware.\n\nTo install the stubs for an older version, such as MicroPython 1.17:  \n`pip install micropython-stm32-stubs==1.17.*` which will install the last post release of the stubs for MicroPython 1.17.\n\n\nAs the creation of the stubs, and merging of the different types is still going though improvements, the stub packages are marked as Beta.\nTo upgrade stubs to the latest stubs for a specific version use `pip install micropython-stm32-stubs==1.17.* --upgrade`\n\nIf you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)\n\nFor an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ \n * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html\n\nIncluded stubs:\n* StubSource.MERGED from `stubs/micropython-v1_20_0-stm32-merged`\n* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`\n* StubSource.CORE from `stubs/micropython-core`\n\n\norigin | Family | Port | Board | Version\n-------|--------|------|-------|--------\nDocumentation | micropython | - | - | v1.20.0 \nCore | micropython | stm32 | - | v1.20.0 \n',
     'author': 'josverl',
     'author_email': 'josverl@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/josverl/micropython-stubs#micropython-stubs',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `micropython_stm32_stubs-1.19.1.post9/PKG-INFO` & `micropython_stm32_stubs-1.20.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-stm32-stubs
-Version: 1.19.1.post9
+Version: 1.20.0.post1
 Summary: MicroPython stubs
 Home-page: https://github.com/josverl/micropython-stubs#micropython-stubs
 License: MIT
 Author: josverl
 Author-email: josverl@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -52,18 +52,17 @@
 
 If you have suggestions or find any issues with the stubs, please report them in the [MicroPython-stubs Discussions](https://github.com/Josverl/micropython-stubs/discussions)
 
 For an overview of  Micropython Stubs please see: https://micropython-stubs.readthedocs.io/en/main/ 
  * List of all stubs : https://micropython-stubs.readthedocs.io/en/main/firmware_grp.html
 
 Included stubs:
-* Merged stubs from `stubs/micropython-v1_19_1-stm32-merged`
-* Frozen stubs from `stubs/micropython-v1_19_1-frozen/stm32/GENERIC`
-* Core Stubs from `stubs/cpython_core-pycopy`
+* StubSource.MERGED from `stubs/micropython-v1_20_0-stm32-merged`
+* StubSource.FROZEN from `stubs/micropython-v1_20_0-frozen/stm32/GENERIC`
+* StubSource.CORE from `stubs/micropython-core`
 
 
 origin | Family | Port | Board | Version
 -------|--------|------|-------|--------
-Firmware | micropython | stm32 | PYBv1.1 with STM32F405RG | v1.19.1 
-Documentation | micropython | - | - | v1.19.1 
-Core | micropython | stm32 | - | v1.19.1 
+Documentation | micropython | - | - | v1.20.0 
+Core | micropython | stm32 | - | v1.20.0
```

