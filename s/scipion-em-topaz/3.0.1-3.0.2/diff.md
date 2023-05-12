# Comparing `tmp/scipion-em-topaz-3.0.1.tar.gz` & `tmp/scipion-em-topaz-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-topaz-3.0.1.tar", last modified: Mon Apr 19 11:14:56 2021, max compression
+gzip compressed data, was "scipion-em-topaz-3.0.2.tar", last modified: Fri May 12 08:40:52 2023, max compression
```

## Comparing `scipion-em-topaz-3.0.1.tar` & `scipion-em-topaz-3.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 11:14:56.096197 scipion-em-topaz-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-04-19 11:14:56.096197 scipion-em-topaz-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 11:14:56.092197 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-04-19 11:14:55.000000 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-04-19 11:14:55.000000 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-19 11:14:55.000000 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-04-19 11:14:55.000000 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-04-19 11:14:55.000000 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-04-19 11:14:55.000000 scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-19 11:14:56.096197 scipion-em-topaz-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 11:14:56.096197 scipion-em-topaz-3.0.1/topaz/
--rw-r--r--   0 runner    (1001) docker     (121)     4362 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4950 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 11:14:56.096197 scipion-em-topaz-3.0.1/topaz/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/protocols/protocol_topaz_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     8581 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/protocols/protocol_topaz_picking.py
--rw-r--r--   0 runner    (1001) docker     (121)    15022 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/protocols/protocol_topaz_training.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-19 11:14:56.096197 scipion-em-topaz-3.0.1/topaz/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/tests/test_protocol_topaz.py
--rw-r--r--   0 runner    (1001) docker     (121)     9179 2021-04-19 11:09:58.000000 scipion-em-topaz-3.0.1/topaz/topaz_logo.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:40:52.248597 scipion-em-topaz-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-12 08:40:52.248597 scipion-em-topaz-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:40:52.244598 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-12 08:40:52.000000 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-12 08:40:52.000000 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:40:52.000000 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-12 08:40:52.000000 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 08:40:52.000000 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 08:40:52.000000 scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:40:52.248597 scipion-em-topaz-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:40:52.244598 scipion-em-topaz-3.0.2/topaz/
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:40:52.248597 scipion-em-topaz-3.0.2/topaz/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/protocols/protocol_topaz_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/protocols/protocol_topaz_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/protocols/protocol_topaz_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:40:52.248597 scipion-em-topaz-3.0.2/topaz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/tests/test_protocol_topaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-12 08:38:28.000000 scipion-em-topaz-3.0.2/topaz/topaz_logo.jpeg
```

### Comparing `scipion-em-topaz-3.0.1/LICENSE` & `scipion-em-topaz-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/scipion_em_topaz.egg-info/SOURCES.txt` & `scipion-em-topaz-3.0.2/scipion_em_topaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/setup.py` & `scipion-em-topaz-3.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,37 +73,37 @@
     # above.
     author_email='scipion@cnb.csic.es',  # Optional
 
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
-    #classifiers=[  # Optional
+    classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-    #   'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
 
         # Indicate who your project is intended for
-    #   'Intended Audience :: Users',
+        #   'Intended Audience :: Users',
 
-    # Pick your license as you wish
-    #   'License :: OSI Approved :: MIT License',
+        # Pick your license as you wish
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 
-    # Specify the Python versions you support here. In particular, ensure
-    # that you indicate whether you support Python 2, Python 3 or both.
-    #   'Programming Language :: Python :: 2.7'
-    #],
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3'
+    ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='scipion cryoem imageprocessing scipion-3.0',  # Optional
+    keywords='scipion cryo-em image-processing scipion-3.0',  # Optional
 
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
@@ -146,14 +146,19 @@
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files
     #
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
     #data_files=[('my_data', ['data/data_file'])],  # Optional
 
+    project_urls={  # Optional
+        'Bug Reports': 'https://github.com/scipion-em/scipion-em-topaz/issues',
+        'Source': 'https://github.com/scipion-em/scipion-em-topaz/',
+    },
+
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
```

### Comparing `scipion-em-topaz-3.0.1/topaz/__init__.py` & `scipion-em-topaz-3.0.2/topaz/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import pwem
 import pyworkflow.utils as pwutils
 import pyworkflow as pw
 
 from .constants import *
 
 
-__version__ = '3.0.1'
+__version__ = '3.0.2'
 _references = ['Bepler2018']
 _logo = "topaz_logo.jpeg"
 
 
 class Plugin(pwem.Plugin):
     _supportedVersions = VERSIONS
     _url = "https://github.com/scipion-em/scipion-em-topaz"
@@ -91,17 +91,21 @@
         # Create the environment
         installationCmd += 'conda create -y -n %s python=3.6 &&'\
                            % ENV_NAME
 
         # Activate the new environment
         installationCmd += 'conda activate %s &&' % ENV_NAME
 
+        cudaVersion = cls.getVersionFromPath(pwem.Config.CUDA_LIB, pattern="cuda",
+                                             default="11.6")
+
+        toolkitVersion = "10.2" if cudaVersion.major == 10 else "11.3"
         # Install downloaded code
-        installationCmd += 'conda install -y topaz=%s cudatoolkit '\
-                           '-c tbepler -c pytorch &&' % version
+        installationCmd += 'conda install -y topaz=%s cudatoolkit=%s '\
+                           '-c tbepler -c pytorch &&' % (version, toolkitVersion)
 
         # Flag installation finished
         installationCmd += 'touch %s' % TOPAZ_INSTALLED
 
         topaz_commands = [(installationCmd, TOPAZ_INSTALLED)]
 
         envPath = os.environ.get('PATH', "")
```

### Comparing `scipion-em-topaz-3.0.1/topaz/bibtex.py` & `scipion-em-topaz-3.0.2/topaz/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/topaz/constants.py` & `scipion-em-topaz-3.0.2/topaz/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 # *
 # **************************************************************************
 
 
 def getTopazEnvName(version):
     return "topaz-%s" % version
 
+V0_2_5 = "0.2.5"
 V0_2_4 = "0.2.4"
 V0_2_3 = "0.2.3"
-VERSIONS = [V0_2_3, V0_2_4]
-TOPAZ_DEFAULT_VER_NUM = V0_2_4
+VERSIONS = [V0_2_3, V0_2_4, V0_2_5]
+TOPAZ_DEFAULT_VER_NUM = V0_2_5
 
 DEFAULT_ENV_NAME = getTopazEnvName(TOPAZ_DEFAULT_VER_NUM)
 DEFAULT_ACTIVATION_CMD = 'conda activate ' + DEFAULT_ENV_NAME
 TOPAZ_ENV_ACTIVATION = 'TOPAZ_ENV_ACTIVATION'
 
 # Topaz supported input formats for micrographs
 TOPAZ_SUPPORTED_FORMATS = [".mrc", ".tiff", ".png"]
```

### Comparing `scipion-em-topaz-3.0.1/topaz/convert.py` & `scipion-em-topaz-3.0.2/topaz/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/topaz/objects.py` & `scipion-em-topaz-3.0.2/topaz/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/topaz/protocols/__init__.py` & `scipion-em-topaz-3.0.2/topaz/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/topaz/protocols/protocol_base.py` & `scipion-em-topaz-3.0.2/topaz/protocols/protocol_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     group.addParam('doDenoise', params.BooleanParam, default=False,
                    label="Denoise micrographs?")
     group.addParam('modelDenoise', params.EnumParam, default=0,
                    condition='doDenoise',
                    choices=['unet', 'unet-small', 'fcnn', 'affineresnet8'],
                    label='Model',
                    help='Denoising model to use on micrographs.')
+    group.addParam('patchSize', params.IntParam, default=-1,
+                   label='Patch Size', condition='doDenoise',
+                   help='Process each micrograph in patches of this size.\n'
+                        'This is useful when using GPU processing and the micrographs '
+                        'are too large to be denoised in one shot on your GPU. '
+                        'By default (<0), it is not used')
     group.addParam('denoiseExtra', params.StringParam, default='',
                    expertLevel=cons.LEVEL_ADVANCED, condition='doDenoise',
                    label="Advanced options",
                    help="Provide advanced command line options here.")
 
     group = form.addGroup('Pre-process')
     group.addParam('scale', params.IntParam, default=4,
@@ -70,28 +76,30 @@
                         " First core index is 0, second 1 and so on.")
 
 
   #UTILS for preprocess steps
   def getDenoiseArgs(self, inputDir, outDir):
       args = ' %s/*.mrc -o %s/' % (inputDir, outDir)
       args += ' --model %s' % self.getEnumText('modelDenoise')
-      args += ' --device %s' % self.gpuList
+      args += ' --device %(GPU)s'  # Add GPU that will be set by the executor
+      if self.patchSize.get() > 0:
+        args += ' --patch-size %s' % self.patchSize.get()
 
       if self.denoiseExtra.hasValue():
         args += ' ' + self.denoiseExtra.get()
       else:
         args += ' --normalize'
 
       return args
 
   def getPreprocessArgs(self, inputDir, outDir):
     args = " %s/*.mrc -o %s/" % (inputDir, outDir)
     args += " --scale %d " % self.scale.get()
     args += ' --num-workers %d' % self.numberOfThreads
-    args += ' --device %s' % self.gpuList
+    args += ' --device %(GPU)s'  # Add GPU that will be set by the executor
 
     if self.preExtra.hasValue():
       args += ' ' + self.preExtra.get()
 
     return args
 
   def getOutputModelPath(self):
```

### Comparing `scipion-em-topaz-3.0.1/topaz/protocols/protocol_topaz_import.py` & `scipion-em-topaz-3.0.2/topaz/protocols/protocol_topaz_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
 from topaz.objects import TopazModel
 
 
 class TopazProtImport(ProtImport):
     """ Protocol to import an existing topaz training model.
     The model will be registered as an output of this protocol and
-    it can be used later for further training or for picking.
+    can be used later for further training or for picking.
     """
-    _label = 'topaz import'
+    _label = 'import training model'
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection(label='Import')
         form.addParam('modelPath', params.PathParam,
                       label="Training model path",
                       help="Provide the path of a previous topaz training "
```

### Comparing `scipion-em-topaz-3.0.1/topaz/protocols/protocol_topaz_picking.py` & `scipion-em-topaz-3.0.2/topaz/protocols/protocol_topaz_picking.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+
 import os
 import time
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 import pyworkflow.protocol.constants as cons
 from pwem.protocols import ProtParticlePickingAuto
@@ -37,17 +38,18 @@
 
 TOPAZ_COORDINATES_FILE = 'topaz_coordinates_file'
 PICKING_DENOISE_FOLDER = 'picking_denoise_folder'
 PICKING_PRE_FOLDER = 'picking_pre_folder'
 PICKING_FOLDER = 'picking_folder'
 MODEL_FOLDER = 'model_folder'
 
+
 class TopazProtPicking(ProtParticlePickingAuto, ProtTopazBase):
   """ Perform a picking using a topaz model """
-  _label = 'topaz picking'
+  _label = 'picking'
 
   ADD_MODEL_TRAIN_TYPES = ["TopazTrained", "TopazGeneral"]
   ADD_MODEL_PRETRAINED = 0
   ADD_MODEL_GENERAL = 1
 
   GENERAL_MODELS = ["resnet16_u64", "resnet16_u32", "resnet8_u64", "resnet8_u32"]
   MODEL_RESNET16_U64 = 0
@@ -82,16 +84,17 @@
                   label='Topaz general model',
                   help='A topaz NN model pretrained and provided in topaz sofware.'
                        '\nMight not be optimized for specific particles')
 
     form.addSection('Picking')
     form.addParam('radius', params.IntParam, default=8,
                   label='Particle radius (px)',
+                  allowsPointers=True,
                   help='Pixel radius around particle centers to consider.')
-    form.addParam('boxSize', params.IntParam, default=-1, expertLevel=cons.LEVEL_ADVANCED,
+    form.addParam('boxSize', params.IntParam, default=-1, expertLevel=cons.LEVEL_ADVANCED, allowsPointers=True,
                   label='Box size (px)', help='Box size in pixels. By default(-1): radius*2*scale')
     form.addParam('threshold', params.FloatParam, default=-6.0,
                   label='Extraction threshold',
                   help='log-likelihood score threshold at which to terminate region extraction. '
                        '\nValue -6 is p>=0.0025 (default: -6)'
                        '\nHigher values will mean a more restrictive picking')
 
@@ -159,15 +162,15 @@
     # Launch process called extract which is rather a prediction
     args = ' -t {}'.format(self.threshold.get())
     args += ' -r %d' % self.radius.get()
     args += ' -m %s' % modelFn
     args += ' -o %s' % self.getPickingFileName(micList,
                                                TOPAZ_COORDINATES_FILE)
     args += ' --num-workers %d' % self.numberOfThreads
-    args += ' --device %s' % self.gpuList
+    args += ' --device %(GPU)s'  # Add GPU that will be set by the executor
     args += ' %s/*.mrc' % preprocessedDir
 
     Plugin.runTopaz(self, 'topaz extract', args)
 
   def readCoordsFromMics(self, outputDir, micDoneList, outputCoords):
     """ Read the coordinates from a given list of micrographs """
 
@@ -189,10 +192,10 @@
     return self._getFileName(key, **{"min": micList[0].strId(),
                                      'max': micList[-1].strId()})
 
 
   def _validate(self):
     validateMsgs = []
     if self.modelInitialization.get() == self.ADD_MODEL_PRETRAINED:
-      if self.prevTopazModel.get() == None:
+      if self.prevTopazModel.get() is None:
         validateMsgs.append('Model not ready')
     return validateMsgs
```

### Comparing `scipion-em-topaz-3.0.1/topaz/protocols/protocol_topaz_training.py` & `scipion-em-topaz-3.0.2/topaz/protocols/protocol_topaz_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 TRAININGTEST = 'trainingtest'
 PARTICLES_TEST_TXT = 'particles_test.txt'
 PARTICLES_TRAIN_TXT = 'particles_train.txt'
 
 
 class TopazProtTraining(ProtParticlePicking, ProtTopazBase):
   """ Train and save a Topaz model"""
-  _label = 'topaz training'
+  _label = 'training'
 
   ADD_MODEL_TRAIN_TYPES = ["New", "TopazModel"]
   ADD_MODEL_TRAIN_NEW = 0
   ADD_MODEL_TRAIN_MODEL = 1
 
   def __init__(self, **args):
     ProtParticlePicking.__init__(self, **args)
@@ -105,14 +105,15 @@
                   label='Micrographs for training', default=5,
                   help='This number will be divided into training and test data.'
                        'If it is not reached wait')
 
     form.addSection('Train')
     form.addParam('radius', params.IntParam, default=3,
                   label='Particle radius (px)',
+                  allowsPointers=True,
                   help='Pixel radius around particle centers to '
                        'consider.')
     form.addParam('autoenc', params.FloatParam, default=0.,
                   label='Autoencoder',
                   help='Augment the method with autoencoder '
                        'where the weight is on reconstruction error.')
     form.addParam('numEpochs', params.IntParam, default=10,
@@ -121,14 +122,15 @@
     form.addParam('method', params.EnumParam, default=2,
                   expertLevel=cons.LEVEL_ADVANCED,
                   choices=['PN', 'GE-KL', 'GE-binomial', 'PU'],
                   label='Method',
                   help='Objective function to use for learning the '
                        'region classifier.')
     form.addParam('numPartPerImg', params.IntParam, default=300,
+                  allowsPointers=True,
                   expertLevel=cons.LEVEL_ADVANCED,
                   label='Number of particles per image',
                   help='Expected number of particles per micrograph.')
     form.addParam('kfold', params.IntParam, default=5,
                   expertLevel=cons.LEVEL_ADVANCED,
                   label='K-fold',
                   help='Number of subsets to divide the training '
```

### Comparing `scipion-em-topaz-3.0.1/topaz/protocols.conf` & `scipion-em-topaz-3.0.2/topaz/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-topaz-3.0.1/topaz/tests/test_protocol_topaz.py` & `scipion-em-topaz-3.0.2/topaz/tests/test_protocol_topaz.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,38 +86,38 @@
             filesPath=TestTopaz.ds.getFile('pickingEman/info/'),
             inputMicrographs=cls.protPreprocess.outputMicrographs,
             filesPattern='*.json',
             boxSize=65)
         cls.launchProtocol(protImportCoords)
         cls.protImportCoords = protImportCoords
 
-    def _runTraining(self, modelInit=0, prevModel=None):
+    def _runTraining(self, modelInit=0, prevModel=None, denoise=False):
         self.runImportCoords()
         # Topaz training
         protTraining = self.newProtocol(
             protocols.TopazProtTraining,
             label='Training 1',
             inputMicrographs=self.protPreprocess.outputMicrographs,
             inputCoordinates=self.protImportCoords.outputCoordinates,
             modelInitialization=modelInit,
             prevTopazModel=prevModel,
-            radius=3, scale=4,
+            radius=3, scale=4, doDenoise=denoise,
             numEpochs=1)
         self.launchProtocol(protTraining)
 
         outputModel = getattr(protTraining, 'outputModel', None)
         self.assertTrue(outputModel is not None)
 
         # Training mode picking
         protPicking = self.newProtocol(
             protocols.TopazProtPicking,
             label="Picking after Training 1",
             inputMicrographs=self.protPreprocess.outputMicrographs,
             prevTopazModel=protTraining.outputModel,
-            boxSize=50,
+            boxSize=50, doDenoise=denoise,
             streamingBatchSize=10)
 
         self.launchProtocol(protPicking)
         return protTraining, protPicking
 
     def _runImportModel(self, prot):
         protImport = self.newProtocol(
@@ -137,13 +137,13 @@
             scale=4,
             boxSize=100,
             streamingBatchSize=10)
         self.launchProtocol(protTopaz)
 
     def testTraining(self):
         #Training a new model and picking
-        protTrained, protPicked = self._runTraining()
+        protTrained, protPicked = self._runTraining(denoise=True)
         #Importing a model from path
         protImported = self._runImportModel(protTrained)
         #Training an imported model and picking
         self._runTraining(modelInit=1, prevModel=protImported.outputModel)
```

### Comparing `scipion-em-topaz-3.0.1/topaz/topaz_logo.jpeg` & `scipion-em-topaz-3.0.2/topaz/topaz_logo.jpeg`

 * *Files identical despite different names*

