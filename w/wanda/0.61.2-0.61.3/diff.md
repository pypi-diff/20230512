# Comparing `tmp/wanda-0.61.2.tar.gz` & `tmp/wanda-0.61.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wanda-0.61.2.tar", max compression
+gzip compressed data, was "wanda-0.61.3.tar", max compression
```

## Comparing `wanda-0.61.2.tar` & `wanda-0.61.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-04-29 06:18:58.249614 wanda-0.61.2/LICENSE
--rw-r--r--   0        0        0     2012 2023-04-29 06:18:58.249614 wanda-0.61.2/README.md
--rw-r--r--   0        0        0      920 2023-04-29 07:47:10.638626 wanda-0.61.2/pyproject.toml
--rw-r--r--   0        0        0        1 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/__init__.py
--rw-r--r--   0        0        0    12124 2023-04-29 07:33:50.334412 wanda-0.61.2/wanda/sources.py
--rw-r--r--   0        0        0        0 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/__init__.py
--rw-r--r--   0        0        0      150 2023-04-29 06:25:38.899989 wanda-0.61.2/wanda/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2499 2023-04-29 06:25:38.899989 wanda-0.61.2/wanda/utils/__pycache__/common_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2997 2023-04-29 06:25:38.956658 wanda-0.61.2/wanda/utils/__pycache__/image_utils.cpython-310.pyc
--rw-r--r--   0        0        0     3245 2023-04-29 06:25:38.956658 wanda-0.61.2/wanda/utils/__pycache__/os_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1708 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/common_utils.py
--rw-r--r--   0        0        0     4189 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/image_utils.py
--rw-r--r--   0        0        0     3201 2023-04-29 06:18:58.249614 wanda-0.61.2/wanda/utils/os_utils.py
--rwxr-xr-x   0        0        0     5741 2023-04-29 06:54:06.187103 wanda-0.61.2/wanda/wanda.py
--rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 wanda-0.61.2/setup.py
--rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 wanda-0.61.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-29 06:18:58.249614 wanda-0.61.3/LICENSE
+-rw-r--r--   0        0        0     2018 2023-04-29 07:55:53.661451 wanda-0.61.3/README.md
+-rw-r--r--   0        0        0      919 2023-05-12 16:52:40.706458 wanda-0.61.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-04-29 06:18:58.249614 wanda-0.61.3/wanda/__init__.py
+-rw-r--r--   0        0        0    12124 2023-04-29 07:33:50.334412 wanda-0.61.3/wanda/sources.py
+-rw-r--r--   0        0        0        0 2023-04-29 06:18:58.249614 wanda-0.61.3/wanda/utils/__init__.py
+-rw-r--r--   0        0        0      150 2023-04-29 06:25:38.899989 wanda-0.61.3/wanda/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2499 2023-04-29 06:25:38.899989 wanda-0.61.3/wanda/utils/__pycache__/common_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2997 2023-04-29 06:25:38.956658 wanda-0.61.3/wanda/utils/__pycache__/image_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3245 2023-04-29 06:25:38.956658 wanda-0.61.3/wanda/utils/__pycache__/os_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1708 2023-04-29 06:18:58.249614 wanda-0.61.3/wanda/utils/common_utils.py
+-rw-r--r--   0        0        0     4189 2023-04-29 06:18:58.249614 wanda-0.61.3/wanda/utils/image_utils.py
+-rw-r--r--   0        0        0     3201 2023-04-29 06:18:58.249614 wanda-0.61.3/wanda/utils/os_utils.py
+-rwxr-xr-x   0        0        0     5933 2023-05-12 16:50:28.534821 wanda-0.61.3/wanda/wanda.py
+-rw-r--r--   0        0        0     3038 1970-01-01 00:00:00.000000 wanda-0.61.3/setup.py
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 wanda-0.61.3/PKG-INFO
```

### Comparing `wanda-0.61.2/LICENSE` & `wanda-0.61.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/README.md` & `wanda-0.61.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,27 +38,27 @@
 
 ## Notes
 - By default, the source is [unsplash](https://unsplash.com).
 - Some sources may have inapt images. Use them at your own risk.
 
 ## Supported sources
 
-- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive.alice.al)
+- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive-media.palanq.win)
 - [500px](https://500px.com)
 - [artstation](https://artstation.com)
 - [imgur](https://imgur.com) via [rimgo](https://rimgo.pussthecat.org)
 - [earthview](https://earthview.withgoogle.com)
 - local
 - [picsum](https://picsum.photos)
 - [reddit](https://reddit.com)
 - [unsplash](https://unsplash.com)
 - [wallhaven](https://wallhaven.cc)
 
 ## Build
-[python](https://www.python.org/downloads/) and [poetry](https://python-poetry.org/) are needed
+[python](https://www.python.org/downloads) and [poetry](https://python-poetry.org) are needed
 ```
 git clone https://github.com/ksh-b/wanda.git
 cd wanda
 poetry install
 poetry build
 poetry run wanda
 ```
```

### Comparing `wanda-0.61.2/pyproject.toml` & `wanda-0.61.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "wanda"
-version = "0.61.2"
+version = "0.61.3"
 description = "Set wallpapers with keywords or randomly"
 authors = ["kshib <ksyko@pm.me>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://gitlab.com/kshib/wanda"
-repository = "https://gitlab.com/kshib/wanda"
+homepage = "https://github.com/ksh-b/wanda"
+repository = "https://github.com/ksh-b/wanda"
 keywords=["wallpaper", "reddit", "wallhaven","unsplash","termux"]
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://gitlab.com/kshib/wanda/-/issues"
+"Bug Tracker" = "https://github.com/ksh-b/wanda/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 lxml = "^4.9.0"
 cloudscraper = "^1.2.60"
 Pillow = "^9.1.0"
 screeninfo = "^0.8"
@@ -32,8 +32,8 @@
 pytest-rerunfailures = "^11"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-wanda = "wanda.wanda:run"
+wanda = "wanda.wanda:run"
```

### Comparing `wanda-0.61.2/wanda/sources.py` & `wanda-0.61.3/wanda/sources.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/utils/__pycache__/common_utils.cpython-310.pyc` & `wanda-0.61.3/wanda/utils/__pycache__/common_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/utils/__pycache__/image_utils.cpython-310.pyc` & `wanda-0.61.3/wanda/utils/__pycache__/image_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/utils/__pycache__/os_utils.cpython-310.pyc` & `wanda-0.61.3/wanda/utils/__pycache__/os_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/utils/common_utils.py` & `wanda-0.61.3/wanda/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/utils/image_utils.py` & `wanda-0.61.3/wanda/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/utils/os_utils.py` & `wanda-0.61.3/wanda/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `wanda-0.61.2/wanda/wanda.py` & `wanda-0.61.3/wanda/wanda.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import wanda.utils.common_utils as common
 import wanda.utils.image_utils as image
 import wanda.utils.os_utils as osu
 import wanda.sources as sources
 
 folder = appdirs.user_cache_dir("wanda")
-version = "0.61.2"
+version = "0.61.3"
 
 
 def usage(level=0):
     cyan = "\033[36m"
     pink = "\033[35m"
     print("Sources:")
     print(f"{cyan}4chan {pink}[keyword]|[keyword@board]")
@@ -131,46 +131,46 @@
     home = True
     lock = True
     fitwp = False
     if "-l" in sys.argv and args.l:
         home = False
     if "-h" in sys.argv and args.h:
         lock = False
-    if "-f" in sys.argv and source not in ('e', 'earthview'):
+    if "-f" in sys.argv and source_map(source) not in ('e', 'earthview'):
         fitwp = True
-    if source != "local" and not common.is_connected():
+    if source_map(source) != "local" and not common.is_connected():
         print("Please check your internet connection and try again")
         exit(1)
-    if source == "fourchan":
+    if source_map(source) == "fourchan":
         wp = sources.fourchan(term)
-    elif source == "reddit":
+    elif source_map(source) == "reddit":
         wp = sources.reddit(term)
-    elif source == "picsum":
+    elif source_map(source) == "picsum":
         wp = sources.picsum(term)
-    elif source == "imgur":
+    elif source_map(source) == "imgur":
         wp = sources.imgur(term)
-    elif source == "fivehundredpx":
+    elif source_map(source) == "fivehundredpx":
         wp = sources.fivehundredpx(term)
-    elif source == "artstation_prints":
+    elif source_map(source) == "artstation_prints":
         wp = sources.artstation_prints(term)
-    elif source == "artstation_artist":
+    elif source_map(source) == "artstation_artist":
         wp = sources.artstation_artist(term)
-    elif source == "artstation_any":
+    elif source_map(source) == "artstation_any":
         wp = sources.artstation_any(term)
-    elif source == "local":
+    elif source_map(source) == "local":
         wp = sources.local(term)
-    elif source == "waifuim":
+    elif source_map(source) == "waifuim":
         wp = sources.waifuim(term)
-    elif source == "musicbrainz":
+    elif source_map(source) == "musicbrainz":
         wp = sources.musicbrainz(term)
-    elif source == "wallhaven":
+    elif source_map(source) == "wallhaven":
         wp = sources.wallhaven(term)
-    elif source == "unsplash":
+    elif source_map(source) == "unsplash":
         wp = sources.unsplash(term)
-    elif source == "earthview":
+    elif source_map(source) == "earthview":
         wp = sources.earthview(term)
     else:
         print(f"Unknown Source: {source}. Using unsplash.")
         wp = sources.unsplash(term)
     image.set_wp(wp, home, lock, fitwp)
     return 0
```

### Comparing `wanda-0.61.2/setup.py` & `wanda-0.61.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
  'screeninfo>=0.8,<0.9']
 
 entry_points = \
 {'console_scripts': ['wanda = wanda.wanda:run']}
 
 setup_kwargs = {
     'name': 'wanda',
-    'version': '0.61.2',
+    'version': '0.61.3',
     'description': 'Set wallpapers with keywords or randomly',
-    'long_description': '# wanda\nScript to set wallpaper using keyword or randomly\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e5aacd529ce04f3fb8c0f9ce6a3bdd9e)](https://www.codacy.com/gh/ksyko/wanda/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ksyko/wanda&amp;utm_campaign=Badge_Grade)[![PyPI](https://img.shields.io/pypi/v/wanda)](https://pypi.org/project/wanda/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/wanda)](https://pypistats.org/packages/wanda)\n[![PyPI - License](https://img.shields.io/pypi/l/wanda)](https://tldrlegal.com/license/mit-license)\n[![codecov](https://codecov.io/gl/kshib/wanda/branch/main/graph/badge.svg?token=L88CXOYRTW)](https://codecov.io/gl/kshib/wanda)\n\n## Installation / Update\n```\npip install wanda -U\n```\n\nOn android (with termux):\n```\npkg in libxml2 libxslt libjpeg-turbo\npip install wanda -U\n```\n\nFor issues installing pillow refer this [document](https://pillow.readthedocs.io/en/stable/installation.html)\n\n\n## Usage\n```\n# Set randomly\nwanda\n\n# Set from a keyword \nwanda -t mountain\n\n# Set from a source\nwanda -s wallhaven\n\n# Set from a source \nwanda -s wallhaven -t japan\n```\n`wanda -h` for more details\n\n## Notes\n- By default, the source is [unsplash](https://unsplash.com).\n- Some sources may have inapt images. Use them at your own risk.\n\n## Supported sources\n\n- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive.alice.al)\n- [500px](https://500px.com)\n- [artstation](https://artstation.com)\n- [imgur](https://imgur.com) via [rimgo](https://rimgo.pussthecat.org)\n- [earthview](https://earthview.withgoogle.com)\n- local\n- [picsum](https://picsum.photos)\n- [reddit](https://reddit.com)\n- [unsplash](https://unsplash.com)\n- [wallhaven](https://wallhaven.cc)\n\n## Build\n[python](https://www.python.org/downloads/) and [poetry](https://python-poetry.org/) are needed\n```\ngit clone https://github.com/ksh-b/wanda.git\ncd wanda\npoetry install\npoetry build\npoetry run wanda\n```\n\n## Uninstall\n```\npip uninstall wanda\n```\n\n## License\nMIT\n',
+    'long_description': '# wanda\nScript to set wallpaper using keyword or randomly\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e5aacd529ce04f3fb8c0f9ce6a3bdd9e)](https://www.codacy.com/gh/ksyko/wanda/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ksyko/wanda&amp;utm_campaign=Badge_Grade)[![PyPI](https://img.shields.io/pypi/v/wanda)](https://pypi.org/project/wanda/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/wanda)](https://pypistats.org/packages/wanda)\n[![PyPI - License](https://img.shields.io/pypi/l/wanda)](https://tldrlegal.com/license/mit-license)\n[![codecov](https://codecov.io/gl/kshib/wanda/branch/main/graph/badge.svg?token=L88CXOYRTW)](https://codecov.io/gl/kshib/wanda)\n\n## Installation / Update\n```\npip install wanda -U\n```\n\nOn android (with termux):\n```\npkg in libxml2 libxslt libjpeg-turbo\npip install wanda -U\n```\n\nFor issues installing pillow refer this [document](https://pillow.readthedocs.io/en/stable/installation.html)\n\n\n## Usage\n```\n# Set randomly\nwanda\n\n# Set from a keyword \nwanda -t mountain\n\n# Set from a source\nwanda -s wallhaven\n\n# Set from a source \nwanda -s wallhaven -t japan\n```\n`wanda -h` for more details\n\n## Notes\n- By default, the source is [unsplash](https://unsplash.com).\n- Some sources may have inapt images. Use them at your own risk.\n\n## Supported sources\n\n- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive-media.palanq.win)\n- [500px](https://500px.com)\n- [artstation](https://artstation.com)\n- [imgur](https://imgur.com) via [rimgo](https://rimgo.pussthecat.org)\n- [earthview](https://earthview.withgoogle.com)\n- local\n- [picsum](https://picsum.photos)\n- [reddit](https://reddit.com)\n- [unsplash](https://unsplash.com)\n- [wallhaven](https://wallhaven.cc)\n\n## Build\n[python](https://www.python.org/downloads) and [poetry](https://python-poetry.org) are needed\n```\ngit clone https://github.com/ksh-b/wanda.git\ncd wanda\npoetry install\npoetry build\npoetry run wanda\n```\n\n## Uninstall\n```\npip uninstall wanda\n```\n\n## License\nMIT\n',
     'author': 'kshib',
     'author_email': 'ksyko@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://gitlab.com/kshib/wanda',
+    'url': 'https://github.com/ksh-b/wanda',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `wanda-0.61.2/PKG-INFO` & `wanda-0.61.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wanda
-Version: 0.61.2
+Version: 0.61.3
 Summary: Set wallpapers with keywords or randomly
-Home-page: https://gitlab.com/kshib/wanda
+Home-page: https://github.com/ksh-b/wanda
 License: MIT
 Keywords: wallpaper,reddit,wallhaven,unsplash,termux
 Author: kshib
 Author-email: ksyko@pm.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,16 +19,16 @@
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: cloudscraper (>=1.2.60,<2.0.0)
 Requires-Dist: colorthief (>=0.2.1,<0.3.0)
 Requires-Dist: filetype (>=1.0.13,<2.0.0)
 Requires-Dist: lxml (>=4.9.0,<5.0.0)
 Requires-Dist: musicbrainzngs (>=0.7.1,<0.8.0)
 Requires-Dist: screeninfo (>=0.8,<0.9)
-Project-URL: Bug Tracker, https://gitlab.com/kshib/wanda/-/issues
-Project-URL: Repository, https://gitlab.com/kshib/wanda
+Project-URL: Bug Tracker, https://github.com/ksh-b/wanda/issues
+Project-URL: Repository, https://github.com/ksh-b/wanda
 Description-Content-Type: text/markdown
 
 # wanda
 Script to set wallpaper using keyword or randomly
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/e5aacd529ce04f3fb8c0f9ce6a3bdd9e)](https://www.codacy.com/gh/ksyko/wanda/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ksyko/wanda&amp;utm_campaign=Badge_Grade)[![PyPI](https://img.shields.io/pypi/v/wanda)](https://pypi.org/project/wanda/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/wanda)](https://pypistats.org/packages/wanda)
@@ -67,27 +67,27 @@
 
 ## Notes
 - By default, the source is [unsplash](https://unsplash.com).
 - Some sources may have inapt images. Use them at your own risk.
 
 ## Supported sources
 
-- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive.alice.al)
+- [4chan](https://boards.4chan.org) via [Rozen Arcana](https://archive-media.palanq.win)
 - [500px](https://500px.com)
 - [artstation](https://artstation.com)
 - [imgur](https://imgur.com) via [rimgo](https://rimgo.pussthecat.org)
 - [earthview](https://earthview.withgoogle.com)
 - local
 - [picsum](https://picsum.photos)
 - [reddit](https://reddit.com)
 - [unsplash](https://unsplash.com)
 - [wallhaven](https://wallhaven.cc)
 
 ## Build
-[python](https://www.python.org/downloads/) and [poetry](https://python-poetry.org/) are needed
+[python](https://www.python.org/downloads) and [poetry](https://python-poetry.org) are needed
 ```
 git clone https://github.com/ksh-b/wanda.git
 cd wanda
 poetry install
 poetry build
 poetry run wanda
 ```
```

