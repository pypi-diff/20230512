# Comparing `tmp/VertFlow-0.3.0.tar.gz` & `tmp/VertFlow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VertFlow-0.3.0.tar", last modified: Fri Mar 31 15:04:05 2023, max compression
+gzip compressed data, was "VertFlow-0.4.0.tar", last modified: Fri May 12 15:20:08 2023, max compression
```

## Comparing `VertFlow-0.3.0.tar` & `VertFlow-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:05.009020 VertFlow-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-31 15:03:47.000000 VertFlow-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-31 15:04:05.009020 VertFlow-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-31 15:03:47.000000 VertFlow-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:05.005020 VertFlow-0.3.0/VertFlow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-31 15:04:04.000000 VertFlow-0.3.0/VertFlow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-31 15:04:05.000000 VertFlow-0.3.0/VertFlow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 15:04:04.000000 VertFlow-0.3.0/VertFlow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 15:04:04.000000 VertFlow-0.3.0/VertFlow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 15:04:04.000000 VertFlow-0.3.0/VertFlow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-31 15:04:05.009020 VertFlow-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-31 15:03:47.000000 VertFlow-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:05.005020 VertFlow-0.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-31 15:03:47.000000 VertFlow-0.3.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-03-31 15:03:47.000000 VertFlow-0.3.0/src/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-31 15:03:47.000000 VertFlow-0.3.0/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-31 15:03:47.000000 VertFlow-0.3.0/src/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-03-31 15:03:47.000000 VertFlow-0.3.0/src/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-31 15:03:47.000000 VertFlow-0.3.0/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:05.009020 VertFlow-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-03-31 15:03:47.000000 VertFlow-0.3.0/test/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-03-31 15:03:47.000000 VertFlow-0.3.0/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-03-31 15:03:47.000000 VertFlow-0.3.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:08.001347 VertFlow-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-12 15:19:53.000000 VertFlow-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-12 15:20:08.001347 VertFlow-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-12 15:19:53.000000 VertFlow-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:07.997347 VertFlow-0.4.0/VertFlow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 15:20:07.000000 VertFlow-0.4.0/VertFlow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-12 15:20:08.001347 VertFlow-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-12 15:19:53.000000 VertFlow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:07.997347 VertFlow-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-12 15:19:53.000000 VertFlow-0.4.0/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:08.001347 VertFlow-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-12 15:19:53.000000 VertFlow-0.4.0/test/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-12 15:19:53.000000 VertFlow-0.4.0/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-12 15:19:53.000000 VertFlow-0.4.0/test/test_utils.py
```

### Comparing `VertFlow-0.3.0/LICENSE` & `VertFlow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/PKG-INFO` & `VertFlow-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VertFlow
-Version: 0.3.0
+Version: 0.4.0
 Summary: Apache Airflow operator for running Google Cloud Run Jobs using green energy
 Home-page: https://github.com/ovotech/VertFlow
 Author: OVO Energy
 Author-email: trading.dl@ovoenergy.com
 License: Apache 2.0
 Keywords: airflow,gcp,google,cloud run,cloud composer,green,environment,sustainability
 Requires-Python: >=3.7
@@ -48,15 +48,15 @@
 > ℹ️ If you're using Cloud Composer, these instructions may be helpful:
 > * [Installing PyPI packages](https://cloud.google.com/composer/docs/how-to/using/installing-python-dependencies#install-package)
 > * [Setting up internet access](https://cloud.google.com/composer/docs/concepts/private-ip#public_internet_access_for_your_workflows)
 > * [About service accounts for Cloud Composer](https://cloud.google.com/composer/docs/composer-2/access-control#about-service)
 
 ## 🖱 How to use
 
-Use the `VertFlowOperator` to instantiate a task in your DAG.
+Use the [`VertFlowOperator`](https://github.com/ovotech/VertFlow/blob/main/src/operator.py#L30) to instantiate a task in your DAG.
 Provide:
 
 * The address of the Docker image to run.
 * A runtime specification, e.g. timeout and memory limits.
 * A set of allowed regions to run the job in, based on your latency, data governance and other considerations. VertFlow
   picks the greenest one.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VertFlow Version: 0.3.0 Summary: Apache Airflow
+Metadata-Version: 2.1 Name: VertFlow Version: 0.4.0 Summary: Apache Airflow
 operator for running Google Cloud Run Jobs using green energy Home-page: https:
 //github.com/ovotech/VertFlow Author: OVO Energy Author-email:
 trading.dl@ovoenergy.com License: Apache 2.0 Keywords: airflow,gcp,google,cloud
 run,cloud composer,green,environment,sustainability Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
                                    VertFlow
@@ -28,19 +28,20 @@
 called `VERTFLOW_API_KEY`. > â¹ï¸ If you're using Cloud Composer, these
 instructions may be helpful: > * [Installing PyPI packages](https://
 cloud.google.com/composer/docs/how-to/using/installing-python-
 dependencies#install-package) > * [Setting up internet access](https://
 cloud.google.com/composer/docs/concepts/private-
 ip#public_internet_access_for_your_workflows) > * [About service accounts for
 Cloud Composer](https://cloud.google.com/composer/docs/composer-2/access-
-control#about-service) ## ð± How to use Use the `VertFlowOperator` to
-instantiate a task in your DAG. Provide: * The address of the Docker image to
-run. * A runtime specification, e.g. timeout and memory limits. * A set of
-allowed regions to run the job in, based on your latency, data governance and
-other considerations. VertFlow picks the greenest one. ```python from
+control#about-service) ## ð± How to use Use the [`VertFlowOperator`](https://
+github.com/ovotech/VertFlow/blob/main/src/operator.py#L30) to instantiate a
+task in your DAG. Provide: * The address of the Docker image to run. * A
+runtime specification, e.g. timeout and memory limits. * A set of allowed
+regions to run the job in, based on your latency, data governance and other
+considerations. VertFlow picks the greenest one. ```python from
 VertFlow.operator import VertFlowOperator from airflow import DAG with DAG
 ( dag_id="hourly_dag_in_green_region", schedule_interval="@hourly" ) as dag:
 task = VertFlowOperator( image_address="us-docker.pkg.dev/cloudrun/container/
 job:latest", name="hello-world", allowed_regions=["europe-west1", "europe-
 west4"], command="echo", arguments=["Hello World"],
 service_account_email_address="my-service-account@embroidered-elephant-
 739.iam.gserviceaccount.com", ... ) ``` ## ððº Shout out to CO2 Signal
```

### Comparing `VertFlow-0.3.0/README.md` & `VertFlow-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 > ℹ️ If you're using Cloud Composer, these instructions may be helpful:
 > * [Installing PyPI packages](https://cloud.google.com/composer/docs/how-to/using/installing-python-dependencies#install-package)
 > * [Setting up internet access](https://cloud.google.com/composer/docs/concepts/private-ip#public_internet_access_for_your_workflows)
 > * [About service accounts for Cloud Composer](https://cloud.google.com/composer/docs/composer-2/access-control#about-service)
 
 ## 🖱 How to use
 
-Use the `VertFlowOperator` to instantiate a task in your DAG.
+Use the [`VertFlowOperator`](https://github.com/ovotech/VertFlow/blob/main/src/operator.py#L30) to instantiate a task in your DAG.
 Provide:
 
 * The address of the Docker image to run.
 * A runtime specification, e.g. timeout and memory limits.
 * A set of allowed regions to run the job in, based on your latency, data governance and other considerations. VertFlow
   picks the greenest one.
```

#### html2text {}

```diff
@@ -22,19 +22,20 @@
 called `VERTFLOW_API_KEY`. > â¹ï¸ If you're using Cloud Composer, these
 instructions may be helpful: > * [Installing PyPI packages](https://
 cloud.google.com/composer/docs/how-to/using/installing-python-
 dependencies#install-package) > * [Setting up internet access](https://
 cloud.google.com/composer/docs/concepts/private-
 ip#public_internet_access_for_your_workflows) > * [About service accounts for
 Cloud Composer](https://cloud.google.com/composer/docs/composer-2/access-
-control#about-service) ## ð± How to use Use the `VertFlowOperator` to
-instantiate a task in your DAG. Provide: * The address of the Docker image to
-run. * A runtime specification, e.g. timeout and memory limits. * A set of
-allowed regions to run the job in, based on your latency, data governance and
-other considerations. VertFlow picks the greenest one. ```python from
+control#about-service) ## ð± How to use Use the [`VertFlowOperator`](https://
+github.com/ovotech/VertFlow/blob/main/src/operator.py#L30) to instantiate a
+task in your DAG. Provide: * The address of the Docker image to run. * A
+runtime specification, e.g. timeout and memory limits. * A set of allowed
+regions to run the job in, based on your latency, data governance and other
+considerations. VertFlow picks the greenest one. ```python from
 VertFlow.operator import VertFlowOperator from airflow import DAG with DAG
 ( dag_id="hourly_dag_in_green_region", schedule_interval="@hourly" ) as dag:
 task = VertFlowOperator( image_address="us-docker.pkg.dev/cloudrun/container/
 job:latest", name="hello-world", allowed_regions=["europe-west1", "europe-
 west4"], command="echo", arguments=["Hello World"],
 service_account_email_address="my-service-account@embroidered-elephant-
 739.iam.gserviceaccount.com", ... ) ``` ## ððº Shout out to CO2 Signal
```

### Comparing `VertFlow-0.3.0/VertFlow.egg-info/PKG-INFO` & `VertFlow-0.4.0/VertFlow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VertFlow
-Version: 0.3.0
+Version: 0.4.0
 Summary: Apache Airflow operator for running Google Cloud Run Jobs using green energy
 Home-page: https://github.com/ovotech/VertFlow
 Author: OVO Energy
 Author-email: trading.dl@ovoenergy.com
 License: Apache 2.0
 Keywords: airflow,gcp,google,cloud run,cloud composer,green,environment,sustainability
 Requires-Python: >=3.7
@@ -48,15 +48,15 @@
 > ℹ️ If you're using Cloud Composer, these instructions may be helpful:
 > * [Installing PyPI packages](https://cloud.google.com/composer/docs/how-to/using/installing-python-dependencies#install-package)
 > * [Setting up internet access](https://cloud.google.com/composer/docs/concepts/private-ip#public_internet_access_for_your_workflows)
 > * [About service accounts for Cloud Composer](https://cloud.google.com/composer/docs/composer-2/access-control#about-service)
 
 ## 🖱 How to use
 
-Use the `VertFlowOperator` to instantiate a task in your DAG.
+Use the [`VertFlowOperator`](https://github.com/ovotech/VertFlow/blob/main/src/operator.py#L30) to instantiate a task in your DAG.
 Provide:
 
 * The address of the Docker image to run.
 * A runtime specification, e.g. timeout and memory limits.
 * A set of allowed regions to run the job in, based on your latency, data governance and other considerations. VertFlow
   picks the greenest one.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VertFlow Version: 0.3.0 Summary: Apache Airflow
+Metadata-Version: 2.1 Name: VertFlow Version: 0.4.0 Summary: Apache Airflow
 operator for running Google Cloud Run Jobs using green energy Home-page: https:
 //github.com/ovotech/VertFlow Author: OVO Energy Author-email:
 trading.dl@ovoenergy.com License: Apache 2.0 Keywords: airflow,gcp,google,cloud
 run,cloud composer,green,environment,sustainability Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
                                    VertFlow
@@ -28,19 +28,20 @@
 called `VERTFLOW_API_KEY`. > â¹ï¸ If you're using Cloud Composer, these
 instructions may be helpful: > * [Installing PyPI packages](https://
 cloud.google.com/composer/docs/how-to/using/installing-python-
 dependencies#install-package) > * [Setting up internet access](https://
 cloud.google.com/composer/docs/concepts/private-
 ip#public_internet_access_for_your_workflows) > * [About service accounts for
 Cloud Composer](https://cloud.google.com/composer/docs/composer-2/access-
-control#about-service) ## ð± How to use Use the `VertFlowOperator` to
-instantiate a task in your DAG. Provide: * The address of the Docker image to
-run. * A runtime specification, e.g. timeout and memory limits. * A set of
-allowed regions to run the job in, based on your latency, data governance and
-other considerations. VertFlow picks the greenest one. ```python from
+control#about-service) ## ð± How to use Use the [`VertFlowOperator`](https://
+github.com/ovotech/VertFlow/blob/main/src/operator.py#L30) to instantiate a
+task in your DAG. Provide: * The address of the Docker image to run. * A
+runtime specification, e.g. timeout and memory limits. * A set of allowed
+regions to run the job in, based on your latency, data governance and other
+considerations. VertFlow picks the greenest one. ```python from
 VertFlow.operator import VertFlowOperator from airflow import DAG with DAG
 ( dag_id="hourly_dag_in_green_region", schedule_interval="@hourly" ) as dag:
 task = VertFlowOperator( image_address="us-docker.pkg.dev/cloudrun/container/
 job:latest", name="hello-world", allowed_regions=["europe-west1", "europe-
 west4"], command="echo", arguments=["Hello World"],
 service_account_email_address="my-service-account@embroidered-elephant-
 739.iam.gserviceaccount.com", ... ) ``` ## ððº Shout out to CO2 Signal
```

### Comparing `VertFlow-0.3.0/setup.py` & `VertFlow-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/src/__init__.py` & `VertFlow-0.4.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/src/cloud_run.py` & `VertFlow-0.4.0/src/cloud_run.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/src/constants.py` & `VertFlow-0.4.0/src/constants.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/src/data.py` & `VertFlow-0.4.0/src/data.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/src/operator.py` & `VertFlow-0.4.0/src/operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import logging
 from typing import Sequence, Optional, List
 
-from .cloud_run import CloudRunJob, Secret
+from .cloud_run import CloudRunJob, Secret, SecretType
 from .data import CloudRunRegions
 from airflow import AirflowException
 from airflow.models import BaseOperator, Variable
 from airflow.utils.context import Context
 from google.auth import default
 
 ENVIRONMENT_GCP_PROJECT: str = default()[1]
@@ -33,15 +33,15 @@
         name: str,
         image_address: str,
         service_account_email_address: str,
         command: Optional[str] = None,
         arguments: Optional[List[str]] = None,
         project_id: Optional[str] = None,
         co2_signal_api_key: Optional[str] = None,
-        working_directory: str = "/",
+        working_directory: str = None,
         port_number: int = 8080,
         max_retries: int = 3,
         timeout_seconds: int = 300,
         initialisation_timeout_seconds: int = 60,
         cpu_limit: int = 1,
         environment_variables: Optional[dict] = None,
         memory_limit: str = "512Mi",
@@ -141,18 +141,27 @@
         logging.info(art)
         logging.info("VertFlow is finding the greenest region for your Cloud Run Job.")
         cloud_run_regions = CloudRunRegions(self.project_id, self.co2_signal_api_key)
 
         try:
             greenest = cloud_run_regions.greenest(self.allowed_regions)
             closest = cloud_run_regions.closest
+
+            saving = float(closest['carbon_intensity']) - float(greenest['carbon_intensity'])
+            if saving > 0:
+                outcome = f"{saving} gCO2eq/kWh less than"
+            elif saving < 0:
+                outcome = f"{saving} gCO2eq/kWh more than"
+            else:
+                outcome = "the same as"
+
             logging.info(
                 f"Deploying Cloud Run Job {self.name} in {greenest['name']} ({greenest['id']}) "
                 f"where carbon intensity is {greenest['carbon_intensity']} gCO2eq/kWh. "
-                f"This is {float(closest['carbon_intensity']) - float(greenest['carbon_intensity'])} gCO2eq/kWh lower than your closest region {closest['name']} ({closest['id']})."
+                f"This is {outcome} your closest region {closest['name']} ({closest['id']})."
             )
 
             greenest_region_id = str(greenest["id"])
 
         except (ConnectionError, LookupError) as e:
             greenest_region_id = str(
                 self.allowed_regions[0]
```

### Comparing `VertFlow-0.3.0/src/utils.py` & `VertFlow-0.4.0/src/utils.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/test/test_cloud_run.py` & `VertFlow-0.4.0/test/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/test/test_data.py` & `VertFlow-0.4.0/test/test_data.py`

 * *Files identical despite different names*

### Comparing `VertFlow-0.3.0/test/test_utils.py` & `VertFlow-0.4.0/test/test_utils.py`

 * *Files identical despite different names*

