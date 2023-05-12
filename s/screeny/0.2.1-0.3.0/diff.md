# Comparing `tmp/screeny-0.2.1.tar.gz` & `tmp/screeny-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.2.1.tar", last modified: Wed May 10 19:38:17 2023, max compression
+gzip compressed data, was "screeny-0.3.0.tar", last modified: Fri May 12 15:35:50 2023, max compression
```

## Comparing `screeny-0.2.1.tar` & `screeny-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 19:38:17.342211 screeny-0.2.1/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.2.1/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    25653 2023-05-10 14:08:09.000000 screeny-0.2.1/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)     1753 2023-05-10 19:38:17.342375 screeny-0.2.1/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)     1373 2023-05-10 14:13:59.000000 screeny-0.2.1/README.md
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.2.1/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 19:38:17.337043 screeny-0.2.1/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.2.1/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)      446 2023-05-10 14:08:09.000000 screeny-0.2.1/screeny/mouse.py
--rw-r--r--   0 paulpol    (501) staff       (20)     4680 2023-05-10 19:32:34.000000 screeny-0.2.1/screeny/screeny.py
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 19:38:17.341832 screeny-0.2.1/screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)     1753 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      274 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       43 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      515 2023-05-10 19:38:17.343171 screeny-0.2.1/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 15:35:50.385030 screeny-0.3.0/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.3.0/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:34:47.000000 screeny-0.3.0/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 15:35:50.385191 screeny-0.3.0/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)     2544 2023-05-12 15:23:58.000000 screeny-0.3.0/README.md
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.3.0/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 15:35:50.382243 screeny-0.3.0/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)      195 2023-05-12 14:29:39.000000 screeny-0.3.0/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     4454 2023-05-12 14:29:39.000000 screeny-0.3.0/screeny/image.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 14:29:39.000000 screeny-0.3.0/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 15:08:56.000000 screeny-0.3.0/screeny/screeny.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 15:35:50.384601 screeny-0.3.0/screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-05-12 15:35:50.385824 screeny-0.3.0/setup.cfg
```

### Comparing `screeny-0.2.1/LICENSE` & `screeny-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.2.1/LICENSE-3RD-Party.txt` & `screeny-0.3.0/LICENSE-3RD-Party.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 ------------------------------------------------------------------------------
-OpenCV library is redistributed within screeny package.
-This license applies to OpenCV.
+OpenCV and Python-tesseract library is redistributed within screeny package.
+This license applies to OpenCV and Python-tesseract.
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `screeny-0.2.1/setup.cfg` & `screeny-0.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = screeny
-version = 0.2.1
+version = 0.3.0
 author = Paul Pol
 author_email = mail@paul-pol.de
 description = A simple python library for working with screens and images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
@@ -16,12 +16,13 @@
 packages = find:
 install_requires = 
 	numpy
 	opencv-python
 	mss
 	PySide6
 	matplotlib
+	pytesseract
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

