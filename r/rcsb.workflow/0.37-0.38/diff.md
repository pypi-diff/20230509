# Comparing `tmp/rcsb.workflow-0.37.tar.gz` & `tmp/rcsb.workflow-0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.workflow-0.37.tar", last modified: Wed Mar 22 20:51:44 2023, max compression
+gzip compressed data, was "rcsb.workflow-0.38.tar", last modified: Tue May  9 18:04:08 2023, max compression
```

## Comparing `rcsb.workflow-0.37.tar` & `rcsb.workflow-0.38.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/
--rw-r--r--   0 vsts      (1001) docker     (122)     2154 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:51:44.149099 rcsb.workflow-0.37/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/rcsb/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/rcsb/workflow/chem/
--rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/chem/ChemCompFileWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/chem/ChemCompImageWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/rcsb/workflow/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)    10200 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28223 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/rcsb/workflow/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/rcsb.workflow.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-03-22 20:51:44.000000 rcsb.workflow-0.37/rcsb.workflow.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-03-22 20:51:44.000000 rcsb.workflow-0.37/rcsb.workflow.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 20:51:44.000000 rcsb.workflow-0.37/rcsb.workflow.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 20:51:41.000000 rcsb.workflow-0.37/rcsb.workflow.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-03-22 20:51:44.000000 rcsb.workflow-0.37/rcsb.workflow.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-22 20:51:44.000000 rcsb.workflow-0.37/rcsb.workflow.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-22 20:51:44.153099 rcsb.workflow-0.37/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-03-22 20:11:33.000000 rcsb.workflow-0.37/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2275 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.950277 rcsb.workflow-0.38/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.954277 rcsb.workflow-0.38/rcsb/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.954277 rcsb.workflow-0.38/rcsb/workflow/chem/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompFileWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompImageWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/rcsb/workflow/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10335 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28640 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/rcsb/workflow/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 18:04:08.950277 rcsb.workflow-0.38/rcsb.workflow.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 18:04:07.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-09 18:04:08.000000 rcsb.workflow-0.38/rcsb.workflow.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-09 18:04:08.958278 rcsb.workflow-0.38/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-05-09 16:59:26.000000 rcsb.workflow-0.38/setup.py
```

### Comparing `rcsb.workflow-0.37/HISTORY.txt` & `rcsb.workflow-0.38/HISTORY.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 29-Jul-2021 - V0.30 Cache taxonomy data at the beginning of the ProteinTargetSequenceWorkflow, force rebuild of DrugBankProvider()
 29-Jul-2021 - V0.31 Broaden cache policy for cofactor providers.
 26-Aug-2021 - V0.32 Update dependencies
 27-Jun-2022 - V0.33 Change the molBuildType value from "model-xyz" to "connection-table" in ChemCompImageWorkflow()
  9-Jan-2023 - V0.34 Configuration changes to support tox 4
  3-Mar-2023 - V0.35 Standardize args in ProteinTargetSequenceExecutionWorkflow
 14-Mar-2023 - V0.36 Generate CARD annotations instead of features during ProteinTargetSequenceExecutionWorkflow
-21-Mar-2023 - V0.37 Allow backing up Pharos-targets to stash
+21-Mar-2023 - V0.37 Allow backing up Pharos-targets to stash
+ 5-May-2023 - V0.38 Add fromDbPharos and reloadPharos parameters to ProteinTargetSequenceExecutionWorkflow.exportFasta()
```

### Comparing `rcsb.workflow-0.37/LICENSE` & `rcsb.workflow-0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.37/PKG-INFO` & `rcsb.workflow-0.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.37
+Version: 0.38
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.37/README.md` & `rcsb.workflow-0.38/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.37/rcsb/workflow/chem/ChemCompFileWorkflow.py` & `rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompFileWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.37/rcsb/workflow/chem/ChemCompImageWorkflow.py` & `rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompImageWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.37/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py` & `rcsb.workflow-0.38/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.37/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py` & `rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # File:    ProteinTargetSequenceExecutionWorkflow.py
 # Author:  J. Westbrook
 # Date:    25-Jun-2021
 #
 # Updates:
 #   3-Mar-2023 Standard args passed into workflow
 #  21-Mar-2023 Allow backing up Pharos-targets to stash, more __init__ improvement
+#   5-May-2023 Pass in fromDbPharos and reloadPharos parameters to exportFasta()
 ##
 """
 Execution workflow for protein target data ETL operations.
 """
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
@@ -129,25 +130,25 @@
         try:
             ptsW = ProteinTargetSequenceWorkflow(self.__cfgOb, self.__cachePath)
             ok = ptsW.exportRCSBLigandNeighborMapping()
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
 
-    def exportFasta(self):
+    def exportFasta(self, reloadPharos=True, fromDbPharos=True):
         """Export FASTA target files (and load Pharos from source)"""
         logger.info("Running exportFasta...")
         ok = False
         try:
             ptsW = ProteinTargetSequenceWorkflow(self.__cfgOb, self.__cachePath)
             ok = ptsW.exportTargetsFasta(
                 useCache=True,
                 addTaxonomy=True,
-                reloadPharos=True,
-                fromDbPharos=True,
+                reloadPharos=reloadPharos,
+                fromDbPharos=fromDbPharos,
                 resourceNameList=["sabdab", "card", "drugbank", "chembl", "pharos"],
                 backupPharos=True,
                 remotePrefix=self.__stashRemotePrefix
             )
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
```

### Comparing `rcsb.workflow-0.37/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py` & `rcsb.workflow-0.38/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #  Updates:
 #  25-Jul-2021 add new StashableBase options for git backup
 #  29-Jul-2021 DrugBankProvider needs useCache=False to always rebuild
 #   3-Mar-2023 Fix error for missing taxonPath
 #  14-Mar-2023 Generate CARD annotations instead of CARD features
 #  21-Mar-2023 Allow backing up Pharos-targets to stash
+#   5-May-2023 Restore from stash if fromDbPharos and reloadPharos parameters are False
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
@@ -177,14 +178,18 @@
                 pw = self.__cfgOb.get("_MYSQL_DB_PASSWORD", sectionName=configName)
                 ptP = PharosTargetProvider(cachePath=self.__cachePath, useCache=useCache, reloadDb=reloadPharos, fromDb=fromDbPharos, mysqlUser=user, mysqlPassword=pw)
                 if ptP.testCache():
                     ok = ptP.exportProteinFasta(fastaPath, taxonPath, addTaxonomy=addTaxonomy)
                     if backupPharos:
                         okB = ptP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
                         logger.info("%r targets backup status (%r)", resourceName, okB)
+                elif not (reloadPharos or fromDbPharos):
+                    ptP.restore(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
+                    if ptP.testCache():
+                        ok = ptP.exportProteinFasta(fastaPath, taxonPath, addTaxonomy=addTaxonomy)
             elif resourceName == "sabdab":
                 stP = SAbDabTargetProvider(cachePath=self.__cachePath, useCache=False)
                 if stP.testCache():
                     ok = stP.exportFasta(fastaPath)
             elif resourceName == "pdbprent":
                 pEx = PolymerEntityExtractor(self.__cfgOb)
                 detailsPath = self.__getDetailsPath(resourceName)
@@ -470,15 +475,15 @@
                     okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
                     logger.info("%r cofactor backup status (%r)", resourceName, okB)
 
             elif resourceName == "pharos":
                 aP = PharosTargetCofactorProvider(cachePath=self.__cachePath, useCache=True, useStash=True, useGit=True)
                 ok = aP.buildCofactorList(resultPath, crmpObj=crmpObj, lnmpObj=lnmpObj, maxActivity=maxActivity)
                 if backup:
-                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix)
+                    okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useGit=True)
                     logger.info("%r cofactor data backup status (%r)", resourceName, okB)
 
             elif resourceName == "drugbank":
                 aP = DrugBankTargetCofactorProvider(cachePath=self.__cachePath, useCache=True)
                 ok = aP.buildCofactorList(resultPath, crmpObj=crmpObj, lnmpObj=lnmpObj)
                 if backup:
                     okB = aP.backup(self.__cfgOb, self.__configName, remotePrefix=remotePrefix, useStash=True, useGit=True)
```

### Comparing `rcsb.workflow-0.37/rcsb.workflow.egg-info/PKG-INFO` & `rcsb.workflow-0.38/rcsb.workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.37
+Version: 0.38
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.37/rcsb.workflow.egg-info/SOURCES.txt` & `rcsb.workflow-0.38/rcsb.workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.37/setup.py` & `rcsb.workflow-0.38/setup.py`

 * *Files identical despite different names*

