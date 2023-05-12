# Comparing `tmp/volttron_dnp3_outstation-0.1.1a4.tar.gz` & `tmp/volttron_dnp3_outstation-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_dnp3_outstation-0.1.1a4.tar", max compression
+gzip compressed data, was "volttron_dnp3_outstation-0.1.1a5.tar", max compression
```

## Comparing `volttron_dnp3_outstation-0.1.1a4.tar` & `volttron_dnp3_outstation-0.1.1a5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-04 15:25:51.487707 volttron_dnp3_outstation-0.1.1a4/LICENSE
--rw-r--r--   0        0        0    16562 2023-05-04 15:25:51.487707 volttron_dnp3_outstation-0.1.1a4/README.md
--rw-r--r--   0        0        0     1996 2023-05-04 15:27:11.649717 volttron_dnp3_outstation-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 15:25:51.491707 volttron_dnp3_outstation-0.1.1a4/src/dnp3_outstation/__init__.py
--rw-r--r--   0        0        0    10014 2023-05-04 15:25:51.491707 volttron_dnp3_outstation-0.1.1a4/src/dnp3_outstation/agent.py
--rw-r--r--   0        0        0        0 2023-05-04 15:25:51.491707 volttron_dnp3_outstation-0.1.1a4/src/vdnp3_outstation/__init__.py
--rw-r--r--   0        0        0       89 2023-05-04 15:25:51.491707 volttron_dnp3_outstation-0.1.1a4/src/vdnp3_outstation/__main__.py
--rw-r--r--   0        0        0    10858 2023-05-04 15:25:51.491707 volttron_dnp3_outstation-0.1.1a4/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py
--rw-r--r--   0        0        0    18139 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.1a4/setup.py
--rw-r--r--   0        0        0    17923 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-05-12 17:50:04.585387 volttron_dnp3_outstation-0.1.1a5/LICENSE
+-rw-r--r--   0        0        0    17123 2023-05-12 17:50:04.585387 volttron_dnp3_outstation-0.1.1a5/README.md
+-rw-r--r--   0        0        0     1996 2023-05-12 17:52:53.693282 volttron_dnp3_outstation-0.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 17:50:04.589387 volttron_dnp3_outstation-0.1.1a5/src/dnp3_outstation/__init__.py
+-rw-r--r--   0        0        0    10014 2023-05-12 17:50:04.589387 volttron_dnp3_outstation-0.1.1a5/src/dnp3_outstation/agent.py
+-rw-r--r--   0        0        0        0 2023-05-12 17:50:04.589387 volttron_dnp3_outstation-0.1.1a5/src/vdnp3_outstation/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-12 17:50:04.589387 volttron_dnp3_outstation-0.1.1a5/src/vdnp3_outstation/__main__.py
+-rw-r--r--   0        0        0    10858 2023-05-12 17:50:04.589387 volttron_dnp3_outstation-0.1.1a5/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py
+-rw-r--r--   0        0        0    18702 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.1a5/setup.py
+-rw-r--r--   0        0        0    18484 1970-01-01 00:00:00.000000 volttron_dnp3_outstation-0.1.1a5/PKG-INFO
```

### Comparing `volttron_dnp3_outstation-0.1.1a4/LICENSE` & `volttron_dnp3_outstation-0.1.1a5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,23 @@
-                                 Apache License
+Copyright 2022 Battelle Memorial Institute
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not
+use this file except in compliance with the License. You may obtain a copy
+of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+License for the specific language governing permissions and limitations
+under the License.
+
+
+                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
@@ -194,8 +209,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `volttron_dnp3_outstation-0.1.1a4/README.md` & `volttron_dnp3_outstation-0.1.1a5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # volttron-dnp3-outstation
 
-[//]: # (TODO: get the badges)
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Pytests](https://github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-dnp3-outstation.svg)](https://pypi.org/project/volttron-dnp3-outstation/)
 
 Distributed Network Protocol (DNP
 or [DNP3](https://en.wikipedia.org/wiki/DNP3))
 has achieved a large-scale acceptance since its introduction in 1993. This
 protocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of
 critical infrastructure status, allowing for reliable remote control.
 
@@ -36,19 +40,19 @@
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
-# install Python 3.8
-pyenv install 3.8.10
+# install Python 3.10
+pyenv install 3.10
 
 # make it available globally
-pyenv global system 3.8.10
+pyenv global system 3.10
 ```
 
 </details>
 
 # Installation
 
 The following recipe walks through the steps to install and configure a DNP3 agent. Note that it uses default setup to
@@ -66,15 +70,14 @@
     ```
 
 1. Install volttron and start the platform.
 
    > **Note**:
    > According to the [volttron-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME
    > environment variable is mandatory:
-
    > ... if you have/had in the past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME
    > $HOME/.volttron. This modular version of VOLTTRON cannot work with volttron_home used by monolithic version of
    > VOLTTRON(version 8.3 or earlier)
 
     ```shell
     # Setup environment variable `VOLTTRON_HOME`
     export VOLTTRON_HOME=<path-to-volttron_home-dir>
@@ -84,16 +87,15 @@
     ```
 
 1. Install the "volttron-dnp3-outstation" dependency.
 
    There are two options to install the DNP3 Driver. You can install this library using the version on PyPi or install
    it from the source code (`git clone` might be required.)
    Note: the `vctl install` command in the following step can handle dependency installation using pypi. However, in
-   this demo we
-   demonstrate what is happening under the neath the hood by separating the dependency installation and agent registry
+   this demo we demonstrate what is happening under the neath the hood by separating the dependency installation and agent registry
    steps.
 
     ```shell
     # option 1: install from pypi
     pip install volttron-dnp3-outstation
     
     # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,43 +1,51 @@
-# volttron-dnp3-outstation [//]: # (TODO: get the badges) Distributed Network
-Protocol (DNP or [DNP3](https://en.wikipedia.org/wiki/DNP3)) has achieved a
-large-scale acceptance since its introduction in 1993. This protocol is an
-immediately deployable solution for monitoring remote sites because it was
-developed for communication of critical infrastructure status, allowing for
-reliable remote control. DNP3 is typically used between centrally located
-masters and distributed remotes. Application layer fragments from Master DNP3
-stations are typically requests for operations on data objects, and application
-layer fragments from Slave DNP3 stations (i.e., Outstation) are typically
-responses to those requests. A DNP3 Outstation may also transmit a message
-without a request (an unsolicited response). The volttron-dnp3-outstation is an
-implementation of the DNP3 master following the [VOLTTRON Agent Specifications]
-(https://volttron.readthedocs.io/en/main/developing-volttron/developing-agents/
-specifications/index.html?highlight=agent#agent-specifications). Note: to fully
-desmonstate the volttron-dnp3-outstation features, including polling data,
-setting point values, etc., it is suggested to establish connection between an
-outstation and a DNP3 master instance. The [dnp3-python](https://github.com/
-VOLTTRON/dnp3-python) can provide the essential master functionality, and as
-part of the volttron-dnp3-outstation dependency, it is immediately available
-after the volttron-dnp3-outstation is installed. # Prerequisites * Python 3
-(tested with Python3.8, Python3.9, Python3.10) ## Python  To install specific
-Python version (e.g., Python 3.8), we recommend using pyenv. ```shell # install
-pyenv git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you
-should also put these three lines in .bashrc or similar) export PATH="$
-{HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv
-init -)" # install Python 3.8 pyenv install 3.8.10 # make it available globally
-pyenv global system 3.8.10 ```  # Installation The following recipe walks
-through the steps to install and configure a DNP3 agent. Note that it uses
-default setup to work out-of-the-box. Please feel free to refer to related
-documentations for details. 1. Create and activate a virtual environment. It is
-recommended to use a virtual environment for installing volttron. ```shell
-python -m venv env source env/bin/activate pip install volttron ``` 1. Install
-volttron and start the platform. > **Note**: > According to the [volttron-
-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup
-VOLTTRON_HOME > environment variable is mandatory: > ... if you have/had in the
-past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME >
+# volttron-dnp3-outstation [![Eclipse VOLTTRONâ¢](https://img.shields.io/
+badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/
+) ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg) ![Python
+3.11](https://img.shields.io/badge/python-3.11-blue.svg) [![Pytests](https://
+github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-
+tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-dnp3-
+outstation/actions/workflows/run-tests.yml) [![pypi version](https://
+img.shields.io/pypi/v/volttron-dnp3-outstation.svg)](https://pypi.org/project/
+volttron-dnp3-outstation/) Distributed Network Protocol (DNP or [DNP3](https://
+en.wikipedia.org/wiki/DNP3)) has achieved a large-scale acceptance since its
+introduction in 1993. This protocol is an immediately deployable solution for
+monitoring remote sites because it was developed for communication of critical
+infrastructure status, allowing for reliable remote control. DNP3 is typically
+used between centrally located masters and distributed remotes. Application
+layer fragments from Master DNP3 stations are typically requests for operations
+on data objects, and application layer fragments from Slave DNP3 stations
+(i.e., Outstation) are typically responses to those requests. A DNP3 Outstation
+may also transmit a message without a request (an unsolicited response). The
+volttron-dnp3-outstation is an implementation of the DNP3 master following the
+[VOLTTRON Agent Specifications](https://volttron.readthedocs.io/en/main/
+developing-volttron/developing-agents/specifications/
+index.html?highlight=agent#agent-specifications). Note: to fully desmonstate
+the volttron-dnp3-outstation features, including polling data, setting point
+values, etc., it is suggested to establish connection between an outstation and
+a DNP3 master instance. The [dnp3-python](https://github.com/VOLTTRON/dnp3-
+python) can provide the essential master functionality, and as part of the
+volttron-dnp3-outstation dependency, it is immediately available after the
+volttron-dnp3-outstation is installed. # Prerequisites * Python 3 (tested with
+Python3.8, Python3.9, Python3.10) ## Python  To install specific Python version
+(e.g., Python 3.8), we recommend using pyenv. ```shell # install pyenv git
+clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also
+put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:$
+{PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install
+Python 3.10 pyenv install 3.10 # make it available globally pyenv global system
+3.10 ```  # Installation The following recipe walks through the steps to
+install and configure a DNP3 agent. Note that it uses default setup to work
+out-of-the-box. Please feel free to refer to related documentations for
+details. 1. Create and activate a virtual environment. It is recommended to use
+a virtual environment for installing volttron. ```shell python -m venv env
+source env/bin/activate pip install volttron ``` 1. Install volttron and start
+the platform. > **Note**: > According to the [volttron-core#README](https://
+github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME >
+environment variable is mandatory: > ... if you have/had in the past, a
+monolithic VOLTTRON version that used the default VOLTTRON_HOME >
 $HOME/.volttron. This modular version of VOLTTRON cannot work with
 volttron_home used by monolithic version of > VOLTTRON(version 8.3 or earlier)
 ```shell # Setup environment variable `VOLTTRON_HOME` export VOLTTRON_HOME= #
 Start platform with output going to volttron.log volttron -vv -l volttron.log &
 ``` 1. Install the "volttron-dnp3-outstation" dependency. There are two options
 to install the DNP3 Driver. You can install this library using the version on
 PyPi or install it from the source code (`git clone` might be required.) Note:
```

### Comparing `volttron_dnp3_outstation-0.1.1a4/pyproject.toml` & `volttron_dnp3_outstation-0.1.1a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-dnp3-outstation"
-version = "0.1.1a4"
+version = "0.1.1a5"
 description = "A Volttron agent that acts as a dnp3 outstation."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-dnp3-outstation"
 repository = "https://github.com/eclipse-volttron/volttron-dnp3-outstation"
```

### Comparing `volttron_dnp3_outstation-0.1.1a4/src/dnp3_outstation/agent.py` & `volttron_dnp3_outstation-0.1.1a5/src/dnp3_outstation/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_dnp3_outstation-0.1.1a4/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py` & `volttron_dnp3_outstation-0.1.1a5/src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py`

 * *Files identical despite different names*

### Comparing `volttron_dnp3_outstation-0.1.1a4/setup.py` & `volttron_dnp3_outstation-0.1.1a5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['dnp3-python>=0.2.3b3', 'volttron>=10.0.2rc0']
 
 entry_points = \
 {'console_scripts': ['volttron-dnp3-outstation = dnp3_outstation.agent:main']}
 
 setup_kwargs = {
     'name': 'volttron-dnp3-outstation',
-    'version': '0.1.1a4',
+    'version': '0.1.1a5',
     'description': 'A Volttron agent that acts as a dnp3 outstation.',
-    'long_description': '# volttron-dnp3-outstation\n\n[//]: # (TODO: get the badges)\n\nDistributed Network Protocol (DNP\nor [DNP3](https://en.wikipedia.org/wiki/DNP3))\nhas achieved a large-scale acceptance since its introduction in 1993. This\nprotocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of\ncritical infrastructure status, allowing for reliable remote control.\n\nDNP3 is typically used between centrally located masters and distributed remotes.\nApplication layer fragments from Master DNP3 stations are typically requests for operations on data\nobjects, and application layer fragments from Slave DNP3 stations (i.e., Outstation) are typically responses to those\nrequests. A DNP3 Outstation may also transmit a message without a request (an unsolicited response).\nThe volttron-dnp3-outstation is an implementation of the DNP3 master following\nthe [VOLTTRON Agent Specifications](https://volttron.readthedocs.io/en/main/developing-volttron/developing-agents/specifications/index.html?highlight=agent#agent-specifications).\n\nNote: to fully desmonstate the volttron-dnp3-outstation features, including polling data, setting point\nvalues, etc., it is suggested to establish connection between an outstation and a DNP3 master instance.\nThe [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can provide the essential master functionality,\nand as\npart of the volttron-dnp3-outstation dependency, it is immediately available after the volttron-dnp3-outstation is\ninstalled.\n\n# Prerequisites\n\n* Python 3 (tested with Python3.8, Python3.9, Python3.10)\n\n## Python\n\n<details>\n<summary>To install specific Python version (e.g., Python 3.8), we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>\n\n```shell\n# install pyenv\ngit clone https://github.com/pyenv/pyenv ~/.pyenv\n\n# setup pyenv (you should also put these three lines in .bashrc or similar)\nexport PATH="${HOME}/.pyenv/bin:${PATH}"\nexport PYENV_ROOT="${HOME}/.pyenv"\neval "$(pyenv init -)"\n\n# install Python 3.8\npyenv install 3.8.10\n\n# make it available globally\npyenv global system 3.8.10\n```\n\n</details>\n\n# Installation\n\nThe following recipe walks through the steps to install and configure a DNP3 agent. Note that it uses default setup to\nwork out-of-the-box. Please feel free to refer to related documentations for details.\n\n1. Create and activate a virtual environment.\n\n   It is recommended to use a virtual environment for installing volttron.\n\n    ```shell\n    python -m venv env\n    source env/bin/activate\n    \n    pip install volttron\n    ```\n\n1. Install volttron and start the platform.\n\n   > **Note**:\n   > According to the [volttron-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME\n   > environment variable is mandatory:\n\n   > ... if you have/had in the past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME\n   > $HOME/.volttron. This modular version of VOLTTRON cannot work with volttron_home used by monolithic version of\n   > VOLTTRON(version 8.3 or earlier)\n\n    ```shell\n    # Setup environment variable `VOLTTRON_HOME`\n    export VOLTTRON_HOME=<path-to-volttron_home-dir>\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n\n1. Install the "volttron-dnp3-outstation" dependency.\n\n   There are two options to install the DNP3 Driver. You can install this library using the version on PyPi or install\n   it from the source code (`git clone` might be required.)\n   Note: the `vctl install` command in the following step can handle dependency installation using pypi. However, in\n   this demo we\n   demonstrate what is happening under the neath the hood by separating the dependency installation and agent registry\n   steps.\n\n    ```shell\n    # option 1: install from pypi\n    pip install volttron-dnp3-outstation\n    \n    # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)\n    pip install [-e] <path-to-the-source-code-root>/volttron-dnp3-outstation/\n    ```\n\n1. Install and start the "volttron-dnp3-outstation" agent.\n\n   Prepare the default config files:\n\n    ```shell\n    # Create config file place holders\n    mkdir config\n    touch config/dnp3-outstation-config.json\n    ```\n\n   Edit the `dnp3-outstation-config.json` as follows:\n    ```json\n    {\n     "outstation_ip": "0.0.0.0",\n     "master_id": 2,\n     "outstation_id": 1,\n     "port":  21000\n    }\n    ```\n\n   Use `vctl install` command to register to the volttron home path.\n   Note: for demo purposes and reproducibility, we assign vip-identity as "dnp3_outstation", but you can choose\n   any other valid agent identity as desired.\n\n    ```shell\n    vctl install volttron-dnp3-outstation --agent-config <path-to-agent-config> \\\n   --vip-identity dnp3_outstation \\\n   --start\n    ```\n\n   (Optional) Use `vctl stauts` to verify the installation\n   ```shell\n   (env) kefei@ubuntu-22:~/sandbox/dnp3-outstation-sandbox$ vctl status\n   UUID   AGENT                             IDENTITY        TAG PRIORITY STATUS          HEALTH\n   e      volttron-dnp3-outstation-0.0.1rc0 dnp3_outstation              running [3408]  GOOD\n   ```\n\n# Basic Usage Example\n\nLike other VOLTTRON agent, the volttron-dnp3-outstation agent provides public interface and can be evoked by VOLTTRON\nRPC calls. The volttron-dnp3-outstation provided a commandline interface `vdnp3_outstation` as an RPC method wrapper.\nPlease see [run_volttron_dnp3_outstation_cli.py](./src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py) for\nimplementation details of the RPC examples.\n\n1. (Optional) Inspect the dnp3 outstation cli help menu.\n\n   ```shell\n   (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli -h\n   usage: dnp3-outstation [-h] [-aid <peer-name>]\n   \n   Run a dnp3 outstation agent. Specify agent identity, by default `dnp3_outstation`\n   \n   options:\n     -h, --help            show this help message and exit\n     -aid <peer-name>, --agent-identity <peer-name>\n                           specify agent identity (parsed as peer-name for rpc call), default \'dnp3_outstation\'.\n\n   ```\n\n1. Start the dnp3 outstation cli\n\n   Start the volttron-dnp3-outstation cli. If you\n   follow along this demo, the agent vip-identity should be "dnp3_outstation".\n\n   ```shell\n   (env) kefei@ubuntu-22:~/sandbox/dnp3-agent-sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli --agent-identity dnp3_outstation\n   2023-03-23 11:51:25,975 root DEBUG: Creating ZMQ Core None\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: address: ipc://@/home/kefei/.volttron/run/vip.socket\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: identity: 08953498-18e6-4070-9576-521bad3e82be\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: agent_uuid: None\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: serverkey: None\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG:  environ keys: dict_keys([\'SHELL\', \'SESSION_MANAGER\', \'QT_ACCESSIBILITY\', \'COLORTERM\', \'XDG_CONFIG_DIRS\', \'SSH_AGENT_LAUNCHER\', \'XDG_MENU_PREFIX\', \'GNOME_DESKTOP_SESSION_ID\', \'CONDA_EXE\', \'_CE_M\', \'GNOME_SHELL_SESSION_MODE\', \'SSH_AUTH_SOCK\', \'HOMEBREW_PREFIX\', \'XMODIFIERS\', \'DESKTOP_SESSION\', \'GTK_MODULES\', \'PWD\', \'LOGNAME\', \'XDG_SESSION_DESKTOP\', \'XDG_SESSION_TYPE\', \'MANPATH\', \'SYSTEMD_EXEC_PID\', \'XAUTHORITY\', \'VOLTTRON_HOME\', \'HOME\', \'USERNAME\', \'IM_CONFIG_PHASE\', \'LANG\', \'LS_COLORS\', \'XDG_CURRENT_DESKTOP\', \'VIRTUAL_ENV\', \'VTE_VERSION\', \'WAYLAND_DISPLAY\', \'GNOME_TERMINAL_SCREEN\', \'INFOPATH\', \'GNOME_SETUP_DISPLAY\', \'LESSCLOSE\', \'XDG_SESSION_CLASS\', \'TERM\', \'_CE_CONDA\', \'LESSOPEN\', \'USER\', \'HOMEBREW_CELLAR\', \'GNOME_TERMINAL_SERVICE\', \'CONDA_SHLVL\', \'DISPLAY\', \'SHLVL\', \'QT_IM_MODULE\', \'HOMEBREW_REPOSITORY\', \'VIRTUAL_ENV_PROMPT\', \'CONDA_PYTHON_EXE\', \'XDG_RUNTIME_DIR\', \'PS1\', \'XDG_DATA_DIRS\', \'PATH\', \'GDMSESSION\', \'DBUS_SESSION_BUS_ADDRESS\', \'_\', \'RABBITMQ_NOT_AVAILABLE\'])\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG: server key from env None\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG: AGENT RUNNING on ZMQ Core 08953498-18e6-4070-9576-521bad3e82be\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG: keys: server: _M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4 public: _M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4, secret: yfjc9g5znWMEjTSX3kfINGwhCvaDI80fK8vN76-C7SQ\n   2023-03-23 11:51:25,977 volttron.client.vip.zmq_connection DEBUG: ZMQ connection 08953498-18e6-4070-9576-521bad3e82be\n   2023-03-23 11:51:25,977 volttron.client.vip.zmq_connection DEBUG: connecting to url ipc://@/home/kefei/.volttron/run/vip.socket?publickey=_M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4&secretkey=yfjc9g5znWMEjTSX3kfINGwhCvaDI80fK8vN76-C7SQ&serverkey=_M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4\n   2023-03-23 11:51:25,977 volttron.client.vip.zmq_connection DEBUG: url type is <class \'str\'>\n   2023-03-23 11:51:25,981 volttron.client.vip.agent.core INFO: Connected to platform: identity: 08953498-18e6-4070-9576-521bad3e82be version: 1.0\n   2023-03-23 11:51:25,981 volttron.client.vip.agent.core DEBUG: Running onstart methods.\n    \n   ========================= MENU ==================================\n   <ai> - set analog-input point value\n   <ao> - set analog-output point value\n   <bi> - set binary-input point value\n   <bo> - set binary-output point value\n    \n   <dd> - display database\n   <di> - display (outstation) info\n   <cr> - config then restart outstation\n   =================================================================\n    \n   !!!!!!!!! WARNING: The outstation is NOT connected !!!!!!!!!\n   {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1, \'peer\': \'dnp3_outstation\'}\n    \n   ======== Your Input Here: ==(DNP3 OutStation Agent)======\n \n   ```\n\n1. Start a dnp3 master to establish connection.\n\n   If there is no connection between an outstation and a master, you may see the\n   warning `!!!!!!!!! WARNING: The outstation is NOT connected !!!!!!!!!`. To establish such a connection, **open\n   another terminal**, and\n   run `dnp3demo master`. (More details about the "dnp3demo" module, please\n   see [dnp3demo-Module.md](https://github.com/VOLTTRON/dnp3-python/blob/main/docs/dnp3demo-Module.md))\n\n   ```shell\n    ===== Master Operation MENU ==================================\n    <ao> - set analog-output point value (for remote control)\n    <bo> - set binary-output point value (for remote control)\n    <dd> - display/polling (outstation) database\n    <dc> - display configuration\n    =================================================================\n\n    \n    ======== Your Input Here: ==(master)======\n    ```\n\n   Note: by default, both the volttron-dnp3-outstation and the dnp3demo master uses configurations to\n   assure valid connection out-of-the-box. e.g., port=20000. Feel free to configure the connection parameters as\n   desired.\n\n1. Basic volttron-dnp3-outstation operations\n     ```\n   ======== Your Input Here: ==(DNP3 OutStation Agent)======\n   ai\n   You chose <ai> - set analog-input point value\n   Type in <float> and <index>. Separate with space, then hit ENTER. e.g., `1.4321, 1`.\n   Type \'q\', \'quit\', \'exit\' to main menu.\n\n    ======== Your Input Here: ==(DNP3 OutStation Agent)======\n    0.1212 0\n    {\'Analog\': {0: 0.1212, 1: None, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n     \n     \n    ======== Your Input Here: ==(DNP3 OutStation Agent)======\n    1.2323 1\n    {\'Analog\': {0: 0.1212, 1: 1.2323, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n   ```\n     <details>\n     <summary>Example of interaction with the `vdnp3_outstation` module </summary>\n\n     ```shell\n     (env) kefei@ubuntu-22:~/sandbox/dnp3-agent-sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli --agent-identity dnp3_outstation\n     dnp3demo.run_outstation {\'command\': \'outstation\', \'outstation_ip=\': \'0.0.0.0\', \'port=\': 20000, \'master_id=\': 2, \'outstation_id=\': 1}\n     ms(1678770551216) INFO    manager - Starting thread (0)\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n     ms(1678770551216) INFO    server - Listening on: 0.0.0.0:20000\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n     Connection error.\n     Connection Config {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1}\n     Start retry...\n     Connection error.\n     Connection Config {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1}\n     ms(1678770565247) INFO    server - Accepted connection from: 127.0.0.1\n     ==== Outstation Operation MENU ==================================\n     <ai> - update analog-input point value (for local reading)\n     <ao> - update analog-output point value (for local control)\n     <bi> - update binary-input point value (for local reading)\n     <bo> - update binary-output point value (for local control)\n     <dd> - display database\n     <dc> - display configuration\n     =================================================================\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     ai\n     You chose <ai> - update analog-input point value (for local reading)\n     Type in <float> and <index>. Separate with space, then hit ENTER.\n     Type \'q\', \'quit\', \'exit\' to main menu.\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     0.1212 0\n     {\'Analog\': {0: 0.1212, 1: None, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n     You chose <ai> - update analog-input point value (for local reading)\n     Type in <float> and <index>. Separate with space, then hit ENTER.\n     Type \'q\', \'quit\', \'exit\' to main menu.\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     1.2323 1\n     {\'Analog\': {0: 0.1212, 1: 1.2323, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n     You chose <ai> - update analog-input point value (for local reading)\n     Type in <float> and <index>. Separate with space, then hit ENTER.\n     Type \'q\', \'quit\', \'exit\' to main menu.\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     ```\n     </details>\n\n# Development\n\nPlease see the following for contributing\nguidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide\nabout [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government. Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
+    'long_description': '# volttron-dnp3-outstation\n\n[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Pytests](https://github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-dnp3-outstation.svg)](https://pypi.org/project/volttron-dnp3-outstation/)\n\nDistributed Network Protocol (DNP\nor [DNP3](https://en.wikipedia.org/wiki/DNP3))\nhas achieved a large-scale acceptance since its introduction in 1993. This\nprotocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of\ncritical infrastructure status, allowing for reliable remote control.\n\nDNP3 is typically used between centrally located masters and distributed remotes.\nApplication layer fragments from Master DNP3 stations are typically requests for operations on data\nobjects, and application layer fragments from Slave DNP3 stations (i.e., Outstation) are typically responses to those\nrequests. A DNP3 Outstation may also transmit a message without a request (an unsolicited response).\nThe volttron-dnp3-outstation is an implementation of the DNP3 master following\nthe [VOLTTRON Agent Specifications](https://volttron.readthedocs.io/en/main/developing-volttron/developing-agents/specifications/index.html?highlight=agent#agent-specifications).\n\nNote: to fully desmonstate the volttron-dnp3-outstation features, including polling data, setting point\nvalues, etc., it is suggested to establish connection between an outstation and a DNP3 master instance.\nThe [dnp3-python](https://github.com/VOLTTRON/dnp3-python) can provide the essential master functionality,\nand as\npart of the volttron-dnp3-outstation dependency, it is immediately available after the volttron-dnp3-outstation is\ninstalled.\n\n# Prerequisites\n\n* Python 3 (tested with Python3.8, Python3.9, Python3.10)\n\n## Python\n\n<details>\n<summary>To install specific Python version (e.g., Python 3.8), we recommend using <a href="https://github.com/pyenv/pyenv"><code>pyenv</code></a>.</summary>\n\n```shell\n# install pyenv\ngit clone https://github.com/pyenv/pyenv ~/.pyenv\n\n# setup pyenv (you should also put these three lines in .bashrc or similar)\nexport PATH="${HOME}/.pyenv/bin:${PATH}"\nexport PYENV_ROOT="${HOME}/.pyenv"\neval "$(pyenv init -)"\n\n# install Python 3.10\npyenv install 3.10\n\n# make it available globally\npyenv global system 3.10\n```\n\n</details>\n\n# Installation\n\nThe following recipe walks through the steps to install and configure a DNP3 agent. Note that it uses default setup to\nwork out-of-the-box. Please feel free to refer to related documentations for details.\n\n1. Create and activate a virtual environment.\n\n   It is recommended to use a virtual environment for installing volttron.\n\n    ```shell\n    python -m venv env\n    source env/bin/activate\n    \n    pip install volttron\n    ```\n\n1. Install volttron and start the platform.\n\n   > **Note**:\n   > According to the [volttron-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME\n   > environment variable is mandatory:\n   > ... if you have/had in the past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME\n   > $HOME/.volttron. This modular version of VOLTTRON cannot work with volttron_home used by monolithic version of\n   > VOLTTRON(version 8.3 or earlier)\n\n    ```shell\n    # Setup environment variable `VOLTTRON_HOME`\n    export VOLTTRON_HOME=<path-to-volttron_home-dir>\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n\n1. Install the "volttron-dnp3-outstation" dependency.\n\n   There are two options to install the DNP3 Driver. You can install this library using the version on PyPi or install\n   it from the source code (`git clone` might be required.)\n   Note: the `vctl install` command in the following step can handle dependency installation using pypi. However, in\n   this demo we demonstrate what is happening under the neath the hood by separating the dependency installation and agent registry\n   steps.\n\n    ```shell\n    # option 1: install from pypi\n    pip install volttron-dnp3-outstation\n    \n    # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)\n    pip install [-e] <path-to-the-source-code-root>/volttron-dnp3-outstation/\n    ```\n\n1. Install and start the "volttron-dnp3-outstation" agent.\n\n   Prepare the default config files:\n\n    ```shell\n    # Create config file place holders\n    mkdir config\n    touch config/dnp3-outstation-config.json\n    ```\n\n   Edit the `dnp3-outstation-config.json` as follows:\n    ```json\n    {\n     "outstation_ip": "0.0.0.0",\n     "master_id": 2,\n     "outstation_id": 1,\n     "port":  21000\n    }\n    ```\n\n   Use `vctl install` command to register to the volttron home path.\n   Note: for demo purposes and reproducibility, we assign vip-identity as "dnp3_outstation", but you can choose\n   any other valid agent identity as desired.\n\n    ```shell\n    vctl install volttron-dnp3-outstation --agent-config <path-to-agent-config> \\\n   --vip-identity dnp3_outstation \\\n   --start\n    ```\n\n   (Optional) Use `vctl stauts` to verify the installation\n   ```shell\n   (env) kefei@ubuntu-22:~/sandbox/dnp3-outstation-sandbox$ vctl status\n   UUID   AGENT                             IDENTITY        TAG PRIORITY STATUS          HEALTH\n   e      volttron-dnp3-outstation-0.0.1rc0 dnp3_outstation              running [3408]  GOOD\n   ```\n\n# Basic Usage Example\n\nLike other VOLTTRON agent, the volttron-dnp3-outstation agent provides public interface and can be evoked by VOLTTRON\nRPC calls. The volttron-dnp3-outstation provided a commandline interface `vdnp3_outstation` as an RPC method wrapper.\nPlease see [run_volttron_dnp3_outstation_cli.py](./src/vdnp3_outstation/run_volttron_dnp3_outstation_cli.py) for\nimplementation details of the RPC examples.\n\n1. (Optional) Inspect the dnp3 outstation cli help menu.\n\n   ```shell\n   (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli -h\n   usage: dnp3-outstation [-h] [-aid <peer-name>]\n   \n   Run a dnp3 outstation agent. Specify agent identity, by default `dnp3_outstation`\n   \n   options:\n     -h, --help            show this help message and exit\n     -aid <peer-name>, --agent-identity <peer-name>\n                           specify agent identity (parsed as peer-name for rpc call), default \'dnp3_outstation\'.\n\n   ```\n\n1. Start the dnp3 outstation cli\n\n   Start the volttron-dnp3-outstation cli. If you\n   follow along this demo, the agent vip-identity should be "dnp3_outstation".\n\n   ```shell\n   (env) kefei@ubuntu-22:~/sandbox/dnp3-agent-sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli --agent-identity dnp3_outstation\n   2023-03-23 11:51:25,975 root DEBUG: Creating ZMQ Core None\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: address: ipc://@/home/kefei/.volttron/run/vip.socket\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: identity: 08953498-18e6-4070-9576-521bad3e82be\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: agent_uuid: None\n   2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: serverkey: None\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG:  environ keys: dict_keys([\'SHELL\', \'SESSION_MANAGER\', \'QT_ACCESSIBILITY\', \'COLORTERM\', \'XDG_CONFIG_DIRS\', \'SSH_AGENT_LAUNCHER\', \'XDG_MENU_PREFIX\', \'GNOME_DESKTOP_SESSION_ID\', \'CONDA_EXE\', \'_CE_M\', \'GNOME_SHELL_SESSION_MODE\', \'SSH_AUTH_SOCK\', \'HOMEBREW_PREFIX\', \'XMODIFIERS\', \'DESKTOP_SESSION\', \'GTK_MODULES\', \'PWD\', \'LOGNAME\', \'XDG_SESSION_DESKTOP\', \'XDG_SESSION_TYPE\', \'MANPATH\', \'SYSTEMD_EXEC_PID\', \'XAUTHORITY\', \'VOLTTRON_HOME\', \'HOME\', \'USERNAME\', \'IM_CONFIG_PHASE\', \'LANG\', \'LS_COLORS\', \'XDG_CURRENT_DESKTOP\', \'VIRTUAL_ENV\', \'VTE_VERSION\', \'WAYLAND_DISPLAY\', \'GNOME_TERMINAL_SCREEN\', \'INFOPATH\', \'GNOME_SETUP_DISPLAY\', \'LESSCLOSE\', \'XDG_SESSION_CLASS\', \'TERM\', \'_CE_CONDA\', \'LESSOPEN\', \'USER\', \'HOMEBREW_CELLAR\', \'GNOME_TERMINAL_SERVICE\', \'CONDA_SHLVL\', \'DISPLAY\', \'SHLVL\', \'QT_IM_MODULE\', \'HOMEBREW_REPOSITORY\', \'VIRTUAL_ENV_PROMPT\', \'CONDA_PYTHON_EXE\', \'XDG_RUNTIME_DIR\', \'PS1\', \'XDG_DATA_DIRS\', \'PATH\', \'GDMSESSION\', \'DBUS_SESSION_BUS_ADDRESS\', \'_\', \'RABBITMQ_NOT_AVAILABLE\'])\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG: server key from env None\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG: AGENT RUNNING on ZMQ Core 08953498-18e6-4070-9576-521bad3e82be\n   2023-03-23 11:51:25,976 volttron.client.vip.agent.core DEBUG: keys: server: _M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4 public: _M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4, secret: yfjc9g5znWMEjTSX3kfINGwhCvaDI80fK8vN76-C7SQ\n   2023-03-23 11:51:25,977 volttron.client.vip.zmq_connection DEBUG: ZMQ connection 08953498-18e6-4070-9576-521bad3e82be\n   2023-03-23 11:51:25,977 volttron.client.vip.zmq_connection DEBUG: connecting to url ipc://@/home/kefei/.volttron/run/vip.socket?publickey=_M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4&secretkey=yfjc9g5znWMEjTSX3kfINGwhCvaDI80fK8vN76-C7SQ&serverkey=_M0Ds3SfjECMrmXulHQZtPIlsYW7JwzXMXJH1Koy2T4\n   2023-03-23 11:51:25,977 volttron.client.vip.zmq_connection DEBUG: url type is <class \'str\'>\n   2023-03-23 11:51:25,981 volttron.client.vip.agent.core INFO: Connected to platform: identity: 08953498-18e6-4070-9576-521bad3e82be version: 1.0\n   2023-03-23 11:51:25,981 volttron.client.vip.agent.core DEBUG: Running onstart methods.\n    \n   ========================= MENU ==================================\n   <ai> - set analog-input point value\n   <ao> - set analog-output point value\n   <bi> - set binary-input point value\n   <bo> - set binary-output point value\n    \n   <dd> - display database\n   <di> - display (outstation) info\n   <cr> - config then restart outstation\n   =================================================================\n    \n   !!!!!!!!! WARNING: The outstation is NOT connected !!!!!!!!!\n   {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1, \'peer\': \'dnp3_outstation\'}\n    \n   ======== Your Input Here: ==(DNP3 OutStation Agent)======\n \n   ```\n\n1. Start a dnp3 master to establish connection.\n\n   If there is no connection between an outstation and a master, you may see the\n   warning `!!!!!!!!! WARNING: The outstation is NOT connected !!!!!!!!!`. To establish such a connection, **open\n   another terminal**, and\n   run `dnp3demo master`. (More details about the "dnp3demo" module, please\n   see [dnp3demo-Module.md](https://github.com/VOLTTRON/dnp3-python/blob/main/docs/dnp3demo-Module.md))\n\n   ```shell\n    ===== Master Operation MENU ==================================\n    <ao> - set analog-output point value (for remote control)\n    <bo> - set binary-output point value (for remote control)\n    <dd> - display/polling (outstation) database\n    <dc> - display configuration\n    =================================================================\n\n    \n    ======== Your Input Here: ==(master)======\n    ```\n\n   Note: by default, both the volttron-dnp3-outstation and the dnp3demo master uses configurations to\n   assure valid connection out-of-the-box. e.g., port=20000. Feel free to configure the connection parameters as\n   desired.\n\n1. Basic volttron-dnp3-outstation operations\n     ```\n   ======== Your Input Here: ==(DNP3 OutStation Agent)======\n   ai\n   You chose <ai> - set analog-input point value\n   Type in <float> and <index>. Separate with space, then hit ENTER. e.g., `1.4321, 1`.\n   Type \'q\', \'quit\', \'exit\' to main menu.\n\n    ======== Your Input Here: ==(DNP3 OutStation Agent)======\n    0.1212 0\n    {\'Analog\': {0: 0.1212, 1: None, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n     \n     \n    ======== Your Input Here: ==(DNP3 OutStation Agent)======\n    1.2323 1\n    {\'Analog\': {0: 0.1212, 1: 1.2323, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n    You chose <ai> - update analog-input point value (for local reading)\n    Type in <float> and <index>. Separate with space, then hit ENTER.\n    Type \'q\', \'quit\', \'exit\' to main menu.\n   ```\n     <details>\n     <summary>Example of interaction with the `vdnp3_outstation` module </summary>\n\n     ```shell\n     (env) kefei@ubuntu-22:~/sandbox/dnp3-agent-sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli --agent-identity dnp3_outstation\n     dnp3demo.run_outstation {\'command\': \'outstation\', \'outstation_ip=\': \'0.0.0.0\', \'port=\': 20000, \'master_id=\': 2, \'outstation_id=\': 1}\n     ms(1678770551216) INFO    manager - Starting thread (0)\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tINFO\tConnection Config\n     ms(1678770551216) INFO    server - Listening on: 0.0.0.0:20000\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n     2023-03-14 00:09:11,216\tcontrol_workflow_demo\tDEBUG\tInitialization complete. Outstation in command loop.\n     Connection error.\n     Connection Config {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1}\n     Start retry...\n     Connection error.\n     Connection Config {\'outstation_ip_str\': \'0.0.0.0\', \'port\': 20000, \'masterstation_id_int\': 2, \'outstation_id_int\': 1}\n     ms(1678770565247) INFO    server - Accepted connection from: 127.0.0.1\n     ==== Outstation Operation MENU ==================================\n     <ai> - update analog-input point value (for local reading)\n     <ao> - update analog-output point value (for local control)\n     <bi> - update binary-input point value (for local reading)\n     <bo> - update binary-output point value (for local control)\n     <dd> - display database\n     <dc> - display configuration\n     =================================================================\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     ai\n     You chose <ai> - update analog-input point value (for local reading)\n     Type in <float> and <index>. Separate with space, then hit ENTER.\n     Type \'q\', \'quit\', \'exit\' to main menu.\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     0.1212 0\n     {\'Analog\': {0: 0.1212, 1: None, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n     You chose <ai> - update analog-input point value (for local reading)\n     Type in <float> and <index>. Separate with space, then hit ENTER.\n     Type \'q\', \'quit\', \'exit\' to main menu.\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     1.2323 1\n     {\'Analog\': {0: 0.1212, 1: 1.2323, 2: None, 3: None, 4: None, 5: None, 6: None, 7: None, 8: None, 9: None}}\n     You chose <ai> - update analog-input point value (for local reading)\n     Type in <float> and <index>. Separate with space, then hit ENTER.\n     Type \'q\', \'quit\', \'exit\' to main menu.\n      \n      \n     ======== Your Input Here: ==(DNP3 OutStation Agent)======\n     ```\n     </details>\n\n# Development\n\nPlease see the following for contributing\nguidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide\nabout [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government. Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
     'author': 'Kefei Mo',
     'author_email': 'kefei.mo@pnnl.gov',
     'maintainer': 'Volttron Team',
     'maintainer_email': 'volttron@pnnl.gov',
     'url': 'https://github.com/eclipse-volttron/volttron-dnp3-outstation',
     'package_dir': package_dir,
     'packages': packages,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,25 +1,33 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src', 'vdnp3_outstation': 'src/vdnp3_outstation'} packages = \
 ['dnp3_outstation', 'vdnp3_outstation'] package_data = \ {'': ['*']}
 install_requires = \ ['dnp3-python>=0.2.3b3', 'volttron>=10.0.2rc0']
 entry_points = \ {'console_scripts': ['volttron-dnp3-outstation =
 dnp3_outstation.agent:main']} setup_kwargs = { 'name': 'volttron-dnp3-
-outstation', 'version': '0.1.1a4', 'description': 'A Volttron agent that acts
-as a dnp3 outstation.', 'long_description': '# volttron-dnp3-outstation\n\n[//
-]: # (TODO: get the badges)\n\nDistributed Network Protocol (DNP\nor [DNP3]
-(https://en.wikipedia.org/wiki/DNP3))\nhas achieved a large-scale acceptance
-since its introduction in 1993. This\nprotocol is an immediately deployable
-solution for monitoring remote sites because it was developed for communication
-of\ncritical infrastructure status, allowing for reliable remote
-control.\n\nDNP3 is typically used between centrally located masters and
-distributed remotes.\nApplication layer fragments from Master DNP3 stations are
-typically requests for operations on data\nobjects, and application layer
-fragments from Slave DNP3 stations (i.e., Outstation) are typically responses
-to those\nrequests. A DNP3 Outstation may also transmit a message without a
+outstation', 'version': '0.1.1a5', 'description': 'A Volttron agent that acts
+as a dnp3 outstation.', 'long_description': '# volttron-dnp3-outstation\n\n[!
+[Eclipse VOLTTRONâ¢](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)]
+(https://volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://
+img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://
+img.shields.io/badge/python-3.11-blue.svg)\n[![Pytests](https://github.com/
+eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml/
+badge.svg)](https://github.com/eclipse-volttron/volttron-dnp3-outstation/
+actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/
+v/volttron-dnp3-outstation.svg)](https://pypi.org/project/volttron-dnp3-
+outstation/)\n\nDistributed Network Protocol (DNP\nor [DNP3](https://
+en.wikipedia.org/wiki/DNP3))\nhas achieved a large-scale acceptance since its
+introduction in 1993. This\nprotocol is an immediately deployable solution for
+monitoring remote sites because it was developed for communication of\ncritical
+infrastructure status, allowing for reliable remote control.\n\nDNP3 is
+typically used between centrally located masters and distributed
+remotes.\nApplication layer fragments from Master DNP3 stations are typically
+requests for operations on data\nobjects, and application layer fragments from
+Slave DNP3 stations (i.e., Outstation) are typically responses to
+those\nrequests. A DNP3 Outstation may also transmit a message without a
 request (an unsolicited response).\nThe volttron-dnp3-outstation is an
 implementation of the DNP3 master following\nthe [VOLTTRON Agent
 Specifications](https://volttron.readthedocs.io/en/main/developing-volttron/
 developing-agents/specifications/index.html?highlight=agent#agent-
 specifications).\n\nNote: to fully desmonstate the volttron-dnp3-outstation
 features, including polling data, setting point\nvalues, etc., it is suggested
 to establish connection between an outstation and a DNP3 master instance.\nThe
@@ -28,73 +36,72 @@
 dependency, it is immediately available after the volttron-dnp3-outstation
 is\ninstalled.\n\n# Prerequisites\n\n* Python 3 (tested with Python3.8,
 Python3.9, Python3.10)\n\n## Python\n\n\nTo install specific Python version
 (e.g., Python 3.8), we recommend using pyenv.\n\n```shell\n# install pyenv\ngit
 clone https://github.com/pyenv/pyenv ~/.pyenv\n\n# setup pyenv (you should also
 put these three lines in .bashrc or similar)\nexport PATH="${HOME}/.pyenv/bin:$
 {PATH}"\nexport PYENV_ROOT="${HOME}/.pyenv"\neval "$(pyenv init -)"\n\n#
-install Python 3.8\npyenv install 3.8.10\n\n# make it available globally\npyenv
-global system 3.8.10\n```\n\n\n\n# Installation\n\nThe following recipe walks
+install Python 3.10\npyenv install 3.10\n\n# make it available globally\npyenv
+global system 3.10\n```\n\n\n\n# Installation\n\nThe following recipe walks
 through the steps to install and configure a DNP3 agent. Note that it uses
 default setup to\nwork out-of-the-box. Please feel free to refer to related
 documentations for details.\n\n1. Create and activate a virtual
 environment.\n\n It is recommended to use a virtual environment for installing
 volttron.\n\n ```shell\n python -m venv env\n source env/bin/activate\n \n pip
 install volttron\n ```\n\n1. Install volttron and start the platform.\n\n >
 **Note**:\n > According to the [volttron-core#README](https://github.com/
 eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME\n > environment
-variable is mandatory:\n\n > ... if you have/had in the past, a monolithic
+variable is mandatory:\n > ... if you have/had in the past, a monolithic
 VOLTTRON version that used the default VOLTTRON_HOME\n > $HOME/.volttron. This
 modular version of VOLTTRON cannot work with volttron_home used by monolithic
 version of\n > VOLTTRON(version 8.3 or earlier)\n\n ```shell\n # Setup
 environment variable `VOLTTRON_HOME`\n export VOLTTRON_HOME=\n \n # Start
 platform with output going to volttron.log\n volttron -vv -l volttron.log &\n
 ```\n\n1. Install the "volttron-dnp3-outstation" dependency.\n\n There are two
 options to install the DNP3 Driver. You can install this library using the
 version on PyPi or install\n it from the source code (`git clone` might be
 required.)\n Note: the `vctl install` command in the following step can handle
-dependency installation using pypi. However, in\n this demo we\n demonstrate
-what is happening under the neath the hood by separating the dependency
-installation and agent registry\n steps.\n\n ```shell\n # option 1: install
-from pypi\n pip install volttron-dnp3-outstation\n \n # option 2: install from
-the source code (Note: `-e` option to use editable mode, useful for
-development.)\n pip install [-e] /volttron-dnp3-outstation/\n ```\n\n1. Install
-and start the "volttron-dnp3-outstation" agent.\n\n Prepare the default config
-files:\n\n ```shell\n # Create config file place holders\n mkdir config\n touch
-config/dnp3-outstation-config.json\n ```\n\n Edit the `dnp3-outstation-
-config.json` as follows:\n ```json\n {\n "outstation_ip": "0.0.0.0",\n
-"master_id": 2,\n "outstation_id": 1,\n "port": 21000\n }\n ```\n\n Use `vctl
-install` command to register to the volttron home path.\n Note: for demo
-purposes and reproducibility, we assign vip-identity as "dnp3_outstation", but
-you can choose\n any other valid agent identity as desired.\n\n ```shell\n vctl
-install volttron-dnp3-outstation --agent-config  \\\n --vip-identity
-dnp3_outstation \\\n --start\n ```\n\n (Optional) Use `vctl stauts` to verify
-the installation\n ```shell\n (env) kefei@ubuntu-22:~/sandbox/dnp3-outstation-
-sandbox$ vctl status\n UUID AGENT IDENTITY TAG PRIORITY STATUS HEALTH\n e
-volttron-dnp3-outstation-0.0.1rc0 dnp3_outstation running [3408] GOOD\n
-```\n\n# Basic Usage Example\n\nLike other VOLTTRON agent, the volttron-dnp3-
-outstation agent provides public interface and can be evoked by VOLTTRON\nRPC
-calls. The volttron-dnp3-outstation provided a commandline interface
-`vdnp3_outstation` as an RPC method wrapper.\nPlease see
-[run_volttron_dnp3_outstation_cli.py](./src/vdnp3_outstation/
-run_volttron_dnp3_outstation_cli.py) for\nimplementation details of the RPC
-examples.\n\n1. (Optional) Inspect the dnp3 outstation cli help menu.\n\n
-```shell\n (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$ python -
-m vdnp3_outstation.run_volttron_dnp3_outstation_cli -h\n usage: dnp3-outstation
-[-h] [-aid ]\n \n Run a dnp3 outstation agent. Specify agent identity, by
-default `dnp3_outstation`\n \n options:\n -h, --help show this help message and
-exit\n -aid , --agent-identity \n specify agent identity (parsed as peer-name
-for rpc call), default \'dnp3_outstation\'.\n\n ```\n\n1. Start the dnp3
-outstation cli\n\n Start the volttron-dnp3-outstation cli. If you\n follow
-along this demo, the agent vip-identity should be "dnp3_outstation".\n\n
-```shell\n (env) kefei@ubuntu-22:~/sandbox/dnp3-agent-sandbox$ python -
-m vdnp3_outstation.run_volttron_dnp3_outstation_cli --agent-identity
-dnp3_outstation\n 2023-03-23 11:51:25,975 root DEBUG: Creating ZMQ Core None\n
-2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG: address: ipc://@/
-home/kefei/.volttron/run/vip.socket\n 2023-03-23 11:51:25,975
+dependency installation using pypi. However, in\n this demo we demonstrate what
+is happening under the neath the hood by separating the dependency installation
+and agent registry\n steps.\n\n ```shell\n # option 1: install from pypi\n pip
+install volttron-dnp3-outstation\n \n # option 2: install from the source code
+(Note: `-e` option to use editable mode, useful for development.)\n pip install
+[-e] /volttron-dnp3-outstation/\n ```\n\n1. Install and start the "volttron-
+dnp3-outstation" agent.\n\n Prepare the default config files:\n\n ```shell\n #
+Create config file place holders\n mkdir config\n touch config/dnp3-outstation-
+config.json\n ```\n\n Edit the `dnp3-outstation-config.json` as follows:\n
+```json\n {\n "outstation_ip": "0.0.0.0",\n "master_id": 2,\n "outstation_id":
+1,\n "port": 21000\n }\n ```\n\n Use `vctl install` command to register to the
+volttron home path.\n Note: for demo purposes and reproducibility, we assign
+vip-identity as "dnp3_outstation", but you can choose\n any other valid agent
+identity as desired.\n\n ```shell\n vctl install volttron-dnp3-outstation --
+agent-config  \\\n --vip-identity dnp3_outstation \\\n --start\n ```\n\n
+(Optional) Use `vctl stauts` to verify the installation\n ```shell\n (env)
+kefei@ubuntu-22:~/sandbox/dnp3-outstation-sandbox$ vctl status\n UUID AGENT
+IDENTITY TAG PRIORITY STATUS HEALTH\n e volttron-dnp3-outstation-0.0.1rc0
+dnp3_outstation running [3408] GOOD\n ```\n\n# Basic Usage Example\n\nLike
+other VOLTTRON agent, the volttron-dnp3-outstation agent provides public
+interface and can be evoked by VOLTTRON\nRPC calls. The volttron-dnp3-
+outstation provided a commandline interface `vdnp3_outstation` as an RPC method
+wrapper.\nPlease see [run_volttron_dnp3_outstation_cli.py](./src/
+vdnp3_outstation/run_volttron_dnp3_outstation_cli.py) for\nimplementation
+details of the RPC examples.\n\n1. (Optional) Inspect the dnp3 outstation cli
+help menu.\n\n ```shell\n (env) kefei@ubuntu-22:~/sandbox/dnp3-driver-sandbox$
+python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli -h\n usage: dnp3-
+outstation [-h] [-aid ]\n \n Run a dnp3 outstation agent. Specify agent
+identity, by default `dnp3_outstation`\n \n options:\n -h, --help show this
+help message and exit\n -aid , --agent-identity \n specify agent identity
+(parsed as peer-name for rpc call), default \'dnp3_outstation\'.\n\n ```\n\n1.
+Start the dnp3 outstation cli\n\n Start the volttron-dnp3-outstation cli. If
+you\n follow along this demo, the agent vip-identity should be
+"dnp3_outstation".\n\n ```shell\n (env) kefei@ubuntu-22:~/sandbox/dnp3-agent-
+sandbox$ python -m vdnp3_outstation.run_volttron_dnp3_outstation_cli --agent-
+identity dnp3_outstation\n 2023-03-23 11:51:25,975 root DEBUG: Creating ZMQ
+Core None\n 2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG:
+address: ipc://@/home/kefei/.volttron/run/vip.socket\n 2023-03-23 11:51:25,975
 volttron.client.vip.agent.core DEBUG: identity: 08953498-18e6-4070-9576-
 521bad3e82be\n 2023-03-23 11:51:25,975 volttron.client.vip.agent.core DEBUG:
 agent_uuid: None\n 2023-03-23 11:51:25,975 volttron.client.vip.agent.core
 DEBUG: serverkey: None\n 2023-03-23 11:51:25,976 volttron.client.vip.agent.core
 DEBUG: environ keys: dict_keys([\'SHELL\', \'SESSION_MANAGER\',
 \'QT_ACCESSIBILITY\', \'COLORTERM\', \'XDG_CONFIG_DIRS\',
 \'SSH_AGENT_LAUNCHER\', \'XDG_MENU_PREFIX\', \'GNOME_DESKTOP_SESSION_ID\',
```

### Comparing `volttron_dnp3_outstation-0.1.1a4/PKG-INFO` & `volttron_dnp3_outstation-0.1.1a5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-dnp3-outstation
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: A Volttron agent that acts as a dnp3 outstation.
 Home-page: https://github.com/eclipse-volttron/volttron-dnp3-outstation
 License: Apache-2.0
 Keywords: volttron,agent,dnp3,outstation,application
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
@@ -27,15 +27,19 @@
 Requires-Dist: volttron (>=10.0.2rc0)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-dnp3-outstation/issues
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-dnp3-outstation
 Description-Content-Type: text/markdown
 
 # volttron-dnp3-outstation
 
-[//]: # (TODO: get the badges)
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Pytests](https://github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-dnp3-outstation.svg)](https://pypi.org/project/volttron-dnp3-outstation/)
 
 Distributed Network Protocol (DNP
 or [DNP3](https://en.wikipedia.org/wiki/DNP3))
 has achieved a large-scale acceptance since its introduction in 1993. This
 protocol is an immediately deployable solution for monitoring remote sites because it was developed for communication of
 critical infrastructure status, allowing for reliable remote control.
 
@@ -67,19 +71,19 @@
 git clone https://github.com/pyenv/pyenv ~/.pyenv
 
 # setup pyenv (you should also put these three lines in .bashrc or similar)
 export PATH="${HOME}/.pyenv/bin:${PATH}"
 export PYENV_ROOT="${HOME}/.pyenv"
 eval "$(pyenv init -)"
 
-# install Python 3.8
-pyenv install 3.8.10
+# install Python 3.10
+pyenv install 3.10
 
 # make it available globally
-pyenv global system 3.8.10
+pyenv global system 3.10
 ```
 
 </details>
 
 # Installation
 
 The following recipe walks through the steps to install and configure a DNP3 agent. Note that it uses default setup to
@@ -97,15 +101,14 @@
     ```
 
 1. Install volttron and start the platform.
 
    > **Note**:
    > According to the [volttron-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME
    > environment variable is mandatory:
-
    > ... if you have/had in the past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME
    > $HOME/.volttron. This modular version of VOLTTRON cannot work with volttron_home used by monolithic version of
    > VOLTTRON(version 8.3 or earlier)
 
     ```shell
     # Setup environment variable `VOLTTRON_HOME`
     export VOLTTRON_HOME=<path-to-volttron_home-dir>
@@ -115,16 +118,15 @@
     ```
 
 1. Install the "volttron-dnp3-outstation" dependency.
 
    There are two options to install the DNP3 Driver. You can install this library using the version on PyPi or install
    it from the source code (`git clone` might be required.)
    Note: the `vctl install` command in the following step can handle dependency installation using pypi. However, in
-   this demo we
-   demonstrate what is happening under the neath the hood by separating the dependency installation and agent registry
+   this demo we demonstrate what is happening under the neath the hood by separating the dependency installation and agent registry
    steps.
 
     ```shell
     # option 1: install from pypi
     pip install volttron-dnp3-outstation
     
     # option 2: install from the source code (Note: `-e` option to use editable mode, useful for development.)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-dnp3-outstation Version: 0.1.1a4 Summary:
+Metadata-Version: 2.1 Name: volttron-dnp3-outstation Version: 0.1.1a5 Summary:
 A Volttron agent that acts as a dnp3 outstation. Home-page: https://github.com/
 eclipse-volttron/volttron-dnp3-outstation License: Apache-2.0 Keywords:
 volttron,agent,dnp3,outstation,application Author: Kefei Mo Author-email:
 kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email: volttron@pnnl.gov
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
@@ -12,50 +12,58 @@
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Home
 Automation Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Dist: dnp3-python (>=0.2.3b3) Requires-Dist: volttron (>=10.0.2rc0)
 Project-URL: Bug Tracker, https://github.com/eclipse-volttron/volttron-dnp3-
 outstation/issues Project-URL: Repository, https://github.com/eclipse-volttron/
 volttron-dnp3-outstation Description-Content-Type: text/markdown # volttron-
-dnp3-outstation [//]: # (TODO: get the badges) Distributed Network Protocol
-(DNP or [DNP3](https://en.wikipedia.org/wiki/DNP3)) has achieved a large-scale
-acceptance since its introduction in 1993. This protocol is an immediately
-deployable solution for monitoring remote sites because it was developed for
-communication of critical infrastructure status, allowing for reliable remote
-control. DNP3 is typically used between centrally located masters and
-distributed remotes. Application layer fragments from Master DNP3 stations are
-typically requests for operations on data objects, and application layer
-fragments from Slave DNP3 stations (i.e., Outstation) are typically responses
-to those requests. A DNP3 Outstation may also transmit a message without a
-request (an unsolicited response). The volttron-dnp3-outstation is an
-implementation of the DNP3 master following the [VOLTTRON Agent Specifications]
-(https://volttron.readthedocs.io/en/main/developing-volttron/developing-agents/
-specifications/index.html?highlight=agent#agent-specifications). Note: to fully
-desmonstate the volttron-dnp3-outstation features, including polling data,
-setting point values, etc., it is suggested to establish connection between an
-outstation and a DNP3 master instance. The [dnp3-python](https://github.com/
-VOLTTRON/dnp3-python) can provide the essential master functionality, and as
-part of the volttron-dnp3-outstation dependency, it is immediately available
-after the volttron-dnp3-outstation is installed. # Prerequisites * Python 3
-(tested with Python3.8, Python3.9, Python3.10) ## Python  To install specific
-Python version (e.g., Python 3.8), we recommend using pyenv. ```shell # install
-pyenv git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you
-should also put these three lines in .bashrc or similar) export PATH="$
-{HOME}/.pyenv/bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv
-init -)" # install Python 3.8 pyenv install 3.8.10 # make it available globally
-pyenv global system 3.8.10 ```  # Installation The following recipe walks
-through the steps to install and configure a DNP3 agent. Note that it uses
-default setup to work out-of-the-box. Please feel free to refer to related
-documentations for details. 1. Create and activate a virtual environment. It is
-recommended to use a virtual environment for installing volttron. ```shell
-python -m venv env source env/bin/activate pip install volttron ``` 1. Install
-volttron and start the platform. > **Note**: > According to the [volttron-
-core#README](https://github.com/eclipse-volttron/volttron-core#readme), setup
-VOLTTRON_HOME > environment variable is mandatory: > ... if you have/had in the
-past, a monolithic VOLTTRON version that used the default VOLTTRON_HOME >
+dnp3-outstation [![Eclipse VOLTTRONâ¢](https://img.shields.io/badge/
+Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/) !
+[Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg) ![Python 3.11]
+(https://img.shields.io/badge/python-3.11-blue.svg) [![Pytests](https://
+github.com/eclipse-volttron/volttron-dnp3-outstation/actions/workflows/run-
+tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-dnp3-
+outstation/actions/workflows/run-tests.yml) [![pypi version](https://
+img.shields.io/pypi/v/volttron-dnp3-outstation.svg)](https://pypi.org/project/
+volttron-dnp3-outstation/) Distributed Network Protocol (DNP or [DNP3](https://
+en.wikipedia.org/wiki/DNP3)) has achieved a large-scale acceptance since its
+introduction in 1993. This protocol is an immediately deployable solution for
+monitoring remote sites because it was developed for communication of critical
+infrastructure status, allowing for reliable remote control. DNP3 is typically
+used between centrally located masters and distributed remotes. Application
+layer fragments from Master DNP3 stations are typically requests for operations
+on data objects, and application layer fragments from Slave DNP3 stations
+(i.e., Outstation) are typically responses to those requests. A DNP3 Outstation
+may also transmit a message without a request (an unsolicited response). The
+volttron-dnp3-outstation is an implementation of the DNP3 master following the
+[VOLTTRON Agent Specifications](https://volttron.readthedocs.io/en/main/
+developing-volttron/developing-agents/specifications/
+index.html?highlight=agent#agent-specifications). Note: to fully desmonstate
+the volttron-dnp3-outstation features, including polling data, setting point
+values, etc., it is suggested to establish connection between an outstation and
+a DNP3 master instance. The [dnp3-python](https://github.com/VOLTTRON/dnp3-
+python) can provide the essential master functionality, and as part of the
+volttron-dnp3-outstation dependency, it is immediately available after the
+volttron-dnp3-outstation is installed. # Prerequisites * Python 3 (tested with
+Python3.8, Python3.9, Python3.10) ## Python  To install specific Python version
+(e.g., Python 3.8), we recommend using pyenv. ```shell # install pyenv git
+clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should also
+put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/bin:$
+{PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install
+Python 3.10 pyenv install 3.10 # make it available globally pyenv global system
+3.10 ```  # Installation The following recipe walks through the steps to
+install and configure a DNP3 agent. Note that it uses default setup to work
+out-of-the-box. Please feel free to refer to related documentations for
+details. 1. Create and activate a virtual environment. It is recommended to use
+a virtual environment for installing volttron. ```shell python -m venv env
+source env/bin/activate pip install volttron ``` 1. Install volttron and start
+the platform. > **Note**: > According to the [volttron-core#README](https://
+github.com/eclipse-volttron/volttron-core#readme), setup VOLTTRON_HOME >
+environment variable is mandatory: > ... if you have/had in the past, a
+monolithic VOLTTRON version that used the default VOLTTRON_HOME >
 $HOME/.volttron. This modular version of VOLTTRON cannot work with
 volttron_home used by monolithic version of > VOLTTRON(version 8.3 or earlier)
 ```shell # Setup environment variable `VOLTTRON_HOME` export VOLTTRON_HOME= #
 Start platform with output going to volttron.log volttron -vv -l volttron.log &
 ``` 1. Install the "volttron-dnp3-outstation" dependency. There are two options
 to install the DNP3 Driver. You can install this library using the version on
 PyPi or install it from the source code (`git clone` might be required.) Note:
```

