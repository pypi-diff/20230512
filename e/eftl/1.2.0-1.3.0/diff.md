# Comparing `tmp/eftl-1.2.0-py3-none-any.whl.zip` & `tmp/eftl-1.3.0-py3-none-any.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,220 +1,380 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                     22209 (00000000000056C1h)
-  Actual end-cent-dir record offset:         22187 (00000000000056ABh)
-  Expected end-cent-dir record offset:       22187 (00000000000056ABh)
+  Zip archive file size:                     25001 (00000000000061A9h)
+  Actual end-cent-dir record offset:         24979 (0000000000006193h)
+  Expected end-cent-dir record offset:       24979 (0000000000006193h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 7 entries.
-  The central directory is 513 (0000000000000201h) bytes long,
+  central directory contains 10 entries.
+  The central directory is 937 (00000000000003A9h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 21674 (00000000000054AAh).
+  is 24042 (0000000000005DEAh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  messaging/__init__.py
+  eftl-1.3.0.dist-info/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:44:38
+  file last modified on (DOS date/time):          2023 May 11 14:54:02
+  file last modified on (UT extra field modtime): 2023 May 11 21:54:01 local
+  file last modified on (UT extra field modtime): 2023 May 11 21:54:01 UTC
   32-bit CRC value (hex):                         00000000
-  compressed size:                                2 bytes
+  compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             21 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  messaging/eftl/__init__.py
+  eftl-1.3.0.dist-info/WHEEL
 
-  offset of local header from start of archive:   53
-                                                  (0000000000000035h) bytes
+  offset of local header from start of archive:   79
+                                                  (000000000000004Fh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:44:38
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                2 bytes
-  uncompressed size:                              0 bytes
+  file last modified on (DOS date/time):          2023 Apr 13 21:31:06
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:31:06 local
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:31:06 UTC
+  32-bit CRC value (hex):                         801a68e9
+  compressed size:                                92 bytes
+  uncompressed size:                              92 bytes
   length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  messaging/eftl/connection.py
+  eftl-1.3.0.dist-info/top_level.txt
 
-  offset of local header from start of archive:   111
-                                                  (000000000000006Fh) bytes
+  offset of local header from start of archive:   255
+                                                  (00000000000000FFh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:48:38
-  32-bit CRC value (hex):                         05a585fd
-  compressed size:                                16950 bytes
-  uncompressed size:                              94765 bytes
-  length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 Apr 13 21:31:06
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:31:06 local
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:31:06 UTC
+  32-bit CRC value (hex):                         088c42e7
+  compressed size:                                10 bytes
+  uncompressed size:                              10 bytes
+  length of filename:                             34 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  eftl-1.2.0.dist-info/METADATA
+  eftl-1.3.0.dist-info/METADATA
 
-  offset of local header from start of archive:   17119
-                                                  (00000000000042DFh) bytes
+  offset of local header from start of archive:   357
+                                                  (0000000000000165h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:48:38
-  32-bit CRC value (hex):                         a139ffaf
-  compressed size:                                3903 bytes
+  file last modified on (DOS date/time):          2023 May 11 14:53:16
+  file last modified on (UT extra field modtime): 2023 May 11 21:53:15 local
+  file last modified on (UT extra field modtime): 2023 May 11 21:53:15 UTC
+  32-bit CRC value (hex):                         06159f2e
+  compressed size:                                3902 bytes
   uncompressed size:                              21432 bytes
   length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  eftl-1.2.0.dist-info/WHEEL
+  eftl-1.3.0.dist-info/RECORD
 
-  offset of local header from start of archive:   21081
-                                                  (0000000000005259h) bytes
+  offset of local header from start of archive:   4346
+                                                  (00000000000010FAh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:48:38
-  32-bit CRC value (hex):                         801a68e9
-  compressed size:                                92 bytes
-  uncompressed size:                              92 bytes
-  length of filename:                             26 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 11 14:53:42
+  file last modified on (UT extra field modtime): 2023 May 11 21:53:41 local
+  file last modified on (UT extra field modtime): 2023 May 11 21:53:41 UTC
+  32-bit CRC value (hex):                         48e16ba0
+  compressed size:                                314 bytes
+  uncompressed size:                              529 bytes
+  length of filename:                             27 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             text
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  eftl-1.2.0.dist-info/top_level.txt
+  messaging/
 
-  offset of local header from start of archive:   21229
-                                                  (00000000000052EDh) bytes
+  offset of local header from start of archive:   4745
+                                                  (0000000000001289h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 11 14:52:00
+  file last modified on (UT extra field modtime): 2023 May 11 21:51:59 local
+  file last modified on (UT extra field modtime): 2023 May 11 21:51:59 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             10 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
+  There is no file comment.
+
+Central directory entry #7:
+---------------------------
+
+  messaging/eftl/
+
+  offset of local header from start of archive:   4813
+                                                  (00000000000012CDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 11 14:52:00
+  file last modified on (UT extra field modtime): 2023 May 11 21:51:59 local
+  file last modified on (UT extra field modtime): 2023 May 11 21:51:59 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             15 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
+  There is no file comment.
+
+Central directory entry #8:
+---------------------------
+
+  messaging/eftl/connection.py
+
+  offset of local header from start of archive:   4886
+                                                  (0000000000001316h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:48:38
-  32-bit CRC value (hex):                         088c42e7
-  compressed size:                                12 bytes
-  uncompressed size:                              10 bytes
-  length of filename:                             34 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 Apr 13 21:31:06
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:31:06 local
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:31:06 UTC
+  32-bit CRC value (hex):                         5c5ae1ab
+  compressed size:                                18907 bytes
+  uncompressed size:                              108577 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
+  There is no file comment.
+
+Central directory entry #9:
+---------------------------
+
+  messaging/eftl/__init__.py
+
+  offset of local header from start of archive:   23879
+                                                  (0000000000005D47h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 13 21:25:24
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:25:24 local
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:25:24 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             26 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #10:
 ---------------------------
 
-  eftl-1.2.0.dist-info/RECORD
+  messaging/__init__.py
 
-  offset of local header from start of archive:   21305
-                                                  (0000000000005339h) bytes
+  offset of local header from start of archive:   23963
+                                                  (0000000000005D9Bh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 27 14:48:38
-  32-bit CRC value (hex):                         752e34ec
-  compressed size:                                312 bytes
-  uncompressed size:                              528 bytes
-  length of filename:                             27 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 Apr 13 21:25:24
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:25:24 local
+  file last modified on (UT extra field modtime): 2023 Apr 14 04:25:24 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             21 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (000664 octal):            ?rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 ba 34 00 00 04 43 23 00 00.
+
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
-Filename: messaging/__init__.py
+Filename: eftl-1.3.0.dist-info/
 Comment: 
 
-Filename: messaging/eftl/__init__.py
+Filename: eftl-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: messaging/eftl/connection.py
+Filename: eftl-1.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: eftl-1.3.0.dist-info/METADATA
+Comment: 
+
+Filename: eftl-1.3.0.dist-info/RECORD
+Comment: 
+
+Filename: messaging/
 Comment: 
 
-Filename: eftl-1.2.0.dist-info/METADATA
+Filename: messaging/eftl/
 Comment: 
 
-Filename: eftl-1.2.0.dist-info/WHEEL
+Filename: messaging/eftl/connection.py
 Comment: 
 
-Filename: eftl-1.2.0.dist-info/top_level.txt
+Filename: messaging/eftl/__init__.py
 Comment: 
 
-Filename: eftl-1.2.0.dist-info/RECORD
+Filename: messaging/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## messaging/eftl/connection.py

```diff
@@ -1,12 +1,10 @@
 '''
- Copyright 2013-2022 TIBCO Software Inc.
- * All Rights Reserved. Confidential and Proprietary.
- * For more information, please contact:
- * TIBCO Software Inc., Palo Alto, California, USA
+ Copyright (c) 2013-2023 Cloud Software Group, Inc. 
+ * All Rights Reserved.
 '''
 
 
 """Documentation of the TIBCO eFTL™ Python application programming interface."""
 
 import asyncio
 import datetime
@@ -30,15 +28,15 @@
 from abc import ABC, abstractmethod
 from autobahn.asyncio.websocket import WebSocketClientProtocol
 from autobahn.asyncio.websocket import WebSocketClientFactory
 
 
 import jsonpickle
 
-_EFTL_VERSION = "6.8.0 V10"
+_EFTL_VERSION = "6.10.0 V4"
 EFTL_WS_PROTOCOL = "v1.eftl.tibco.com"
 
 OP_HEARTBEAT        = 0
 OP_LOGIN            = 1
 OP_WELCOME          = 2
 OP_SUBSCRIBE        = 3
 OP_SUBSCRIBED       = 4
@@ -54,14 +52,17 @@
 OP_REPLY            = 15
 OP_MAP_CREATE       = 16
 OP_MAP_DESTROY      = 18
 OP_MAP_SET          = 20
 OP_MAP_GET          = 22
 OP_MAP_REMOVE       = 24
 OP_MAP_RESPONSE     = 26
+OP_STOP             = 28
+OP_START            = 30
+OP_STARTED          = 31
 ERR_PUBLISH_FAILED  = 11
 
 WS_NORMAL_CLOSE     = 1000
 WS_ABNORMAL_CLOSE   = 1006
 RESTART             = 1012
 
 # subscription related constants
@@ -70,17 +71,25 @@
 SUBSCRIPTION_INVALID = 22
 
 # request/reply related constants
 REQUEST_FAILED = 41
 REQUEST_DISALLOWED = 40
 REQUEST_TIMEOUT = 99
 
+# stop/start related constants
+STOP_FAILED = 50
+START_FAILED = 51
+
 #PROPERTY_TIMEOUT                    = "timeout"
 #PROPERTY_NOTIFICATION_TOKEN         = "notification_token"
 
+SUB_STOPPED  = 0
+SUB_STARTING = 1
+SUB_STARTED  = 2
+
 ACKNOWLEDGE_MODE_CLIENT             = "client"
 ACKNOWLEDGE_MODE_NONE               = "none"
 ACKNOWLEDGE_MODE_AUTO               = "auto"
 ACKNOWLEDGE_MODE                    = "ack_mode"
 ACK_FIELD                           = "ack"
 
 PROPERTY_USERNAME                   = "username"
@@ -124,14 +133,16 @@
 LOGIN_OPTIONS_FIELD     = "login_options"
 RESUME_FIELD            = "_resume"
 QOS_FIELD               = "_qos"
 REPLY_TO_FIELD          = "reply_to"
 REQ_ID_FIELD            = "req"
 DEL_FIELD               = "del"
 MAX_PENDING_ACKS_FIELD  = "max_pending_acks"
+STOPPED_FIELD           = "stopped"
+STOP_SUPPORTED_FIELD    = "stop_supported"
 
 MAP_FIELD               = "map"
 KEY_FIELD               = "key"
 VALUE_FIELD             = "value"
 DOUBLE_FIELD            = "_d_"
 MILLISECOND_FIELD       = "_m_"
 OPAQUE_FIELD            = "_o_"
@@ -153,14 +164,17 @@
 
 class EftlMessageSizeTooLarge(Exception):
     """Raise when EftlMesssage size is larger than the maximum allowed size."""
 
 class EftlAlreadyConnected(Exception):
     """Raise when connect method is called but connection is already connected."""
 
+class EftlUnsupportedError(Exception):
+    """Raise when unsupported behavior is attempted."""
+
 def _call_dict_function(dic, name, **kwargs):
     """Call dic[name](**kwargs), if it exists."""
     try:
         logger.debug("name %s", name)
         func = dic.get(name)
         if func is None:
             logger.debug("User did not give a callback for this event. kwargs:\n{}".format(kwargs))
@@ -219,64 +233,103 @@
         use to publish and subscribe.
 
         When a pipe-separated list of URLs is specified this call will attempt
         a connection to each in turn, in a random order, until one is connected.
         A program that uses more than one server channel must connect
         separately to each channel.
 
-        :param:
-        url:
+        Parameters
+	----------
+        url : 
+	
             The call connects to the eFTL server at this URL. This can be
             a single URL, or a pipe ('|') separated list of URLs. URLs can
             be in either of these forms
 
                 ws://host:port/channel
                 wss://host:port/channel
 
             Optionally, the URLs can contain the username, password,
             and/or client identifier
 
                 ws://username:password@host:port/channel?clientId=<identifier>
                 wss://username:password@host:port/channel?clientId=<identifier
+        kwargs :
+
+            auto_reconnect_attempts (int): Maximum number of reconnect attempts. The default is 256 attempts
+            auto_reconnect_max_delay (int): Maximum reconnect delay in milliseconds. The default is 30 seconds.
+            max_pending_acks (int): optional
+                              Maximum number of unacknowledged messages allowed for the
+                              client.
+            user : optional
+                        Login credentials to use if not found in the url.
+            password : optional
+                        Login credentials to use if not found in the url.
+            client_id : optional
+                       User-specified client identifier.
+            handshake_timeout : optional
+                         Seconds to wait for websocket handshake to complete.
+            login_timeout : optional
+                         Seconds to halt waiting for a login message reply. If a
+                         reply is not received in time, raise an EftlClientError.
+            polling_interval : optional
+                        Seconds to wait between each message reply check.
+            trust_all : true/false (optional)
+            trust_store :  certificate path (optional)
+            loop : event loop provided by user (optional)
+
+            Callbacks :
+
+               'on_connect(connection):'
+			A new connection to the eFTL server is ready to use.
+
+               Parameters
+	       ----------
+               connection : The connection that is ready to use.
+
+               'on_disconnect(connection, loop, code, reason):' A connection to the eFTL server has closed.
+
+               Parameters
+	       ----------
+               connection : The connection that closed.
+               loop : the event loop used servicing connection events
+               code : A code categorizes the error. Your program can use this value in its response logic.
+               reason : This string provides more detail. Your program can use this value in error reporting and logging.
+
+               'on_reconnect(connection):' A connection to the eFTL server has re-opened and is ready to use.
+                                           The eFTL library invokes this method only after your 
+                                           program calls `messaging.eftl.connection.reconnect` and not `messaging.eftl.connection.connect`.
+
+               Parameters
+	       ----------
+               connection: The connection that reconnected.
+
+               'on_error(connection, code, reason):' An error prevented an operation.
+
+               Parameters
+	       ----------
+               connection : connection object. For publish errors, this argument is the message that was not published. 
+                                               For subscription errors, this argument is an object that represents 
+                                               a subscription identifier.
+               code: A code categorizes the error. Your program can use this value in its response logic.
+               reason: This string provides more detail. Your program can use this value in error reporting and logging.
+
+               'on_state_change(connection, state):' The connection state has changed
+	                                             The eFTL library invokes this method whenever the connection state changes.
+
+                Parameters
+	        ----------
+                connection: The connection whose state has changed.
+	        state: The connection has changed to this state
+
+	Returns
+        ----------
 
-        :param:
-        kwargs
-            auto_reconnect_attempts : int, optional
-                Maximum number of reconnect attempts. The default is 
-                256 attempts.
-           auto_reconnect_max_delay : optional
-                Maximum reconnect delay in milliseconds. The default is
-                30 seconds.
-           max_pending_acks : optional
-                Maximum number of unacknowledged messages allowed for the
-                client.
-           user : optional
-                Login credentials to use if not found in the url.
-           password : optional
-                Login credentials to use if not found in the url.
-           client_id : optional
-                User-specified client identifier.
-           handshake_timeout : optional
-                Seconds to wait for websocket handshake to complete.
-           login_timeout : optional
-                Seconds to halt waiting for a login message reply. If a
-                reply is not received in time, raise an EftlClientError.
-           polling_interval : optional
-                Seconds to wait between each message reply check.
-           trust_all : true/false (optional)
-           trust_store :  certificate path (optional)
-           loop : event loop provided by user (optional)
-           Callbacks :
-                on_connect(connection):
-                on_disconnect(connection, loop, code, reason):
-                on_reconnect(connection):
-                on_error(connection, code, reason):
-                on_state_change(connection, state):
-        :return:
             The EftlConnection object that can used to publish and subscribe
+
         Raises
         ------
         ValueError
             If any provided urls lack a host name or the correct scheme.
         EftlClientError
             If the connection is not established in time.
         """
@@ -427,33 +480,40 @@
         return self.__reply_to_
 
     # public APIs
     def set_string(self, field_name, value):
         """
         Set a string field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name : The call sets this field
+            value : The call sets this value.
+        Return
+        ------
+
         """
         if isinstance(field_name, str):
             if isinstance(value, str):
                 self._set_field(field_name, value)
             else:
                 raise TypeError("Expected to have 'value' of type 'str'")
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_string_array(self, field_name, values):
         """
         Set a string array field in a message.
 
-        :param field_name: The call sets this field
-        :param values: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            values: The call sets this value.
+        Return
+        -------
         """
         if isinstance(field_name, str):
             if isinstance(values, list):
                 if len(values) > 0:
                     for value in values:
                         if not isinstance(value, str):
                             raise TypeError("Expected to have 'list' of elements of type 'str'")
@@ -464,33 +524,39 @@
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
 
     def set_long(self, field_name, value):
         """
         Set a long field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        -------
         """
         if isinstance(field_name, str):
             if isinstance(value, int):
                 self._set_field(field_name, value)
             else:
                 raise TypeError("Expected to have 'value' of type 'int'")
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_long_array(self, field_name, values):
         """
         Set a long array field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        -------
         """
         if isinstance(field_name, str):
             if isinstance(values, list):
                 if len(values) > 0:
                     for value in values:
                         if not isinstance(value, int):
                             raise TypeError("Expected to have 'list' of elements of type 'int'")
@@ -500,17 +566,20 @@
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_double(self, field_name, value):
         """
         Set a double field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if isinstance(value, float):
                 if math.isnan(value):
                     dvalue = "NaN"
                     encoded_value = {DOUBLE_FIELD : dvalue}
                 elif value == float('inf'):
@@ -528,17 +597,20 @@
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_double_array(self, field_name, values):
         """
         Set a double array field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if isinstance(values, list):
                 if len(values) > 0:
                     encode_values_array = []
                     for value in values:
                         if isinstance(value, float):
@@ -553,34 +625,40 @@
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_datetime(self, field_name, value):
         """
         Set a datetime field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if isinstance(value, datetime.datetime):
                 encoded_value = { MILLISECOND_FIELD : int(value.timestamp() * 1000) }
                 self._set_field(field_name, encoded_value)
             else:
                 raise TypeError("Expected to have 'value' of type 'datetime.datetime'")
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_datetime_array(self, field_name, values):
         """
         Set a datetime array field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if isinstance(values, list):
                 if len(values) > 0:
                     encode_values_array = []
                     for value in values:
                         if isinstance(value, datetime.datetime):
@@ -595,33 +673,39 @@
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_message(self, field_name, value):
         """
         Set a message field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if isinstance(value, EftlMessage):
                 self._set_field(field_name, value)
             else:
                 raise TypeError("Expected to have 'value' of type 'EftlMessage'")
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_message_array(self, field_name, values):
         """
         Set a message array field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if isinstance(values, list):
                 if len(values) > 0:
                     for value in values:
                         if not isinstance(value, EftlMessage):
                              raise TypeError("Expected to have 'list' of elements of type 'EftlMessage'")
@@ -631,17 +715,20 @@
         else:
             raise TypeError("Expected to have 'field_name' of type 'str'")
 
     def set_opaque(self, field_name, value):
         """
         Set an opaque field in a message.
 
-        :param field_name: The call sets this field
-        :param value: The call sets this value.
-        :return:
+        Parameters
+        ----------
+            field_name: The call sets this field
+            value: The call sets this value.
+        Return
+        ------
         """
         if isinstance(field_name, str):
             if value is not None:
                 encoded_data = base64.b64encode(value).decode("ascii")
                 encoded_value_str = { OPAQUE_FIELD : encoded_data}
                 self._set_field(field_name, encoded_value_str)
         else:
@@ -830,176 +917,225 @@
 
     # public APIs getters methods for EFTLMessage
 
     def get_store_message_id(self):
         """
         Message's unique store identifier assigned by the persistence service.
 
-        :return:
-              A monotonically increasing long value that represents
-              message's unique store identifier
+        Return
+        ------
+            A monotonically increasing long value that represents
+            message's unique store identifier
         """
         return self.__sid_
 
     def get_delivery_count(self):
         """
         Message's delivery count assigned by the persistence service.
 
-        :return:
+        Return
+        ------
               The message delivery count.
         """
         return self.__cnt_
 
     def get_string(self, field_name):
         """
         Get the value of a string field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type string
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type string
         """
         return self._get_field(field_name, "string_type")
 
     def get_string_array(self, field_name):
         """
         Get the value of a string array field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type string array
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type string array
         """
         return self._get_array(field_name, "string_type")
 
     def get_long(self, field_name):
         """
         Get the value of a long field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type long
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type long
         """
         return self._get_field(field_name, "long_type")
 
     def get_long_array(self, field_name):
         """
         Get the value of a long array field from a message.
         
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type long array
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type long array
         """
         return self._get_array(field_name, "long_type")
 
     def get_double(self, field_name):
         """
         Get the value of a long field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type double
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type double
         """
         return self._get_field(field_name, "double_type")
 
     def get_double_array(self, field_name):
         """
         Get the value of a long field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type double array
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        --------
+            The value of the field if the field is present
+            and has type double array
         """
         return self._get_array(field_name, "double_type")
 
     def get_datetime(self, field_name):
         """
         Get the value of a long field from a message.
-
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type datetime
+ 
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type datetime
         """
         return self._get_field(field_name, "datetime_type")
 
     def get_datetime_array(self, field_name):
         """
         Get the value of a long field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type datetime array
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type datetime array
         """
         return self._get_array(field_name, "datetime_type")
 
     def get_message(self, field_name):
         """
         Get the value of a long field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type message
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type message
         """
         return self._get_field(field_name, "message_type")
 
     def get_message_array(self, field_name):
         """
         Get the value of a message array field from a message.
 
-        :param field_name: The name of the field
-
-        :return: The value of the field if the field is present
-                 and has type message array (list of messages)
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
+            and has type message array (list of messages)
         """
         return self._get_array(field_name, "message_type")
 
     def get_opaque(self, field_name):
         """
         Get the value of opaque field from a message.
         
-        :param field_name: The name of the field
-        :return: The value of the field if the field is present
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            The value of the field if the field is present
         """
         return self._get_field(field_name, "opaque_type")
 
     def get_field_names(self):
         """
         Return the list of field names.
         
-        :return: The field names of this message as a list object.
+        Parameters
+        ----------
+            The field names of this message as a list object.
+        Return
+        ------
+
         """
         return self.__msg_obj.keys()
 
     def is_field_set(self, field_name):
         """
         Return True if the field is set, False otherwise.
 
-        :param field_name: The name of the field
-        :return: True if the field is set, False otherwise
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        ------
+            True if the field is set, False otherwise
 
         """
         field_present = self.__msg_obj.get(field_name)
         if field_present is not None:
             return True
         else:
             return False
 
     def get_field_type(self, field_name):
         """
         Return the type of value of this field.
-        
-        :param field_name: The name of the field
-        :return: type of value of this field.
+
+        Parameters
+        ----------
+            field_name: The name of the field
+        Return
+        -------
+            Type of value of this field.
         
             Possible return values : 
 	            'int' represents Integer
 	            'str' represents String
 	            'float' represents Float
 	            'datetime.datetime' represents datetime.datetime 
 	            'message' represents EftlMessage object type
@@ -1010,45 +1146,80 @@
 
     ########################## Other Public methods for EftlMessage ##############################
 
     def clear_field(self, field_name):
         """
         Remove the given field from this message.
         
-        :param field_name: 
+        Parameters
+        ----------
+            field_name: field_name to clear
         """
         self._remove_field(field_name)
 
     def clear_all_fields(self):
         """Remove all the fields in this message."""
         self.__msg_obj.clear()
 
 class EftlKVMap():
     """
     A key-value map  object represents a program's connection to an FTL map.
 
     Programs use key-value map objects to set, get, and remove key-value
     pairs in an FTL map.
 
+    Callbacks:
+        'on_success(key, message):' A key-value map operation has completed successfully.
+
+        Parameters
+        __________
+            key: The key being operated upon.
+            message: The value of the key.
+
+        'on_error(key, message, code, reason):' An error prevented a key-value map operation.
+
+        Parameters
+        __________
+            key: The key being operated upon.
+            message: The value of the key.
+            code: A code categorizes the error. Your program can use this value in its response logic.
+            reason: This string provides more detail. Your program can use this value in error reporting and logging.
     """
 
     def __init__(self, connection, name):
         self.connection = connection
         self.name = name
 
     async def get(self, key, **kwargs):
         """
         Get the value of a key from the map, or <c>null</c> if the key is not set.
         
-        :param key: Get the value for this key
-        :param kwargs:
-            Callbacks:
-                on_success:
-                on_error:
-        :return: The value as a EftlMessage
+	Parameters
+	__________
+            key: Get the value for this key
+            kwargs:
+                Callbacks:
+
+                'on_success(key, message):' A key-value map operation has completed successfully.
+                Parameters
+                __________
+                key: The key being operated upon.
+                message: The value of the key.
+
+                'on_error(key, message, code, reason):' An error prevented a key-value map operation.
+                Parameters
+                __________
+                key: The key being operated upon.
+                message: The value of the key.
+                code: A code categorizes the error. Your program can use this value in its response logic.
+                reason: This string provides more detail. Your program can use this value in error reporting and logging.
+       Return
+       ------
+           The value as a EftlMessage
+
         """
         if not self.connection._permanently_closed():
             if isinstance(key, str):
                 self._create_kv_request(OP_MAP_GET, key, None, **kwargs)
             else:
                 raise TypeError("key should be of type 'str'")
         else:
@@ -1058,20 +1229,38 @@
         """
         Set a key-value pair in the map, overwriting any existing value.
 
         This call returns immediately; setting continues
         asynchronously.  When the set completes successfully,
         the eFTL library calls your on_success callback.
 
-        :param key: Set the value for this key.
-        :param value: Set this value for the key.
-        :param kwargs:
-              on_success
-              on_error
-        :return:
+        Parameters
+        ----------
+            key: Set the value for this key.
+    	    value: Set this value for the key.
+    	    kwargs:
+                Callbacks:
+
+                'on_success(key, message):' A key-value map operation has completed successfully.
+                Parameters
+                __________
+                key: The key being operated upon.
+                message: The value of the key.
+  
+                'on_error(key, message, code, reason):' An error prevented a key-value map operation.
+                Parameters
+                __________
+                key: The key being operated upon.
+                message: The value of the key.
+                code: A code categorizes the error. Your program can use this value in its response logic.
+                reason: This string provides more detail. Your program can use this value in error reporting and logging.
+  	
+        Return
+        -----
+	
         """
         if not self.connection._permanently_closed():
             if isinstance(key, str):
                 if isinstance(value, EftlMessage):
                     self._create_kv_request(OP_MAP_SET, key, value, **kwargs)
                 else:
                     raise TypeError("Only EftlMessage is allowed as value.")
@@ -1084,19 +1273,35 @@
         """
         Remove a key-value pair from the map.
 
         This call returns immediately; removing continues
         asynchronously.  When the remove completes successfully,
         the eFTL library calls your on_success callback.
 
-        :param key:  Revove the value for this key.
-        :param kwargs:
-               on_success
-               on_error
-        :return:
+        Parameters
+        ----------
+            key: Remove the value for this key
+            kwargs:
+                Callbacks:
+                'on_success(key, message):' A key-value map operation has completed successfully.
+                Parameters
+                __________
+                key: The key being operated upon.
+                message: The value of the key.
+               
+                'on_error(key, message, code, reason):' An error prevented a key-value map operation.
+                Parameters
+                __________
+                key: The key being operated upon.
+                message: The value of the key.
+                code: A code categorizes the error. Your program can use this value in its response logic.
+                reason: This string provides more detail. Your program can use this value in error reporting and logging.
+        Return
+        ------
+
         """
         if not self.connection._permanently_closed():
             if isinstance(key, str):
                 self._create_kv_request(OP_MAP_REMOVE, key, **kwargs)
             else:
                 raise TypeError("key should be of type 'str'")
         else:
@@ -1206,15 +1411,17 @@
                 connection=self, state=self.status
             )
 
     def get_clientId(self):
         """
         Get the client identifier for this connection.
 
-        :return: The client's identifier.
+        Return
+        ------
+            The client's identifier.
 
         """
         return self.client_id
 
     async def _async_connect(self, url, polling_interval):
         if url.scheme == "wss":
             logger.debug("url scheme is wss, creating a secure connection to eFTLserver")
@@ -1302,15 +1509,16 @@
         When the connection is ready to use, the eFTL library calls your
         on_reconnect callback
 
         Reconnecting automatically re-activates all subscriptions
         on the connection. The eFTL library invokes your
         on_subscribe callback for each successful resubscription.
 
-        :return:
+        Return
+        ------
         """
         if not self.is_connected():
             if self.previously_connected:
                 self.attempt_manual_reconnect = True
                 await self._attempt_connection()
                 _call_dict_function(
                 self.connect_options,
@@ -1448,15 +1656,17 @@
 
         raise EftlClientError("Connection failed across all provided urls")
 
     def is_connected(self):
         """
         Determine whether this connection to the eFTL server is open or closed.
 
-        :return: True if this connection is open, False otherwise
+        Return
+        ------
+            True if this connection is open, False otherwise
         """
         return self._ws is not None and self.status == Eftl.CONNECTED
 
     def _permanently_closed(self, error="Attempted op while connection is closed.", warn=True):
         if self.status == Eftl.DISCONNECTED:
             return True
 
@@ -1470,44 +1680,75 @@
 
         This call returns immediately; disconnecting continues
         asynchronously.
 
         When the connection has closed, the eFTL library calls your
         on_disconnect callback.
         
-        :return:
+        Return
+        ------
         """
         if not self._permanently_closed():
             self._ws._disconnect()
         else:
             raise ConnectionError("Connection is closed.")
 
     async def subscribe(self, **kwargs):
         """
-        Send a message to register a matcher-based subscription.
 
+        Subscribe to messages.
+        Register a subscription for one-to-many messages.
+        This call returns immediately; subscribing continues asynchronously. When the subscription is ready to
+        receive messages, the eFTL library calls your on_subscribe callback.
+        
+        A matcher can narrow subscription interest in the inbound message stream.
+        
+        An acknowledgment mode for the subscription can be set to automatically acknowledge consumed
+        messages, require explicit client acknowledgment of the consumed messages, or to disable
+        message acknowledgment altogether. The default is to automatically acknowledge consumed messages.
+
+        When explicit client acknowledgment is specified the eFTL server will stop delivering messages
+        to the client once the server's configured maximum number of unacknowledged messages is reached.
+        
+        When communicating with EMS, to subscribe to messages published on a specific EMS
+        destination use a subscription matcher that includes the message field name <code>_dest</code>.
+        To distinguish between topics and queues the destination name can be prefixed with
+        either "TOPIC:" or "QUEUE:", for example "TOPIC:MyDest" or "QUEUE:MyDest". A destination name
+        with no prefix is a topic.
+
+        example
+        To subscribe to messages published on a specific EMS destination,
+        create a subscription matcher for that destination;
+        for example:
+        var matcher = '{"_dest":"MyDest"}';
+       
         Parameters
         ----------
-        timeout : optional
-            Number of seconds to halt waiting on acknowledgement from
-            the server (default set in EftlConnection.connect()).
-        matcher : str, optional
-            JSON content matcher to subscribe to.
-        type : {"standard", "shared", "last-value"}, optional
-            Durable type.
-        key : optional
-            The last-value index key, if `type` is "last-value".
-        durable : str, optional
-            Name to give the durable.
-        ack_mode: client, None. Default is auto
+	kwargs:
+
+            timeout : optional
+                Number of seconds to halt waiting on acknowledgement from
+                the server messaging.eftl.connect().
+
+            matcher : str, optional
+                JSON content matcher to subscribe to.
+
+            type : {"standard", "shared", "last-value"}, optional
+                Durable type.
+
+            key : optional
+                The last-value index key, if `type` is "last-value".
 
+            durable : str, optional
+                Name to give the durable.
+
+            ack_mode: client, None. Default is auto
         Returns
         -------
-        sub_id
-            The subcription identifier of the new subscription.
+            sub_id: The subcription identifier of the new subscription.
         """
         if not self._permanently_closed():
             #check if matcher is valid JSON string
             try:
                 sub_matcher = kwargs.get(MATCHER_FIELD)
                 if sub_matcher is not None:
                     valid_matcher = json.loads(sub_matcher)
@@ -1534,16 +1775,20 @@
         Acknowledge this message.
 
         Messages consumed from subscriptions with a client acknowledgment mode
         must be explicitly acknowledged. The eFTL server will stop delivering
         messages to the client once the server's configured maximum number of
         unacknowledged messages is reached.
 
-        :param message: The message being acknowledged
-        :return:
+	Parameters
+        ----------
+        message: The message being acknowledged
+	
+	Returns
+        --------
         """
         seq_num = message._get_sequence_number_()
         sub_id = message._get_subscriber_id_()
 
         if not self._permanently_closed():
             if self._get_acknowledgement_mode(sub_id) == ACKNOWLEDGE_MODE_CLIENT:
                 if seq_num is not None and sub_id is not None:
@@ -1560,16 +1805,20 @@
         Acknowledge all messages up to and including this message.
 
         Messages consumed from subscriptions with a client acknowledgment mode
         must be explicitly acknowledged. The eFTL server will stop delivering
         messages to the client once the server's configured maximum number of
         unacknowledged messages is reached.
 
-        :param message: The message being acknowledged1
-        :return:
+	Parameters
+	----------
+	message: The message being acknowledged1
+
+	Returns
+	--------
         """
         seq_num = message._get_sequence_number_()
         sub_id = message._get_subscriber_id_()
 
         if not self._permanently_closed():
             if self._get_acknowledgement_mode(sub_id) == ACKNOWLEDGE_MODE_CLIENT:
                 if seq_num is not None and sub_id is not None:
@@ -1582,22 +1831,28 @@
             raise ConnectionError("Connection is closed.")
 
     async def send_request(self, message, timeout, **kwargs):
         """
         Publish a request message.
 
         This call returns immediately. When the reply is received
-        the eFTL library calls your {@link RequestListener#onReply}
-        callback.
+        the eFTL library calls your 'on_reply' callback.
 
-        :param message: The request message to publish.
-        :param timeout: timeout seconds to wait for reply
-        :param kwargs:
-              callbacks:
-        :return:
+	Parameters
+	----------
+            message: The request message to publish.
+            timeout: timeout seconds to wait for reply
+            kwargs:
+                Callbacks:
+                    'on_reply(message):' A request operation has received a reply.
+	       	    Parameters
+		    ----------
+        	        message: The reply message.
+	Returns
+        -------
         """
         if not self._permanently_closed():
             if isinstance(message, EftlMessage):
                 request_metadata ={}
                 request_metadata["is_request"] = True
                 request_metadata["timeout"] = timeout
                 self._ws._send_request(message, request_metadata, kwargs)
@@ -1607,22 +1862,28 @@
             raise ConnectionError("Connection is closed.")
 
     async def send_reply(self, requestMessage, replyMessage, **kwargs):
         """
         Send a reply message in response to a request message.
 
         This call returns immediately. When the send completes successfully
-        the eFTL library calls your {@link CompletionListener#onCompletion}
-        callback.
+        the eFTL library calls your on_complete callback.
 
-        :param requestMessage: The reply message to send
-        :param replyMessage: The request msg
-        :param kwargs:
-               callbacks
-        :return:
+        Parameters
+	----------
+            requestMessage: The reply message to send
+            replyMessage: The request msg
+            kwargs:
+                Callbacks
+                    'on_complete(message):'
+                    Parameters
+                    ----------
+                        message: The reply message that completed successfully
+	Return
+        -------
         """
         if not self._permanently_closed():
             if isinstance(requestMessage, EftlMessage) and isinstance(replyMessage, EftlMessage):
                 reply_to = requestMessage._get_reply_to_()
                 if reply_to is not None:
                     reply_metadata = {}
                     reply_metadata["to_field"] = reply_to
@@ -1642,32 +1903,32 @@
         For durable subscriptions, this call will cause the persistence
         service to remove the durable subscription, along with any
         persisted messages.
 
         Programs receive subscription identifiers through their
         methods.
 
-        :param sub_id:  Subscription identifier of the subscription to delete.
-        timeout`
-        :return:
+        Parameters
+        ----------
+            sub_id:  Subscription identifier of the subscription to delete.
+        Return
+        -------
         """
         if not self._permanently_closed():
             self._ws._unsubscribe(sub_id)
         else:
             raise ConnectionError("Connection is closed.")
 
     async def unsubscribe_all(self):
         """
-        Unsubscribe from all subscriptions.
+        Unsubscribe from messages on all subscriptions.
+        For durable subscriptions, this call will cause the persistence
+        service to remove the durable subscription, along with any
+        persisted messages.
 
-        Parameters
-        ----------
-        timeout : optional
-            Number of seconds to halt waiting on acknowledgement from
-            the server (default set in EftlConnection.connect()).
         """
         if not self._permanently_closed():
             self._ws._unsubscribe_all()
         else:
             raise ConnectionError("Connection is closed.")
 
     async def close_subscription(self, subscription_id):
@@ -1702,80 +1963,147 @@
 
         """
         if not self._permanently_closed():
             self._ws._close_all_subscriptions()
         else:
             raise ConnectionError("Connection is closed.")
 
+    async def stop_subscription(self, subscription_id):
+        """
+        Stop message delivery to the specified subscription.
+
+        Parameters
+        __________
+            subscription_id: Subscription identifier of the subscription to stop.
+        """
+        if not self.stop_supported:
+            raise EftlUnsupportedError("stop subscription is not supported with this server")
+
+        sub = self.subscriptions.get(subscription_id)
+        if sub["state"] != SUB_STOPPED:
+            sub["state"] = SUB_STOPPED
+            self._ws._stop_subscription(subscription_id=subscription_id)
+
+    async def start_subscription(self, subscription_id):
+        """
+        Resume message delivery to the specified subscription if stopped.
+
+        Parameters
+        __________
+            subscription_id: Subscription identifier of the subscription to start.
+        """
+        if not self.stop_supported:
+            raise EftlUnsupportedError("stop subscription is not supported with this server")
+
+        sub = self.subscriptions.get(subscription_id)
+        if sub["state"] == SUB_STOPPED:
+            sub["state"] = SUB_STARTING
+            self._ws._start_subscription(subscription_id=subscription_id)
+
     async def publish(self, message, **kwargs):
         """
         Publish a one-to-many message to all subscribing clients.
+        This call returns immediately; publishing continues asynchronously.
+        When the publish completes successfully, the eFTL library calls your
+        on_completel callback. 
+
+        When communicating with EMS, to publish a messages on a specific EMS
+        destination include the message field name <code>_dest</code>.
+        To distinguish between topics and queues the destination can be prefixed with
+        either "TOPIC:" or "QUEUE:", for example "TOPIC:MyDest" or "QUEUE:MyDest". A
+        destination with no prefix is a topic.
+   
+        example
+        To publish a message on a specific EMS destination
+        add a string field to the message; for example:</caption>
+        message.set("_dest", "MyDest");
+
+	Parameters
+	__________
+        message: Publish this message.
 
-        This call returns immediately; publishing continues
-        asynchronously.  When the publish completes successfully,
-        the eFTL library calls your
-
-        :param message: Publish this message.
-        :param kwargs:
-               callbacks:
-               on_publish
-               on_error
-        :return:
+        kwargs:
 
-        ValueError
-            If the message size exceeds the maximum.
-        TypeError
-            If the message is not of type EftlMessage
-        ConnectionError
-            If the connection is closed.
+            Callbacks:
+
+               'on_publish(message):' A publish operation has completed successfully
+	
+               Parameters
+    	       __________
+	       message: This message has been published.
+
+               'on_error(connection, code, reason):' An error prevented an operation.
+               Parameters
+	       ----------
+               connection : connection object. For publish errors, this argument is the message that was not published. 
+                                               For subscription errors, this argument is an object that represents 
+                                               a subscription identifier.
+               code: A code categorizes the error. Your program can use this value in its response logic.
+               reason: This string provides more detail. Your program can use this value in error reporting and logging.
+        Return
+        ------
+            ValueError: If the message size exceeds the maximum.
+            TypeError: If the message is not of type EftlMessage
+            ConnectionError: If the connection is closed.
 
         """
         if not self._permanently_closed():
             if isinstance(message, EftlMessage):
                 self._ws._publish(message, None, None, kwargs)
             else:
                 raise TypeError("Only message of type 'EftlMessage' is allowed to publish.")
         else:
             raise ConnectionError("Connection is closed.")
 
     async def create_kv_map(self, name):
         """
         Return a new EftlKVMap associated with this connection.
         
-        :param name: name of the KVMap
-        :return:  The KVmap object
+        Parameters
+        ----------
+            name: name of the KVMap
+        Return
+        ------
+            The KVmap object
         """
         if not self._permanently_closed():
             if isinstance(name, str):
                 return EftlKVMap(self, name)
             else:
                 raise TypeError("kv_map name should be of type 'str'")
         else:
             raise ConnectionError("Connection is closed.")
 
     async def remove_kv_map(self, name):
         """
         Remove a EftlKVMap object.
         
-        :param name: the name of the map
-        :return:
+        Parameters
+        ----------
+        name: the name of the map
+
+        Return
+        ------
+
         """
         if not self._permanently_closed():
             if isinstance(name, str):
                 self._ws._remove_kv_map(name)
             else:
                 raise TypeError("kv_map name should be of type 'str'")
         else:
             raise ConnectionError("Connection is closed.")
 
     def create_message(self):
         """
         Create an EftlMessage that can be used to publish or send request/replies.
 
-        :return: The EftlMessage object
+        Return
+        ------
+            The EftlMessage Object
 
         """
         return EftlMessage()
 
     async def _async_sleep(self, t):
         await asyncio.sleep(t)
 
@@ -1918,14 +2246,16 @@
                     self._handle_error(msg)
                 elif op_code == OP_ACK:
                     self._handle_ack(msg)
                 elif op_code == OP_REQUEST_REPLY:
                     self._handle_reply(msg)
                 elif op_code == OP_MAP_RESPONSE:
                     self._handle_map_response(msg)
+                elif op_code == OP_STARTED:
+                    self._handle_started(msg)
                 else:
                     logger.debug("Received unknown op code ({}):\n{}".format(op_code, msg))
 
             def onClose(self, was_clean, code, reason="connection failed"):
 
                 self.factory.conn.connection_closed = True
                 self.factory.conn.got_login_reply = False
@@ -1972,14 +2302,15 @@
                 self.factory.conn.previously_connected = True
                 resume = str(message.get(RESUME_FIELD, "")).lower() == "true"
                 self.factory.conn.client_id = message.get(CLIENT_ID_FIELD)
                 self.factory.conn.reconnect_token = message.get(ID_TOKEN_FIELD)
                 self.timeout = message.get(TIMEOUT_FIELD)
                 self.heartbeat = message.get(HEARTBEAT_FIELD)
                 self.max_message_size = message.get(MAX_SIZE_FIELD)
+                self.factory.conn.stop_supported = str(message.get(STOP_SUPPORTED_FIELD)).lower() == "true"
 
                 self.qos = str(message.get(QOS_FIELD, "")).lower() == "true"
 
                 self.timeout_check = threading.Timer(
                     self.timeout,
                     self._do_timeout_check)
 
@@ -2031,14 +2362,17 @@
             def _subscribe(self, sub_id, subscriber_obj_exist, **kwargs):
                 if not subscriber_obj_exist:
                     subscription = {
                         "options": kwargs,
                         "id": sub_id,
                         "pending": True,
                         "last_received_sequence_number": -1,
+                        "state": SUB_STARTED,
+                        "dispatcher_active": False,
+                        "message_queue": [],
                         }
 
                     ack_mode_str = kwargs.get(ACK_FIELD)
                     if ack_mode_str is not None:
                         if ack_mode_str == ACKNOWLEDGE_MODE_CLIENT:
                             subscription[ACKNOWLEDGE_MODE] = ACKNOWLEDGE_MODE_CLIENT
                         elif ack_mode_str == ACKNOWLEDGE_MODE_NONE:
@@ -2050,14 +2384,15 @@
                         # ack mode is auto by default
                         subscription[ACKNOWLEDGE_MODE] = ACKNOWLEDGE_MODE_AUTO
                     self.factory.conn.subscriptions[sub_id] = subscription
 
                 sub_message = {
                     OP_FIELD: OP_SUBSCRIBE,
                     ID_FIELD: sub_id,
+                    STOPPED_FIELD: self.factory.conn.subscriptions[sub_id]["state"] == SUB_STOPPED,
                 }
 
                 sub_matcher = kwargs.get(MATCHER_FIELD)
                 if sub_matcher:
                     sub_message[MATCHER_FIELD] = sub_matcher
                 sub_durable = kwargs.get(DURABLE_FIELD)
                 if sub_durable:
@@ -2081,14 +2416,16 @@
 
             def _handle_subscribed(self, message):
                 sub_id = message.get(ID_FIELD)
 
                 sub = self.factory.conn.subscriptions.get(sub_id)
                 if sub and sub.get("pending") is not None:
                     sub["pending"] = False
+                    if self.factory.conn.subscriptions[sub_id]["state"] == SUB_STARTING:
+                        self.factory.conn.subscriptions[sub_id]["state"] = SUB_STARTED
                     _call_dict_function(sub.get("options"), "on_subscribe", id=sub_id, )
 
             def _remove_kv_map(self, name):
                 remove_map_message = {
                     OP_FIELD: OP_MAP_DESTROY,
                     MAP_FIELD: name
                     }
@@ -2296,26 +2633,46 @@
                         if value is not None:
                             eftl_message = EftlMessage(value)
 
                         self._pending_response(sequence, eftl_message)
                     else:
                         self._pending_error(sequence, err_code, reason)
 
-
             def _handle_message(self, message):
-                sub        = self.factory.conn.subscriptions.get(message.get(TO_FIELD))
+                sub = self.factory.conn.subscriptions.get(message.get(TO_FIELD))
+                if sub is None:
+                    return
+
+                sub["message_queue"].append(message)
+                # If one isn't already active, launch a dispatcher to handle existing
+                # backlog of messages for subscriber
+                if not sub["dispatcher_active"]:
+                    # This is decremented by dispatcher
+                    sub["dispatcher_active"] = True
+                    event_loop = asyncio.get_event_loop()
+                    event_loop.create_task(self._message_dispatcher(sub))
+
+            async def _message_dispatcher(self, sub):
+                while sub["message_queue"]:
+                    message = sub["message_queue"].pop(0)
+                    await self._dispatch_message(sub, message)
+
+                sub["dispatcher_active"] = False
+
+            async def _dispatch_message(self, sub, message):
                 seq_num    = message.get(SEQ_NUM_FIELD)
                 data       = message.get(BODY_FIELD)
                 sid        = message.get(STORE_MSG_ID_FIELD)
                 cnt        = message.get(DELIVERY_COUNT_FIELD)
                 reply_to   = message.get(REPLY_TO_FIELD)
                 request_id = message.get(REQ_ID_FIELD)
 
-                if sub is not None and seq_num is not None:
+                if sub is not None and seq_num is not None and sub["state"] == SUB_STARTED:
                     if seq_num > sub.get('last_received_sequence_number'):
+                        sub['last_received_sequence_number'] = seq_num
                         if sub.get("options") is not None:
 
                             if data is not None:
                                 eftl_message = EftlMessage(data)
 
                                 eftl_message._set_sequence_number_(seq_num)
 
@@ -2331,36 +2688,60 @@
 
                                 if reply_to is not None:
                                     eftl_message._set_reply_to_(reply_to)
 
                                 if request_id is not None:
                                     eftl_message._set_request_id_(request_id)
 
-                                _call_dict_function(sub.get("options"), "on_message", message=eftl_message)
+                                callback = sub.get("options").get("on_message")
+                                if callback is not None:
+                                    await callback(message=eftl_message)
 
-                        sub['last_received_sequence_number'] = seq_num
 
                     if sub.get(ACKNOWLEDGE_MODE) == ACKNOWLEDGE_MODE_AUTO:
                         sub_id = sub.get(ID_FIELD)
                         self._ack(seq_num, sub_id)
 
+            def _handle_started(self, message):
+                sub = self.factory.conn.subscriptions.get(message.get(TO_FIELD))
+                if sub is not None and sub["state"] == SUB_STARTING:
+                    sub["state"] = SUB_STARTED
+
 
             def _ack(self, seq_num, sub_id=None):
                 if seq_num <= 0:
                     return
 
                 envelope = {
                     OP_FIELD: OP_ACK,
                     SEQ_NUM_FIELD: seq_num
                     }
 
                 if sub_id is not None:
                     envelope[ID_FIELD] = sub_id
                 self._send(envelope, 0, False)
 
+            def _stop_subscription(self, subscription_id):
+                sub = self.factory.conn.subscriptions.get(subscription_id)
+                seq_num = sub["last_received_sequence_number"]
+                envelope = {
+                    OP_FIELD: OP_STOP,
+                    SEQ_NUM_FIELD: seq_num,
+                    ID_FIELD: subscription_id,
+                }
+
+                self._send(envelope, 0, False)
+
+            def _start_subscription(self, subscription_id):
+                envelope = {
+                    OP_FIELD: OP_START,
+                    ID_FIELD: subscription_id,
+                }
+
+                self._send(envelope, 0, False)
 
             def _handle_error(self, message):
                 err_code = message.get(ERR_CODE_FIELD)
                 reason = message.get(REASON_FIELD)
 
                 _call_dict_function(
                     self.factory.conn.connect_options,
```

## Comparing `eftl-1.2.0.dist-info/METADATA` & `eftl-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eftl
-Version: 1.2.0
+Version: 1.3.0
 Summary: TIBCO eFTL client for Python
 Home-page: https://www.tibco.com
 Author: TIBCO Software Inc.
 Author-email: support@tibco.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `eftl-1.2.0.dist-info/RECORD` & `eftl-1.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 messaging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 messaging/eftl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-messaging/eftl/connection.py,sha256=LCf2VKnGlWozCbq6QhIMZ8zjIl4GXNx6FwimglIiGcY,94765
-eftl-1.2.0.dist-info/METADATA,sha256=LJ1GZpuK3uLjWNhNcOcrT48elxEodqQHB0XzmfgjZls,21432
-eftl-1.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-eftl-1.2.0.dist-info/top_level.txt,sha256=CE3ua24gYbyHhWjQNGzNHZ1-hxYH0OUDnQoj4Xni5zw,10
-eftl-1.2.0.dist-info/RECORD,,
+messaging/eftl/connection.py,sha256=WBETuKrfU0-sgrsqPy2-eBmjO-717qTIyuoJHQYh0v8,108577
+eftl-1.3.0.dist-info/METADATA,sha256=LJ1GZpuK3uLjWNhNcOcrT48elxEodqQHB0XzmfgjZls,21432
+eftl-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+eftl-1.3.0.dist-info/top_level.txt,sha256=CE3ua24gYbyHhWjQNGzNHZ1-hxYH0OUDnQoj4Xni5zw,10
+eftl-1.3.0.dist-info/RECORD,,
```

