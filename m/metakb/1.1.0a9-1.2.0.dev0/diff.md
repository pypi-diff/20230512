# Comparing `tmp/metakb-1.1.0a9.tar.gz` & `tmp/metakb-1.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metakb-1.1.0a9.tar", last modified: Tue Jun 14 21:03:31 2022, max compression
+gzip compressed data, was "metakb-1.2.0.dev0.tar", last modified: Fri May 12 17:55:44 2023, max compression
```

## Comparing `metakb-1.1.0a9.tar` & `metakb-1.2.0.dev0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 21:03:31.281808 metakb-1.1.0a9/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-06-14 21:03:23.000000 metakb-1.1.0a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7313 2022-06-14 21:03:31.281808 metakb-1.1.0a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6523 2022-06-14 21:03:23.000000 metakb-1.1.0a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 21:03:31.281808 metakb-1.1.0a9/metakb/
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14037 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    21517 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/delta.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 21:03:31.281808 metakb-1.1.0a9/metakb/harvesters/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/harvesters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17841 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/harvesters/civic.py
--rw-r--r--   0 runner    (1001) docker     (121)     9070 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/harvesters/moa.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     7949 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (121)    52777 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/query.py
--rw-r--r--   0 runner    (1001) docker     (121)    45315 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 21:03:31.281808 metakb-1.1.0a9/metakb/transform/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6115 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    33474 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/transform/civic.py
--rw-r--r--   0 runner    (1001) docker     (121)    16898 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/transform/moa.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-14 21:03:23.000000 metakb-1.1.0a9/metakb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 21:03:31.281808 metakb-1.1.0a9/metakb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7313 2022-06-14 21:03:31.000000 metakb-1.1.0a9/metakb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-06-14 21:03:31.000000 metakb-1.1.0a9/metakb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 21:03:31.000000 metakb-1.1.0a9/metakb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 21:03:31.000000 metakb-1.1.0a9/metakb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-14 21:03:31.000000 metakb-1.1.0a9/metakb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-14 21:03:31.000000 metakb-1.1.0a9/metakb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-06-14 21:03:31.285808 metakb-1.1.0a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-14 21:03:23.000000 metakb-1.1.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.701232 metakb-1.2.0.dev0/metakb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.701232 metakb-1.2.0.dev0/metakb/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/moa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/oncokb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55043 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41922 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/metakb/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32381 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/moa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/oncokb.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.701232 metakb-1.2.0.dev0/metakb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/setup.py
```

### Comparing `metakb-1.1.0a9/LICENSE` & `metakb-1.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `metakb-1.1.0a9/PKG-INFO` & `metakb-1.2.0.dev0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: metakb
-Version: 1.1.0a9
-Summary: A search interface for cancer variant interpretations assembled by aggregating and harmonizing across multiple cancer variant interpretation knowledgebases.
-Home-page: https://github.com/cancervariants/metakb
-Author: VICC
-Author-email: help@cancervariants.org
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/vicc-metakb/badge/?version=latest)](https://vicc-metakb.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.org/cancervariants/metakb.svg?branch=main)](https://travis-ci.org/cancervariants/metakb) [![Coverage Status](https://coveralls.io/repos/github/cancervariants/metakb/badge.svg?branch=main)](https://coveralls.io/github/cancervariants/metakb?branch=main)
 
 # metakb
 
 The intent of the project is to leverage the collective knowledge of the disparate existing resources of the VICC to improve the comprehensiveness of clinical interpretation of genomic variation. An ongoing goal will be to provide and improve upon standards and guidelines by which other groups with clinical interpretation data may make it accessible and visible to the public. We have released a preprint discussing our initial harmonization effort and observed disparities in the structure and content of variant interpretations.
 
 ## Getting Started
@@ -46,82 +26,149 @@
 
 
 Once Pipenv is installed, clone the repo and install the package requirements into a Pipenv environment:
 
 ```sh
 git clone https://github.com/cancervariants/metakb
 cd metakb
-pipenv lock
-pipenv sync
+pipenv lock && pipenv sync
 ```
 
 If you intend to provide development support, install the development dependencies:
 
 ```sh
-pipenv lock --dev
-pipenv sync
+pipenv lock --dev && pipenv sync
 ```
 
 ### Setting up Neo4j
 
 The MetaKB uses [Neo4j](https://neo4j.com/) for its database backend. To run a local MetaKB instance, you'll need to run a Neo4j database instance as well. The easiest way to do this is from Neo4j Desktop.
 
 First, follow the [desktop setup instructions](https://neo4j.com/developer/neo4j-desktop) to download, install, and open Neo4j Desktop for the first time.
 
 Once you have opened Neo4j desktop, use the "New" button in the upper-left region of the window to create a new project. Within that project, click the "Add" button in the upper-right region of the window and select "Local DBMS". The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using "admin" by default). Click "Create". Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green "Start" button to start the database service.
 
-The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:5818"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
+The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:1409"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
 
 
 ### Setting up normalizers
 
 The MetaKB calls a number of normalizer libraries to transform resource data and resolve incoming search queries. These will be installed as part of the package requirements, but require additional setup.
 
-First, [download and install Amazon's DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html). Once installed, in a separate terminal instance, navigate to its source directory and run the following to start the database instance:
+First, [follow these instructions for deploying DynamoDB locally on your computer](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html). Once setup, in a separate terminal instance, navigate to its source directory and run the following to start the database instance:
 
 ```sh
 java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
 ```
 
 Next, navigate to the `site-packages` directory of your virtual environment. Assuming Pipenv is installed to your user directory, this should be something like:
 
 ```sh
-cd ~/.local/share/virtualenvs/metakb-<various characters>/python3.7/site-packages/  # replace <various characters>
+cd ~/.local/share/virtualenvs/metakb-<various characters>/lib/python<python-version>/site-packages/  # replace <various characters> and <python-version>
 ```
 
-Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation).
+Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation). When setting up the UTA database, [these](https://github.com/ga4gh/vrs-python/tree/main/docs/setup_help) docs may be helpful.
 
 
 The MetaKB can acquire all other needed normalizer data, except for that of [OMIM](https://www.omim.org/downloads), which must be manually placed:
 
 ```sh
 cd disease/  # starting from the site-packages dir of your virtual environment's Python instance
 mkdir -p data/omim
 cp ~/YOUR/PATH/TO/mimTitles.txt data/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
 ```
 
+### Environment Variables
+
+MetaKB relies on environment variables to set in order to work.
+
+* Always Required:
+  * `UTA_DB_URL`
+    * Used in Variation Normalizer which relies on UTA Tools
+    * Format: `driver://user:pass@host/database/schema`
+    * More info can be found [here](https://github.com/GenomicMedLab/uta-tools#connecting-to-the-database)
+
+    Example:
+
+    ```shell script
+    export UTA_DB_URL=postgresql://uta_admin:password@localhost:5432/uta/uta_20210129
+    ```
+
+  * `ONCOKB_API_TOKEN`
+    * Required to harvest OncoKB data. If you do not set this environment variable, you can set during the initialization of the OncoKBHarvester.
+    * Used to access OncoKB data via their REST API. See [here](https://www.oncokb.org/apiAccess) for more information on how to register an account and get an OncoKB API token.
+
+    Example for setting environment variable:
+    ```shell script
+    export ONCOKB_API_TOKEN={api_token}
+    ```
+
+    Example for setting during OncoKB Harvester initialization:
+    ```python
+    OncoKBHarvester(api_token={api_token})
+    ```
+
+* Required when using the `--load_normalizers_db` or `--force_load_normalizers_db` arguments in CLI commands
+  * `RXNORM_API_KEY`
+    * Used in Therapy Normalizer to retrieve RxNorm data
+    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `RxNORM_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
+
+    Example:
+
+    ```shell script
+    export RXNORM_API_KEY={rxnorm_api_key}
+    ```
+
+  * `DATAVERSE_API_KEY`
+    * Used in Therapy Normalizer to retrieve HemOnc data
+    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `DATAVERSE_API_KEY` environment variable to your API key.
+
+    Example:
+
+    ```shell script
+    export DATAVERSE_API_KEY={dataverse_api_key}
+    ```
+
+### Data files
+
+Some sources in MetaKB require user provided files to harvest data.
+
+* OncoKB
+  * In addition to setting the `ONCOKB_API_TOKEN` environment variable to harvest OncoKB data, you also need to provide a CSV file containing a header row with `hugo_symbol` and `protein_change`, associated rows containing protein variants you wish to harvest, and using a comma as the delimiter. The file will look something like:
+
+    ```csv
+    hugo_symbol,protein_change
+    BRAF,V600E
+    ...
+    ```
+  * This file will harvest OncoKB evidence based on the variants provided.
+
 ### Loading data
 
-Once Neo4j and DynamoDB instances are both active, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
+Once Neo4j and DynamoDB instances are both running, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
 
 In the MetaKB project root, run the following:
 
 ```sh
 pipenv shell
 python3 -m metakb.cli --db_url=bolt://localhost:7687 --db_username=neo4j --db_password=<neo4j-password-here> --load_normalizers_db
 ```
 
+For more information on the different CLI arguments, see the [CLI README](docs/cli/README.md).
+
 ### Starting the server
 
 Once data has been loaded successfully, use the following to start service on localhost port 8000:
 
 ```sh
 uvicorn metakb.main:app --reload
 ```
 
+Ensure that both the MetaKB Neo4j and Normalizers databases are running.
+
 Navigate to [http://localhost:8000/api/v2](http://localhost:8000/api/v2) in your browser to enter queries.
 
 ## Running tests
 
 ### Unit tests
 
 Explain how to run the automated tests for this system
@@ -164,9 +211,7 @@
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/cancervariants/metakb/tags).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-
```

### Comparing `metakb-1.1.0a9/metakb/__init__.py` & `metakb-1.2.0.dev0/metakb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 import logging
 from os import environ
 
 APP_ROOT = Path(__file__).resolve().parents[0]
 PROJECT_ROOT = Path(__file__).resolve().parents[1]
 
 if 'METAKB_NORM_EB_PROD' in environ:
-    environ['VARIATION_NORM_EB_PROD'] = "true"
-    environ['GENE_NORM_EB_PROD'] = "true"
-    environ['THERAPY_NORM_EB_PROD'] = "true"
-    environ['DISEASE_NORM_EB_PROD'] = "true"
     LOG_FN = "/tmp/metakb.log"
 else:
     LOG_FN = "metakb.log"
 
 logging.basicConfig(
     filename=LOG_FN,
     format='[%(asctime)s] - %(name)s - %(levelname)s : %(message)s')
```

### Comparing `metakb-1.1.0a9/metakb/cli.py` & `metakb-1.2.0.dev0/metakb/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 import asyncclick as click
 from disease.database import Database as DiseaseDatabase
 from disease.schemas import SourceName as DiseaseSources
 from disease.cli import CLI as DiseaseCLI
 from therapy.database import Database as TherapyDatabase
 from therapy.schemas import SourceName as TherapySources
 from therapy.cli import CLI as TherapyCLI
-from gene.database import Database as GeneDatabase
+from gene.database.dynamodb import DynamoDbDatabase as GeneDatabase
 from gene.schemas import SourceName as GeneSources
-from gene.cli import CLI as GeneCLI
+import gene.cli as GeneCLI
 import boto3
 from boto3.exceptions import ResourceLoadException
 from botocore.config import Config
 
 from metakb import APP_ROOT
 from metakb.database import Graph
 from metakb.schemas import SourceName
-from metakb.harvesters import Harvester, CIViCHarvester, MOAHarvester
-from metakb.transform import Transform, CIViCTransform, MOATransform
+from metakb.harvesters import Harvester, CIViCHarvester, MOAHarvester, OncoKBHarvester
+from metakb.transform import Transform, CIViCTransform, MOATransform, OncoKBTransform
 
 
 logger = logging.getLogger('metakb.cli')
 logger.setLevel(logging.DEBUG)
 
 
 def echo_info(msg: str):
@@ -108,21 +108,53 @@
         "--load_latest_s3_cdms",
         "-s",
         is_flag=True,
         default=False,
         required=False,
         help=("Clear MetaKB database, retrieve most recent data available "
               "from VICC S3 bucket, and load the database with retrieved "
-              "data. Exclusive with --load_latest_cdms and load_target_cdm.")
+              "data. Will not download OncoKB transformed data. Exclusive with"
+              " --load_latest_cdms and load_target_cdm.")
+    )
+    @click.option(
+        "--update_cached",
+        "-uc",
+        is_flag=True,
+        default=False,
+        required=False,
+        help=("`True` if civicpy cache should be updated. Note this will take serveral"
+              "minutes. `False` if local cache should be used")
+    )
+    @click.option(
+        "--update_from_remote",
+        "-ur",
+        is_flag=True,
+        default=False,
+        required=False,
+        help=("If set to `True`, civicpy.update_cache will first download the remote "
+              "cache designated by REMOTE_CACHE_URL, store it to LOCAL_CACHE_PATH, "
+              "and then load the downloaded cache into memory.")
+    )
+    @click.option(
+        "--oncokb_variants_by_protein_change_path",
+        "-k",
+        required=False,
+        type=click.Path(exists=True, dir_okay=False, readable=True, path_type=Path),
+        help=("Path to CSV file containing header row with `hugo_symbol` and "
+              "`protein_change` and associated rows containing protein variants you "
+              "wish to harvest using a comma as the delimiter. Not required if using "
+              "`--load_latest_cdms`, `--load_target_cdm`, or `--load_latest_s3_cdms`")
     )
     async def update_metakb_db(
         db_url: str, db_username: str, db_password: str,
         load_normalizers_db: bool, force_load_normalizers_db: bool,
         normalizers_db_url: str, load_latest_cdms: bool,
-        load_target_cdm: Optional[Path], load_latest_s3_cdms: bool
+        load_target_cdm: Optional[Path], load_latest_s3_cdms: bool,
+        update_cached: bool, update_from_remote: bool,
+        oncokb_variants_by_protein_change_path: Optional[Path]
     ):
         """Execute data harvest and transformation from resources and upload
         to graph datastore.
         """
         if sum([load_latest_cdms, bool(load_target_cdm),
                 load_latest_s3_cdms]) > 1:
             CLI()._help_msg("Error: Can only use one of `--load_latest_cdms`, "
@@ -137,15 +169,20 @@
                                  'DISEASE_NORM_DB_URL']:
                 environ[env_var_name] = normalizers_db_url
 
         if not any([load_latest_cdms, load_target_cdm, load_latest_s3_cdms]):
             if load_normalizers_db or force_load_normalizers_db:
                 CLI()._load_normalizers_db(force_load_normalizers_db)
 
-            CLI()._harvest_sources()
+            if not oncokb_variants_by_protein_change_path:
+                CLI()._help_msg(
+                    "Error: Must provide `--oncokb_variants_by_protein_change_path`")
+
+            CLI()._harvest_sources(update_cached, update_from_remote,
+                                   oncokb_variants_by_protein_change_path)
             await CLI()._transform_sources()
 
         # Load neo4j database
         start = timer()
         echo_info("Loading neo4j database...")
 
         g = Graph(uri=db_url, credentials=(db_username, db_password))
@@ -164,14 +201,15 @@
                     pattern = f"{src}_cdm_*.json"
                 globbed = (APP_ROOT / "data" / src / "transform").glob(pattern)
                 try:
                     path = sorted(globbed)[-1]
                 except IndexError:
                     raise FileNotFoundError(f"No valid transform file found "
                                             f"matching pattern: {pattern}")
+                click.echo(f"\tLoading {src} CDM from path...: {path}")
                 g.load_from_json(path)
         g.close()
         end = timer()
         echo_info(
             f"Successfully loaded neo4j database in {(end-start):.5f} s\n"
         )
 
@@ -221,28 +259,46 @@
         if newest_version is None:
             raise FileNotFoundError("Unable to locate files matching expected "
                                     "resource pattern in VICC s3 bucket")
         echo_info(f"Retrieved CDM files dated {newest_version}")
         return newest_version
 
     @staticmethod
-    def _harvest_sources() -> None:
+    def _harvest_sources(
+        update_cached, update_from_remote, oncokb_variants_by_protein_change_path
+    ) -> None:
         """Run harvesting procedure for all sources."""
         echo_info("Harvesting sources...")
         # TODO: Switch to using constant
         harvester_sources = {
-            'civic': CIViCHarvester,
-            'moa': MOAHarvester
+            SourceName.CIVIC.value: CIViCHarvester,
+            SourceName.MOA.value: MOAHarvester,
+            SourceName.ONCOKB.value: OncoKBHarvester
         }
         total_start = timer()
         for source_str, source_class in harvester_sources.items():
             echo_info(f"Harvesting {source_str}...")
             start = timer()
-            source: Harvester = source_class()
-            source_successful = source.harvest()
+
+            if source_str == SourceName.CIVIC and update_cached:
+                echo_info("(civicpy cache is also being updated)")
+                source: Harvester = source_class(
+                    update_cache=update_cached, update_from_remote=update_from_remote
+                )
+                # Use latest civic data
+                source_successful = source.harvest()
+            else:
+                source: Harvester = source_class()
+                if source_str == SourceName.ONCOKB:
+                    source_successful = source.harvest(
+                        oncokb_variants_by_protein_change_path
+                    )
+                else:
+                    source_successful = source.harvest()
+
             end = timer()
             if not source_successful:
                 echo_info(f'{source_str} harvest failed.')
                 click.get_current_context().exit()
             echo_info(
                 f"{source_str} harvest finished in {(end - start):.5f} s")
         total_end = timer()
@@ -253,16 +309,17 @@
 
     @staticmethod
     async def _transform_sources() -> None:
         """Run transformation procedure for all sources."""
         echo_info("Transforming harvested data to CDM...")
         # TODO: Switch to using constant
         transform_sources = {
-            'civic': CIViCTransform,
-            'moa': MOATransform
+            SourceName.CIVIC.value: CIViCTransform,
+            SourceName.MOA.value: MOATransform,
+            SourceName.ONCOKB.value: OncoKBTransform
         }
         total_start = timer()
         for src_str, src_name in transform_sources.items():
             echo_info(f"Transforming {src_str}...")
             start = timer()
             source: Transform = src_name()
             await source.transform()
```

### Comparing `metakb-1.1.0a9/metakb/database.py` & `metakb-1.2.0.dev0/metakb/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Graph database for storing harvested data."""
 from neo4j import GraphDatabase
 from neo4j.exceptions import ServiceUnavailable, ConstraintError
-from typing import Tuple, Dict, Set
+from typing import List, Tuple, Dict, Set
 import logging
 import json
 from pathlib import Path
 from os import environ
 import boto3
 import base64
 from botocore.exceptions import ClientError
@@ -175,15 +175,32 @@
                 tx.run(query, **method)
             except ServiceUnavailable as exception:
                 logging.error(f"Failed to add Method object\nQuery: "
                               f"{query}\nAssertionMethod: {method}")
                 raise exception
 
     @staticmethod
-    def _add_descriptor(tx, descriptor: Dict, added_ids: Set[str]):
+    def _update_fmt_key_extensions(fmt_keys: str, extensions: List[Dict],
+                                   obj: Dict) -> str:
+        """Return an updated formatted string containing extensions data.
+        Will mutate `obj` with extensions names + values.
+
+        :param str fmt_keys: Formatted String for use in Cypher query
+        :param List[Dict] extensions: List of extensions represented as dicts
+        :param Dict obj: The object to update with the extension name and value. This
+            will be mutated.
+        :return: Updated formatted string that includes extension data
+        """
+        for ext in extensions:
+            name = ext["name"]
+            obj[name] = json.dumps(ext["value"])
+            fmt_keys += f", {name}:${name}"
+        return fmt_keys
+
+    def _add_descriptor(self, tx, descriptor: Dict, added_ids: Set[str]):
         """Add gene, therapy, or disease descriptor object to DB.
         :param Dict descriptor: must contain a `value` field with `type`
             and `<type>_id` fields. `type` field must be one of
             {'TherapyDescriptor', 'DiseaseDescriptor', 'GeneDescriptor'}
         :param set added_ids: IDs found in statements
         """
         if descriptor['id'] not in added_ids:
@@ -199,22 +216,18 @@
             raise TypeError(f"Invalid Descriptor type: {descr_type}")
 
         value_id = f"{value_type.lower()}_id"
         descr_keys = _create_keys_string(descriptor, ('id', 'label',
                                                       'description', 'xrefs',
                                                       'alternate_labels'))
 
-        if descr_type == 'TherapyDescriptor':
-            # capture regulatory_approval field in therapy descriptor extensions
-            extensions = descriptor.get('extensions', [])
-            for ext in extensions:
-                name = ext['name']
-                if name == 'regulatory_approval':
-                    descriptor[name] = json.dumps(ext['value'])
-                    descr_keys += f", {name}:${name}"
+        extensions = descriptor.get('extensions', [])
+        if descr_type in {"TherapyDescriptor", "GeneDescriptor", "DiseaseDescriptor"}:
+            descr_keys = self._update_fmt_key_extensions(descr_keys, extensions,
+                                                         descriptor)
 
         query = f'''
         MERGE (descr:{descr_type} {{ {descr_keys} }})
         MERGE (value:{value_type} {{ id:${value_id} }})
         MERGE (descr) -[:DESCRIBES]-> (value)
         '''
         try:
@@ -396,26 +409,30 @@
         for node_id in [statement.get('therapy_descriptor'),
                         statement.get('variation_descriptor'),
                         statement.get('disease_descriptor'),
                         statement.get('method')]:
             if node_id:
                 added_ids.add(node_id)
 
-    @staticmethod
-    def _add_statement(tx, statement: Dict, added_ids: Set[str]):
+    def _add_statement(self, tx, statement: Dict, added_ids: Set[str]):
         """Add Statement object to DB.
         :param Dict statement: must include `id`, `variation_descriptor`,
             `disease_descriptor`, `method`, and `supported_by` fields as well
             as optional `therapy_descriptor` field
         :param set added_ids: IDs found in statements
         """
         formatted_keys = _create_keys_string(statement, ('id', 'description',
                                                          'direction',
                                                          'variation_origin',
                                                          'evidence_level'))
+
+        extensions = statement.get("extensions", [])
+        formatted_keys = self._update_fmt_key_extensions(formatted_keys, extensions,
+                                                         statement)
+
         match_line = ""
         rel_line = ""
         supported_by = statement.get('supported_by', [])
         if supported_by:
             for i, ev in enumerate(supported_by):
                 name = f"doc_{i}"
                 statement[name] = ev
@@ -453,15 +470,15 @@
             logging.error(f"Failed to add Evidence object\n"
                           f"Query: {query}\nEvidence: {statement}")
             raise exception
 
     @staticmethod
     def get_secret():
         """Get secrets for MetaKB instances."""
-        secret_name = environ['METAKB_DB_PASSWORD']
+        secret_name = environ['METAKB_DB_SECRET']
         region_name = "us-east-2"
 
         # Create a Secrets Manager client
         session = boto3.session.Session()
         client = session.client(
             service_name='secretsmanager',
             region_name=region_name
```

### Comparing `metakb-1.1.0a9/metakb/delta.py` & `metakb-1.2.0.dev0/metakb/delta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 """A module for computing deltas."""
-from metakb import APP_ROOT
 import json
 import logging
-from jsondiff import diff
 from datetime import date
-from metakb.harvesters import CIViCHarvester, MOAHarvester
+
+from jsondiff import diff
+from civicpy.__version__ import __version__ as civicpy_version
+
+from metakb import APP_ROOT
+from metakb.schemas import SourceName
+from metakb.version import __version__
+from metakb.harvesters import CIViCHarvester, MOAHarvester, OncoKBHarvester
+
+
 HARVESTER_CLASS = {
-    'civic': CIViCHarvester,
-    'moa': MOAHarvester
+    SourceName.CIVIC.value: CIViCHarvester,
+    SourceName.MOA.value: MOAHarvester,
+    SourceName.ONCOKB.value: OncoKBHarvester
 }
 logger = logging.getLogger('metakb.delta')
 logger.setLevel(logging.DEBUG)
 
 
 class Delta:
     """A class for computing deltas."""
@@ -53,23 +61,28 @@
             fn = f"{self._src}_harvester_{current_date}.json"
             HARVESTER_CLASS[self._src]().harvest(filename=fn)
             with open(f"{APP_ROOT}/data/{self._src}/harvester/{fn}", 'r') as f:
                 updated_json = json.load(f)
 
         delta = {
             '_meta': {
-                'metakb_version': '1.0.1',
+                'metakb_version': __version__,
                 'date_harvested': current_date
             }
         }
 
-        if self._src == 'civic':
-            delta['_meta']['civicpy_version'] = '1.1.2'
-        elif self._src == 'moa':
+        if self._src == SourceName.CIVIC:
+            delta['_meta']['civicpy_version'] = civicpy_version
+        elif self._src == SourceName.MOA:
             delta['_meta']['moa_api_version'] = '0.2'
+        elif self._src == SourceName.ONCOKB:
+            delta["_meta"]["oncokb_app_version"] = updated_json["appVersion"]["version"]
+            delta["_meta"]["oncokb_api_version"] = updated_json["apiVersion"]["version"]
+            delta["_meta"]["oncokb_data_version"] = \
+                updated_json["dataVersion"]["version"]
 
         for record_type in main_json.keys():
             delta[record_type] = {
                 'DELETE': [],
                 'INSERT': [],
                 'UPDATE': []
             }
```

### Comparing `metakb-1.1.0a9/metakb/harvesters/base.py` & `metakb-1.2.0.dev0/metakb/harvesters/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,31 @@
 from typing import List, Dict, Optional
 import json
 import logging
 from datetime import datetime as dt
 
 from metakb import APP_ROOT, DATE_FMT
 
-logger = logging.getLogger('metakb')
+logger = logging.getLogger("metakb.harvesters.base")
 logger.setLevel(logging.DEBUG)
 
 
 class Harvester:
     """A base class for content harvesters."""
 
-    def __init__(self):
-        """Initialize Harvester class."""
-        self.assertions = []
-
-    def harvest(self):
+    def harvest(self) -> bool:
         """
         Retrieve and store records from a resource. Records may be stored in
         any manner, but must be retrievable by :method:`iterate_records`.
 
         :return: `True` if operation was successful, `False` otherwise.
         :rtype: bool
         """
         raise NotImplementedError
 
-    def iter_assertions(self):
-        """
-        Yield all :class:`ClinSigAssertion` records for the resource.
-
-        :return: An iterator
-        :rtype: Iterator[:class:`ClinSigAssertion`]
-        """
-        for statement in self.assertions:
-            yield statement
-
     def create_json(self, items: Dict[str, List],
                     filename: Optional[str] = None) -> bool:
         """Create composite and individual JSON for harvested data.
 
         :param Dict items: item types keyed to Lists of values
         :param Optional[str] filename: custom filename for composite document
         :return: `True` if JSON creation was successful. `False` otherwise.
@@ -52,15 +38,15 @@
         today = dt.strftime(dt.today(), DATE_FMT)
         try:
             for item_type, item_list in items.items():
                 composite_dict[item_type] = item_list
 
                 with open(src_dir / f"{item_type}_{today}.json", "w+") as f:
                     f.write(json.dumps(item_list, indent=4))
-            if filename is None:
+            if not filename:
                 filename = f"{src}_harvester_{today}.json"
             with open(src_dir / filename, "w+") as f:
-                json.dump(composite_dict, f, indent=4)
+                f.write(json.dumps(composite_dict, indent=4))
         except Exception as e:
             logger.error(f"Unable to create json: {e}")
             return False
         return True
```

### Comparing `metakb-1.1.0a9/metakb/harvesters/moa.py` & `metakb-1.2.0.dev0/metakb/harvesters/moa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,90 @@
 """A module for the Molecular Oncology Almanac harvester"""
 import logging
-from typing import Optional
+from typing import Optional, List, Dict
 
 import requests
 import requests_cache
 
-from metakb.harvesters.base import Harvester
+from metakb.harvesters.base import Harvester  # noqa: I202
 
 
-logger = logging.getLogger('metakb.harvesters.moa')
+logger = logging.getLogger("metakb.harvesters.moa")
 logger.setLevel(logging.DEBUG)
 
 
 class MOAHarvester(Harvester):
     """A class for the Molecular Oncology Almanac harvester."""
 
-    def harvest(self, filename: Optional[str] = None):
+    def harvest(self, filename: Optional[str] = None) -> bool:
         """
         Retrieve and store sources, variants, and assertions
         records from MOAlmanac in composite and individual JSON files.
 
         :param Optional[str] filename: File name for composite json
         :return: True if successfully retreived, False otherwise
         :rtype: bool
         """
         try:
             assertion_resp = self._get_all_assertions()
             sources = self._harvest_sources(assertion_resp)
-            variants, variants_list = self._harvest_variants()
-            assertions = \
-                self._harvest_assertions(assertion_resp, variants_list)
+            variants, variants_list = self.harvest_variants()
+            assertions = self.harvest_assertions(assertion_resp, variants_list)
+            genes = self._harvest_genes()
             json_created = self.create_json(
                 {
                     "assertions": assertions,
                     "sources": sources,
-                    "variants": variants
+                    "variants": variants,
+                    "genes": genes
                 },
                 filename
             )
             if not json_created:
                 logger.error("MOAlmanac Harvester was not successful.")
                 return False
         except Exception as e:  # noqa: E722
-            logger.error(f'MOAlmanac Harvester was not successful: {e}')
+            logger.error(f"MOAlmanac Harvester was not successful: {e}")
             return False
         else:
-            logger.info('MOAlmanac Harvester was successful.')
+            logger.info("MOAlmanac Harvester was successful.")
             return True
 
-    def _harvest_sources(self, assertion_resp):
+    @staticmethod
+    def _harvest_genes() -> List[Dict]:
+        """Harvest all genes from MOAlamanc
+
+        :return: List of MOA gene records
+        """
+        genes = list()
+        with requests_cache.disabled():
+            r = requests.get("https://moalmanac.org/api/genes")
+            if r.status_code == 200:
+                genes = r.json()
+        return genes
+
+    def _harvest_sources(self, assertion_resp: List[Dict]) -> List[Dict]:
         """
         Harvest all MOA sources
 
-        :param: A list of MOA assertion records
+        :param List[Dict] assertion_resp: A list of MOA assertion records
         :return: A list of sources
         :rtype: list
         """
         sources = []
 
         for assertion in assertion_resp:
-            source = assertion['sources'][0]
+            source = assertion["sources"][0]
             s = self._source_item(source)
             if s not in sources:
                 sources.append(s)
 
         return sources
 
-    def _harvest_variants(self):
+    def harvest_variants(self) -> List[Dict]:
         """
         Harvest all MOA variants
 
         :return: A list of variants
         :rtype: list
         """
         variants_list = self._get_all_variants()
@@ -78,184 +92,186 @@
 
         for variant in variants_list:
             v = self._harvest_variant(variant)
             variants.append(v)
 
         return variants, variants_list
 
-    def _harvest_assertions(self, assertion_resp, variants_list):
+    def harvest_assertions(self, assertion_resp: List[Dict],
+                           variants_list: List[Dict]) -> List[Dict]:
         """
         Harvest all MOA assertions
 
-        :param: A list of MOA assertion records
-        :param: A list of MOA variant records
+        :param List[Dict] assertion_resp: A list of MOA assertion records
+        :param List[Dict] variants_list: A list of MOA variant records
         :return: A list of assertions
         :rtype: list
         """
         assertions = []
         for assertion in assertion_resp:
             a = self._harvest_assertion(assertion, variants_list)
             assertions.append(a)
 
         return assertions
 
-    def _get_all_assertions(self):
+    def _get_all_assertions(self) -> List[Dict]:
         """
         Return all assertion records.
 
         :return: All moa assertion records
         """
         with requests_cache.disabled():
-            r = requests.get('https://moalmanac.org/api/assertions')
+            r = requests.get("https://moalmanac.org/api/assertions")
             assertions = r.json()
 
         return assertions
 
-    def _get_all_variants(self):
+    def _get_all_variants(self) -> List[Dict]:
         """
         Return all variant records
 
         :return: All moa variant records
         """
         with requests_cache.disabled():
-            r = requests.get('https://moalmanac.org/api/features')
+            r = requests.get("https://moalmanac.org/api/features")
             variants = r.json()
 
         return variants
 
-    def _source_item(self, source):
+    def _source_item(self, source: Dict) -> Dict:
         """
         Harvest an individual MOA source of evidence
 
-        :param: source record of each assertion record
+        :param Dict source: source record of each assertion record
         :return: a dictionary containing MOA source of evidence data
         :rtype: dict
         """
         source_record = {
-            'id': source['source_id'],
-            'type': source['source_type'],
-            'doi': source['doi'],
-            'nct': source['nct'],
-            'pmid': source['pmid'],
-            'url': source['url'],
-            'citation': source['citation']
+            "id": source["source_id"],
+            "type": source["source_type"],
+            "doi": source["doi"],
+            "nct": source["nct"],
+            "pmid": source["pmid"],
+            "url": source["url"],
+            "citation": source["citation"]
         }
         return source_record
 
-    def _harvest_variant(self, variant):
-        """
-        Harvest an individual MOA variant record.
+    def _harvest_variant(self, variant: Dict) -> Dict:
+        """Harvest an individual MOA variant record.
 
-        :param: A MOA variant record
+        :param Dict variant: A MOA variant record
         :return: A dictionary containing MOA variant data
         :rtype: dict
         """
         variant_record = {
-            'id': variant['feature_id']
+            "id": variant["feature_id"]
         }
 
-        variant_record.update({k: v for k, v in variant['attributes'][0].items()})  # noqa: E501
+        variant_record.update({k: v for k, v in variant["attributes"][0].items()})  # noqa: E501
         variant_record.update(self._get_feature(variant_record))
 
         return variant_record
 
-    def _harvest_assertion(self, assertion, variants_list):
+    def _harvest_assertion(self, assertion: Dict, variants_list: List[Dict]) -> Dict:
         """
         Harvest an individual MOA assertion record
 
-        :param: a MOA assertion record
-        :param: a list of MOA variant records
+        :param Dict assertion: a MOA assertion record
+        :param List[Dict] variants_list: a list of MOA variant records
         :return: A dictionary containing MOA assertion data
         :rtype: dict
         """
         assertion_record = {
-            'id': assertion['assertion_id'],
-            'context': assertion['context'],
-            'description': assertion['description'],
-            'disease': {
-                'name': assertion['disease'],
-                'oncotree_code': assertion['oncotree_code'],
-                'oncotree_term': assertion['oncotree_term']
+            "id": assertion["assertion_id"],
+            "context": assertion["context"],
+            "description": assertion["description"],
+            "disease": {
+                "name": assertion["disease"],
+                "oncotree_code": assertion["oncotree_code"],
+                "oncotree_term": assertion["oncotree_term"]
             },
-            'therapy_name': assertion['therapy_name'],
-            'therapy_type': assertion['therapy_type'],
-            'clinical_significance': self._get_therapy(
-                assertion['therapy_resistance'],
-                assertion['therapy_sensitivity']),
-            'predictive_implication': assertion["predictive_implication"],
-            'favorable_prognosis': assertion['favorable_prognosis'],
-            'created_on': assertion['created_on'],
-            'last_updated': assertion['last_updated'],
-            'submitted_by': assertion['submitted_by'],
-            'validated': assertion['validated'],
-            'source_ids': assertion['sources'][0]['source_id']
+            "therapy_name": assertion["therapy_name"],
+            "therapy_type": assertion["therapy_type"],
+            "clinical_significance": self._get_therapy(
+                assertion["therapy_resistance"],
+                assertion["therapy_sensitivity"]),
+            "predictive_implication": assertion["predictive_implication"],
+            "favorable_prognosis": assertion["favorable_prognosis"],
+            "created_on": assertion["created_on"],
+            "last_updated": assertion["last_updated"],
+            "submitted_by": assertion["submitted_by"],
+            "validated": assertion["validated"],
+            "source_ids": assertion["sources"][0]["source_id"]
         }
 
         for v in variants_list:
-            if v['attributes'][0] == assertion['features'][0]['attributes'][0]:
-                assertion_record.update({'variant': self._harvest_variant(v)})
+            if v["attributes"][0] == assertion["features"][0]["attributes"][0]:
+                assertion_record.update({"variant": self._harvest_variant(v)})
 
         return assertion_record
 
-    def _get_therapy(self, resistance, sensitivity):
+    def _get_therapy(self, resistance: bool, sensitivity: bool) -> Optional[str]:
         """
         Get therapy response data.
 
-        :param: therapy_resistance
-        :param: therapy_sensitivity
+        :param bool resistance: `True` if Therapy Resistance.
+            `False` if not Therapy Resistance
+        :param bool sensitivity: `True` if Therapy Sensitivity.
+            `False` if not Therapy Sensitivity
         :return: whether the therapy response is resistance or sensitivity
         :rtype: str
         """
         if resistance:
             return "resistance"
         elif sensitivity:
             return "sensitivity"
         else:
-            return
+            return None
 
-    def _get_feature(self, v):
+    def _get_feature(self, v: Dict) -> Dict:
         """
         Get feature name from the harvested variants
 
-        :param: harvested MOA variant
+        :param Dict v: harvested MOA variant
         :return: feature name same format as displayed in moalmanac.org
         :rtype: dict
         """
-        feature_type = v['feature_type']
-        if feature_type == 'rearrangement':
-            feature = '{}{}{}'.format(v['gene1'],
-                                      f"--{v['gene2']}" if v['gene2'] else '',
+        feature_type = v["feature_type"]
+        if feature_type == "rearrangement":
+            feature = "{}{}{}".format(v["gene1"],
+                                      f"--{v['gene2']}" if v["gene2"] else "",
                                       f" {v['rearrangement_type']}"
-                                      if v['rearrangement_type'] else '')
-        elif feature_type == 'somatic_variant':
-            feature = '{}{}{}'.format(v['gene'],
+                                      if v["rearrangement_type"] else "")
+        elif feature_type == "somatic_variant":
+            feature = "{}{}{}".format(v["gene"],
                                       f" {v['protein_change']}"
-                                      if v['protein_change'] else '',
+                                      if v["protein_change"] else "",
                                       f" ({v['variant_annotation']})"
-                                      if v['variant_annotation'] else '')
-        elif feature_type == 'germline_variant':
-            feature = '{}{}'.format(v['gene'], ' (Pathogenic)'
-                                    if v['pathogenic'] == '1.0' else '')
-        elif feature_type == 'copy_number':
-            feature = '{} {}'.format(v['gene'], v['direction'])
-        elif feature_type == 'microsatellite_stability':
-            feature = '{}'.format(v.get('status'))
-        elif feature_type == 'mutational_signature':
-            csn = v['cosmic_signature_number']
-            feature = 'COSMIC Signature {}'.format(csn)
-        elif feature_type == 'mutational_burden':
-            clss = v['classification']
-            min_mut = v['minimum_mutations']
-            mut_per_mb = v['mutations_per_mb']
-            feature = '{}{}'.format(clss,
+                                      if v["variant_annotation"] else "")
+        elif feature_type == "germline_variant":
+            feature = "{}{}".format(v["gene"], " (Pathogenic)"
+                                    if v["pathogenic"] == "1.0" else "")
+        elif feature_type == "copy_number":
+            feature = "{} {}".format(v["gene"], v["direction"])
+        elif feature_type == "microsatellite_stability":
+            feature = "{}".format(v.get("status"))
+        elif feature_type == "mutational_signature":
+            csn = v["cosmic_signature_number"]
+            feature = "COSMIC Signature {}".format(csn)
+        elif feature_type == "mutational_burden":
+            clss = v["classification"]
+            min_mut = v["minimum_mutations"]
+            mut_per_mb = v["mutations_per_mb"]
+            feature = "{}{}".format(clss,
                                     f" (>= {min_mut} mutations)" if min_mut
                                     else (f" (>= {mut_per_mb} mutations/Mb)"
-                                          if mut_per_mb else ''))
-        elif feature_type == 'neoantigen_burden':
-            feature = '{}'.format(v['classification'])
-        elif feature_type == 'knockdown' or feature_type == 'silencing':
-            feature = '{}{}'.format(v['gene'], f" ({v['technique']})"
-                                    if v['technique'] else '')
+                                          if mut_per_mb else ""))
+        elif feature_type == "neoantigen_burden":
+            feature = "{}".format(v["classification"])
+        elif feature_type == "knockdown" or feature_type == "silencing":
+            feature = "{}{}".format(v["gene"], f" ({v['technique']})"
+                                    if v["technique"] else "")
         else:
-            feature = '{}'.format(v['event'])
+            feature = "{}".format(v["event"])
 
-        return {'feature': feature.strip()}
+        return {"feature": feature.strip()}
```

### Comparing `metakb-1.1.0a9/metakb/main.py` & `metakb-1.2.0.dev0/metakb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Main application for FastAPI."""
-from fastapi import FastAPI, Query
+from fastapi import FastAPI, Query, Path
 from fastapi.openapi.utils import get_openapi
 from metakb.query import QueryHandler
 from metakb.version import __version__
 from metakb.schemas import SearchService, SearchIDService, \
     SearchStatementsService
 from typing import Optional
 
@@ -104,10 +104,10 @@
 
 @app.get('/api/v2/search/{id}',
          summary=id_query_desc,
          response_description=search_response_description,
          response_model=SearchIDService,
          description=id_search_description,
          response_model_exclude_none=True)
-async def search_by_id(id: str = Query(None, description=id_description)):
+async def search_by_id(id: str = Path(description=id_description)):
     """Search by ID endpoint"""
     return query.search_by_id(id)
```

### Comparing `metakb-1.1.0a9/metakb/normalizers.py` & `metakb-1.2.0.dev0/metakb/normalizers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,105 @@
 """Module for VICC normalizers."""
-from typing import Optional, Tuple
+import logging
+from typing import List, Optional, Tuple
 
-from ga4gh.vrsatile.pydantic.vrs_models import VRSTypes
 from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor, Extension
 from variation.query import QueryHandler as VariationQueryHandler
 from therapy.query import QueryHandler as TherapyQueryHandler
 from therapy.schemas import NormalizationService as NormalizedTherapy, ApprovalRating
 from disease.query import QueryHandler as DiseaseQueryHandler
 from disease.schemas import NormalizationService as NormalizedDisease
+from gene.database.dynamodb import DynamoDbDatabase
 from gene.query import QueryHandler as GeneQueryHandler
 from gene.schemas import NormalizeService as NormalizedGene
-import logging
 
-logger = logging.getLogger('metakb.normalizers')
-logger.setLevel(logging.DEBUG)
+
+logger = logging.getLogger(__name__)
 
 
 class VICCNormalizers:
     """A class for normalizing terms using VICC normalizers."""
 
-    def __init__(self):
-        """Initialize the VICC Normalizers."""
-        self.gene_query_handler = GeneQueryHandler()
-        self.variation_normalizer = VariationQueryHandler()
-        self.disease_query_handler = DiseaseQueryHandler()
-        self.therapy_query_handler = TherapyQueryHandler()
-
-    async def normalize_variation(self,
-                                  queries) -> Optional[VariationDescriptor]:
+    def __init__(
+        self, gene_query_handler: Optional[GeneQueryHandler] = None,
+        variation_query_handler: Optional[VariationQueryHandler] = None,
+        disease_query_handler: Optional[DiseaseQueryHandler] = None,
+        therapy_query_handler: Optional[TherapyQueryHandler] = None
+    ) -> None:
+        """Initialize the VICC Normalizers.
+
+        :param gene_query_handler: Gene QueryHandler instance
+        :param variation_query_handler: Variation QueryHandler instance
+        :param disease_query_handler: Disease QueryHandler instance
+        :param therapy_query_handler: Therapy QueryHandler instance
+        """
+        self.disease_query_handler = disease_query_handler or DiseaseQueryHandler()
+        self.therapy_query_handler = therapy_query_handler or TherapyQueryHandler()
+        self.gene_query_handler = (gene_query_handler or GeneQueryHandler(DynamoDbDatabase()))  # noqa: E501
+
+        if variation_query_handler:
+            self.variation_query_handler = variation_query_handler
+        else:
+            self.variation_query_handler = VariationQueryHandler(
+                gene_query_handler=self.gene_query_handler
+            )
+
+    async def normalize_variation(
+        self, queries: List[str]
+    ) -> Optional[VariationDescriptor]:
         """Normalize variation queries.
 
-        :param list queries: Possible query strings to try to normalize
+        :param queries: Possible query strings to try to normalize
             which are used in the event that a MANE transcript cannot be found
         :return: A normalized variation
         """
         for query in queries:
             if not query:
                 continue
-
             try:
-                variation_norm_resp = \
-                    await self.variation_normalizer.normalize(query)
-                if variation_norm_resp:
-                    if variation_norm_resp.variation.type != VRSTypes.TEXT:
-                        return variation_norm_resp
+                variation_norm_resp = await self.variation_query_handler.normalize_handler.normalize(query)  # noqa: E501
+                if variation_norm_resp and variation_norm_resp.variation_descriptor:
+                    return variation_norm_resp.variation_descriptor
             except Exception as e:  # noqa: E722
-                logger.warning(f"Variation Normalizer raised an exception "
-                               f"using query {query}: {e}")
+                logger.warning(f"Variation Normalizer raised an exception using query"
+                               f" {query}: {e}")
         return None
 
-    def normalize_gene(self, queries)\
-            -> Tuple[Optional[NormalizedGene], Optional[str]]:
+    def normalize_gene(
+        self, queries: List[str]
+    ) -> Tuple[Optional[NormalizedGene], Optional[str]]:
         """Normalize gene queries
 
-        :param list queries: Gene queries to normalize
-        :return: The highest matched gene's normalized response and ID
+        :param queries: Gene queries to normalize
+        :return: The highest matched gene's normalized response and ID, if successful
         """
         gene_norm_resp = None
         normalized_gene_id = None
         highest_match = 0
         for query_str in queries:
             if not query_str:
                 continue
 
             try:
                 gene_norm_resp = self.gene_query_handler.normalize(query_str)
             except Exception as e:
-                logger.warning(f"Gene Normalizer raised an exception using "
-                               f"query {query_str}: {e}")
+                logger.warning(f"Gene Normalizer raised an exception using query "
+                               f"{query_str}: {e}")
             else:
                 if gene_norm_resp.match_type > highest_match:
                     highest_match = gene_norm_resp.match_type
                     normalized_gene_id = \
                         gene_norm_resp.gene_descriptor.gene_id
                     if highest_match == 100:
                         break
         return gene_norm_resp, normalized_gene_id
 
-    def normalize_disease(self, queries)\
-            -> Tuple[Optional[NormalizedDisease], Optional[str]]:
+    def normalize_disease(
+        self, queries: List[str]
+    ) -> Tuple[Optional[NormalizedDisease], Optional[str]]:
         """Normalize disease queries
 
         :param list queries: Disease queries to normalize
         :return: The highest matched disease's normalized response and ID
         """
         highest_match = 0
         normalized_disease_id = None
@@ -91,27 +108,28 @@
         for query in queries:
             if not query:
                 continue
 
             try:
                 disease_norm_resp = self.disease_query_handler.normalize(query)
             except Exception as e:
-                logger.warning(f"Disease Normalizer raised an exception using "
-                               f"query {query}: {e}")
+                logger.warning(f"Disease Normalizer raised an exception using query "
+                               f"{query}: {e}")
             else:
                 if disease_norm_resp.match_type > highest_match:
                     highest_match = disease_norm_resp.match_type
                     normalized_disease_id = \
                         disease_norm_resp.disease_descriptor.disease_id
                     if highest_match == 100:
                         break
         return disease_norm_resp, normalized_disease_id
 
-    def normalize_therapy(self, queries)\
-            -> Tuple[Optional[NormalizedTherapy], Optional[str]]:
+    def normalize_therapy(
+        self, queries: List[str]
+    ) -> Tuple[Optional[NormalizedTherapy], Optional[str]]:
         """Normalize therapy queries
 
         :param list queries: Therapy queries to normalize
         :return: The highest matched therapy's normalized response and ID
         """
         highest_match = 0
         normalized_therapy_id = None
```

### Comparing `metakb-1.1.0a9/metakb/query.py` & `metakb-1.2.0.dev0/metakb/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,36 @@
 import logging
 import json
 from json.decoder import JSONDecodeError
 from urllib.parse import quote
 
 from ga4gh.vrsatile.pydantic.vrsatile_models import Extension, Expression
 from neo4j.graph import Node
-from neo4j.data import Record
-from neo4j.work.transaction import Transaction
-from neo4j.work.simple import Session
+from neo4j import Transaction, Session, Record
 
 from metakb.database import Graph
 from metakb.normalizers import VICCNormalizers
-from metakb.schemas import SearchService, StatementResponse, \
+from metakb.schemas import SearchService, SourceName, StatementResponse, \
     TherapeuticResponseProposition, VariationDescriptor, \
     ValueObjectDescriptor, GeneDescriptor, Method, \
     Document, SearchIDService, DiagnosticProposition, PrognosticProposition, \
     SearchStatementsService, NestedStatementResponse, PropositionType, \
     Proposition, ServiceMeta, Predicate
+from metakb.transform.oncokb import GENE_EXT_CONVERSIONS, VARIATION_EXT_CONVERSIONS, \
+    DISEASE_EXT_CONVERSIONS
 
 logger = logging.getLogger("metakb.query")
 logger.setLevel(logging.DEBUG)
 
 
+ONCOKB_GENE_EXT_NAMES = [i[1] for i in GENE_EXT_CONVERSIONS]
+ONCOKB_VARIATION_EXT_NAMES = [i[1] for i in VARIATION_EXT_CONVERSIONS]
+ONCOKB_DISEASE_EXT_NAMES = [i[1] for i in DISEASE_EXT_CONVERSIONS]
+
+
 class QueryHandler:
     """Class for handling queries."""
 
     def __init__(self, uri: str = "",
                  creds: Tuple[str, str] = ("", ""),
                  normalizers: VICCNormalizers = VICCNormalizers()) -> None:
         """Initialize neo4j driver and the VICC normalizers.
@@ -677,15 +682,14 @@
             "gene_context": None,
             "molecule_context": variation_descriptor.get("molecule_context"),
             "structural_type": variation_descriptor.get("structural_type"),
             "vrs_ref_allele_seq": variation_descriptor.get("vrs_ref_allele_seq"),  # noqa: E501
             "expressions": [],
             "xrefs": variation_descriptor.get("xrefs"),
             "alternate_labels": variation_descriptor.get("alternate_labels"),
-            "extensions": []
         }
 
         # Get Gene Descriptor / gene context
         with self.driver.session() as session:
             gene_descriptor = session.read_transaction(
                 self._get_variation_descriptors_gene, vd_params["id"]
             )
@@ -719,20 +723,21 @@
                             syntax=f"hgvs.{key.split('_')[-1]}",
                             value=value
                         ).dict()
                     )
         if not vd_params["expressions"]:
             del vd_params["expressions"]
 
+        extensions = []
         # Get Variation Descriptor Extensions
         if vd_params["id"].startswith("civic.vid"):
             for field in ["civic_representative_coordinate",
                           "civic_actionability_score"]:
                 if field in keys:
-                    vd_params["extensions"].append(
+                    extensions.append(
                         Extension(
                             name=field,
                             value=json.loads(variation_descriptor.get(field))
                         ).dict()
                     )
             with self.driver.session() as session:
                 variant_group = session.read_transaction(
@@ -748,24 +753,36 @@
                             "description": variant_group.get("description"),
                             "type": "variant_group"
                         }]
                     ).dict()
                     for v in vg["value"]:
                         if not v["description"]:
                             del v["description"]
-                    vd_params["extensions"].append(vg)
+                    extensions.append(vg)
         elif vd_params["id"].startswith("moa.variant"):
             for field in ["moa_representative_coordinate", "moa_rsid"]:
                 if field in keys:
-                    vd_params["extensions"].append(
+                    extensions.append(
                         Extension(
                             name=field,
                             value=json.loads(variation_descriptor.get(field))
                         ).dict()
                     )
+        elif vd_params["id"].startswith("oncokb.variant"):
+            for field in ONCOKB_VARIATION_EXT_NAMES:
+                if field in keys:
+                    extensions.append(
+                        Extension(
+                            name=field,
+                            value=json.loads(variation_descriptor[field])
+                        ).dict()
+                    )
+
+        if extensions:
+            vd_params["extensions"] = extensions
 
         with self.driver.session() as session:
             value_object = session.read_transaction(
                 self._find_descriptor_value_object, vd_params["id"]
             )
             vd_params["variation_id"] = value_object.get("id")
             vd_params["variation"] = json.loads(value_object["variation"])
@@ -813,17 +830,32 @@
         gd_params = {
             "id": gene_descriptor.get("id"),
             "type": "GeneDescriptor",
             "label": gene_descriptor.get("label"),
             "description": gene_descriptor.get("description"),
             "gene_id": gene_value_object.get("id"),
             "alternate_labels": gene_descriptor.get("alternate_labels"),
-            "xrefs": gene_descriptor.get("xrefs")
+            "xrefs": gene_descriptor.get("xrefs"),
         }
 
+        extensions = []
+        if gd_params["id"].startswith(SourceName.ONCOKB):
+            keys = gene_descriptor.keys()
+            for field in ONCOKB_GENE_EXT_NAMES:
+                if field in keys:
+                    extensions.append(
+                        Extension(
+                            name=field,
+                            value=json.loads(gene_descriptor[field])
+                        ).dict()
+                    )
+
+            if extensions:
+                gd_params["extensions"] = extensions
+
         return GeneDescriptor(**gd_params)
 
     def _get_therapy_descriptor(
         self, therapy_descriptor: Node
     ) -> ValueObjectDescriptor:
         """Get therapy descriptor.
 
@@ -864,16 +896,31 @@
         :return: Value Object Descriptor for disease
         """
         dd_params = {
             "id": disease_descriptor.get("id"),
             "type": "DiseaseDescriptor",
             "label": disease_descriptor.get("label"),
             "disease_id": None,
-            "xrefs": disease_descriptor.get("xrefs")
+            "xrefs": disease_descriptor.get("xrefs"),
+            "extensions": []
         }
+        keys = disease_descriptor.keys()
+
+        if dd_params["id"].startswith(SourceName.ONCOKB):
+            for field in ONCOKB_DISEASE_EXT_NAMES:
+                if field in keys:
+                    dd_params["extensions"].append(
+                        Extension(
+                            name=field,
+                            value=json.loads(disease_descriptor[field])
+                        ).dict()
+                    )
+
+        if not dd_params["extensions"]:
+            del dd_params["extensions"]
 
         with self.driver.session() as session:
             value_object = session.read_transaction(
                 self._find_descriptor_value_object, dd_params["id"]
             )
             dd_params["disease_id"] = value_object.get("id")
 
@@ -1244,26 +1291,38 @@
         with self.driver.session() as session:
             statement_id = s.get("id")
             response = session.read_transaction(
                 self._find_and_return_statement_response, statement_id)
             se_list = session.read_transaction(
                 self._find_and_return_supported_by, statement_id)
 
+            extensions = []
+            # Right now, only OncoKB has Statement extensions
+            if statement_id.startswith(SourceName.ONCOKB):
+                if "onckb_fda_level" in s.keys():
+                    extensions.append(
+                        Extension(
+                            name="onckb_fda_level",
+                            value=json.loads(s["onckb_fda_level"])
+                        ).dict()
+                    )
+
             statement = StatementResponse(
                 id=statement_id,
                 description=s.get("description"),
                 direction=s.get("direction"),
                 evidence_level=s.get("evidence_level"),
                 variation_origin=s.get("variation_origin"),
                 proposition=response["p_id"],
                 variation_descriptor=response["vid"],
                 therapy_descriptor=response["tid"] if "tid" in response.keys() else None,  # noqa: E501
                 disease_descriptor=response["did"],
                 method=response["m"]["id"],
-                supported_by=[se["id"] for se in se_list]
+                supported_by=[se["id"] for se in se_list],
+                extensions=extensions if extensions else None
             ).dict(exclude_none=True)
             return statement
 
     @staticmethod
     def _get_documents(tx: Transaction, **parameters) -> List[Node]:
         """Get Document nodes matching provided parameters. Provide as callback
         to Neo4j session methods.
```

### Comparing `metakb-1.1.0a9/metakb/schemas.py` & `metakb-1.2.0.dev0/metakb/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Common data model"""
 from enum import Enum, IntEnum
 from typing import List, Optional, Union, Dict, Any, Type
 
 from ga4gh.vrsatile.pydantic.vrs_models import CURIE
 from ga4gh.vrsatile.pydantic.vrsatile_models import ValueObjectDescriptor, \
-    GeneDescriptor, VariationDescriptor
+    GeneDescriptor, VariationDescriptor, Extension
 from pydantic import BaseModel
 from pydantic.types import StrictBool
 
-from metakb.version import __version__, LAST_UPDATED
+from metakb.version import __version__
 
 
 class SourceName(str, Enum):
-    """Resources we import directly."""
+    """Resources we import directly. Values are all lowercase."""
 
-    CIVIC = 'civic'
-    MOA = 'moa'
+    CIVIC = "civic"
+    MOA = "moa"
+    ONCOKB = "oncokb"
 
 
 class XrefSystem(str, Enum):
     """Define constraints for System in xrefs."""
 
     CLINVAR = 'clinvar'
     CLINGEN = 'caid'
@@ -176,32 +177,34 @@
 class MethodID(IntEnum):
     """Create AssertionMethod id constants for harvested sources."""
 
     CIVIC_EID_SOP = 1
     CIVIC_AID_AMP_ASCO_CAP = 2
     CIVIC_AID_ACMG = 3
     MOA_ASSERTION_BIORXIV = 4
+    ONCOKB_SOP = 5
 
 
 class Statement(BaseModel):
     """Define Statement model."""
 
     id: CURIE
     type = 'Statement'
-    description: str
+    description: Optional[str]
     direction: Optional[Direction]
     evidence_level: CURIE
     proposition: CURIE
     variation_origin: Optional[VariationOrigin]
     variation_descriptor: CURIE
     therapy_descriptor: Optional[CURIE]
     disease_descriptor: CURIE
     method: CURIE
     supported_by: List[CURIE]
     # contribution: str  TODO: After metakb first pass
+    extensions: Optional[List[Extension]]
 
 
 class Document(BaseModel):
     """Define model for Source."""
 
     id: CURIE
     document_id: Optional[CURIE]
@@ -263,24 +266,25 @@
 
 
 class StatementResponse(BaseModel):
     """Define Statement Response for Search Endpoint."""
 
     id: CURIE
     type = 'Statement'
-    description: str
+    description: Optional[str]
     direction: Optional[Direction]
     evidence_level: CURIE
     variation_origin: Optional[VariationOrigin]
     proposition: CURIE
     variation_descriptor: CURIE
     therapy_descriptor: Optional[CURIE]
     disease_descriptor: CURIE
     method: CURIE
     supported_by: List[CURIE]
+    extensions: Optional[List[Extension]]
 
     class Config:
         """Configure examples."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
                          model: Type['StatementResponse']) -> None:
@@ -308,26 +312,27 @@
 
 
 class NestedStatementResponse(BaseModel):
     """Define Statement Response for Search Endpoint."""
 
     id: CURIE
     type = 'Statement'
-    description: str
+    description: Optional[str]
     direction: Optional[Direction]
     evidence_level: CURIE
     variation_origin: Optional[VariationOrigin]
     proposition: Union[TherapeuticResponseProposition,
                        PrognosticProposition,
                        DiagnosticProposition]
     variation_descriptor: VariationDescriptor
     therapy_descriptor: Optional[ValueObjectDescriptor]
     disease_descriptor: ValueObjectDescriptor
     method: Method
     supported_by: List[Union[Document, CURIE]]
+    extensions: Optional[List[Extension]]
 
     class Config:
         """Configure examples."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
                          model: Type['NestedStatementResponse']) -> None:
@@ -350,15 +355,14 @@
                     "object_qualifier": "ncit:C2926",
                     "object": "rxcui:1430438"
                 },
                 "variation_descriptor": {
                     "id": "civic.vid:33",
                     "type": "VariationDescriptor",
                     "label": "L858R",
-                    "description": "EGFR L858R has long been recognized as a functionally significant mutation in cancer, and is one of the most prevalent single mutations in lung cancer. Best described in non-small cell lung cancer (NSCLC), the mutation seems to confer sensitivity to first and second generation TKI's like gefitinib and neratinib. NSCLC patients with this mutation treated with TKI's show increased overall and progression-free survival, as compared to chemotherapy alone. Third generation TKI's are currently in clinical trials that specifically focus on mutant forms of EGFR, a few of which have shown efficacy in treating patients that failed to respond to earlier generation TKI therapies.",  # noqa: E501
                     "xrefs": [
                         "clinvar:376280",
                         "clinvar:16609",
                         "clinvar:376282",
                         "caid:CA126713",
                         "dbsnp:121434568"
                     ],
@@ -374,21 +378,17 @@
                                 "start": 55259515,
                                 "stop": 55259515,
                                 "reference_bases": "T",
                                 "variant_bases": "G",
                                 "representative_transcript":
                                     "ENST00000275493.2",
                                 "ensembl_version": 75,
-                                "reference_build": "GRCh37"
+                                "reference_build": "GRCh37",
+                                "type": "coordinates"
                             }
-                        },
-                        {
-                            "type": "Extension",
-                            "name": "civic_actionability_score",
-                            "value": 375
                         }
                     ],
                     "variation_id":
                         "ga4gh:VA.kgjrhgf84CEndyLjKdAO0RxN-e3pJjxA",
                     "variation": {
                         "_id": "ga4gh:VA.kgjrhgf84CEndyLjKdAO0RxN-e3pJjxA",
                         "type": "Allele",
@@ -588,15 +588,14 @@
 
 
 class ServiceMeta(BaseModel):
     """Metadata for MetaKB service."""
 
     name = "metakb"
     version = __version__
-    last_updated = LAST_UPDATED
     url = "https://github.com/cancervariants/metakb"
 
     class Config:
         """Configure schema example."""
 
         @staticmethod
         def schema_extra(schema: Dict[str, Any],
@@ -605,15 +604,14 @@
             if "title" in schema.keys():
                 schema.pop("title", None)
             for prop in schema.get("properties", {}).values():
                 prop.pop("title", None)
             schema["example"] = {
                 "name": "metakb",
                 "version": "1.1.0-alpha.4",
-                "last_updated": "2021-12-16",
                 "url": "https://github.com/cancervariants/metakb"
             }
 
 
 class SearchService(BaseModel):
     """Define model for Search Endpoint Response."""
 
@@ -730,35 +728,14 @@
                     "node": "civic.vid:33"
                 },
                 "variation_descriptors": [
                     {
                         "id": "civic.vid:33",
                         "type": "VariationDescriptor",
                         "label": "L858R",
-                        "description": "EGFR L858R has long been recognized "
-                                       "as a functionally significant "
-                                       "mutation in cancer, and is one of "
-                                       "he most prevalent single mutations in"
-                                       " lung cancer. Best described in "
-                                       "non-small cell lung cancer (NSCLC), "
-                                       "the mutation seems to confer "
-                                       "sensitivity to first and second "
-                                       "generation TKI's like gefitinib and"
-                                       " neratinib. NSCLC patients with this"
-                                       " mutation treated with TKI's show "
-                                       "increased overall and "
-                                       "progression-free survival, as "
-                                       "compared to chemotherapy alone. "
-                                       "Third generation TKI's are currently"
-                                       " in clinical trials that specifically"
-                                       " focus on mutant forms of EGFR, a few"
-                                       " of which have shown efficacy in "
-                                       "treating patients that failed to "
-                                       "respond to earlier generation "
-                                       "TKI therapies.",
                         "value_id": "ga4gh:VA.WyOqFMhc8aOnMFgdY0uM7nSLNqxVPAiR",  # noqa: E501
                         "value": {
                             "location": {
                                 "interval": {
                                     "end": 858,
                                     "start": 857,
                                     "type": "SimpleInterval"
@@ -789,22 +766,18 @@
                                     "chromosome": "7",
                                     "start": 55259515,
                                     "stop": 55259515,
                                     "reference_bases": "T",
                                     "variant_bases": "G",
                                     "representative_transcript": "ENST00000275493.2",  # noqa: E501
                                     "ensembl_version": 75,
-                                    "reference_build": "GRCh37"
+                                    "reference_build": "GRCh37",
+                                    "type": "coordinates"
                                 },
                                 "type": "Extension"
-                            },
-                            {
-                                "name": "civic_actionability_score",
-                                "value": "352.5",
-                                "type": "Extension"
                             }
                         ],
                         "structural_type": "SO:0001583",
                         "expressions": [
                             {
                                 "syntax": "hgvs.g",
                                 "value": "NC_000007.13:g.55259515T>G",
@@ -885,15 +858,14 @@
                             "object_qualifier": "ncit:C2926",
                             "object": "rxcui:1430438"
                         },
                         "variation_descriptor": {
                             "id": "civic.vid:33",
                             "type": "VariationDescriptor",
                             "label": "L858R",
-                            "description": "EGFR L858R has long been recognized as a functionally significant mutation in cancer, and is one of the most prevalent single mutations in lung cancer. Best described in non-small cell lung cancer (NSCLC), the mutation seems to confer sensitivity to first and second generation TKI's like gefitinib and neratinib. NSCLC patients with this mutation treated with TKI's show increased overall and progression-free survival, as compared to chemotherapy alone. Third generation TKI's are currently in clinical trials that specifically focus on mutant forms of EGFR, a few of which have shown efficacy in treating patients that failed to respond to earlier generation TKI therapies.",  # noqa: E501
                             "xrefs": [
                                 "clinvar:376280",
                                 "clinvar:16609",
                                 "clinvar:376282",
                                 "caid:CA126713",
                                 "dbsnp:121434568"
                             ],
@@ -909,21 +881,17 @@
                                         "start": 55259515,
                                         "stop": 55259515,
                                         "reference_bases": "T",
                                         "variant_bases": "G",
                                         "representative_transcript":
                                             "ENST00000275493.2",
                                         "ensembl_version": 75,
-                                        "reference_build": "GRCh37"
+                                        "reference_build": "GRCh37",
+                                        "type": "coordinates"
                                     }
-                                },
-                                {
-                                    "type": "Extension",
-                                    "name": "civic_actionability_score",
-                                    "value": 375
                                 }
                             ],
                             "variation_id":
                                 "ga4gh:VA.kgjrhgf84CEndyLjKdAO0RxN-e3pJjxA",
                             "variation": {
                                 "_id": "ga4gh:VA.kgjrhgf84CEndyLjKdAO0RxN-e3pJjxA",  # noqa: E501
                                 "type": "Allele",
```

### Comparing `metakb-1.1.0a9/metakb/transform/base.py` & `metakb-1.2.0.dev0/metakb/transform/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """A module for the Transform base class."""
 from typing import Dict, Optional, List
 import json
+import canonicaljson
 import logging
 from pathlib import Path
 from datetime import datetime as dt
 
 from ga4gh.core import sha512t24u
 
 from metakb import APP_ROOT, DATE_FMT
-from metakb.schemas import PropositionType, Predicate, DiagnosticPredicate, \
+from metakb.schemas import DiagnosticProposition, PrognosticProposition, \
+    PropositionType, Predicate, DiagnosticPredicate, \
     PrognosticPredicate, PredictivePredicate, FunctionalPredicate, \
-    PathogenicPredicate
+    PathogenicPredicate, TherapeuticResponseProposition
 from metakb.normalizers import VICCNormalizers
 
 logger = logging.getLogger('metakb')
 logger.setLevel(logging.DEBUG)
 
 
 class Transform:
@@ -81,14 +83,24 @@
         PropositionType.PREDICTIVE: PredictivePredicate,
         PropositionType.DIAGNOSTIC: DiagnosticPredicate,
         PropositionType.PROGNOSTIC: PrognosticPredicate,
         PropositionType.PATHOGENIC: PathogenicPredicate,
         PropositionType.FUNCTIONAL: FunctionalPredicate
     }
 
+    @staticmethod
+    def _generate_digest(data: Dict) -> str:
+        """Generate digest given dictionary
+
+        :param Dict data: Data to generate digest for
+        :return: Digest
+        """
+        blob = canonicaljson.encode_canonical_json(data)
+        return sha512t24u(blob)
+
     def _get_proposition_id(
         self,
         prop_type: PropositionType,
         pred: Predicate,
         variation_ids: List[str] = [],
         disease_ids: List[str] = [],
         therapy_ids: List[str] = []
@@ -111,14 +123,72 @@
         concept_ids = variation_ids + disease_ids + therapy_ids
         terms = [prop_type.value, pred.value] + concept_ids
         terms_sorted = sorted([t.lower() for t in terms])
         blob = json.dumps(terms_sorted).encode("ascii")
         digest = sha512t24u(blob=blob)
         return f"proposition:{digest}"
 
+    def _get_proposition(
+        self, proposition_type: PropositionType, predicate: Predicate, subject: str,
+        object_qualifier: str, object: Optional[str] = None
+    ) -> Optional[Dict]:
+        """Get proposition parameters. Updates the `propositions` instance variable
+        if proposition params were successfully created.
+
+        :param PropositionType proposition_type: Proposition type for evidence
+        :param Predicate predicate: Predicate for evidence
+        :param str subject: Subject (variation) for proposition
+        :param str object_qualifier: Object qualifier (disease) for proposition
+        :param Optional[str] object: Object (therapy) for proposition. Only required
+            if Therapeutic proposition
+        :return: Proposition represented as dict if valid, else None
+        """
+        params = {
+            "id": "",
+            "type": proposition_type,
+            "predicate": predicate,
+            "subject": subject,
+            "object_qualifier": object_qualifier
+        }
+
+        if proposition_type == PropositionType.PREDICTIVE:
+            params["object"] = object
+            proposition_id = self._get_proposition_id(
+                params["type"],
+                params["predicate"],
+                [params["subject"]],
+                [params["object_qualifier"]],
+                [params["object"]]
+            )
+        else:
+            proposition_id = self._get_proposition_id(
+                params["type"],
+                params["predicate"],
+                [params["subject"]],
+                [params["object_qualifier"]]
+            )
+        if proposition_id is None:
+            return None
+        else:
+            params["id"] = proposition_id
+
+        if proposition_type == PropositionType.PROGNOSTIC.value:
+            proposition = PrognosticProposition(**params).dict(exclude_none=True)
+        elif proposition_type == PropositionType.PREDICTIVE.value:
+            proposition = TherapeuticResponseProposition(**params).dict(
+                exclude_none=True)
+        elif proposition_type == PropositionType.DIAGNOSTIC.value:
+            proposition = DiagnosticProposition(**params).dict(exclude_none=True)
+        else:
+            proposition = None
+
+        if proposition and proposition not in self.propositions:
+            self.propositions.append(proposition)
+        return proposition
+
     @staticmethod
     def _get_document_id(**parameters) -> str:
         """Retrieve stable ID for a document.
         :parameters: property names and values to get ID for. Assumes values
             are strings.
         :return: identifying document ID value
         """
```

### Comparing `metakb-1.1.0a9/metakb/transform/civic.py` & `metakb-1.2.0.dev0/metakb/transform/civic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """A module for to transform CIViC."""
 from typing import Optional, Dict, List, Set
 from pathlib import Path
 import logging
+import re
 
 from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor, \
     Extension, Expression, GeneDescriptor, ValueObjectDescriptor
 
 from metakb import APP_ROOT
 from metakb.normalizers import VICCNormalizers
 from metakb.transform.base import Transform
 import metakb.schemas as schemas
 
 
-logger = logging.getLogger('metakb.transform.civic')
-logger.setLevel(logging.DEBUG)
+logger = logging.getLogger(__name__)
 
 
 class CIViCTransform(Transform):
     """A class for transforming CIViC to the common data model."""
 
     def __init__(self,
                  data_dir: Path = APP_ROOT / "data",
@@ -39,70 +39,108 @@
         }
         # Unable to normalize these IDs
         self.invalid_ids = {
             'therapy_descriptors': list(),
             'disease_descriptors': list()
         }
 
+    @staticmethod
+    def _mp_to_variant_mapping(molecular_profiles: List[Dict]) -> Dict:
+        """Get mapping from Molecular Profile ID to Variant ID. We currently do not
+        handle complex molecular profiles (> 1 variant associated).
+
+        :param molecular_profiles: List of civic molecular profiles represented as
+            dictionaries
+        :return: Molecular Profile ID to Variant ID mapping {mp_id: v_id}
+        """
+        mapping: Dict = {}
+        not_supported_mps = set()
+        for mp in molecular_profiles:
+            mp_id = mp["id"]
+            mp_variant_ids = mp["variant_ids"]
+            if len(mp_variant_ids) != 1:
+                mapping[mp_id] = None
+                not_supported_mps.add(mp_id)
+            else:
+                mapping[mp_id] = mp_variant_ids[0]
+
+        logger.debug(f"{len(not_supported_mps)} Molecular Profiles not supported: "
+                     f"{not_supported_mps}")
+        return mapping
+
     async def transform(self):
         """Transform CIViC harvested json to common data model."""
         data = self.extract_harvester()
         evidence_items = data['evidence']
         assertions = data['assertions']
+        molecular_profiles = data["molecular_profiles"]
         variants = data['variants']
         genes = data['genes']
+        mp_id_to_v_id_mapping = self._mp_to_variant_mapping(molecular_profiles)
+
+        # Only want evidence with approved status
+        evidence_items = [e for e in evidence_items if e["status"] == "accepted"]
 
-        # Filter Variant IDs for
-        # Prognostic, Predictive, and Diagnostic evidence
-        supported_evidence_types = ['Prognostic', 'Predictive', 'Diagnostic']
-        vids = {e['variant_id'] for e in evidence_items
-                if e['evidence_type'] in supported_evidence_types}
-        vids |= {a['variant']['id'] for a in assertions
-                 if a['evidence_type'] in supported_evidence_types}
+        # Filter Variant IDs for Prognostic, Predictive, and Diagnostic evidence
+        supported_evidence_types = ['PROGNOSTIC', 'PREDICTIVE', 'DIAGNOSTIC']
+        evidence_items = [e for e in evidence_items
+                          if e["evidence_type"].upper() in supported_evidence_types]
+        assertions = [a for a in assertions
+                      if a["assertion_type"].upper() in supported_evidence_types]
+
+        vids = {mp_id_to_v_id_mapping[e["molecular_profile_id"]]
+                for e in evidence_items if e["molecular_profile_id"]}
+        vids |= {mp_id_to_v_id_mapping[a["molecular_profile_id"]]
+                 for a in assertions if a["molecular_profile_id"]}
 
         await self._add_variation_descriptors(variants, vids)
         self._add_gene_descriptors(genes)
         self._add_methods()
-        self._transform_evidence_and_assertions(evidence_items)
-        self._transform_evidence_and_assertions(assertions, is_evidence=False)
-
-    def _transform_evidence_and_assertions(self, records: List[Dict],
-                                           is_evidence=True) -> None:
+        self._transform_evidence_and_assertions(evidence_items, mp_id_to_v_id_mapping)
+        self._transform_evidence_and_assertions(
+            assertions, mp_id_to_v_id_mapping, is_evidence=False
+        )
+
+    def _transform_evidence_and_assertions(
+        self, records: List[Dict], mp_id_to_v_id_mapping: Dict, is_evidence=True
+    ) -> None:
         """Transform statements, propositions, descriptors, and documents
         from CIViC evidence items and assertions.
 
-        :param list records: CIViC Evidence Items or Assertions
-        :param bool is_evidence: `True` if records are evidence items.
+        :param records: CIViC Evidence Items or Assertions
+        :param mp_id_to_v_id_mapping: Molecular Profile ID to Variant ID mappin
+            {mp_id: v_id}
+        :param is_evidence: `True` if records are evidence items.
             `False` if records are assertions.
         """
         for r in records:
             name_lower = r['name'].lower()
             if name_lower.startswith('eid'):
                 civic_id = name_lower.replace('eid', 'civic.eid:')
             else:
                 civic_id = name_lower.replace('aid', 'civic.aid:')
 
             # Omit entries that are not in an accepted state
             if r['status'] != 'accepted':
                 logger.warning(f"{civic_id} has status: {r['status']}")
                 continue
 
-            if r['evidence_type'] not in ['Predictive', 'Prognostic',
-                                          'Diagnostic']:
+            record_type = r["evidence_type"] if is_evidence else r["assertion_type"]
+            if record_type not in ["PREDICTIVE", "PROGNOSTIC", "DIAGNOSTIC"]:
                 continue
             else:
                 # Functional Evidence types do not have a disease
                 if not r['disease']:
                     continue
 
-            if r['evidence_type'] == 'Predictive':
-                if len(r['drugs']) != 1:
+            if record_type == "PREDICTIVE":
+                if len(r["therapies"]) != 1:
                     continue
                 else:
-                    therapy_id = f"civic.tid:{r['drugs'][0]['id']}"
+                    therapy_id = f"civic.tid:{r['therapies'][0]['id']}"
                     therapy_descriptor = \
                         self._add_therapy_descriptor(therapy_id, r)
                     if not therapy_descriptor:
                         continue
 
                     if therapy_descriptor not in self.therapy_descriptors:
                         self.therapy_descriptors.append(therapy_descriptor)
@@ -114,35 +152,43 @@
             disease_descriptor = self._add_disease_descriptor(disease_id, r)
             if not disease_descriptor:
                 continue
 
             if disease_descriptor not in self.disease_descriptors:
                 self.disease_descriptors.append(disease_descriptor)
 
-            if is_evidence:
-                variant_id = f"civic.vid:{r['variant_id']}"
-            else:
-                variant_id = f"civic.vid:{r['variant']['id']}"
+            variant_id = f"civic.vid:{mp_id_to_v_id_mapping[r['molecular_profile_id']]}"
             variation_descriptor = \
                 self.valid_ids['variation_descriptors'].get(variant_id)
             if not variation_descriptor:
                 continue
 
+            try:
+                proposition_type = self._get_proposition_type(record_type)
+            except KeyError:
+                continue
+
+            predicate = self._get_predicate(proposition_type, r["significance"])
+
+            # Don't support TR that has  `None`, "N/A", or "Unknown" predicate
+            if not predicate:
+                continue
+
+            object = None
+            if therapy_descriptor:
+                object = therapy_descriptor["therapy_id"]
+
             proposition = self._get_proposition(
-                r, variation_descriptor, disease_descriptor,
-                therapy_descriptor
-            )
+                proposition_type, predicate, variation_descriptor["variation_id"],
+                disease_descriptor["disease_id"], object)
 
             # Only support Therapeutic Response and Prognostic
             if not proposition:
                 continue
 
-            if proposition not in self.propositions:
-                self.propositions.append(proposition)
-
             if is_evidence:
                 # Evidence items's method and evidence level
                 method = f'method:{schemas.MethodID.CIVIC_EID_SOP}'
                 evidence_level = f"civic.evidence_level:{r['evidence_level']}"
 
                 # Supported by evidence for evidence item
                 document = self._get_eid_document(r['source'])
@@ -170,23 +216,24 @@
                 supported_by = list()
                 documents = \
                     self._get_aid_document(r)
                 for d in documents:
                     if d not in self.documents:
                         self.documents.append(d)
                     supported_by.append(d['id'])
-                for evidence_item in r['evidence_items']:
-                    supported_by.append(f"civic.eid:"
-                                        f"{evidence_item['id']}")
+
+                for ev_id in r["evidence_ids"]:
+                    supported_by.append(f"civic.eid:{ev_id}")
 
             statement = schemas.Statement(
                 id=civic_id,
                 description=r['description'],
                 direction=self._get_evidence_direction(
-                    r['evidence_direction']),
+                    r["evidence_direction"] if is_evidence else r["assertion_direction"]
+                ),
                 evidence_level=evidence_level,
                 proposition=proposition['id'],
                 variation_origin=self._get_variation_origin(
                     r['variant_origin']),
                 variation_descriptor=variant_id,
                 therapy_descriptor=therapy_id,
                 disease_descriptor=disease_id,
@@ -197,17 +244,18 @@
 
     def _get_evidence_direction(self, direction) -> Optional[str]:
         """Return the evidence direction.
 
         :param str direction: The civic evidence_direction value
         :return: `supports` or `does_not_support` or None
         """
-        if direction == 'Supports':
+        direction_upper = direction.upper()
+        if direction_upper == "SUPPORTS":
             return schemas.Direction.SUPPORTS.value
-        elif direction == 'Does Not Support':
+        elif direction_upper == "DOES_NOT_SUPPORT":
             return schemas.Direction.DOES_NOT_SUPPORT.value
         else:
             return None
 
     def _get_assertion_evidence_level(self, assertion) -> Optional[str]:
         """Return evidence_level for CIViC assertion.
 
@@ -216,97 +264,36 @@
         """
         evidence_level = None
         # TODO: CHECK
         if assertion['amp_level']:
             if assertion['amp_level'] == 'Not Applicable':
                 evidence_level = None
             else:
-                tier, level = assertion['amp_level'].split(' - ')
-                tier = tier.split()[1]
-                if tier == 'I':
-                    tier = 1
-                elif tier == 'II':
-                    tier = 2
-                elif tier == 'III':
-                    tier = 3
-                elif tier == 'IV':
-                    tier = 4
-                evidence_level = f"amp_asco_cap_2017_level:" \
-                                 f"{tier}{level.split()[1]}"
-        return evidence_level
-
-    def _get_proposition(self, record, variation_descriptor,
-                         disease_descriptor, therapy_descriptor
-                         ) -> Optional[dict]:
-        """Return a proposition for a record.
-
-        :param dict record: CIViC EID or AID
-        :param dict variation_descriptor: The record's variation descriptor
-        :param dict disease_descriptor: The record's disease descriptor
-        :param dict therapy_descriptor: The record's therapy descriptor
-        :return: A proposition
-        """
-        try:
-            proposition_type = \
-                self._get_proposition_type(record["evidence_type"])
-        except KeyError:
-            return None
-
-        predicate = self._get_predicate(proposition_type,
-                                        record["clinical_significance"])
-
-        # Don't support TR that has  `None`, "N/A", or "Unknown" predicate
-        if not predicate:
-            return None
-
-        params = {
-            "id": "",
-            "type": proposition_type,
-            "predicate": predicate,
-            "subject": variation_descriptor["variation_id"],
-            "object_qualifier": disease_descriptor["disease_id"]
-        }
-
-        if proposition_type == schemas.PropositionType.PREDICTIVE:
-            params["object"] = therapy_descriptor["therapy_id"]
-            proposition_id = self._get_proposition_id(
-                params["type"],
-                params["predicate"],
-                [params["subject"]],
-                [params["object_qualifier"]],
-                [params["object"]]
-            )
-        else:
-            proposition_id = self._get_proposition_id(
-                params["type"],
-                params["predicate"],
-                [params["subject"]],
-                [params["object_qualifier"]]
-            )
-        if proposition_id is None:
-            return None
-        else:
-            params["id"] = proposition_id
+                amp_level = assertion["amp_level"]
+                regex = re.compile(r"TIER_(?P<tier>\w+)_LEVEL_(?P<level>\w+)")
+                match = regex.match(amp_level)
+                if match:
+                    match = match.groupdict()
+                    tier = match["tier"]
+                    level = match["level"]
+
+                    if tier == 'I':
+                        tier = 1
+                    elif tier == 'II':
+                        tier = 2
+                    elif tier == 'III':
+                        tier = 3
+                    elif tier == 'IV':
+                        tier = 4
 
-        if proposition_type == schemas.PropositionType.PROGNOSTIC.value:
-            proposition = \
-                schemas.PrognosticProposition(**params).dict(exclude_none=True)
-        elif proposition_type == schemas.PropositionType.PREDICTIVE.value:
-            params["object"] = therapy_descriptor["therapy_id"]
-            proposition =\
-                schemas.TherapeuticResponseProposition(**params).dict(
-                    exclude_none=True
-                )
-        elif proposition_type == schemas.PropositionType.DIAGNOSTIC.value:
-            proposition = \
-                schemas.DiagnosticProposition(**params).dict(
-                    exclude_none=True)
-        else:
-            proposition = None
-        return proposition
+                    evidence_level = f"amp_asco_cap_2017_level:" \
+                                     f"{tier}{level}"
+                else:
+                    raise Exception(f"{amp_level} not supported with regex")
+        return evidence_level
 
     def _get_proposition_type(self,
                               evidence_type,
                               is_evidence=True) -> Optional[schemas.PropositionType]:  # noqa: E501
         """Return proposition type for a given EID or AID.
 
         :param str evidence_type: CIViC evidence type
@@ -329,19 +316,20 @@
 
     def _get_variation_origin(self, variant_origin) -> Optional[str]:
         """Return variant origin.
 
         :param str variant_origin: CIViC variant origin
         :return: Variation origin
         """
-        if variant_origin == 'Somatic':
+        variant_origin = variant_origin.upper()
+        if variant_origin == "SOMATIC":
             origin = schemas.VariationOrigin.SOMATIC.value
-        elif variant_origin in ['Rare Germline', 'Common Germline']:
+        elif variant_origin in ["RARE_GERMLINE", "COMMON_GERMLINE"]:
             origin = schemas.VariationOrigin.GERMLINE.value
-        elif variant_origin == 'N/A':
+        elif variant_origin == "NA":
             origin = schemas.VariationOrigin.NOT_APPLICABLE.value
         else:
             origin = None
         return origin
 
     def _get_predicate(self, proposition_type,
                        clin_sig) -> Optional[schemas.Predicate]:
@@ -351,18 +339,21 @@
         :param str clin_sig: The evidence item's clinical significance
         :return: Predicate for proposition if valid
         """
         if clin_sig is None or clin_sig.upper() in ['N/A', 'UNKNOWN']:
             return None
 
         clin_sig = '_'.join(clin_sig.upper().split())
+        if clin_sig == "NA":
+            logger.info("NA predicate not supported")
+            return None
         predicate = None
 
         if proposition_type == schemas.PropositionType.PREDICTIVE:
-            if clin_sig == 'SENSITIVITY/RESPONSE':
+            if clin_sig == 'SENSITIVITYRESPONSE':
                 predicate = schemas.PredictivePredicate.SENSITIVITY
             elif clin_sig == 'RESISTANCE':
                 predicate = schemas.PredictivePredicate.RESISTANCE
         elif proposition_type == schemas.PropositionType.DIAGNOSTIC:
             predicate = schemas.DiagnosticPredicate[clin_sig]
         elif proposition_type == schemas.PropositionType.PROGNOSTIC:
             if clin_sig == 'POSITIVE':
@@ -412,51 +403,50 @@
             if vname_lower.endswith("fs") or "-" in vname_lower or "/" in vname_lower:  # noqa: E501
                 if not hgvs_exprs:
                     logger.warning("Variation Normalizer does not support "
                                    f"{variant_id}: {variant_query}")
                     continue
 
             unable_to_normalize = {
-                "mutation", "amplification", "exon", "overexpression",
+                "mutation", "exon", "overexpression",
                 "frameshift", "promoter", "deletion", "type", "insertion",
                 "expression", "duplication", "copy", "underexpression",
                 "number", "variation", "repeat", "rearrangement", "activation",
                 "expression", "mislocalization", "translocation", "wild",
                 "polymorphism", "frame", "shift", "loss", "function", "levels",
                 "inactivation", "snp", "fusion", "dup", "truncation",
-                "homozygosity", "gain", "phosphorylation",
+                "homozygosity", "gain", "phosphorylation"
             }
 
             if set(vname_lower.split()) & unable_to_normalize:
                 logger.warning("Variation Normalizer does not support "
                                f"{variant_id}: {variant_query}")
                 continue
 
-            variation_norm_resp = await self.vicc_normalizers.normalize_variation(
+            variation_descriptor = await self.vicc_normalizers.normalize_variation(
                 [variant_query]
             )
 
             # Couldn't find normalized concept
-            if not variation_norm_resp:
+            if not variation_descriptor:
                 logger.warning("Variation Normalizer unable to normalize "
                                f"civic.vid:{variant['id']} using query "
                                f"{variant_query}")
                 continue
 
             if variant["variant_types"]:
                 structural_type = variant["variant_types"][0]["so_id"]
             else:
                 structural_type = None
 
             variation_descriptor = VariationDescriptor(
                 id=variant_id,
                 label=variant["name"],
-                description=variant["description"] if variant["description"] else None,  # noqa: E501
-                variation_id=variation_norm_resp.variation_id,
-                variation=variation_norm_resp.variation,
+                variation_id=variation_descriptor.variation_id,
+                variation=variation_descriptor.variation,
                 gene_context=f"civic.gid:{variant['gene_id']}",
                 structural_type=structural_type,
                 expressions=hgvs_exprs,
                 xrefs=self._get_variant_xrefs(variant),
                 alternate_labels=[v_alias for v_alias in
                                   variant["variant_aliases"] if not
                                   v_alias.startswith("RS")],
@@ -470,45 +460,22 @@
 
     def _get_variant_extensions(self, variant) -> list:
         """Return a list of extensions for a variant.
 
         :param dict variant: A CIViC variant record
         :return: A list of extensions
         """
-        extensions = [
+        return [
             Extension(
                 name='civic_representative_coordinate',
                 value={k: v for k, v in variant['coordinates'].items()
                        if v is not None}
-            ).dict(exclude_none=True),
-            Extension(
-                name='civic_actionability_score',
-                value=variant['civic_actionability_score']
             ).dict(exclude_none=True)
         ]
 
-        variant_groups = variant['variant_groups']
-        if variant_groups:
-            v_groups = list()
-            for v_group in variant_groups:
-                params = {
-                    'id': f"civic.variant_group:{v_group['id']}",
-                    'label': v_group['name'],
-                    'description': v_group['description'],
-                    'type': 'variant_group'
-                }
-                if v_group['description'] == '':
-                    del params['description']
-                v_groups.append(params)
-            extensions.append(Extension(
-                name='variant_group',
-                value=v_groups
-            ).dict(exclude_none=True))
-        return extensions
-
     def _get_variant_xrefs(self, v) -> Optional[List[str]]:
         """Return a list of xrefs for a variant.
 
         :param dict v: A CIViC variant record
         :return: A dictionary of xrefs
         """
         xrefs = []
@@ -614,19 +581,19 @@
             return None
 
         disease_id = f"civic.did:{disease['id']}"
         display_name = disease['display_name']
         doid = disease['doid']
 
         if not doid:
-            logger.warning(f"{disease_id} ({display_name}) has null DOID")
+            logger.debug(f"{disease_id} ({display_name}) has null DOID")
             queries = [display_name]
             xrefs = []
         else:
-            doid = f"DOID:{disease['doid']}"
+            doid = f"DOID:{doid}"
             queries = [doid, display_name]
             xrefs = [doid]
 
         _, normalized_disease_id = \
             self.vicc_normalizers.normalize_disease(queries)
 
         if not normalized_disease_id:
@@ -655,15 +622,15 @@
             self.valid_ids['therapy_descriptors'].get(therapy_id)
         if therapy_descriptor:
             return therapy_descriptor
         else:
             therapy_descriptor = None
             if therapy_id not in self.invalid_ids['therapy_descriptors']:
                 therapy_descriptor = \
-                    self._get_therapy_descriptor(record['drugs'][0])
+                    self._get_therapy_descriptor(record["therapies"][0])
                 if therapy_descriptor:
                     self.valid_ids['therapy_descriptors'][therapy_id] = \
                         therapy_descriptor
                 else:
                     self.invalid_ids['therapy_descriptors'].append(therapy_id)
             return therapy_descriptor
 
@@ -760,30 +727,31 @@
                 xrefs.append(f"asco.abstract:{source['asco_abstract_id']}")
             if source['pmc_id']:
                 xrefs.append(f"pmc:{source['pmc_id']}")
 
             document = schemas.Document(
                 id=document_id,
                 label=source['citation'],
-                description=source['name'],
+                description=source["title"],
                 xrefs=xrefs if xrefs else None
             ).dict(exclude_none=True)
             return document
         else:
             logger.warning(f"{source_type} not in schemas.SourcePrefix")
 
     def _get_aid_document(self, assertion: Dict) -> List[schemas.Document]:
         """Get an AID's documents.
 
         :param dict assertion: A CIViC Assertion
         :return: A list of AID documents
         """
         # NCCN Guidlines
         documents = list()
-        label = assertion["nccn_guideline"]
+        nccn_guideline = assertion["nccn_guideline"] or dict()
+        label = nccn_guideline.get("name")
         version = assertion["nccn_guideline_version"]
         if label and version:
             doc_id = "https://www.nccn.org/professionals/physician_gls/default.aspx"  # noqa: E501
             doc_label = f"NCCN Guidelines: {label} version {version}"
             db_id = self._get_document_id(document_id=doc_id, label=doc_label)
             documents = list()
             documents.append(schemas.Document(
```

### Comparing `metakb-1.1.0a9/metakb/transform/moa.py` & `metakb-1.2.0.dev0/metakb/transform/moa.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,38 +230,38 @@
 
         :param: single assertion record from MOA
         :return: list of variation descriptor
         """
         vrs_ref_allele_seq = variant['protein_change'][2] \
             if 'protein_change' in variant and variant['protein_change'] else None  # noqa: E501
 
-        v_norm_resp = None
+        variation_descriptor = None
         # For now, the normalizer only support a.a substitution
         if g_descriptors and 'protein_change' in variant and variant['protein_change']:  # noqa: E501
             gene = g_descriptors[0]['label']
             query = f"{gene} {variant['protein_change'][2:]}"
-            v_norm_resp = \
+            variation_descriptor = \
                 await self.vicc_normalizers.normalize_variation([query])
 
-            if not v_norm_resp:
+            if not variation_descriptor:
                 logger.warning(f"Variant Normalizer unable to normalize: "
                                f"moa.variant:{variant['id']}.")
                 return []
         else:
             logger.warning(f"Variation Normalizer does not support "
                            f"moa.variant:{variant['id']}: {variant}")
             return []
 
         gene_context = g_descriptors[0]['id'] if g_descriptors else None
 
         variation_descriptor = VariationDescriptor(
             id=f"moa.variant:{variant['id']}",
             label=variant['feature'],
-            variation_id=v_norm_resp.variation_id,
-            variation=v_norm_resp.variation,
+            variation_id=variation_descriptor.variation_id,
+            variation=variation_descriptor.variation,
             gene_context=gene_context,
             vrs_ref_allele_seq=vrs_ref_allele_seq,
             extensions=self._get_variant_extensions(variant)
         ).dict(by_alias=True, exclude_none=True)
         return [variation_descriptor]
 
     def _get_variant_extensions(self, variant):
@@ -323,23 +323,23 @@
 
     def _get_documents(self, source):
         """Get an assertion's documents.
 
         :param: An evidence source
         :param: Keeps track of proposition and documents indexes
         """
-        if source['pmid'] != "None":
+        if source['pmid']:
             documents_id = f"pmid:{source['pmid']}"
         else:
             documents_id = source['url']
 
         xrefs = []
         if source['doi']:
             xrefs.append(f"doi:{source['doi']}")
-        if source['nct'] != "None":
+        if source['nct']:
             xrefs.append(f"nct:{source['nct']}")
 
         documents = schemas.Document(
             id=documents_id,
             label=source['citation'],
             xrefs=xrefs if xrefs else None
         ).dict(exclude_none=True)
```

### Comparing `metakb-1.1.0a9/metakb.egg-info/PKG-INFO` & `metakb-1.2.0.dev0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metakb
-Version: 1.1.0a9
+Version: 1.2.0.dev0
 Summary: A search interface for cancer variant interpretations assembled by aggregating and harmonizing across multiple cancer variant interpretation knowledgebases.
 Home-page: https://github.com/cancervariants/metakb
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tests
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/vicc-metakb/badge/?version=latest)](https://vicc-metakb.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.org/cancervariants/metakb.svg?branch=main)](https://travis-ci.org/cancervariants/metakb) [![Coverage Status](https://coveralls.io/repos/github/cancervariants/metakb/badge.svg?branch=main)](https://coveralls.io/github/cancervariants/metakb?branch=main)
 
 # metakb
 
 The intent of the project is to leverage the collective knowledge of the disparate existing resources of the VICC to improve the comprehensiveness of clinical interpretation of genomic variation. An ongoing goal will be to provide and improve upon standards and guidelines by which other groups with clinical interpretation data may make it accessible and visible to the public. We have released a preprint discussing our initial harmonization effort and observed disparities in the structure and content of variant interpretations.
@@ -46,82 +48,149 @@
 
 
 Once Pipenv is installed, clone the repo and install the package requirements into a Pipenv environment:
 
 ```sh
 git clone https://github.com/cancervariants/metakb
 cd metakb
-pipenv lock
-pipenv sync
+pipenv lock && pipenv sync
 ```
 
 If you intend to provide development support, install the development dependencies:
 
 ```sh
-pipenv lock --dev
-pipenv sync
+pipenv lock --dev && pipenv sync
 ```
 
 ### Setting up Neo4j
 
 The MetaKB uses [Neo4j](https://neo4j.com/) for its database backend. To run a local MetaKB instance, you'll need to run a Neo4j database instance as well. The easiest way to do this is from Neo4j Desktop.
 
 First, follow the [desktop setup instructions](https://neo4j.com/developer/neo4j-desktop) to download, install, and open Neo4j Desktop for the first time.
 
 Once you have opened Neo4j desktop, use the "New" button in the upper-left region of the window to create a new project. Within that project, click the "Add" button in the upper-right region of the window and select "Local DBMS". The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using "admin" by default). Click "Create". Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green "Start" button to start the database service.
 
-The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:5818"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
+The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:1409"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
 
 
 ### Setting up normalizers
 
 The MetaKB calls a number of normalizer libraries to transform resource data and resolve incoming search queries. These will be installed as part of the package requirements, but require additional setup.
 
-First, [download and install Amazon's DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html). Once installed, in a separate terminal instance, navigate to its source directory and run the following to start the database instance:
+First, [follow these instructions for deploying DynamoDB locally on your computer](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html). Once setup, in a separate terminal instance, navigate to its source directory and run the following to start the database instance:
 
 ```sh
 java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
 ```
 
 Next, navigate to the `site-packages` directory of your virtual environment. Assuming Pipenv is installed to your user directory, this should be something like:
 
 ```sh
-cd ~/.local/share/virtualenvs/metakb-<various characters>/python3.7/site-packages/  # replace <various characters>
+cd ~/.local/share/virtualenvs/metakb-<various characters>/lib/python<python-version>/site-packages/  # replace <various characters> and <python-version>
 ```
 
-Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation).
+Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation). When setting up the UTA database, [these](https://github.com/ga4gh/vrs-python/tree/main/docs/setup_help) docs may be helpful.
 
 
 The MetaKB can acquire all other needed normalizer data, except for that of [OMIM](https://www.omim.org/downloads), which must be manually placed:
 
 ```sh
 cd disease/  # starting from the site-packages dir of your virtual environment's Python instance
 mkdir -p data/omim
 cp ~/YOUR/PATH/TO/mimTitles.txt data/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
 ```
 
+### Environment Variables
+
+MetaKB relies on environment variables to set in order to work.
+
+* Always Required:
+  * `UTA_DB_URL`
+    * Used in Variation Normalizer which relies on UTA Tools
+    * Format: `driver://user:pass@host/database/schema`
+    * More info can be found [here](https://github.com/GenomicMedLab/uta-tools#connecting-to-the-database)
+
+    Example:
+
+    ```shell script
+    export UTA_DB_URL=postgresql://uta_admin:password@localhost:5432/uta/uta_20210129
+    ```
+
+  * `ONCOKB_API_TOKEN`
+    * Required to harvest OncoKB data. If you do not set this environment variable, you can set during the initialization of the OncoKBHarvester.
+    * Used to access OncoKB data via their REST API. See [here](https://www.oncokb.org/apiAccess) for more information on how to register an account and get an OncoKB API token.
+
+    Example for setting environment variable:
+    ```shell script
+    export ONCOKB_API_TOKEN={api_token}
+    ```
+
+    Example for setting during OncoKB Harvester initialization:
+    ```python
+    OncoKBHarvester(api_token={api_token})
+    ```
+
+* Required when using the `--load_normalizers_db` or `--force_load_normalizers_db` arguments in CLI commands
+  * `RXNORM_API_KEY`
+    * Used in Therapy Normalizer to retrieve RxNorm data
+    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `RxNORM_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
+
+    Example:
+
+    ```shell script
+    export RXNORM_API_KEY={rxnorm_api_key}
+    ```
+
+  * `DATAVERSE_API_KEY`
+    * Used in Therapy Normalizer to retrieve HemOnc data
+    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `DATAVERSE_API_KEY` environment variable to your API key.
+
+    Example:
+
+    ```shell script
+    export DATAVERSE_API_KEY={dataverse_api_key}
+    ```
+
+### Data files
+
+Some sources in MetaKB require user provided files to harvest data.
+
+* OncoKB
+  * In addition to setting the `ONCOKB_API_TOKEN` environment variable to harvest OncoKB data, you also need to provide a CSV file containing a header row with `hugo_symbol` and `protein_change`, associated rows containing protein variants you wish to harvest, and using a comma as the delimiter. The file will look something like:
+
+    ```csv
+    hugo_symbol,protein_change
+    BRAF,V600E
+    ...
+    ```
+  * This file will harvest OncoKB evidence based on the variants provided.
+
 ### Loading data
 
-Once Neo4j and DynamoDB instances are both active, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
+Once Neo4j and DynamoDB instances are both running, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
 
 In the MetaKB project root, run the following:
 
 ```sh
 pipenv shell
 python3 -m metakb.cli --db_url=bolt://localhost:7687 --db_username=neo4j --db_password=<neo4j-password-here> --load_normalizers_db
 ```
 
+For more information on the different CLI arguments, see the [CLI README](docs/cli/README.md).
+
 ### Starting the server
 
 Once data has been loaded successfully, use the following to start service on localhost port 8000:
 
 ```sh
 uvicorn metakb.main:app --reload
 ```
 
+Ensure that both the MetaKB Neo4j and Normalizers databases are running.
+
 Navigate to [http://localhost:8000/api/v2](http://localhost:8000/api/v2) in your browser to enter queries.
 
 ## Running tests
 
 ### Unit tests
 
 Explain how to run the automated tests for this system
```

### Comparing `metakb-1.1.0a9/metakb.egg-info/SOURCES.txt` & `metakb-1.2.0.dev0/metakb.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 metakb.egg-info/not-zip-safe
 metakb.egg-info/requires.txt
 metakb.egg-info/top_level.txt
 metakb/harvesters/__init__.py
 metakb/harvesters/base.py
 metakb/harvesters/civic.py
 metakb/harvesters/moa.py
+metakb/harvesters/oncokb.py
 metakb/transform/__init__.py
 metakb/transform/base.py
 metakb/transform/civic.py
-metakb/transform/moa.py
+metakb/transform/moa.py
+metakb/transform/oncokb.py
```

### Comparing `metakb-1.1.0a9/setup.cfg` & `metakb-1.2.0.dev0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = metakb
 author = VICC
 author_email = help@cancervariants.org
 description = A search interface for cancer variant interpretations assembled by aggregating and harmonizing across multiple cancer variant interpretation knowledgebases.
 long_description = file:README.md
 long_description_content_type = text/markdown
 home-page = https://github.com/cancervariants/metakb
-license-file = LICENSE
+license_files = LICENSE
 license = MIT
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	License :: OSI Approved :: MIT License
@@ -18,33 +18,39 @@
 	Programming Language :: Python :: 3.8
 
 [options]
 packages = find:
 python_requires = >=3.8
 zip_safe = False
 install_requires = 
-	ga4gh.vrs[extras] >=0.7.5.dev1
-	civicpy
+	civicpy ~= 3.0.0
+	ga4gh.vrs ~= 0.8.1
+	ga4gh.vrsatile.pydantic ~= 0.0.12
+	gene-normalizer[etl] ~= 0.1.36
+	variation-normalizer ~= 0.5.5
+	disease-normalizer[dev] ~= 0.2.20
+	thera-py[dev] ~= 0.3.10
 	requests
+	requests-cache
 	jsondiff
 	pydantic
-	requests-cache
-	gene-normalizer >=0.1.25
-	disease-normalizer >=0.2.12
-	thera-py >= 0.3.4
-	neo4j
 	uvicorn
 	fastapi
 	asyncclick
-	typing-extensions
+	neo4j
 	boto3
 	botocore
-	variation-normalizer >=0.4.0a7
-	ga4gh.vrsatile.pydantic >=0.0.11
-tests_require = 
+
+[options.extras_require]
+dev = 
+	pre-commit
+	flake8
+	flake8-docstrings
+	ipykernel
+tests = 
 	pytest
 	pytest-cov
 	mock
 	pytest-asyncio
 
 [tool:pytest]
 addopts = --ignore=setup.py --ignore=docs/__authors__.py --ignore=docs/conf.py --ignore analysis/ --ignore codebuild/ --doctest-modules --cov-report term-missing --cov .
```

