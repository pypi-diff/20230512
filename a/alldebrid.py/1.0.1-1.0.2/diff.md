# Comparing `tmp/alldebrid.py-1.0.1.tar.gz` & `tmp/alldebrid.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alldebrid.py-1.0.1.tar", last modified: Thu May 11 11:56:16 2023, max compression
+gzip compressed data, was "alldebrid.py-1.0.2.tar", last modified: Fri May 12 14:57:18 2023, max compression
```

## Comparing `alldebrid.py-1.0.1.tar` & `alldebrid.py-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:56:16.061893 alldebrid.py-1.0.1/
--rw-rw-rw-   0        0        0      100 2023-05-11 11:56:16.023236 alldebrid.py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-11 11:31:41.000000 alldebrid.py-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 11:56:15.624121 alldebrid.py-1.0.1/alldebrid/
--rw-rw-rw-   0        0        0       83 2023-05-11 11:51:51.000000 alldebrid.py-1.0.1/alldebrid/__init__.py
--rw-rw-rw-   0        0        0    42184 2023-05-11 11:49:35.000000 alldebrid.py-1.0.1/alldebrid/alldebrid.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:56:15.959778 alldebrid.py-1.0.1/alldebrid.py.egg-info/
--rw-rw-rw-   0        0        0      100 2023-05-11 11:56:15.000000 alldebrid.py-1.0.1/alldebrid.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-11 11:56:15.000000 alldebrid.py-1.0.1/alldebrid.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:56:15.000000 alldebrid.py-1.0.1/alldebrid.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-11 11:56:15.000000 alldebrid.py-1.0.1/alldebrid.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 11:56:15.000000 alldebrid.py-1.0.1/alldebrid.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 11:56:16.062918 alldebrid.py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      285 2023-05-11 11:56:04.000000 alldebrid.py-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:57:18.307587 alldebrid.py-1.0.2/
+-rw-rw-rw-   0        0        0      100 2023-05-12 14:57:18.281301 alldebrid.py-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-11 11:31:41.000000 alldebrid.py-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 14:57:17.818729 alldebrid.py-1.0.2/alldebrid/
+-rw-rw-rw-   0        0        0      103 2023-05-12 14:57:07.000000 alldebrid.py-1.0.2/alldebrid/__init__.py
+-rw-rw-rw-   0        0        0    43242 2023-05-12 14:57:06.000000 alldebrid.py-1.0.2/alldebrid/alldebrid.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:57:18.164788 alldebrid.py-1.0.2/alldebrid.py.egg-info/
+-rw-rw-rw-   0        0        0      100 2023-05-12 14:57:17.000000 alldebrid.py-1.0.2/alldebrid.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-12 14:57:17.000000 alldebrid.py-1.0.2/alldebrid.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 14:57:17.000000 alldebrid.py-1.0.2/alldebrid.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 14:57:17.000000 alldebrid.py-1.0.2/alldebrid.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 14:57:17.000000 alldebrid.py-1.0.2/alldebrid.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 14:57:18.307587 alldebrid.py-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      285 2023-05-12 14:56:14.000000 alldebrid.py-1.0.2/setup.py
```

### Comparing `alldebrid.py-1.0.1/README.md` & `alldebrid.py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alldebrid.py-1.0.1/alldebrid/alldebrid.py` & `alldebrid.py-1.0.2/alldebrid/alldebrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,43 @@
         The error message.
 
         Returns:
             str: The error message.
         """
         return self._message
     
+class InvalidLinkError(Exception):
+    """
+    Invalid link error.
+
+    Attributes:
+        _link (str): The link that was invalid.
+    """
+    link: str
+
+    def __init__(self, link: str) -> None:
+        """
+        Initializes a new instance of the InvalidLinkError class.
+
+        Args:
+            link (str): The link that was invalid.
+        """
+        super().__init__(f"Invalid link: {link}")
+        self._link = link
+
+    @property
+    def link(self) -> str:
+        """
+        The link that was invalid.
+
+        Returns:
+            str: The link that was invalid.
+        """
+        return self._link
+    
 class EndpointNotFoundError(Exception):
     """
     Endpoint not found error.
 
     Attributes:
         _endpoint (str): The endpoint that was not found.
     """
@@ -936,22 +965,29 @@
 
         Raises
         ------
         APIError
             If request is unsuccessful.
         ValueError
             If endpoint is not found.
+        InvalidLinkError
+            If link is invalid.
         """
+
         if not link:
             raise ValueError("No link id to save")
 
         endpoint = self.endpoints.get("save a link")
         if not endpoint:
             raise ValueError("Endpoint not found for save new link")
         
+        for l in link:
+            if not re.match(r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+', l):
+                raise InvalidLinkError(l)
+        
         response = self._request(method="POST", endpoint=endpoint, links=link)
 
         if response.get("status") == "error":
             error = response["error"]
             raise APIError(error["code"], error["message"])
         
         return response
@@ -1276,7 +1312,13 @@
             params=params,
             files=files,
             timeout=timeout,
             session=session,
         )
 
         return response
+
+ad = AllDebrid(apikey="tXQQw2JPx8iKEyeeOoJE")
+try:
+    response = ad.save_new_link("invalid_link")
+except InvalidLinkError as e:
+    print(e)
```

