# Comparing `tmp/ntheory-0.0.1.tar.gz` & `tmp/ntheory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntheory-0.0.1.tar", last modified: Fri May 12 22:00:20 2023, max compression
+gzip compressed data, was "ntheory-0.0.2.tar", last modified: Fri May 12 22:27:55 2023, max compression
```

## Comparing `ntheory-0.0.1.tar` & `ntheory-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 22:00:20.250717 ntheory-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-05-12 21:31:16.000000 ntheory-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1793 2023-05-12 22:00:20.248725 ntheory-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-12 21:37:10.000000 ntheory-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 22:00:20.193868 ntheory-0.0.1/ntheory/
--rw-rw-rw-   0        0        0       22 2023-05-12 21:45:43.000000 ntheory-0.0.1/ntheory/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-12 21:38:33.000000 ntheory-0.0.1/ntheory/greet.py
-drwxrwxrwx   0        0        0        0 2023-05-12 22:00:20.243745 ntheory-0.0.1/ntheory.egg-info/
--rw-rw-rw-   0        0        0     1793 2023-05-12 22:00:20.000000 ntheory-0.0.1/ntheory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-12 22:00:20.000000 ntheory-0.0.1/ntheory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 22:00:20.000000 ntheory-0.0.1/ntheory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 22:00:20.000000 ntheory-0.0.1/ntheory.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2023-05-12 22:00:20.000000 ntheory-0.0.1/ntheory.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 22:00:20.000000 ntheory-0.0.1/ntheory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      882 2023-05-12 21:59:45.000000 ntheory-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 22:00:20.250717 ntheory-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      372 2023-05-12 21:45:49.000000 ntheory-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 22:00:20.245729 ntheory-0.0.1/tests/
--rw-rw-rw-   0        0        0       79 2023-05-12 21:45:00.000000 ntheory-0.0.1/tests/test_greet.py
+drwxrwxrwx   0        0        0        0 2023-05-12 22:27:55.653299 ntheory-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-12 21:31:16.000000 ntheory-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1797 2023-05-12 22:27:55.652300 ntheory-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-12 21:37:10.000000 ntheory-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 22:27:55.606423 ntheory-0.0.2/ntheory/
+-rw-rw-rw-   0        0        0       22 2023-05-12 21:45:43.000000 ntheory-0.0.2/ntheory/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-05-12 22:27:15.000000 ntheory-0.0.2/ntheory/greet.py
+drwxrwxrwx   0        0        0        0 2023-05-12 22:27:55.646322 ntheory-0.0.2/ntheory.egg-info/
+-rw-rw-rw-   0        0        0     1797 2023-05-12 22:27:55.000000 ntheory-0.0.2/ntheory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-12 22:27:55.000000 ntheory-0.0.2/ntheory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 22:27:55.000000 ntheory-0.0.2/ntheory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 22:27:55.000000 ntheory-0.0.2/ntheory.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2023-05-12 22:27:55.000000 ntheory-0.0.2/ntheory.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 22:27:55.000000 ntheory-0.0.2/ntheory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      886 2023-05-12 22:27:00.000000 ntheory-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 22:27:55.653299 ntheory-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      372 2023-05-12 21:45:49.000000 ntheory-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 22:27:55.649310 ntheory-0.0.2/tests/
+-rw-rw-rw-   0        0        0       79 2023-05-12 21:45:00.000000 ntheory-0.0.2/tests/test_greet.py
```

### Comparing `ntheory-0.0.1/LICENSE` & `ntheory-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ntheory-0.0.1/PKG-INFO` & `ntheory-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntheory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read the latest Real Python tutorials
 Author: Kasper Arfman
 Author-email: KasperArfman <kasper.arf@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kasper Arfman
         
@@ -22,15 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/realpython/reader
+Project-URL: Homepage, https://github.com/Kasper-Arfman/ntheory
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ntheory-0.0.1/ntheory.egg-info/PKG-INFO` & `ntheory-0.0.2/ntheory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntheory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Read the latest Real Python tutorials
 Author: Kasper Arfman
 Author-email: KasperArfman <kasper.arf@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kasper Arfman
         
@@ -22,15 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/realpython/reader
+Project-URL: Homepage, https://github.com/Kasper-Arfman/ntheory
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ntheory-0.0.1/pyproject.toml` & `ntheory-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ntheory"
-version = "0.0.1"
+version = "0.0.2"
 description = "Read the latest Real Python tutorials"
 readme = "README.md"
 authors = [{ name = "KasperArfman", email = "kasper.arf@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -22,11 +22,11 @@
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
-Homepage = "https://github.com/realpython/reader"
+Homepage = "https://github.com/Kasper-Arfman/ntheory"
 
 [project.scripts]
 realpython = "reader.__main__:main"
```

