# Comparing `tmp/volttron_lib_modbus_driver-0.1.1a1.tar.gz` & `tmp/volttron_lib_modbus_driver-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_modbus_driver-0.1.1a1.tar", max compression
+gzip compressed data, was "volttron_lib_modbus_driver-0.2.1rc0.tar", max compression
```

## Comparing `volttron_lib_modbus_driver-0.1.1a1.tar` & `volttron_lib_modbus_driver-0.2.1rc0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7944 2023-04-18 17:49:49.972229 volttron_lib_modbus_driver-0.1.1a1/README.md
--rw-r--r--   0        0        0     1720 2023-04-18 17:52:00.698105 volttron_lib_modbus_driver-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-18 17:49:49.972229 volttron_lib_modbus_driver-0.1.1a1/src/volttron/driver/interfaces/modbus/__init__.py
--rw-r--r--   0        0        0    17114 2023-04-18 17:49:49.972229 volttron_lib_modbus_driver-0.1.1a1/src/volttron/driver/interfaces/modbus/modbus.py
--rw-r--r--   0        0        0     8981 1970-01-01 00:00:00.000000 volttron_lib_modbus_driver-0.1.1a1/setup.py
--rw-r--r--   0        0        0     9045 1970-01-01 00:00:00.000000 volttron_lib_modbus_driver-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-05-12 16:52:39.656147 volttron_lib_modbus_driver-0.2.1rc0/LICENSE
+-rw-r--r--   0        0        0     7889 2023-05-12 16:52:39.656147 volttron_lib_modbus_driver-0.2.1rc0/README.md
+-rw-r--r--   0        0        0     1716 2023-05-12 16:54:11.571832 volttron_lib_modbus_driver-0.2.1rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 16:51:48.254724 volttron_lib_modbus_driver-0.2.1rc0/src/volttron/driver/interfaces/modbus/__init__.py
+-rw-r--r--   0        0        0    17114 2023-05-12 16:52:39.656147 volttron_lib_modbus_driver-0.2.1rc0/src/volttron/driver/interfaces/modbus/modbus.py
+-rw-r--r--   0        0        0     8892 1970-01-01 00:00:00.000000 volttron_lib_modbus_driver-0.2.1rc0/PKG-INFO
```

### Comparing `volttron_lib_modbus_driver-0.1.1a1/README.md` & `volttron_lib_modbus_driver-0.2.1rc0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,52 @@
 # volttron-lib-modbus-driver
 
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 ![Passing?](https://github.com/VOLTTRON/volttron-lib-modbus-driver/actions/workflows/run-tests.yml/badge.svg)
 [![pypi version](https://img.shields.io/pypi/v/volttron-lib-modbus-driver.svg)](https://pypi.org/project/volttron-lib-modbus-driver/)
 
-VOLTTRON’s modbus driver supports the Modbus over TCP/IP protocol only.
+> **Note**
+> VOLTTRON’s modbus driver supports the Modbus over TCP/IP protocol only.
 
-# Prerequisites
 
-* Python 3.8
+## Requires
 
-# Installation
+* python >=3.10
+* volttron-lib-base-driver
+* pymodbus >= 2.3.5
 
-1. Create and activate a virtual environment.
 
-    ```shell
-    python -m venv env
-    source env/bin/activate
-    ```
+# Documentation
+More detailed documentation can be found on [ReadTheDocs](https://volttron.readthedocs.io/en/modular/). The RST source
+of the documentation for this component is located in the "docs" directory of this repository.
 
-1. Install volttron and start the platform.
 
-    ```shell
-    pip install volttron
+# Installation
 
-    # Start platform with output going to volttron.log
-    volttron -vv -l volttron.log &
-    ```
+Before installing, VOLTTRON should be installed and running.  Its virtual environment should be active.
+Information on how to install of the VOLTTRON platform can be found
+[here](https://github.com/eclipse-volttron/volttron-core).
 
-1. Install the volttron platform driver:
+1. If it is not already, install the VOLTTRON Platform Driver Agent:
 
     ```shell
     vctl install volttron-platform-driver --vip-identity platform.driver --start
     ```
 
-1. Install the volttron-lib-modbus-driver library.
+2. Install the volttron-lib-modbus-driver library.
 
     ```shell
     pip install volttron-lib-modbus-driver
     ```
 
-1. Install the driver onto the Platform Driver.
-
-    Installing a driver in the Platform Driver Agent requires adding copies of the device configuration and registry configuration files to the Platform Driver’s configuration store.
-
-    Create a config directory and navigate to it:
-
-    ```shell
-    mkdir config
-    cd config
-    ```
+3. Store device and registry files for the Modbus device to the Platform Driver configuration store:
 
-    Navigate to the config directory and create a driver configuration file called `modbus.config`. There are three arguments for the driver_config section of the device configuration file:
+    Create a driver configuration file called `modbus.config`. There are three arguments for the driver_config section of the device configuration file:
 
     * device_address:  IP Address of the device.
 
     * port: Port the device is listening on. Defaults to 502 which is the standard port for Modbus devices.
 
     * slave_id:  Slave ID of the device. Defaults to 0. Use 0 for no slave.
 
@@ -76,31 +68,31 @@
     }
     ```
 
     Create another file called `mobus.csv`. This CSV file will be your modbus registry configuration file. Each row configures a point on the device.
 
     The following columns are required for each row:
 
-    * Volttron Point Name - The name by which the platform and agents running on the platform will refer to this point. For instance, if the Volttron Point Name is HeatCall1 (and using the example device configuration above) then an agent would use pnnl/isb2/hvac1/HeatCall1 to refer to the point when using the RPC interface of the actuator agent.
+    * Volttron Point Name - The name by which the platform and agents will refer to this point.
 
     * Units - Used for meta data when creating point information on the historian.
 
-    * Modbus Register - A string representing how to interpret the data register and how to read it from the device. The string takes two forms:
+    * Modbus Register - A string representing how to interpret the binary format of the data register. The string takes two forms:
 
         * “BOOL” for coils and discrete inputs.
 
-        * A format string for the Python struct module. See the Python3 Struct docs for full documentation. The supplied format string must only represent one value. See the documentation of your device to determine how to interpret the registers. Some Examples:
+        * A format string for the Python struct module. See the [Python3 Struct docs](http://docs.python.org/3/library/struct.html) for full documentation. The supplied format string must only represent one value. See the documentation of your device to determine how to interpret the registers. Some Examples:
 
         * “>f” - A big endian 32-bit floating point number.
 
         * “<H” - A little endian 16-bit unsigned integer.
 
         * “>l” - A big endian 32-bit integer.
 
-    * Writable - Either TRUE or FALSE. Determines if the point can be written to. Only points labeled TRUE can be written to through the ActuatorAgent.
+    * Writable - Either TRUE or FALSE. Determines if the point can be written to.
 
     * Point Address - Modbus address of the point. Cannot include any offset value, it must be the exact value of the address.
 
     * Mixed Endian - (Optional) Either TRUE or FALSE. For mixed endian values. This will reverse the order of the Modbus registers that make up this point before parsing the value or writing it out to the device. Has no effect on bit values.
 
     The following column is optional:
 
@@ -128,15 +120,15 @@
     Add modbus.csv and modbus.config to the configuration store:
 
     ```
     vctl config store platform.driver devices/campus/building/modbus modbus.config
     vctl config store platform.driver modbus.csv modbus.csv --csv
     ```
 
-1. Observe Data
+4. Observe Data
 
     To see data being published to the bus, install a [Listener Agent](https://pypi.org/project/volttron-listener/):
 
     ```
     vctl install volttron-listener --start
     ```
```

### Comparing `volttron_lib_modbus_driver-0.1.1a1/pyproject.toml` & `volttron_lib_modbus_driver-0.2.1rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 exclude = ['docs/']
 
 [tool.mypy-six.moves]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-modbus-driver"
-version = "0.1.1a1"
+version = "0.2.1rc0"
 description = "Modbus driver supported and maintained by the Volttron team."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-lib-modbus-driver"
 homepage = "https://github.com/VOLTTRON/volttron-lib-modbus-driver"
 keywords = []
@@ -29,16 +29,16 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-volttron-lib-base-driver="^0.2.0rc0"
+python = "^3.10"
+volttron-lib-base-driver="^0.2.1rc0"
 pymodbus = "^2.5.3"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.3.1a9"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 modbus-tk= "^1.1.2"
```

### Comparing `volttron_lib_modbus_driver-0.1.1a1/src/volttron/driver/interfaces/modbus/modbus.py` & `volttron_lib_modbus_driver-0.2.1rc0/src/volttron/driver/interfaces/modbus/modbus.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbus_driver-0.1.1a1/setup.py` & `volttron_lib_modbus_driver-0.2.1rc0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,189 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volttron-lib-modbus-driver
+Version: 0.2.1rc0
+Summary: Modbus driver supported and maintained by the Volttron team.
+Home-page: https://github.com/VOLTTRON/volttron-lib-modbus-driver
+License: Apache-2.0
+Author: Mark Bonicillo
+Author-email: volttron@pnnl.gov
+Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: pymodbus (>=2.5.3,<3.0.0)
+Requires-Dist: volttron-lib-base-driver (>=0.2.1rc0,<0.3.0)
+Project-URL: Repository, https://github.com/VOLTTRON/volttron-lib-modbus-driver
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# volttron-lib-modbus-driver
 
-packages = \
-['volttron', 'volttron.driver.interfaces.modbus']
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Passing?](https://github.com/VOLTTRON/volttron-lib-modbus-driver/actions/workflows/run-tests.yml/badge.svg)
+[![pypi version](https://img.shields.io/pypi/v/volttron-lib-modbus-driver.svg)](https://pypi.org/project/volttron-lib-modbus-driver/)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pymodbus>=2.5.3,<3.0.0', 'volttron-lib-base-driver>=0.2.0rc0,<0.3.0']
-
-setup_kwargs = {
-    'name': 'volttron-lib-modbus-driver',
-    'version': '0.1.1a1',
-    'description': 'Modbus driver supported and maintained by the Volttron team.',
-    'long_description': '# volttron-lib-modbus-driver\n\n![Passing?](https://github.com/VOLTTRON/volttron-lib-modbus-driver/actions/workflows/run-tests.yml/badge.svg)\n[![pypi version](https://img.shields.io/pypi/v/volttron-lib-modbus-driver.svg)](https://pypi.org/project/volttron-lib-modbus-driver/)\n\nVOLTTRON’s modbus driver supports the Modbus over TCP/IP protocol only.\n\n# Prerequisites\n\n* Python 3.8\n\n# Installation\n\n1. Create and activate a virtual environment.\n\n    ```shell\n    python -m venv env\n    source env/bin/activate\n    ```\n\n1. Install volttron and start the platform.\n\n    ```shell\n    pip install volttron\n\n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n\n1. Install the volttron platform driver:\n\n    ```shell\n    vctl install volttron-platform-driver --vip-identity platform.driver --start\n    ```\n\n1. Install the volttron-lib-modbus-driver library.\n\n    ```shell\n    pip install volttron-lib-modbus-driver\n    ```\n\n1. Install the driver onto the Platform Driver.\n\n    Installing a driver in the Platform Driver Agent requires adding copies of the device configuration and registry configuration files to the Platform Driver’s configuration store.\n\n    Create a config directory and navigate to it:\n\n    ```shell\n    mkdir config\n    cd config\n    ```\n\n    Navigate to the config directory and create a driver configuration file called `modbus.config`. There are three arguments for the driver_config section of the device configuration file:\n\n    * device_address:  IP Address of the device.\n\n    * port: Port the device is listening on. Defaults to 502 which is the standard port for Modbus devices.\n\n    * slave_id:  Slave ID of the device. Defaults to 0. Use 0 for no slave.\n\n    This repo provides an example configuration in the file "modbus_example.config".\n\n    Here is an example device configuration file:\n\n    ```json\n    {\n        "driver_config": {"device_address": "10.0.0.4"},\n        "driver_type": "modbus",\n        "registry_config":"config://catalyst371.csv",\n        "interval": 120,\n        "timezone": "UTC",\n        "campus": "campus",\n        "building": "building",\n        "unit": "modbus1",\n        "heart_beat_point": "ESMMode"\n    }\n    ```\n\n    Create another file called `mobus.csv`. This CSV file will be your modbus registry configuration file. Each row configures a point on the device.\n\n    The following columns are required for each row:\n\n    * Volttron Point Name - The name by which the platform and agents running on the platform will refer to this point. For instance, if the Volttron Point Name is HeatCall1 (and using the example device configuration above) then an agent would use pnnl/isb2/hvac1/HeatCall1 to refer to the point when using the RPC interface of the actuator agent.\n\n    * Units - Used for meta data when creating point information on the historian.\n\n    * Modbus Register - A string representing how to interpret the data register and how to read it from the device. The string takes two forms:\n\n        * “BOOL” for coils and discrete inputs.\n\n        * A format string for the Python struct module. See the Python3 Struct docs for full documentation. The supplied format string must only represent one value. See the documentation of your device to determine how to interpret the registers. Some Examples:\n\n        * “>f” - A big endian 32-bit floating point number.\n\n        * “<H” - A little endian 16-bit unsigned integer.\n\n        * “>l” - A big endian 32-bit integer.\n\n    * Writable - Either TRUE or FALSE. Determines if the point can be written to. Only points labeled TRUE can be written to through the ActuatorAgent.\n\n    * Point Address - Modbus address of the point. Cannot include any offset value, it must be the exact value of the address.\n\n    * Mixed Endian - (Optional) Either TRUE or FALSE. For mixed endian values. This will reverse the order of the Modbus registers that make up this point before parsing the value or writing it out to the device. Has no effect on bit values.\n\n    The following column is optional:\n\n    * Default Value - The default value for the point. When the point is reverted by an agent it will change back to this value. If this value is missing it will revert to the last known value not set by an agent.\n\n    Any additional columns will be ignored. It is common practice to include a Point Name or Reference Point Name to include the device documentation’s name for the point and Notes and Unit Details for additional information about a point.\n\n    The following is an example of a Modbus registry configuration file:\n\n    ```csv\n    Reference Point Name,Volttron Point Name,Units,Units Details,Modbus Register,Writable,Point Address,Default Value,Notes\n    CO2Sensor,ReturnAirCO2,PPM,0.00-2000.00,>f,FALSE,1001,,CO2 Reading 0.00-2000.0 ppm\n    CO2Stpt,ReturnAirCO2Stpt,PPM,1000.00 (default),>f,TRUE,1011,1000,Setpoint to enable demand control ventilation\n    Cool1Spd,CoolSupplyFanSpeed1,%,0.00 to 100.00 (75 default),>f,TRUE,1005,75,Fan speed on cool 1 call\n    Cool2Spd,CoolSupplyFanSpeed2,%,0.00 to 100.00 (90 default),>f,TRUE,1007,90,Fan speed on Cool2 Call\n    Damper,DamperSignal,%,0.00 - 100.00,>f,FALSE,1023,,Output to the economizer damper\n    DaTemp,DischargeAirTemperature,F,(-)39.99 to 248.00,>f,FALSE,1009,,Discharge air reading\n    ESMEconMin,ESMDamperMinPosition,%,0.00 to 100.00 (5 default),>f,TRUE,1013,5,Minimum damper position during the energy savings mode\n    FanPower,SupplyFanPower, kW,0.00 to 100.00,>f,FALSE,1015,,Fan power from drive\n    FanSpeed,SupplyFanSpeed,%,0.00 to 100.00,>f,FALSE,1003,,Fan speed from drive\n    HeatCall1,HeatCall1,On / Off,on/off,BOOL,FALSE,1113,,Status indicator of heating stage 1 need\n    HeartBeat,heartbeat,On / Off,on/off,BOOL,FALSE,1114,,Status indicator of heating stage 2 need\n    ```\n\n    Add modbus.csv and modbus.config to the configuration store:\n\n    ```\n    vctl config store platform.driver devices/campus/building/modbus modbus.config\n    vctl config store platform.driver modbus.csv modbus.csv --csv\n    ```\n\n1. Observe Data\n\n    To see data being published to the bus, install a [Listener Agent](https://pypi.org/project/volttron-listener/):\n\n    ```\n    vctl install volttron-listener --start\n    ```\n\n    Once installed, you should see the data being published by viewing the Volttron logs file that was created in step 2.\n    To watch the logs, open a separate terminal and run the following command:\n\n    ```\n    tail -f <path to folder containing volttron.log>/volttron.log\n    ```\n\n# Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
-    'author': 'Mark Bonicillo',
-    'author_email': 'volttron@pnnl.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/VOLTTRON/volttron-lib-modbus-driver',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+> **Note**
+> VOLTTRON’s modbus driver supports the Modbus over TCP/IP protocol only.
 
 
-setup(**setup_kwargs)
+## Requires
+
+* python >=3.10
+* volttron-lib-base-driver
+* pymodbus >= 2.3.5
+
+
+# Documentation
+More detailed documentation can be found on [ReadTheDocs](https://volttron.readthedocs.io/en/modular/). The RST source
+of the documentation for this component is located in the "docs" directory of this repository.
+
+
+# Installation
+
+Before installing, VOLTTRON should be installed and running.  Its virtual environment should be active.
+Information on how to install of the VOLTTRON platform can be found
+[here](https://github.com/eclipse-volttron/volttron-core).
+
+1. If it is not already, install the VOLTTRON Platform Driver Agent:
+
+    ```shell
+    vctl install volttron-platform-driver --vip-identity platform.driver --start
+    ```
+
+2. Install the volttron-lib-modbus-driver library.
+
+    ```shell
+    pip install volttron-lib-modbus-driver
+    ```
+
+3. Store device and registry files for the Modbus device to the Platform Driver configuration store:
+
+    Create a driver configuration file called `modbus.config`. There are three arguments for the driver_config section of the device configuration file:
+
+    * device_address:  IP Address of the device.
+
+    * port: Port the device is listening on. Defaults to 502 which is the standard port for Modbus devices.
+
+    * slave_id:  Slave ID of the device. Defaults to 0. Use 0 for no slave.
+
+    This repo provides an example configuration in the file "modbus_example.config".
+
+    Here is an example device configuration file:
+
+    ```json
+    {
+        "driver_config": {"device_address": "10.0.0.4"},
+        "driver_type": "modbus",
+        "registry_config":"config://catalyst371.csv",
+        "interval": 120,
+        "timezone": "UTC",
+        "campus": "campus",
+        "building": "building",
+        "unit": "modbus1",
+        "heart_beat_point": "ESMMode"
+    }
+    ```
+
+    Create another file called `mobus.csv`. This CSV file will be your modbus registry configuration file. Each row configures a point on the device.
+
+    The following columns are required for each row:
+
+    * Volttron Point Name - The name by which the platform and agents will refer to this point.
+
+    * Units - Used for meta data when creating point information on the historian.
+
+    * Modbus Register - A string representing how to interpret the binary format of the data register. The string takes two forms:
+
+        * “BOOL” for coils and discrete inputs.
+
+        * A format string for the Python struct module. See the [Python3 Struct docs](http://docs.python.org/3/library/struct.html) for full documentation. The supplied format string must only represent one value. See the documentation of your device to determine how to interpret the registers. Some Examples:
+
+        * “>f” - A big endian 32-bit floating point number.
+
+        * “<H” - A little endian 16-bit unsigned integer.
+
+        * “>l” - A big endian 32-bit integer.
+
+    * Writable - Either TRUE or FALSE. Determines if the point can be written to.
+
+    * Point Address - Modbus address of the point. Cannot include any offset value, it must be the exact value of the address.
+
+    * Mixed Endian - (Optional) Either TRUE or FALSE. For mixed endian values. This will reverse the order of the Modbus registers that make up this point before parsing the value or writing it out to the device. Has no effect on bit values.
+
+    The following column is optional:
+
+    * Default Value - The default value for the point. When the point is reverted by an agent it will change back to this value. If this value is missing it will revert to the last known value not set by an agent.
+
+    Any additional columns will be ignored. It is common practice to include a Point Name or Reference Point Name to include the device documentation’s name for the point and Notes and Unit Details for additional information about a point.
+
+    The following is an example of a Modbus registry configuration file:
+
+    ```csv
+    Reference Point Name,Volttron Point Name,Units,Units Details,Modbus Register,Writable,Point Address,Default Value,Notes
+    CO2Sensor,ReturnAirCO2,PPM,0.00-2000.00,>f,FALSE,1001,,CO2 Reading 0.00-2000.0 ppm
+    CO2Stpt,ReturnAirCO2Stpt,PPM,1000.00 (default),>f,TRUE,1011,1000,Setpoint to enable demand control ventilation
+    Cool1Spd,CoolSupplyFanSpeed1,%,0.00 to 100.00 (75 default),>f,TRUE,1005,75,Fan speed on cool 1 call
+    Cool2Spd,CoolSupplyFanSpeed2,%,0.00 to 100.00 (90 default),>f,TRUE,1007,90,Fan speed on Cool2 Call
+    Damper,DamperSignal,%,0.00 - 100.00,>f,FALSE,1023,,Output to the economizer damper
+    DaTemp,DischargeAirTemperature,F,(-)39.99 to 248.00,>f,FALSE,1009,,Discharge air reading
+    ESMEconMin,ESMDamperMinPosition,%,0.00 to 100.00 (5 default),>f,TRUE,1013,5,Minimum damper position during the energy savings mode
+    FanPower,SupplyFanPower, kW,0.00 to 100.00,>f,FALSE,1015,,Fan power from drive
+    FanSpeed,SupplyFanSpeed,%,0.00 to 100.00,>f,FALSE,1003,,Fan speed from drive
+    HeatCall1,HeatCall1,On / Off,on/off,BOOL,FALSE,1113,,Status indicator of heating stage 1 need
+    HeartBeat,heartbeat,On / Off,on/off,BOOL,FALSE,1114,,Status indicator of heating stage 2 need
+    ```
+
+    Add modbus.csv and modbus.config to the configuration store:
+
+    ```
+    vctl config store platform.driver devices/campus/building/modbus modbus.config
+    vctl config store platform.driver modbus.csv modbus.csv --csv
+    ```
+
+4. Observe Data
+
+    To see data being published to the bus, install a [Listener Agent](https://pypi.org/project/volttron-listener/):
+
+    ```
+    vctl install volttron-listener --start
+    ```
+
+    Once installed, you should see the data being published by viewing the Volttron logs file that was created in step 2.
+    To watch the logs, open a separate terminal and run the following command:
+
+    ```
+    tail -f <path to folder containing volttron.log>/volttron.log
+    ```
+
+# Development
+
+Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).
+
+Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)
+
+
+# Disclaimer Notice
+
+This material was prepared as an account of work sponsored by an agency of the
+United States Government.  Neither the United States Government nor the United
+States Department of Energy, nor Battelle, nor any of their employees, nor any
+jurisdiction or organization that has cooperated in the development of these
+materials, makes any warranty, express or implied, or assumes any legal
+liability or responsibility for the accuracy, completeness, or usefulness or any
+information, apparatus, product, software, or process disclosed, or represents
+that its use would not infringe privately owned rights.
+
+Reference herein to any specific commercial product, process, or service by
+trade name, trademark, manufacturer, or otherwise does not necessarily
+constitute or imply its endorsement, recommendation, or favoring by the United
+States Government or any agency thereof, or Battelle Memorial Institute. The
+views and opinions of authors expressed herein do not necessarily state or
+reflect those of the United States Government or any agency thereof.
+
```

