# Comparing `tmp/eeecalc-0.1.0.tar.gz` & `tmp/eeecalc-0.1.1.tar.gz`

## Comparing `eeecalc-0.1.0.tar` & `eeecalc-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/base-eeeCalc.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/.DS_Store
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/__init__.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/dBtoRatio.py
--rwxr-xr-x   0        0        0     4904 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/filter.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/general.py
--rwxr-xr-x   0        0        0     2662 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/phasors.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/secondDegreeDiffEq.py
--rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/signalFunctions.py
--rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/transferFunctionPlot.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/eeeCalc.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/modules.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.1.0/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 eeecalc-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.1.0/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.1.0/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/base-eeeCalc.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    12556 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/.DS_Store
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/__init__.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/dBtoRatio.py
+-rwxr-xr-x   0        0        0     5308 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/filter.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/general.py
+-rwxr-xr-x   0        0        0     2662 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/phasors.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/secondDegreeDiffEq.py
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/signalFunctions.py
+-rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/transferFunctionPlot.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/.idea/eeeCalc.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/.idea/modules.xml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.1.1/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 eeecalc-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.1.1/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.1.1/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.1.1/PKG-INFO
```

### Comparing `eeecalc-0.1.0/.DS_Store` & `eeecalc-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/.idea/workspace.xml` & `eeecalc-0.1.1/.idea/workspace.xml`

 * *Files 19% similar despite different names*

#### Comparing `eeecalc-0.1.0/.idea/workspace.xml` & `eeecalc-0.1.1/.idea/workspace.xml`

```diff
@@ -1,38 +1,34 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="b760d63e-7a17-4aba-ba56-d8314c16af6d" name="Changes" comment="3.8 support">
-      <change beforePath="$PROJECT_DIR$/.gitignore" beforeDir="false" afterPath="$PROJECT_DIR$/.gitignore" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/eeeCalc/filter.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/eeeCalc/filter.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/eeeCalc/phasors.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/eeeCalc/phasors.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/eeeCalc/trigFunc.py" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/filterTest.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/filterTest.py" afterDir="false"/>
+    <list default="true" id="b760d63e-7a17-4aba-ba56-d8314c16af6d" name="Changes" comment="added instructions file to .gitignore">
+      <change beforePath="$PROJECT_DIR$/howToBuildAndUpload.txt" beforeDir="false" afterPath="$PROJECT_DIR$/howToBuildAndUpload.txt" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_BRANCH_BY_REPOSITORY">
       <map>
         <entry key="$PROJECT_DIR$" value="main"/>
       </map>
     </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
-  <component name="GitHubPullRequestSearchHistory"><![CDATA[{
-  "lastFilter": {
-    "state": "OPEN"
+  <component name="GitHubPullRequestSearchHistory">{
+  &quot;lastFilter&quot;: {
+    &quot;state&quot;: &quot;OPEN&quot;
   }
-}]]></component>
+}</component>
   <component name="GithubPullRequestsUISettings">
     <option name="selectedUrlAndAccountId">
       <UrlAndAccount>
         <option name="accountId" value="26c5797c-67ef-4f21-8070-ee6ef1752506"/>
         <option name="url" value="https://github.com/xkjjx/eeecalc.git"/>
       </UrlAndAccount>
     </option>
@@ -191,15 +187,48 @@
     <task id="LOCAL-00009" summary="3.8 support">
       <created>1683773728911</created>
       <option name="number" value="00009"/>
       <option name="presentableId" value="LOCAL-00009"/>
       <option name="project" value="LOCAL"/>
       <updated>1683773728911</updated>
     </task>
-    <option name="localTasksCounter" value="10"/>
+    <task id="LOCAL-00010" summary=".git ignore now ignores tests
+filter.py is properly commented
+trigFunc.py is deleted as it's use is not needed - import trig functions from cmath instead
+phasors is refined and properly commented">
+      <created>1683847212680</created>
+      <option name="number" value="00010"/>
+      <option name="presentableId" value="LOCAL-00010"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683847212680</updated>
+    </task>
+    <task id="LOCAL-00011" summary="changed version number
+removed experimental attempts at implementing chebyshev type 2 filter - will be pasted on a separate branch">
+      <created>1683847317630</created>
+      <option name="number" value="00011"/>
+      <option name="presentableId" value="LOCAL-00011"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683847317630</updated>
+    </task>
+    <task id="LOCAL-00012" summary="changed version number
+improved the filter method by adding better unit support and making the distinctions clearer">
+      <created>1683865043232</created>
+      <option name="number" value="00012"/>
+      <option name="presentableId" value="LOCAL-00012"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683865043232</updated>
+    </task>
+    <task id="LOCAL-00013" summary="added instructions file to .gitignore">
+      <created>1683865163787</created>
+      <option name="number" value="00013"/>
+      <option name="presentableId" value="LOCAL-00013"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683865163787</updated>
+    </task>
+    <option name="localTasksCounter" value="14"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -225,10 +254,19 @@
     <MESSAGE value="transfer function refined with comments and better more accurate experience, specifically with differences between Hz and rad/s"/>
     <MESSAGE value="refined .gitignore and some api stuff"/>
     <MESSAGE value="changed version number from 0.0.8 to 0.0.9"/>
     <MESSAGE value="rewrote diffeq function name"/>
     <MESSAGE value="Merge remote-tracking branch 'origin/transferFunction'"/>
     <MESSAGE value="name change"/>
     <MESSAGE value="3.8 support"/>
-    <option name="LAST_COMMIT_MESSAGE" value="3.8 support"/>
+    <MESSAGE value=".git ignore now ignores tests
+filter.py is properly commented
+trigFunc.py is deleted as it's use is not needed - import trig functions from cmath instead
+phasors is refined and properly commented"/>
+    <MESSAGE value="changed version number
+removed experimental attempts at implementing chebyshev type 2 filter - will be pasted on a separate branch"/>
+    <MESSAGE value="changed version number
+improved the filter method by adding better unit support and making the distinctions clearer"/>
+    <MESSAGE value="added instructions file to .gitignore"/>
+    <option name="LAST_COMMIT_MESSAGE" value="added instructions file to .gitignore"/>
   </component>
 </project>
```

### Comparing `eeecalc-0.1.0/src/.DS_Store` & `eeecalc-0.1.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/src/eeeCalc/dBtoRatio.py` & `eeecalc-0.1.1/src/eeeCalc/dBtoRatio.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/src/eeeCalc/filter.py` & `eeecalc-0.1.1/src/eeeCalc/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,78 +33,93 @@
     initializes the abstract filter class,
     parent of the four different types of filter -
     lowpass, highpass, bandpass, bandstop
     ASSUMES SYMMETRIC PASSBAND AND STOPBAND GAIN FOR BANDPASS/BANDSTOP FILTERS,
     THUS USE STRICTEST AND FASTEST DROPOFF
     """
     passBandGainDB = 0
-    stopBaandGainDB = -20
+    stopBandGainDB = -20
+    passBandPowerGain = 1
+    stopBandPowerGain = 0.01
     degree = 0
     poles = []
     zeroes = []
     implemented = False
     FilterType = ""
-    def tfunc(s):
-        return
+    transferFunction = None
     def __init__(self):
         pass
-    def __init__(self,passBandGain,stopBandGain,DB=True):
+    def __init__(self,passBandGain,stopBandGain,DB=True,power=True):
+
         if (stopBandGain >= passBandGain):
             raise ValueError("Passband gain has to be higher than stopband gain")
-        self.passBandGainDB = passBandGain
-        self.stopBandGainDB = stopBandGain
-    def setPassBandGain(self,passBandGain,DB=True):
-        self.passBandGainDB = passBandGain
+
+        if DB:
+            self.passBandGainDB = passBandGain
+            self.passBandPowerGain = dBToPowRatio(self.passBandGainDB)
+            self.stopBandGainDB = stopBandGain
+            self.stopBandPowerGain = dBToPowRatio(self.stopBandGainDB)
+        else:
+            self.passBandGainDB = powRatioToDB(passBandGain) * 2**(not power)
+
+            if power:
+                self.passBandPowerGain = passBandGain
+            else:
+                self.passBandPowerGain = sqrt(passBandGain)
+
+            self.stopBandGainDB = powRatioToDB(stopBandGain) * 2**(not power)
+
+            if power:
+                self.stopBandPowerGain = stopBandGain
+            else:
+                self.stopBandPowerGain = sqrt(stopBandGain)
 
 
 
 class LPF(Filter):
     """
     LOWPASS FILTER CLASS:
     first set it's pasband frequency, stopband frequency, stopband gain, passband gain
     before calling the implementChebyshevTypeI() or implementButterworth() methods
     more implementations will be supported soon
     after implementation, poles, zeroes, and transfer functions can be requested
     """
-    def __init__(self,passBandGain,stopBandGain,passBandFrequency,stopBandFrequency,DB=True,kHz=False,power=False):
-        if(stopBandGain >= passBandGain):
-            raise ValueError("Passband gain has to be higher than stopband gain")
+    def __init__(self, passBandGain, stopBandGain, passBandFrequency, stopBandFrequency, DB=True, kHz=False,power=True):
+        super().__init__(passBandGain,stopBandGain,DB,power)
+
         if (passBandFrequency >= stopBandFrequency):
             raise ValueError("Passband frequency has to be lower than stopband frequency in a LPF")
-        self.passBandGainDB = passBandGain
-        self.passBandPowerGain = dBToPowRatio(self.passBandGainDB)
-        self.stopBandGainDB = stopBandGain
-        self.stopBandPowerGain = dBToPowRatio(self.stopBandGainDB)
-        self.passBandFrequency = passBandFrequency
-        self.stopBandFrequency = stopBandFrequency
+
+        self.passBandFrequency = passBandFrequency * (1000)**kHz
+        self.stopBandFrequency = stopBandFrequency * (1000)**kHz
 
     def implementButterworth(self):
         self.FilterType = "Butterworth"
         self.degree = ceil(0.5*log((1/self.stopBandPowerGain - 1)/(1/self.passBandPowerGain - 1))/log(self.stopBandFrequency/self.passBandFrequency))
         f3 = 0.5*((self.passBandFrequency)/(1/self.passBandPowerGain - 1)**(1/(2*self.degree)) + ((self.stopBandFrequency)/(1/self.stopBandPowerGain - 1)**(1/(2*self.degree))))
         for i in range(self.degree):
             self.poles.append(polarComplex(2*pi*f3,pi/(2*self.degree) + pi*i/self.degree + pi/2))
-        self.tfunc = lambda s: 1/zeroMultiplierFuncGenerator(self.poles,s)
+        self.transferFunction = lambda s: 1 / zeroMultiplierFuncGenerator(self.poles, s)
         self.implemented = True
 
     def implementChebyshevTypeI(self):
         self.FilterType = "Chebyshev Type I"
         self.degree = ceil(acosh(sqrt((1/self.stopBandPowerGain - 1)/(1/self.passBandPowerGain - 1)))/acosh(self.stopBandFrequency/self.passBandFrequency))
         eps = 0.5 * ((1/self.passBandPowerGain - 1) + (1/self.stopBandPowerGain - 1)/(ChebyshevPolynomial(self.degree,self.stopBandFrequency/self.passBandFrequency)**2))
         z = asinh(sqrt(1/eps))/self.degree
         for i in range(self.degree * 2):
             x = complex(2*pi*self.passBandFrequency*sin((2*i - 1)*pi/(2*self.degree))*sinh(z),2*pi*self.passBandFrequency*cos((2*i - 1)*pi/(2*self.degree))*cosh(z))
             if(fabs(pol(x)[1]) >= pi/2):
                 self.poles.append(x)
-        self.tfunc = lambda s : 1/zeroMultiplierFuncGenerator(self.poles,s)
+        self.transferFunction = lambda s : 1 / zeroMultiplierFuncGenerator(self.poles, s)
         self.implemented = True
 
 
     def getTransferFunction(self):
-        return self.tfunc
+        return self.transferFunction
 
     def getDegree(self):
         return self.degree
 
     def getPoles(self):
         return self.poles
```

### Comparing `eeecalc-0.1.0/src/eeeCalc/general.py` & `eeecalc-0.1.1/src/eeeCalc/general.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/src/eeeCalc/phasors.py` & `eeecalc-0.1.1/src/eeeCalc/phasors.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/src/eeeCalc/secondDegreeDiffEq.py` & `eeecalc-0.1.1/src/eeeCalc/secondDegreeDiffEq.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/src/eeeCalc/transferFunctionPlot.py` & `eeecalc-0.1.1/src/eeeCalc/transferFunctionPlot.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/src/eeeCalc/.idea/workspace.xml` & `eeecalc-0.1.1/src/eeeCalc/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/.gitignore` & `eeecalc-0.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -157,8 +157,10 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 githubtoken.txt
 
-tests/
+tests/
+
+howToBuildAndUpload.txt
```

### Comparing `eeecalc-0.1.0/LICENSE` & `eeecalc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eeecalc-0.1.0/pyproject.toml` & `eeecalc-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "eeeCalc"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Kevin Johnson", email="john2003.kjj@gmail.com" },
 ]
 description = "Package to aid electrical engineering calculations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

