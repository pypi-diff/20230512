# Comparing `tmp/Semicolonizer-1.0.tar.gz` & `tmp/Semicolonizer-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Semicolonizer-1.0.tar", last modified: Fri May 12 10:04:21 2023, max compression
+gzip compressed data, was "Semicolonizer-1.2.tar", last modified: Fri May 12 10:36:54 2023, max compression
```

## Comparing `Semicolonizer-1.0.tar` & `Semicolonizer-1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:04:21.221321 Semicolonizer-1.0/
--rw-rw-rw-   0        0        0      186 2023-05-12 10:04:21.221321 Semicolonizer-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 10:04:21.218281 Semicolonizer-1.0/Semicolonizer/
--rw-rw-rw-   0        0        0     3566 2023-05-12 09:53:15.000000 Semicolonizer-1.0/Semicolonizer/Semicolonizer.py
--rw-rw-rw-   0        0        0        0 2023-05-12 09:52:26.000000 Semicolonizer-1.0/Semicolonizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:04:21.220315 Semicolonizer-1.0/Semicolonizer.egg-info/
--rw-rw-rw-   0        0        0      186 2023-05-12 10:04:21.000000 Semicolonizer-1.0/Semicolonizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-12 10:04:21.000000 Semicolonizer-1.0/Semicolonizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:04:21.000000 Semicolonizer-1.0/Semicolonizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 10:04:21.000000 Semicolonizer-1.0/Semicolonizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 10:04:21.221321 Semicolonizer-1.0/setup.cfg
--rw-rw-rw-   0        0        0      426 2023-05-12 10:04:05.000000 Semicolonizer-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:36:54.396391 Semicolonizer-1.2/
+-rw-rw-rw-   0        0        0      186 2023-05-12 10:36:54.396391 Semicolonizer-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-12 10:36:54.393386 Semicolonizer-1.2/Semicolonizer/
+-rw-rw-rw-   0        0        0     3640 2023-05-12 10:34:51.000000 Semicolonizer-1.2/Semicolonizer/Semicolonizer.py
+-rw-rw-rw-   0        0        0       38 2023-05-12 10:13:52.000000 Semicolonizer-1.2/Semicolonizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:36:54.395389 Semicolonizer-1.2/Semicolonizer.egg-info/
+-rw-rw-rw-   0        0        0      186 2023-05-12 10:36:54.000000 Semicolonizer-1.2/Semicolonizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-12 10:36:54.000000 Semicolonizer-1.2/Semicolonizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:36:54.000000 Semicolonizer-1.2/Semicolonizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-12 10:36:54.000000 Semicolonizer-1.2/Semicolonizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-12 10:36:54.000000 Semicolonizer-1.2/Semicolonizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:36:54.396391 Semicolonizer-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-05-12 10:36:50.000000 Semicolonizer-1.2/setup.py
```

### Comparing `Semicolonizer-1.0/Semicolonizer/Semicolonizer.py` & `Semicolonizer-1.2/Semicolonizer/Semicolonizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,17 +85,22 @@
             else:
                 return
 
         with keyboard.Listener(on_press=on_pressed) as listener:
             listener.join()
 
 
-if __name__ == "__main__":
+def main():
     lst = Listener()
     if len(sys.argv) > 1:
         lst.file_name = sys.argv[1]
     file_name = lst.file_name
     print(f"{file_name = }")
     print("f5 to enable/disable the Semicolonizer")
-    print("f2 to Semicolonize the php file")
+    print("f4 to Semicolonize the php file")
+    print("f2 to change default file_name")
     print("f6 to quit")
     lst.mainloop()
+
+
+if __name__ == "__main__":
+    main()
```

