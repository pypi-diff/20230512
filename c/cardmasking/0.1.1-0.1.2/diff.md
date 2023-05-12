# Comparing `tmp/cardmasking-0.1.1-py3-none-any.whl.zip` & `tmp/cardmasking-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1557 bytes, number of entries: 6
+Zip file size: 1585 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 05:29 cardmasking/__init__.py
--rw-rw-rw-  2.0 fat      374 b- defN 23-May-12 06:05 cardmasking/masking.py
--rw-rw-rw-  2.0 fat      158 b- defN 23-May-12 06:14 cardmasking-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 06:14 cardmasking-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-12 06:14 cardmasking-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      468 b- defN 23-May-12 06:14 cardmasking-0.1.1.dist-info/RECORD
-6 files, 1104 bytes uncompressed, 701 bytes compressed:  36.5%
+-rw-rw-rw-  2.0 fat      461 b- defN 23-May-12 06:22 cardmasking/masking.py
+-rw-rw-rw-  2.0 fat      161 b- defN 23-May-12 06:23 cardmasking-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 06:23 cardmasking-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-12 06:23 cardmasking-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      468 b- defN 23-May-12 06:23 cardmasking-0.1.2.dist-info/RECORD
+6 files, 1194 bytes uncompressed, 729 bytes compressed:  38.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: cardmasking/__init__.py
 Comment: 
 
 Filename: cardmasking/masking.py
 Comment: 
 
-Filename: cardmasking-0.1.1.dist-info/METADATA
+Filename: cardmasking-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: cardmasking-0.1.1.dist-info/WHEEL
+Filename: cardmasking-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: cardmasking-0.1.1.dist-info/top_level.txt
+Filename: cardmasking-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cardmasking-0.1.1.dist-info/RECORD
+Filename: cardmasking-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cardmasking/masking.py

```diff
@@ -12,9 +12,15 @@
         x+=1
 
     for i in cvv:
         cvv_num += "*"
 
     for i in ExpiryDate:
         expiry += "*"
+
+    response = {
+        "card":card_num,
+        "cvv":cvv_num,
+        "expiry":expiry
+    }
         
-    return card_num,cvv_num,expiry
+    return response
```

