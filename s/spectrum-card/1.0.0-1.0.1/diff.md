# Comparing `tmp/spectrum_card-1.0.0.tar.gz` & `tmp/spectrum_card-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_card-1.0.0.tar", max compression
+gzip compressed data, was "spectrum_card-1.0.1.tar", max compression
```

## Comparing `spectrum_card-1.0.0.tar` & `spectrum_card-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1537 2023-04-06 02:01:50.678562 spectrum_card-1.0.0/LICENSE
--rw-r--r--   0        0        0      389 2023-04-18 03:18:51.141492 spectrum_card-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-06 02:01:50.678562 spectrum_card-1.0.0/README.md
--rw-r--r--   0        0        0   155889 2023-04-14 05:22:15.115304 spectrum_card-1.0.0/spectrum_card/__init__.py
--rw-r--r--   0        0        0    83349 2022-11-08 15:04:34.000000 spectrum_card-1.0.0/spectrum_card/spectrum_header/py_header/regs.py
--rw-r--r--   0        0        0     2124 2022-11-08 15:04:34.000000 spectrum_card-1.0.0/spectrum_card/spectrum_header/py_header/spcerr.py
--rw-r--r--   0        0        0     7999 2023-04-14 06:30:18.580788 spectrum_card-1.0.0/spectrum_card/spectrum_header/pyspcm.py
--rw-r--r--   0        0        0     2025 2023-04-06 01:54:09.473754 spectrum_card-1.0.0/spectrum_card/spectrum_header/spcm_tools.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 spectrum_card-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1537 2023-04-06 02:01:50.678562 spectrum_card-1.0.1/LICENSE
+-rw-r--r--   0        0        0      389 2023-05-12 07:08:28.077948 spectrum_card-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-04-06 02:01:50.678562 spectrum_card-1.0.1/README.md
+-rw-r--r--   0        0        0   155889 2023-05-12 07:08:54.332975 spectrum_card-1.0.1/spectrum_card/__init__.py
+-rw-r--r--   0        0        0    83349 2022-11-08 15:04:34.000000 spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/regs.py
+-rw-r--r--   0        0        0     2124 2022-11-08 15:04:34.000000 spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/spcerr.py
+-rw-r--r--   0        0        0     8681 2023-05-12 07:04:19.611035 spectrum_card-1.0.1/spectrum_card/spectrum_header/pyspcm.py
+-rw-r--r--   0        0        0     2025 2023-04-06 01:54:09.473754 spectrum_card-1.0.1/spectrum_card/spectrum_header/spcm_tools.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 spectrum_card-1.0.1/PKG-INFO
```

### Comparing `spectrum_card-1.0.0/LICENSE` & `spectrum_card-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.0/spectrum_card/__init__.py` & `spectrum_card-1.0.1/spectrum_card/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
   ----------
   device_address : :obj:`str`
     Directory to the card.
   """
   def __init__(self, device_address = b"/dev/spcm0"):
     self.is_alive = False
     self.card_handle = spcm.spcm_hOpen(spcm.create_string_buffer(device_address))
-    if self.card_handle == None:
+    if self.card_handle is None:
       raise Exception("No card found...")
     self.is_alive = True
     
   def close(self):
     """
     Closes the connection to the card.
     """
```

### Comparing `spectrum_card-1.0.0/spectrum_card/spectrum_header/py_header/regs.py` & `spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/regs.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.0/spectrum_card/spectrum_header/py_header/spcerr.py` & `spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/spcerr.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.0/spectrum_card/spectrum_header/pyspcm.py` & `spectrum_card-1.0.1/spectrum_card/spectrum_header/pyspcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,192 +41,194 @@
 uint64 = c_uint64
 
 uptr8  = POINTER (uint8)
 uptr16 = POINTER (uint16)
 uptr32 = POINTER (uint32)
 uptr64 = POINTER (uint64)
 
+try:
+    # Windows
+    if os.name == 'nt':
+        # sys.stdout.write("Python Version: {0} on Windows\n\n".format (platform.python_version()))
+
+        # define card handle type
+        if (bIs64Bit):
+            # for unknown reasons c_void_p gets messed up on Win7/64bit, but this works:
+            drv_handle = POINTER(c_uint64)
+        else:
+            drv_handle = c_void_p
+
+        # Load DLL into memory.
+        # use windll because all driver access functions use _stdcall calling convention under windows
+        if (bIs64Bit == 1):
+            spcmDll = windll.LoadLibrary ("c:\\windows\\system32\\spcm_win64.dll")
+        else:
+            spcmDll = windll.LoadLibrary ("c:\\windows\\system32\\spcm_win32.dll")
+
+        # load spcm_hOpen
+        if (bIs64Bit):
+            spcm_hOpen = getattr (spcmDll, "spcm_hOpen")
+        else:
+            spcm_hOpen = getattr (spcmDll, "_spcm_hOpen@4")
+        spcm_hOpen.argtype = [c_char_p]
+        spcm_hOpen.restype = drv_handle 
+
+        # load spcm_vClose
+        if (bIs64Bit):
+            spcm_vClose = getattr (spcmDll, "spcm_vClose")
+        else:
+            spcm_vClose = getattr (spcmDll, "_spcm_vClose@4")
+        spcm_vClose.argtype = [drv_handle]
+        spcm_vClose.restype = None
+
+        # load spcm_dwGetErrorInfo
+        if (bIs64Bit):
+            spcm_dwGetErrorInfo_i32 = getattr (spcmDll, "spcm_dwGetErrorInfo_i32")
+        else:
+            spcm_dwGetErrorInfo_i32 = getattr (spcmDll, "_spcm_dwGetErrorInfo_i32@16")
+        spcm_dwGetErrorInfo_i32.argtype = [drv_handle, uptr32, ptr32, c_char_p]
+        spcm_dwGetErrorInfo_i32.restype = uint32
+
+        # load spcm_dwGetParam_i32
+        if (bIs64Bit):
+            spcm_dwGetParam_i32 = getattr (spcmDll, "spcm_dwGetParam_i32")
+        else:
+            spcm_dwGetParam_i32 = getattr (spcmDll, "_spcm_dwGetParam_i32@12")
+        spcm_dwGetParam_i32.argtype = [drv_handle, int32, ptr32]
+        spcm_dwGetParam_i32.restype = uint32
+
+        # load spcm_dwGetParam_i64
+        if (bIs64Bit):
+            spcm_dwGetParam_i64 = getattr (spcmDll, "spcm_dwGetParam_i64")
+        else:
+            spcm_dwGetParam_i64 = getattr (spcmDll, "_spcm_dwGetParam_i64@12")
+        spcm_dwGetParam_i64.argtype = [drv_handle, int32, ptr64]
+        spcm_dwGetParam_i64.restype = uint32
+
+        # load spcm_dwSetParam_i32
+        if (bIs64Bit):
+            spcm_dwSetParam_i32 = getattr (spcmDll, "spcm_dwSetParam_i32")
+        else:
+            spcm_dwSetParam_i32 = getattr (spcmDll, "_spcm_dwSetParam_i32@12")
+        spcm_dwSetParam_i32.argtype = [drv_handle, int32, int32]
+        spcm_dwSetParam_i32.restype = uint32
+
+        # load spcm_dwSetParam_i64
+        if (bIs64Bit):
+            spcm_dwSetParam_i64_ = getattr (spcmDll, "spcm_dwSetParam_i64")
+        else:
+            spcm_dwSetParam_i64_ = getattr (spcmDll, "_spcm_dwSetParam_i64@16")
+        spcm_dwSetParam_i64_.argtype = [drv_handle, int32, int64]
+        spcm_dwSetParam_i64_.restype = uint32
+        
+        def spcm_dwSetParam_i64 (hDrv, lReg, Val):
+            try:
+                llVal = int64(Val.value)
+            except AttributeError:
+                llVal = int64(Val)	
+            return spcm_dwSetParam_i64_ (hDrv, lReg, llVal)
+        
+        # load spcm_dwSetParam_i64m
+        if (bIs64Bit):
+            spcm_dwSetParam_i64m = getattr (spcmDll, "spcm_dwSetParam_i64m")
+        else:
+            spcm_dwSetParam_i64m = getattr (spcmDll, "_spcm_dwSetParam_i64m@16")
+        spcm_dwSetParam_i64m.argtype = [drv_handle, int32, int32, int32]
+        spcm_dwSetParam_i64m.restype = uint32
+
+        # load spcm_dwDefTransfer_i64
+        if (bIs64Bit):
+            spcm_dwDefTransfer_i64 = getattr (spcmDll, "spcm_dwDefTransfer_i64")
+        else:
+            spcm_dwDefTransfer_i64 = getattr (spcmDll, "_spcm_dwDefTransfer_i64@36")
+        spcm_dwDefTransfer_i64.argtype = [drv_handle, uint32, uint32, uint32, c_void_p, uint64, uint64]
+        spcm_dwDefTransfer_i64.restype = uint32
+
+        # load spcm_dwInvalidateBuf
+        if (bIs64Bit):
+            spcm_dwInvalidateBuf = getattr (spcmDll, "spcm_dwInvalidateBuf")
+        else:
+            spcm_dwInvalidateBuf = getattr (spcmDll, "_spcm_dwInvalidateBuf@8")
+        spcm_dwInvalidateBuf.argtype = [drv_handle, uint32]
+        spcm_dwInvalidateBuf.restype = uint32
+
+        # load spcm_dwGetContBuf_i64
+        if (bIs64Bit):
+            spcm_dwGetContBuf_i64 = getattr (spcmDll, "spcm_dwGetContBuf_i64")
+        else:
+            spcm_dwGetContBuf_i64 = getattr (spcmDll, "_spcm_dwGetContBuf_i64@16")
+        spcm_dwGetContBuf_i64.argtype = [drv_handle, uint32, POINTER(c_void_p), uptr64]
+        spcm_dwGetContBuf_i64.restype = uint32
+
+
+    elif os.name == 'posix':
+        # sys.stdout.write("Python Version: {0} on Linux\n\n".format (platform.python_version()))
+
+        # define card handle type
+        if (bIs64Bit):
+            drv_handle = POINTER(c_uint64)
+        else:
+            drv_handle = c_void_p
+
+        # Load DLL into memory.
+        # use cdll because all driver access functions use cdecl calling convention under linux 
+        spcmDll = cdll.LoadLibrary ("libspcm_linux.so")
 
-# Windows
-if os.name == 'nt':
-    # sys.stdout.write("Python Version: {0} on Windows\n\n".format (platform.python_version()))
-
-    # define card handle type
-    if (bIs64Bit):
-        # for unknown reasons c_void_p gets messed up on Win7/64bit, but this works:
-        drv_handle = POINTER(c_uint64)
-    else:
-        drv_handle = c_void_p
-
-    # Load DLL into memory.
-    # use windll because all driver access functions use _stdcall calling convention under windows
-    if (bIs64Bit == 1):
-        spcmDll = windll.LoadLibrary ("c:\\windows\\system32\\spcm_win64.dll")
-    else:
-        spcmDll = windll.LoadLibrary ("c:\\windows\\system32\\spcm_win32.dll")
-
-    # load spcm_hOpen
-    if (bIs64Bit):
+        # load spcm_hOpen
         spcm_hOpen = getattr (spcmDll, "spcm_hOpen")
-    else:
-        spcm_hOpen = getattr (spcmDll, "_spcm_hOpen@4")
-    spcm_hOpen.argtype = [c_char_p]
-    spcm_hOpen.restype = drv_handle 
+        spcm_hOpen.argtype = [c_char_p]
+        spcm_hOpen.restype = drv_handle 
 
-    # load spcm_vClose
-    if (bIs64Bit):
+        # load spcm_vClose
         spcm_vClose = getattr (spcmDll, "spcm_vClose")
-    else:
-        spcm_vClose = getattr (spcmDll, "_spcm_vClose@4")
-    spcm_vClose.argtype = [drv_handle]
-    spcm_vClose.restype = None
+        spcm_vClose.argtype = [drv_handle]
+        spcm_vClose.restype = None
 
-    # load spcm_dwGetErrorInfo
-    if (bIs64Bit):
+        # load spcm_dwGetErrorInfo
         spcm_dwGetErrorInfo_i32 = getattr (spcmDll, "spcm_dwGetErrorInfo_i32")
-    else:
-        spcm_dwGetErrorInfo_i32 = getattr (spcmDll, "_spcm_dwGetErrorInfo_i32@16")
-    spcm_dwGetErrorInfo_i32.argtype = [drv_handle, uptr32, ptr32, c_char_p]
-    spcm_dwGetErrorInfo_i32.restype = uint32
+        spcm_dwGetErrorInfo_i32.argtype = [drv_handle, uptr32, ptr32, c_char_p]
+        spcm_dwGetErrorInfo_i32.restype = uint32
 
-    # load spcm_dwGetParam_i32
-    if (bIs64Bit):
+        # load spcm_dwGetParam_i32
         spcm_dwGetParam_i32 = getattr (spcmDll, "spcm_dwGetParam_i32")
-    else:
-        spcm_dwGetParam_i32 = getattr (spcmDll, "_spcm_dwGetParam_i32@12")
-    spcm_dwGetParam_i32.argtype = [drv_handle, int32, ptr32]
-    spcm_dwGetParam_i32.restype = uint32
+        spcm_dwGetParam_i32.argtype = [drv_handle, int32, ptr32]
+        spcm_dwGetParam_i32.restype = uint32
 
-    # load spcm_dwGetParam_i64
-    if (bIs64Bit):
+        # load spcm_dwGetParam_i64
         spcm_dwGetParam_i64 = getattr (spcmDll, "spcm_dwGetParam_i64")
-    else:
-        spcm_dwGetParam_i64 = getattr (spcmDll, "_spcm_dwGetParam_i64@12")
-    spcm_dwGetParam_i64.argtype = [drv_handle, int32, ptr64]
-    spcm_dwGetParam_i64.restype = uint32
+        spcm_dwGetParam_i64.argtype = [drv_handle, int32, ptr64]
+        spcm_dwGetParam_i64.restype = uint32
 
-    # load spcm_dwSetParam_i32
-    if (bIs64Bit):
+        # load spcm_dwSetParam_i32
         spcm_dwSetParam_i32 = getattr (spcmDll, "spcm_dwSetParam_i32")
-    else:
-        spcm_dwSetParam_i32 = getattr (spcmDll, "_spcm_dwSetParam_i32@12")
-    spcm_dwSetParam_i32.argtype = [drv_handle, int32, int32]
-    spcm_dwSetParam_i32.restype = uint32
-
-    # load spcm_dwSetParam_i64
-    if (bIs64Bit):
-        spcm_dwSetParam_i64_ = getattr (spcmDll, "spcm_dwSetParam_i64")
-    else:
-        spcm_dwSetParam_i64_ = getattr (spcmDll, "_spcm_dwSetParam_i64@16")
-    spcm_dwSetParam_i64_.argtype = [drv_handle, int32, int64]
-    spcm_dwSetParam_i64_.restype = uint32
-    
-    def spcm_dwSetParam_i64 (hDrv, lReg, Val):
-        try:
-            llVal = int64(Val.value)
-        except AttributeError:
-            llVal = int64(Val)	
-        return spcm_dwSetParam_i64_ (hDrv, lReg, llVal)
-	
-    # load spcm_dwSetParam_i64m
-    if (bIs64Bit):
+        spcm_dwSetParam_i32.argtype = [drv_handle, int32, int32]
+        spcm_dwSetParam_i32.restype = uint32
+
+        # load spcm_dwSetParam_i64
+        spcm_dwSetParam_i64 = getattr (spcmDll, "spcm_dwSetParam_i64")
+        spcm_dwSetParam_i64.argtype = [drv_handle, int32, int64]
+        spcm_dwSetParam_i64.restype = uint32
+
+        # load spcm_dwSetParam_i64m
         spcm_dwSetParam_i64m = getattr (spcmDll, "spcm_dwSetParam_i64m")
-    else:
-        spcm_dwSetParam_i64m = getattr (spcmDll, "_spcm_dwSetParam_i64m@16")
-    spcm_dwSetParam_i64m.argtype = [drv_handle, int32, int32, int32]
-    spcm_dwSetParam_i64m.restype = uint32
+        spcm_dwSetParam_i64m.argtype = [drv_handle, int32, int32, int32]
+        spcm_dwSetParam_i64m.restype = uint32
 
-    # load spcm_dwDefTransfer_i64
-    if (bIs64Bit):
+        # load spcm_dwDefTransfer_i64
         spcm_dwDefTransfer_i64 = getattr (spcmDll, "spcm_dwDefTransfer_i64")
-    else:
-        spcm_dwDefTransfer_i64 = getattr (spcmDll, "_spcm_dwDefTransfer_i64@36")
-    spcm_dwDefTransfer_i64.argtype = [drv_handle, uint32, uint32, uint32, c_void_p, uint64, uint64]
-    spcm_dwDefTransfer_i64.restype = uint32
+        spcm_dwDefTransfer_i64.argtype = [drv_handle, uint32, uint32, uint32, c_void_p, uint64, uint64]
+        spcm_dwDefTransfer_i64.restype = uint32
 
-    # load spcm_dwInvalidateBuf
-    if (bIs64Bit):
+        # load spcm_dwInvalidateBuf
         spcm_dwInvalidateBuf = getattr (spcmDll, "spcm_dwInvalidateBuf")
-    else:
-        spcm_dwInvalidateBuf = getattr (spcmDll, "_spcm_dwInvalidateBuf@8")
-    spcm_dwInvalidateBuf.argtype = [drv_handle, uint32]
-    spcm_dwInvalidateBuf.restype = uint32
+        spcm_dwInvalidateBuf.argtype = [drv_handle, uint32]
+        spcm_dwInvalidateBuf.restype = uint32
 
-    # load spcm_dwGetContBuf_i64
-    if (bIs64Bit):
+        # load spcm_dwGetContBuf_i64
         spcm_dwGetContBuf_i64 = getattr (spcmDll, "spcm_dwGetContBuf_i64")
-    else:
-        spcm_dwGetContBuf_i64 = getattr (spcmDll, "_spcm_dwGetContBuf_i64@16")
-    spcm_dwGetContBuf_i64.argtype = [drv_handle, uint32, POINTER(c_void_p), uptr64]
-    spcm_dwGetContBuf_i64.restype = uint32
-
-
-elif os.name == 'posix':
-    # sys.stdout.write("Python Version: {0} on Linux\n\n".format (platform.python_version()))
+        spcm_dwGetContBuf_i64.argtype = [drv_handle, uint32, POINTER(c_void_p), uptr64]
+        spcm_dwGetContBuf_i64.restype = uint32
 
-    # define card handle type
-    if (bIs64Bit):
-        drv_handle = POINTER(c_uint64)
     else:
-        drv_handle = c_void_p
-
-    # Load DLL into memory.
-    # use cdll because all driver access functions use cdecl calling convention under linux 
-    spcmDll = cdll.LoadLibrary ("libspcm_linux.so")
-
-    # load spcm_hOpen
-    spcm_hOpen = getattr (spcmDll, "spcm_hOpen")
-    spcm_hOpen.argtype = [c_char_p]
-    spcm_hOpen.restype = drv_handle 
-
-    # load spcm_vClose
-    spcm_vClose = getattr (spcmDll, "spcm_vClose")
-    spcm_vClose.argtype = [drv_handle]
-    spcm_vClose.restype = None
-
-    # load spcm_dwGetErrorInfo
-    spcm_dwGetErrorInfo_i32 = getattr (spcmDll, "spcm_dwGetErrorInfo_i32")
-    spcm_dwGetErrorInfo_i32.argtype = [drv_handle, uptr32, ptr32, c_char_p]
-    spcm_dwGetErrorInfo_i32.restype = uint32
-
-    # load spcm_dwGetParam_i32
-    spcm_dwGetParam_i32 = getattr (spcmDll, "spcm_dwGetParam_i32")
-    spcm_dwGetParam_i32.argtype = [drv_handle, int32, ptr32]
-    spcm_dwGetParam_i32.restype = uint32
-
-    # load spcm_dwGetParam_i64
-    spcm_dwGetParam_i64 = getattr (spcmDll, "spcm_dwGetParam_i64")
-    spcm_dwGetParam_i64.argtype = [drv_handle, int32, ptr64]
-    spcm_dwGetParam_i64.restype = uint32
-
-    # load spcm_dwSetParam_i32
-    spcm_dwSetParam_i32 = getattr (spcmDll, "spcm_dwSetParam_i32")
-    spcm_dwSetParam_i32.argtype = [drv_handle, int32, int32]
-    spcm_dwSetParam_i32.restype = uint32
-
-    # load spcm_dwSetParam_i64
-    spcm_dwSetParam_i64 = getattr (spcmDll, "spcm_dwSetParam_i64")
-    spcm_dwSetParam_i64.argtype = [drv_handle, int32, int64]
-    spcm_dwSetParam_i64.restype = uint32
-
-    # load spcm_dwSetParam_i64m
-    spcm_dwSetParam_i64m = getattr (spcmDll, "spcm_dwSetParam_i64m")
-    spcm_dwSetParam_i64m.argtype = [drv_handle, int32, int32, int32]
-    spcm_dwSetParam_i64m.restype = uint32
-
-    # load spcm_dwDefTransfer_i64
-    spcm_dwDefTransfer_i64 = getattr (spcmDll, "spcm_dwDefTransfer_i64")
-    spcm_dwDefTransfer_i64.argtype = [drv_handle, uint32, uint32, uint32, c_void_p, uint64, uint64]
-    spcm_dwDefTransfer_i64.restype = uint32
-
-    # load spcm_dwInvalidateBuf
-    spcm_dwInvalidateBuf = getattr (spcmDll, "spcm_dwInvalidateBuf")
-    spcm_dwInvalidateBuf.argtype = [drv_handle, uint32]
-    spcm_dwInvalidateBuf.restype = uint32
-
-    # load spcm_dwGetContBuf_i64
-    spcm_dwGetContBuf_i64 = getattr (spcmDll, "spcm_dwGetContBuf_i64")
-    spcm_dwGetContBuf_i64.argtype = [drv_handle, uint32, POINTER(c_void_p), uptr64]
-    spcm_dwGetContBuf_i64.restype = uint32
-
-else:
-    raise Exception ('Operating system not supported by pySpcm')
+        raise Exception ('Operating system not supported by pySpcm')
+except Exception as exception:
+    print(exception)
```

### Comparing `spectrum_card-1.0.0/spectrum_card/spectrum_header/spcm_tools.py` & `spectrum_card-1.0.1/spectrum_card/spectrum_header/spcm_tools.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.0/PKG-INFO` & `spectrum_card-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-card
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper to be used with AWG cards from Spectrum Instruments.
 License: BSD 3 Clause
 Author: Alexander Tritt Monash
 Author-email: alexander.tritt@monash.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

