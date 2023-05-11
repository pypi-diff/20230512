# Comparing `tmp/eeecalc-0.0.91.tar.gz` & `tmp/eeecalc-0.1.0.tar.gz`

## Comparing `eeecalc-0.0.91.tar` & `eeecalc-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/base-eeeCalc.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/vcs.xml
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/.DS_Store
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/__init__.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/dBtoRatio.py
--rwxr-xr-x   0        0        0     4721 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/filter.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/general.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/phasors.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/secondDegreeDiffEq.py
--rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/signalFunctions.py
--rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/transferFunctionPlot.py
--rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/trigFunc.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/eeeCalc.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/modules.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.91/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eeecalc-0.0.91/tests/filterTest.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 eeecalc-0.0.91/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.91/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.91/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 eeecalc-0.0.91/pyproject.toml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 eeecalc-0.0.91/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/base-eeeCalc.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/.DS_Store
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/__init__.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/dBtoRatio.py
+-rwxr-xr-x   0        0        0     4904 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/filter.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/general.py
+-rwxr-xr-x   0        0        0     2662 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/phasors.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/secondDegreeDiffEq.py
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/signalFunctions.py
+-rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/transferFunctionPlot.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/eeeCalc.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/modules.xml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.1.0/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.1.0/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.1.0/PKG-INFO
```

### Comparing `eeecalc-0.0.91/.DS_Store` & `eeecalc-0.1.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/.idea/workspace.xml` & `eeecalc-0.1.0/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `eeecalc-0.0.91/.idea/workspace.xml` & `eeecalc-0.1.0/.idea/workspace.xml`

```diff
@@ -1,14 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="b760d63e-7a17-4aba-ba56-d8314c16af6d" name="Changes" comment="name change"/>
+    <list default="true" id="b760d63e-7a17-4aba-ba56-d8314c16af6d" name="Changes" comment="3.8 support">
+      <change beforePath="$PROJECT_DIR$/.gitignore" beforeDir="false" afterPath="$PROJECT_DIR$/.gitignore" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/eeeCalc/filter.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/eeeCalc/filter.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/eeeCalc/phasors.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/eeeCalc/phasors.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/eeeCalc/trigFunc.py" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/filterTest.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/filterTest.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
@@ -41,15 +47,15 @@
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
     &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
     &quot;last_opened_file_path&quot;: &quot;/Users/kjj/Library/CloudStorage/OneDrive-TexasA&amp;MUniversity/Texas A&amp;M College Work/base-eeeCalc&quot;
   }
 }</component>
-  <component name="RunManager" selected="Python.transferFunctionPlot">
+  <component name="RunManager" selected="Python.filterTest">
     <configuration name="filter" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="base-eeeCalc"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -107,16 +113,16 @@
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
-        <item itemvalue="Python.transferFunctionPlot"/>
         <item itemvalue="Python.filterTest"/>
+        <item itemvalue="Python.transferFunctionPlot"/>
         <item itemvalue="Python.filter"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
@@ -178,15 +184,22 @@
     <task id="LOCAL-00008" summary="name change">
       <created>1683769439669</created>
       <option name="number" value="00008"/>
       <option name="presentableId" value="LOCAL-00008"/>
       <option name="project" value="LOCAL"/>
       <updated>1683769439669</updated>
     </task>
-    <option name="localTasksCounter" value="9"/>
+    <task id="LOCAL-00009" summary="3.8 support">
+      <created>1683773728911</created>
+      <option name="number" value="00009"/>
+      <option name="presentableId" value="LOCAL-00009"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683773728911</updated>
+    </task>
+    <option name="localTasksCounter" value="10"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -211,10 +224,11 @@
   <component name="VcsManagerConfiguration">
     <MESSAGE value="transfer function refined with comments and better more accurate experience, specifically with differences between Hz and rad/s"/>
     <MESSAGE value="refined .gitignore and some api stuff"/>
     <MESSAGE value="changed version number from 0.0.8 to 0.0.9"/>
     <MESSAGE value="rewrote diffeq function name"/>
     <MESSAGE value="Merge remote-tracking branch 'origin/transferFunction'"/>
     <MESSAGE value="name change"/>
-    <option name="LAST_COMMIT_MESSAGE" value="name change"/>
+    <MESSAGE value="3.8 support"/>
+    <option name="LAST_COMMIT_MESSAGE" value="3.8 support"/>
   </component>
 </project>
```

### Comparing `eeecalc-0.0.91/src/.DS_Store` & `eeecalc-0.1.0/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/src/eeeCalc/dBtoRatio.py` & `eeecalc-0.1.0/src/eeeCalc/dBtoRatio.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/src/eeeCalc/filter.py` & `eeecalc-0.1.0/src/eeeCalc/filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,20 +14,32 @@
         return x
     return 2*x*ChebyshevPolynomial(n-1,x) - ChebyshevPolynomial(n-2,x)
 
 def polarComplex(m,th):
     return complex(m*cos(th),m*sin(th))
 
 def zeroMultiplierFuncGenerator(poles,s):
+    """
+    :param poles: list of values s1,s2,s3,...
+    :param s: point where output needs to be evaluated
+    :return: value of (1 + s/s1)(1 + s/s2)(1 + s/s3)...
+    """
     outP = 1
     for pole in poles:
         outP *= (1+s/pole)
     return outP
 
 class Filter:
+    """
+    initializes the abstract filter class,
+    parent of the four different types of filter -
+    lowpass, highpass, bandpass, bandstop
+    ASSUMES SYMMETRIC PASSBAND AND STOPBAND GAIN FOR BANDPASS/BANDSTOP FILTERS,
+    THUS USE STRICTEST AND FASTEST DROPOFF
+    """
     passBandGainDB = 0
     stopBaandGainDB = -20
     degree = 0
     poles = []
     zeroes = []
     implemented = False
     FilterType = ""
@@ -42,14 +54,21 @@
         self.stopBandGainDB = stopBandGain
     def setPassBandGain(self,passBandGain,DB=True):
         self.passBandGainDB = passBandGain
 
 
 
 class LPF(Filter):
+    """
+    LOWPASS FILTER CLASS:
+    first set it's pasband frequency, stopband frequency, stopband gain, passband gain
+    before calling the implementChebyshevTypeI() or implementButterworth() methods
+    more implementations will be supported soon
+    after implementation, poles, zeroes, and transfer functions can be requested
+    """
     def __init__(self,passBandGain,stopBandGain,passBandFrequency,stopBandFrequency,DB=True,kHz=False,power=False):
         if(stopBandGain >= passBandGain):
             raise ValueError("Passband gain has to be higher than stopband gain")
         if (passBandFrequency >= stopBandFrequency):
             raise ValueError("Passband frequency has to be lower than stopband frequency in a LPF")
         self.passBandGainDB = passBandGain
         self.passBandPowerGain = dBToPowRatio(self.passBandGainDB)
@@ -75,21 +94,14 @@
         for i in range(self.degree * 2):
             x = complex(2*pi*self.passBandFrequency*sin((2*i - 1)*pi/(2*self.degree))*sinh(z),2*pi*self.passBandFrequency*cos((2*i - 1)*pi/(2*self.degree))*cosh(z))
             if(fabs(pol(x)[1]) >= pi/2):
                 self.poles.append(x)
         self.tfunc = lambda s : 1/zeroMultiplierFuncGenerator(self.poles,s)
         self.implemented = True
 
-    def implementChebyshevTypeII(self):
-        self.FilterType = "Chebyshev Type II"
-        self.degree = ceil(acosh(sqrt((1 / self.stopBandPowerGain - 1) / (1 / self.passBandPowerGain - 1))) / acosh(self.stopBandFrequency / self.passBandFrequency))
-        eps = 0.5 * ((1/(1 / self.stopBandPowerGain - 1)) + (1/(1 /self.passBandPowerGain - 1)) / (ChebyshevPolynomial(self.degree, self.stopBandFrequency / self.passBandFrequency) ** 2))
-        for i in range(0,self.degree):
-            self.zeroes.append(self.stopBandFrequency*cos((2*i - 1)*pi/(2*self.degree))/(eps*2*pi))
-        print(self.zeroes)
 
     def getTransferFunction(self):
         return self.tfunc
 
     def getDegree(self):
         return self.degree
```

### Comparing `eeecalc-0.0.91/src/eeeCalc/general.py` & `eeecalc-0.1.0/src/eeeCalc/general.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/src/eeeCalc/secondDegreeDiffEq.py` & `eeecalc-0.1.0/src/eeeCalc/secondDegreeDiffEq.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/src/eeeCalc/transferFunctionPlot.py` & `eeecalc-0.1.0/src/eeeCalc/transferFunctionPlot.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/src/eeeCalc/.idea/workspace.xml` & `eeecalc-0.1.0/src/eeeCalc/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/.gitignore` & `eeecalc-0.1.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -155,8 +155,10 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
-githubtoken.txt
+githubtoken.txt
+
+tests/
```

### Comparing `eeecalc-0.0.91/LICENSE` & `eeecalc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.91/pyproject.toml` & `eeecalc-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "eeeCalc"
-version = "0.0.91"
+version = "0.1.0"
 authors = [
   { name="Kevin Johnson", email="john2003.kjj@gmail.com" },
 ]
 description = "Package to aid electrical engineering calculations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

