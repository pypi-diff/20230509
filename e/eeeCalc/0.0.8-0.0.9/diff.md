# Comparing `tmp/eeecalc-0.0.8.tar.gz` & `tmp/eeecalc-0.0.9.tar.gz`

## Comparing `eeecalc-0.0.8.tar` & `eeecalc-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.idea/base-eeeCalc.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/.DS_Store
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/__init__.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/dBtoRatio.py
--rwxr-xr-x   0        0        0     4721 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/filter.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/general.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/phasors.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/secondDegreeDiffEq.py
--rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/signalFunctions.py
--rwxr-xr-x   0        0        0     2244 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/transferFunctionPlot.py
--rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/trigFunc.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/.idea/.gitignore
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/.idea/eeeCalc.iml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/.idea/misc.xml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/.idea/modules.xml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.8/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eeecalc-0.0.8/tests/filterTest.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.8/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.8/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/base-eeeCalc.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/.DS_Store
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/__init__.py
+-rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/dBtoRatio.py
+-rwxr-xr-x   0        0        0     4721 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/filter.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/general.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/phasors.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/secondDegreeDiffEq.py
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/signalFunctions.py
+-rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/transferFunctionPlot.py
+-rwxr-xr-x   0        0        0      338 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/trigFunc.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/.gitignore
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/eeeCalc.iml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/misc.xml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/modules.xml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eeecalc-0.0.9/src/eeeCalc/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eeecalc-0.0.9/tests/filterTest.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 eeecalc-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 eeecalc-0.0.9/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 eeecalc-0.0.9/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 eeecalc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 eeecalc-0.0.9/PKG-INFO
```

### Comparing `eeecalc-0.0.8/.DS_Store` & `eeecalc-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/.DS_Store` & `eeecalc-0.0.9/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/eeeCalc/dBtoRatio.py` & `eeecalc-0.0.9/src/eeeCalc/dBtoRatio.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/eeeCalc/filter.py` & `eeecalc-0.0.9/src/eeeCalc/filter.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/eeeCalc/general.py` & `eeecalc-0.0.9/src/eeeCalc/general.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/eeeCalc/phasors.py` & `eeecalc-0.0.9/src/eeeCalc/phasors.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/eeeCalc/secondDegreeDiffEq.py` & `eeecalc-0.0.9/src/eeeCalc/secondDegreeDiffEq.py`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/src/eeeCalc/transferFunctionPlot.py` & `eeecalc-0.0.9/src/eeeCalc/transferFunctionPlot.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,63 +13,69 @@
     :param Hz: True uses Hz for frequency, False uses rad/s for frequency
     :param dB: True uses dB for magnitude, False uses just log base 10 of gain for magnitude
     :param degrees: True uses degrees for phase, False uses radians for phase
     :param saveFig: True saves fig, False displays it
     :param fileName: Name of file to be saved - default is "transferPlot.png"
     :return: nothing - plot is either displayed or saved
     """
+
+    #calculates total number of points on graph and uses it to create three ararys representing frequency values,
+    #magnitude values, and phase values
     pointsTot = pointsPerDecade*(upperLog-lowerLog)
     inp = np.linspace(lowerLog,upperLog,pointsTot)
-    x = np.zeros(pointsTot)
     yMag = np.zeros(pointsTot)
     yPhase = np.zeros(pointsTot)
-    jwFunc = lambda x : sDomainFunc(x*complex(0,1))
 
+
+
+
+    #defines basic multipliers for easy switching between units later
     magMult = 1
     if dB:
         magMult = 20
-
     phaseMult = 1
     if degrees:
         phaseMult = 180/pi
 
-    for i,val in enumerate(inp):
-        yMag[i] = magMult*log(pol(jwFunc(10 ** val))[0])
-        yPhase[i] = phaseMult*pol(jwFunc(10 ** val))[1]
-
+    #defines unit to be used for xaxis and
+    #converts transfer function from H(s) to H(jw) or H(j2pif) depending on units
     if Hz:
         xunit = "Hz"
+        jwFunc = lambda x: sDomainFunc(x * complex(0, 1) * 2 * pi)
     else:
         xunit = "rad/s"
+        jwFunc = lambda x: sDomainFunc(x * complex(0, 1))
+
+    #calculates phase and magnitude values
+    for i,val in enumerate(inp):
+        yMag[i] = magMult*log(pol(jwFunc(10 ** val))[0])
+        yPhase[i] = phaseMult*pol(jwFunc(10 ** val))[1]
 
+    #plots values using matplotlib
     plt.rcParams["figure.figsize"] = [7.50, 3.50]
     plt.rcParams["figure.autolayout"] = True
-
     ax1 = plt.subplot()
     l1, = ax1.plot(inp,yMag, color='blue')
     ax2 = ax1.twinx()
     l2, = ax2.plot(inp,yPhase, color='orange')
-    plt.legend([l1, l2], ["Magnitude", "Phase"])
-
-
 
+    #adds legends and labels
+    plt.legend([l1, l2], ["Magnitude", "Phase"])
     ax1.set_xlabel("Frequency in {}".format(xunit))
-
-
     if dB:
         ax1.set_ylabel("Gain in dB")
     else:
         ax1.set_ylabel("Gain")
-
     if degrees:
         ax2.set_ylabel("Phase shift in degrees")
     else:
         ax2.set_ylabel("Phase shift in radians")
 
+    #saves or shows graph depending on what's chosen
     if saveFig:
         plt.savefig(fileName)
     else:
         plt.show()
 
-
-def transientPlot(tFunc,inp,numFourierTerms=1000):
-    return
+if __name__=="__main__":
+    func = lambda s: (2000+s)/((1000+s))
+    transferFunctionPlot(func,Hz=True)
```

### Comparing `eeecalc-0.0.8/src/eeeCalc/.idea/workspace.xml` & `eeecalc-0.0.9/src/eeeCalc/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/LICENSE` & `eeecalc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eeecalc-0.0.8/pyproject.toml` & `eeecalc-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "eeeCalc"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Kevin Johnson", email="john2003.kjj@gmail.com" },
 ]
 description = "Package to aid electrical engineering calculations"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

