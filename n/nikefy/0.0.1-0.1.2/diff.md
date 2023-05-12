# Comparing `tmp/nikefy-0.0.1.tar.gz` & `tmp/nikefy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nikefy-0.0.1.tar", last modified: Sun Apr 16 22:17:43 2023, max compression
+gzip compressed data, was "nikefy-0.1.2.tar", last modified: Fri May 12 16:03:04 2023, max compression
```

## Comparing `nikefy-0.0.1.tar` & `nikefy-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-04-16 22:17:43.536224 nikefy-0.0.1/
--rw-r--r--   0 carlosraymundo   (501) staff       (20)      657 2023-04-16 21:35:04.000000 nikefy-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 carlosraymundo   (501) staff       (20)    11357 2023-04-12 05:35:33.000000 nikefy-0.0.1/LICENSE
--rw-r--r--   0 carlosraymundo   (501) staff       (20)      365 2023-04-16 21:35:04.000000 nikefy-0.0.1/MANIFEST.in
--rw-r--r--   0 carlosraymundo   (501) staff       (20)     2216 2023-04-12 05:35:33.000000 nikefy-0.0.1/Makefile
--rw-r--r--   0 carlosraymundo   (501) staff       (20)    17104 2023-04-16 22:17:43.532554 nikefy-0.0.1/PKG-INFO
--rw-r--r--   0 carlosraymundo   (501) staff       (20)     3282 2023-04-16 21:35:04.000000 nikefy-0.0.1/README.md
-drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-04-16 22:17:43.519573 nikefy-0.0.1/nikefy/
--rw-r--r--   0 carlosraymundo   (501) staff       (20)       56 2023-04-12 05:35:33.000000 nikefy-0.0.1/nikefy/__init__.py
--rw-r--r--   0 carlosraymundo   (501) staff       (20)      321 2023-04-16 21:35:04.000000 nikefy-0.0.1/nikefy/__main__.py
--rw-r--r--   0 carlosraymundo   (501) staff       (20)       22 2023-04-16 22:03:52.000000 nikefy-0.0.1/nikefy/_version.py
--rw-r--r--   0 carlosraymundo   (501) staff       (20)     1987 2023-04-16 21:35:04.000000 nikefy-0.0.1/nikefy/nikefy.py
-drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-04-16 22:17:43.528371 nikefy-0.0.1/nikefy/tests/
--rw-r--r--   0 carlosraymundo   (501) staff       (20)     4376 2023-04-16 21:35:04.000000 nikefy-0.0.1/nikefy/tests/test_all.py
-drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-04-16 22:17:43.527030 nikefy-0.0.1/nikefy.egg-info/
--rw-r--r--   0 carlosraymundo   (501) staff       (20)    17104 2023-04-16 22:17:43.000000 nikefy-0.0.1/nikefy.egg-info/PKG-INFO
--rw-r--r--   0 carlosraymundo   (501) staff       (20)      326 2023-04-16 22:17:43.000000 nikefy-0.0.1/nikefy.egg-info/SOURCES.txt
--rw-r--r--   0 carlosraymundo   (501) staff       (20)        1 2023-04-16 22:17:43.000000 nikefy-0.0.1/nikefy.egg-info/dependency_links.txt
--rw-r--r--   0 carlosraymundo   (501) staff       (20)      178 2023-04-16 22:17:43.000000 nikefy-0.0.1/nikefy.egg-info/requires.txt
--rw-r--r--   0 carlosraymundo   (501) staff       (20)        7 2023-04-16 22:17:43.000000 nikefy-0.0.1/nikefy.egg-info/top_level.txt
--rw-r--r--   0 carlosraymundo   (501) staff       (20)     2226 2023-04-16 21:35:04.000000 nikefy-0.0.1/pyproject.toml
--rw-r--r--   0 carlosraymundo   (501) staff       (20)       38 2023-04-16 22:17:43.536419 nikefy-0.0.1/setup.cfg
--rw-r--r--   0 carlosraymundo   (501) staff       (20)       39 2023-04-12 05:35:33.000000 nikefy-0.0.1/setup.py
+drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-05-12 16:03:04.216388 nikefy-0.1.2/
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      657 2023-05-11 17:45:56.000000 nikefy-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)    11357 2023-05-11 17:45:56.000000 nikefy-0.1.2/LICENSE
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      512 2023-05-11 17:45:56.000000 nikefy-0.1.2/MANIFEST.in
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     2537 2023-05-11 17:45:56.000000 nikefy-0.1.2/Makefile
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)    17522 2023-05-12 16:03:04.215694 nikefy-0.1.2/PKG-INFO
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     3700 2023-05-12 15:47:37.000000 nikefy-0.1.2/README.md
+drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-05-12 16:03:04.136692 nikefy-0.1.2/docs/
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      634 2023-05-11 17:45:56.000000 nikefy-0.1.2/docs/Makefile
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     2290 2023-05-11 17:45:56.000000 nikefy-0.1.2/docs/conf.py
+drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-05-12 16:03:04.140696 nikefy-0.1.2/docs/img/
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)  6199139 2023-05-11 17:45:56.000000 nikefy-0.1.2/docs/img/demo.gif
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     2449 2023-05-12 15:47:37.000000 nikefy-0.1.2/docs/index.md
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      800 2023-05-11 17:45:56.000000 nikefy-0.1.2/docs/make.bat
+drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-05-12 16:03:04.199312 nikefy-0.1.2/nikefy/
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)       56 2023-05-11 17:45:56.000000 nikefy-0.1.2/nikefy/__init__.py
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      494 2023-05-11 18:31:20.000000 nikefy-0.1.2/nikefy/__main__.py
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)       22 2023-05-12 15:47:37.000000 nikefy-0.1.2/nikefy/_version.py
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     3761 2023-05-12 15:47:37.000000 nikefy-0.1.2/nikefy/nikefy.py
+drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-05-12 16:03:04.212573 nikefy-0.1.2/nikefy/tests/
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     6132 2023-05-12 15:47:37.000000 nikefy-0.1.2/nikefy/tests/test_all.py
+drwxr-xr-x   0 carlosraymundo   (501) staff       (20)        0 2023-05-12 16:03:04.211928 nikefy-0.1.2/nikefy.egg-info/
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)    17522 2023-05-12 16:03:03.000000 nikefy-0.1.2/nikefy.egg-info/PKG-INFO
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      399 2023-05-12 16:03:04.000000 nikefy-0.1.2/nikefy.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)        1 2023-05-12 16:03:03.000000 nikefy-0.1.2/nikefy.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)      178 2023-05-12 16:03:03.000000 nikefy-0.1.2/nikefy.egg-info/requires.txt
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)        7 2023-05-12 16:03:03.000000 nikefy-0.1.2/nikefy.egg-info/top_level.txt
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)     2226 2023-05-12 15:57:19.000000 nikefy-0.1.2/pyproject.toml
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)       38 2023-05-12 16:03:04.216616 nikefy-0.1.2/setup.cfg
+-rw-r--r--   0 carlosraymundo   (501) staff       (20)       39 2023-05-11 17:52:23.000000 nikefy-0.1.2/setup.py
```

### Comparing `nikefy-0.0.1/CONTRIBUTING.md` & `nikefy-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nikefy-0.0.1/LICENSE` & `nikefy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nikefy-0.0.1/Makefile` & `nikefy-0.1.2/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+TMPREPO=/tmp/docs/nikefy
+
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
 	python -m pip install -e .[develop]
 
 build:  ## build the python library
@@ -81,14 +83,28 @@
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
 
+docs:
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages:
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/cgr2134/nikefy.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
 ############################################################################################
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
```

### Comparing `nikefy-0.0.1/PKG-INFO` & `nikefy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nikefy
-Version: 0.0.1
+Version: 0.1.2
 Summary: This python library acquires metadata from products in the Nike.com website
 Author-email: Carlos Raymundo <cgr2134@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,14 +224,15 @@
 Python library that amasses metadata from Nike.com website.
 
 ![GitHub](https://img.shields.io/badge/license-Apache--2.0-ffa500)
 ![GitHub](https://img.shields.io/github/issues/cgr2134/nikefy?color=aqua)
 [![Build Status](https://github.com/cgr2134/nikefy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/cgr2134/nikefy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/cgr2134/nikefy/branch/main/graph/badge.svg)](https://codecov.io/gh/cgr2134/nikefy)
 [![PyPI](https://img.shields.io/pypi/v/nikefy)](https://pypi.org/project/nikefy/)
+[![Documentation Status](https://readthedocs.org/projects/nikefy/badge/?version=latest)](https://nikefy.readthedocs.io/en/latest/?badge=latest)
 ## Overview
 
 Nikefy will allow users to quickly access metadata from Nike.com website such as products and prices data.
 
 * Create a database that easily queries shoes
 * Easily find sold out products
 * Find out most popular products via ratings
@@ -246,41 +247,46 @@
 ```python
 import nikefy as nf
 
 url = 'https://www.nike.com/w/mens-shoes-nik1zy7ok'
 nf.get_nike_products(url)
 nike_products = nf.get_nike_products(url)
 sorted_nike_products = sort_nike_products(nike_products, sort_order='asc')
+filtered_nike_products = filter_nike_products(nike_products, price_range=(100, 150), product_type="Men's Shoes")
 ```
 
 `get_nike_products()` gets Men's shoes products from Nike.com website and returns a dataframe
 
 `sort_nike_products()` sorts Men's shoes products based on price
 
+`filter_nike_products()` filters Men's shoes based on price range and type
+
 # Example
 Running the following code
 ```python
 import nikefy as nf
 
 url = 'https://www.nike.com/w/mens-shoes-nik1zy7ok'
 nike_products = nf.get_nike_products(url)
 print(nike_products)
-
 ```
 Outputs something like this to the console
 ```
                              Product Name Price  ...                                        Description                                        Product URL
 0                         Nike Pegasus 40  $130  ...  A springy ride for every run, the Peg’s famili...  https://www.nike.com/t/pegasus-40-mens-road-ru...
 1                     Nike Dunk Low Retro  $110  ...  Created for the hardwood but taken to the stre...  https://www.nike.com/t/dunk-low-retro-mens-sho...
 2                        Air Jordan 1 Low  $110  ...  Inspired by the original that debuted in 1985,...  https://www.nike.com/t/air-jordan-1-low-mens-s...
 3                        Air Jordan 1 Mid  $125  ...  Inspired by the original AJ1, this mid-top edi...  https://www.nike.com/t/air-jordan-1-mid-mens-s...
 4                      Nike Free Metcon 5  $120  ...  When your workouts wade into the nitty gritty,...  https://www.nike.com/t/free-metcon-5-mens-trai...
 5                          Cosmic Unity 3  $170  ...  Better for your game, designed with sustainabi...  https://www.nike.com/t/cosmic-unity-3-basketba...
 ```
 
+## Demo
+![](https://raw.githubusercontent.com/cgr2134/nikefy/main/docs/img/demo.gif)
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
```

### Comparing `nikefy-0.0.1/README.md` & `nikefy-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Python library that amasses metadata from Nike.com website.
 
 ![GitHub](https://img.shields.io/badge/license-Apache--2.0-ffa500)
 ![GitHub](https://img.shields.io/github/issues/cgr2134/nikefy?color=aqua)
 [![Build Status](https://github.com/cgr2134/nikefy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/cgr2134/nikefy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/cgr2134/nikefy/branch/main/graph/badge.svg)](https://codecov.io/gh/cgr2134/nikefy)
 [![PyPI](https://img.shields.io/pypi/v/nikefy)](https://pypi.org/project/nikefy/)
+[![Documentation Status](https://readthedocs.org/projects/nikefy/badge/?version=latest)](https://nikefy.readthedocs.io/en/latest/?badge=latest)
 ## Overview
 
 Nikefy will allow users to quickly access metadata from Nike.com website such as products and prices data.
 
 * Create a database that easily queries shoes
 * Easily find sold out products
 * Find out most popular products via ratings
@@ -24,41 +25,46 @@
 ```python
 import nikefy as nf
 
 url = 'https://www.nike.com/w/mens-shoes-nik1zy7ok'
 nf.get_nike_products(url)
 nike_products = nf.get_nike_products(url)
 sorted_nike_products = sort_nike_products(nike_products, sort_order='asc')
+filtered_nike_products = filter_nike_products(nike_products, price_range=(100, 150), product_type="Men's Shoes")
 ```
 
 `get_nike_products()` gets Men's shoes products from Nike.com website and returns a dataframe
 
 `sort_nike_products()` sorts Men's shoes products based on price
 
+`filter_nike_products()` filters Men's shoes based on price range and type
+
 # Example
 Running the following code
 ```python
 import nikefy as nf
 
 url = 'https://www.nike.com/w/mens-shoes-nik1zy7ok'
 nike_products = nf.get_nike_products(url)
 print(nike_products)
-
 ```
 Outputs something like this to the console
 ```
                              Product Name Price  ...                                        Description                                        Product URL
 0                         Nike Pegasus 40  $130  ...  A springy ride for every run, the Peg’s famili...  https://www.nike.com/t/pegasus-40-mens-road-ru...
 1                     Nike Dunk Low Retro  $110  ...  Created for the hardwood but taken to the stre...  https://www.nike.com/t/dunk-low-retro-mens-sho...
 2                        Air Jordan 1 Low  $110  ...  Inspired by the original that debuted in 1985,...  https://www.nike.com/t/air-jordan-1-low-mens-s...
 3                        Air Jordan 1 Mid  $125  ...  Inspired by the original AJ1, this mid-top edi...  https://www.nike.com/t/air-jordan-1-mid-mens-s...
 4                      Nike Free Metcon 5  $120  ...  When your workouts wade into the nitty gritty,...  https://www.nike.com/t/free-metcon-5-mens-trai...
 5                          Cosmic Unity 3  $170  ...  Better for your game, designed with sustainabi...  https://www.nike.com/t/cosmic-unity-3-basketba...
 ```
 
+## Demo
+![](https://raw.githubusercontent.com/cgr2134/nikefy/main/docs/img/demo.gif)
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
```

### Comparing `nikefy-0.0.1/nikefy.egg-info/PKG-INFO` & `nikefy-0.1.2/nikefy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nikefy
-Version: 0.0.1
+Version: 0.1.2
 Summary: This python library acquires metadata from products in the Nike.com website
 Author-email: Carlos Raymundo <cgr2134@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,14 +224,15 @@
 Python library that amasses metadata from Nike.com website.
 
 ![GitHub](https://img.shields.io/badge/license-Apache--2.0-ffa500)
 ![GitHub](https://img.shields.io/github/issues/cgr2134/nikefy?color=aqua)
 [![Build Status](https://github.com/cgr2134/nikefy/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/cgr2134/nikefy/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/cgr2134/nikefy/branch/main/graph/badge.svg)](https://codecov.io/gh/cgr2134/nikefy)
 [![PyPI](https://img.shields.io/pypi/v/nikefy)](https://pypi.org/project/nikefy/)
+[![Documentation Status](https://readthedocs.org/projects/nikefy/badge/?version=latest)](https://nikefy.readthedocs.io/en/latest/?badge=latest)
 ## Overview
 
 Nikefy will allow users to quickly access metadata from Nike.com website such as products and prices data.
 
 * Create a database that easily queries shoes
 * Easily find sold out products
 * Find out most popular products via ratings
@@ -246,41 +247,46 @@
 ```python
 import nikefy as nf
 
 url = 'https://www.nike.com/w/mens-shoes-nik1zy7ok'
 nf.get_nike_products(url)
 nike_products = nf.get_nike_products(url)
 sorted_nike_products = sort_nike_products(nike_products, sort_order='asc')
+filtered_nike_products = filter_nike_products(nike_products, price_range=(100, 150), product_type="Men's Shoes")
 ```
 
 `get_nike_products()` gets Men's shoes products from Nike.com website and returns a dataframe
 
 `sort_nike_products()` sorts Men's shoes products based on price
 
+`filter_nike_products()` filters Men's shoes based on price range and type
+
 # Example
 Running the following code
 ```python
 import nikefy as nf
 
 url = 'https://www.nike.com/w/mens-shoes-nik1zy7ok'
 nike_products = nf.get_nike_products(url)
 print(nike_products)
-
 ```
 Outputs something like this to the console
 ```
                              Product Name Price  ...                                        Description                                        Product URL
 0                         Nike Pegasus 40  $130  ...  A springy ride for every run, the Peg’s famili...  https://www.nike.com/t/pegasus-40-mens-road-ru...
 1                     Nike Dunk Low Retro  $110  ...  Created for the hardwood but taken to the stre...  https://www.nike.com/t/dunk-low-retro-mens-sho...
 2                        Air Jordan 1 Low  $110  ...  Inspired by the original that debuted in 1985,...  https://www.nike.com/t/air-jordan-1-low-mens-s...
 3                        Air Jordan 1 Mid  $125  ...  Inspired by the original AJ1, this mid-top edi...  https://www.nike.com/t/air-jordan-1-mid-mens-s...
 4                      Nike Free Metcon 5  $120  ...  When your workouts wade into the nitty gritty,...  https://www.nike.com/t/free-metcon-5-mens-trai...
 5                          Cosmic Unity 3  $170  ...  Better for your game, designed with sustainabi...  https://www.nike.com/t/cosmic-unity-3-basketba...
 ```
 
+## Demo
+![](https://raw.githubusercontent.com/cgr2134/nikefy/main/docs/img/demo.gif)
+
 ## Details
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
```

### Comparing `nikefy-0.0.1/pyproject.toml` & `nikefy-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "nikefy"
 authors = [{name = "Carlos Raymundo", email = "cgr2134@columbia.edu"}]
 description="This python library acquires metadata from products in the Nike.com website"
 readme = "README.md"
-version = "0.0.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = [
     "pandas",
     "beautifulsoup4"
 ]
```

