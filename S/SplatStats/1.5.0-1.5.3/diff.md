# Comparing `tmp/SplatStats-1.5.0.tar.gz` & `tmp/SplatStats-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-1.5.0.tar", last modified: Mon May  8 00:36:46 2023, max compression
+gzip compressed data, was "SplatStats-1.5.3.tar", last modified: Tue May  9 17:06:45 2023, max compression
```

## Comparing `SplatStats-1.5.0.tar` & `SplatStats-1.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-08 00:36:46.681797 SplatStats-1.5.0/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-09-17 20:12:28.000000 SplatStats-1.5.0/LICENSE
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-08 00:36:46.681797 SplatStats-1.5.0/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6368 2023-01-25 04:16:56.000000 SplatStats-1.5.0/README.md
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-08 00:36:46.673797 SplatStats-1.5.0/SplatStats/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10828 2023-03-14 03:30:29.000000 SplatStats-1.5.0/SplatStats/Battle.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10240 2022-11-24 03:14:30.000000 SplatStats-1.5.0/SplatStats/Player.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2750 2023-04-05 03:12:55.000000 SplatStats-1.5.0/SplatStats/StatInk.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2477 2022-11-01 00:29:50.000000 SplatStats-1.5.0/SplatStats/Team.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      896 2023-03-19 21:08:44.000000 SplatStats-1.5.0/SplatStats/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       21 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6148 2022-12-04 18:34:39.000000 SplatStats-1.5.0/SplatStats/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13947 2023-05-08 00:35:21.000000 SplatStats-1.5.0/SplatStats/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     5393 2023-02-27 04:39:12.000000 SplatStats-1.5.0/SplatStats/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4137 2023-03-14 03:19:39.000000 SplatStats-1.5.0/SplatStats/files.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8663 2023-02-17 22:36:56.000000 SplatStats-1.5.0/SplatStats/parsers.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    46328 2023-04-06 00:24:58.000000 SplatStats-1.5.0/SplatStats/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1428 2022-09-29 02:14:29.000000 SplatStats-1.5.0/SplatStats/plotsAux.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1709 2022-11-14 00:32:41.000000 SplatStats-1.5.0/SplatStats/plotsTeam.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10176 2023-04-06 04:24:33.000000 SplatStats-1.5.0/SplatStats/statInkConstants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10543 2023-04-28 00:57:38.000000 SplatStats-1.5.0/SplatStats/statInkPlots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8511 2023-04-06 03:09:35.000000 SplatStats-1.5.0/SplatStats/statInkStats.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13660 2023-04-13 18:00:01.000000 SplatStats-1.5.0/SplatStats/stats.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-08 00:36:46.681797 SplatStats-1.5.0/SplatStats.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      607 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      159 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       11 2023-05-08 00:36:46.000000 SplatStats-1.5.0/SplatStats.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-05-08 00:36:46.681797 SplatStats-1.5.0/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1251 2023-02-19 19:16:43.000000 SplatStats-1.5.0/setup.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-09 17:06:45.269565 SplatStats-1.5.3/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-09-17 20:12:28.000000 SplatStats-1.5.3/LICENSE
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-09 17:06:45.265565 SplatStats-1.5.3/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6368 2023-01-25 04:16:56.000000 SplatStats-1.5.3/README.md
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-09 17:06:45.265565 SplatStats-1.5.3/SplatStats/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10828 2023-03-14 03:30:29.000000 SplatStats-1.5.3/SplatStats/Battle.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10398 2023-05-09 04:00:59.000000 SplatStats-1.5.3/SplatStats/Player.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     3058 2023-05-08 04:02:05.000000 SplatStats-1.5.3/SplatStats/StatInk.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2477 2022-11-01 00:29:50.000000 SplatStats-1.5.3/SplatStats/Team.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      896 2023-03-19 21:08:44.000000 SplatStats-1.5.3/SplatStats/__init__.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       21 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats/_version.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6148 2022-12-04 18:34:39.000000 SplatStats-1.5.3/SplatStats/auxiliary.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13947 2023-05-08 00:35:21.000000 SplatStats-1.5.3/SplatStats/colors.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     5393 2023-05-09 16:49:18.000000 SplatStats-1.5.3/SplatStats/constants.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4137 2023-03-14 03:19:39.000000 SplatStats-1.5.3/SplatStats/files.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8663 2023-02-17 22:36:56.000000 SplatStats-1.5.3/SplatStats/parsers.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    56269 2023-05-09 05:39:51.000000 SplatStats-1.5.3/SplatStats/plots.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1428 2022-09-29 02:14:29.000000 SplatStats-1.5.3/SplatStats/plotsAux.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1709 2022-11-14 00:32:41.000000 SplatStats-1.5.3/SplatStats/plotsTeam.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10176 2023-04-06 04:24:33.000000 SplatStats-1.5.3/SplatStats/statInkConstants.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10543 2023-04-28 00:57:38.000000 SplatStats-1.5.3/SplatStats/statInkPlots.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8511 2023-04-06 03:09:35.000000 SplatStats-1.5.3/SplatStats/statInkStats.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13991 2023-05-09 04:12:42.000000 SplatStats-1.5.3/SplatStats/stats.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-09 17:06:45.265565 SplatStats-1.5.3/SplatStats.egg-info/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      607 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/SOURCES.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/dependency_links.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      159 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/requires.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       11 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/top_level.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-05-09 17:06:45.269565 SplatStats-1.5.3/setup.cfg
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1251 2023-02-19 19:16:43.000000 SplatStats-1.5.3/setup.py
```

### Comparing `SplatStats-1.5.0/LICENSE` & `SplatStats-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/PKG-INFO` & `SplatStats-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.5.0
+Version: 1.5.3
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.5.0/README.md` & `SplatStats-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/Battle.py` & `SplatStats-1.5.3/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/Player.py` & `SplatStats-1.5.3/SplatStats/Player.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,30 +71,33 @@
             battle = aux.loadBattle(batFile)
             battleRecords.append(battle)
         return battleRecords
 
     ###########################################################################
     # Get player history dataframe
     ###########################################################################
-    def parsePlayerHistoryFromBattles(self, validOnly=True):
+    def parsePlayerHistoryFromBattles(self, validOnly=True, ammendWeapons=True):
         """Extracts the player's history from the battle records by matching the name in the dataframes.
 
         Args:
             validOnly (bool, optional): Filters out battles which didn't finish correctly (disconnects). Defaults to True.
 
         Returns:
             dataframe: Full battle history dataframe for the player, in which each row is the result of a match.
         """        
         battlesHistory = par.parsePlayerHistoryFromBattles(
             self.battleRecords, self.name, 
             validOnly=validOnly, timezone=self.timezone
         )
         battlesHistory['winBool'] = [1 if i=='W' else 0 for i in battlesHistory['win']]
         battlesHistory['loseBool'] = [1 if i=='L' else 0 for i in battlesHistory['win']]
-        self.battlesHistory = battlesHistory
+        if ammendWeapons:
+            self.battlesHistory = battlesHistory.replace('Hero Shot Replica', 'Splattershot')
+        else:
+            self.battlesHistory = battlesHistory
         return self.battlesHistory
     
     def getPlayerHistoryByTypes(self):
         """Groups the player history into dictionary items corresponding to the match type played.
 
         Returns:
             dict of dataframes: Dictionary containing the different battle history dataframes.
```

### Comparing `SplatStats-1.5.0/SplatStats/StatInk.py` & `SplatStats-1.5.3/SplatStats/StatInk.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,41 +13,51 @@
     fPaths: list of paths
         Filepaths of the battle results csv files loaded for analysis
     rawResults: dataframe
         Dataframe containing battle results information directly from stat.ink
     battleResults: dataframe
         Clean dataframe containing results in human-readable form
     """
-    def __init__(self, resultsPaths, fNamePattern='*-*-*.csv'):
+    def __init__(
+            self, resultsPaths, 
+            fNamePattern='*-*-*.csv'
+        ):
         self.fPaths = glob(path.join(resultsPaths, fNamePattern))
         # Read csv's into a dataframe ----------------------------------------
         rawDFList = [
             pd.read_csv(
-                f, parse_dates=['period'], dtype=ink.STATINK_DTYPES, 
+                f, 
+                parse_dates=['period'], 
+                dtype=ink.STATINK_DTYPES, 
+                on_bad_lines='skip'
             ) for f in self.fPaths
         ]
         self.rawResults = pd.concat(rawDFList)
         # Clean dataframe to standard names/times ----------------------------
         self.battlesResults = self.cleanBattlesDataframe(self.rawResults)
         
     def cleanBattlesDataframe(
             self, rawResults,
-            naColor='#00000000', naBool=-1, naString='NA', naInt=0
+            naColor='#00000000', naBool=-1, naString='NA', 
+            naInt=0, ammendWeapons=True
         ):
         df = rawResults.copy()
         # Cleaning column names ----------------------------------------------
         df.columns = [i.replace('#', '').strip() for i in list(rawResults.columns)]
         # Replace simple columns ---------------------------------------------
         df['lobby'] = [ink.LOBBY_MODE[l] for l in df['lobby']]
         df['mode']  = [ink.GAME_MODE[m] for m in df['mode']]
         df['stage'] = [ink.STGS_DICT[s] for s in df['stage']]
         # Replace weapon names (US standard) ---------------------------------
         for i in range(1, 5):
             df[f'A{i}-weapon'] = [ink.WPNS_DICT[w] for w in df[f'A{i}-weapon']]
             df[f'B{i}-weapon'] = [ink.WPNS_DICT[w] for w in df[f'B{i}-weapon']]
+        # Ammend Duplicate Weapons (US standard) -----------------------------
+        if ammendWeapons:
+            df = df.replace('Hero Shot Replica', 'Splattershot')
         # Replace knockouts, ranks and wins ----------------------------------
         df['knockout'] = [int(k) if (type(k) is bool) else naBool for k in df['knockout']]
         df['rank'] = [r if type(r) is str else naString for r in df['rank']]
         df['power'] = df['power'].fillna(naInt)
         df['win'] = [True if (i=='alpha') else False for i in df['win']]
         # Cleanup colors -----------------------------------------------------
         df['alpha-color'] = [f'#{c}' if type(c) is str else naColor for c in df['alpha-color']]
```

### Comparing `SplatStats-1.5.0/SplatStats/Team.py` & `SplatStats-1.5.3/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/__init__.py` & `SplatStats-1.5.3/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/auxiliary.py` & `SplatStats-1.5.3/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/colors.py` & `SplatStats-1.5.3/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/constants.py` & `SplatStats-1.5.3/SplatStats/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,24 +94,24 @@
 CLR_WEAPON = {
     'Clash Blaster': '#0D37C3',
     'Hero Shot Replica': '#FDFF00',
     'Splattershot': '#4F55ED',
     'Tentatek Splattershot': '#C920B7',
 }
 CLR_CLS_LONG = [
+    clr.TSUBUAN_V_KOSHIAN_S2[1],
+    clr.FAM_V_FRIEND_S2[1],
+    clr.DBLUE_V_YELLOW_S1[0],
+    clr.YELLOW_V_DTEAL_LK_S3[0], clr.YELLOW_V_DTEAL_LK_S3[1], clr.YELLOW_V_DTEAL_LK_S3[2],
+    clr.WINNERW_V_WOUTERW_S2[0], clr.WINNERW_V_WOUTERW_S2[1], clr.WINNERW_V_WOUTERW_S2[2],
     clr.LPINK_V_BLUE_S2[0], clr.LPINK_V_BLUE_S2[1],
     clr.NPINK_V_NGREEN_S2[1], 
     clr.RASPBERRY_V_NYELLOW_S2[1],
-    clr.WINNERW_V_WOUTERW_S2[0], clr.WINNERW_V_WOUTERW_S2[1], clr.WINNERW_V_WOUTERW_S2[2],
     clr.YELLOW_V_LBLU_V_DBLU_LK_S3[1], clr.BLUE_FRYE_S3[2],
-    clr.GRAPE_V_TURQUOISE_S2[0], clr.GRAPE_V_TURQUOISE_S2[1],
-    clr.TSUBUAN_V_KOSHIAN_S2[1],
-    clr.FAM_V_FRIEND_S2[1],
-    clr.DBLUE_V_YELLOW_S1[0],
-    clr.YELLOW_V_DTEAL_LK_S3[0], clr.YELLOW_V_DTEAL_LK_S3[1], clr.YELLOW_V_DTEAL_LK_S3[2]
+    clr.GRAPE_V_TURQUOISE_S2[0], clr.GRAPE_V_TURQUOISE_S2[1]
 ]
 CLR_BAR = clr.SMUSHROOM_V_SSTAR_S2[-1]
 ###############################################################################
 # Weapons Classes
 ###############################################################################
 WPN_CLASS = {
     'Blaster': {
```

### Comparing `SplatStats-1.5.0/SplatStats/files.py` & `SplatStats-1.5.3/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/parsers.py` & `SplatStats-1.5.3/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/plots.py` & `SplatStats-1.5.3/SplatStats/plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 
+import math
 import squarify
 import pandas as pd
 import numpy as np
 import seaborn as sns
 from pywaffle import Waffle
 import matplotlib.pyplot as plt
 from math import radians, log10
+import matplotlib.colors as mcolors
 from matplotlib.patches import Rectangle
 import SplatStats.constants as cst
 import SplatStats.stats as stats
 import SplatStats.auxiliary as aux
 import SplatStats.colors as clr
 import SplatStats.plotsAux as paux
 import warnings
@@ -1044,7 +1046,275 @@
     )
     ax_p.set_thetamin(thetaRange[0]); ax_p.set_thetamax(thetaRange[1])
     ax_p.text(.75, .1, cats[2], fontsize=15, ha='left', transform=ax_p.transAxes)
     [x.set_linewidth(1.5) for x in ax_p.spines.values()]
     # ax.set(frame_on=False)
     # Return ------------------------------------------------------------------
     return (fig, (ax_k, ax_d, ax_a, ax_p))
+
+
+
+
+
+def plotIrisKDP(
+        playerHistory, figAx, 
+        kassist=True, paint=True, 
+        clockwise=True, innerOffset=2,
+        colorsKD=('#4E4EDDCC', '#CD2D7ECC'), colorP='#6A1EC111',
+        rangeKD=(0, 40), rangeP=(0, 3500),
+        lw=0.25
+    ):
+    (fig, ax) = figAx
+    # Calculate numbers -------------------------------------------------------
+    (outer, inner) = (
+        np.array(playerHistory['kill']), 
+        np.array(playerHistory['death'])
+    )
+    bar = (np.array(playerHistory['paint']) if paint else None)
+    if kassist:
+        outer = outer + (.5*np.array(playerHistory['assist']))
+    kdRatio = np.sum(outer)/np.sum(inner)
+    (topArray, bottomArray, barArray) = (outer, inner, bar)
+    # Calculate angles for marker lines ---------------------------------------
+    DLEN = topArray.shape[0]
+    (astart, aend) = ((2*np.pi, 0) if clockwise else (0, 2*np.pi))
+    ANGLES = np.linspace(astart, aend, DLEN, endpoint=False)
+    # Draw top-bottom (kill-death) --------------------------------------------
+    if bottomArray is None:
+        bottomArray = np.zeros(topArray.shape)
+    heights = topArray-bottomArray
+    colors = [colorsKD[0] if (h>=0) else colorsKD[1] for h in heights]
+    ax.vlines(
+        ANGLES, innerOffset+bottomArray, innerOffset+topArray, 
+        lw=lw, colors=colors
+    )
+    # Draw bar ----------------------------------------------------------------
+    if barArray is None:
+        barScaled = np.zeros(topArray.shape)
+    else:
+        barScaled = np.interp(barArray, rangeP, (rangeKD[0]*2, rangeKD[1]*2))
+    ax.vlines(
+        ANGLES, innerOffset, innerOffset+barScaled,  
+        lw=lw, colors=colorP
+    )
+    # Return figAx and stats --------------------------------------------------
+    return ((fig, ax), kdRatio)
+
+
+def plotIrisMatch(
+        playerHistory, figAx,
+        innerRadius=40, typeLineLength=10, lw=0.25,
+        colorsKO=('#311AA8', '#E70F21', '#ffffff'),
+        offsets=(2, 5, 7), clockwise=True,
+        mTypeColors = {
+            'Clam Blitz': '#D60E6E',
+            'Rainmaker': '#7D26B5',
+            'Splat Zones': '#3D59DE',
+            'Tower Control': '#8ACF47',
+            'Tricolor Turf War': '#88214D',
+            'Turf War': '#D1D1D1'
+        },
+        winColors={True: '#6BD52C', False: '#D1D1D1'}
+    ):
+    (fig, ax) = figAx
+    # Calculate angles for marker lines ---------------------------------------
+    DLEN = np.array(playerHistory['kill']).shape[0]
+    (astart, aend) = ((2*np.pi, 0) if clockwise else (0, 2*np.pi))
+    ANGLES = np.linspace(astart, aend, DLEN, endpoint=False)
+    # Match type --------------------------------------------------------------
+    (mTypeOff, mTypeHeight) = (innerRadius+offsets[0], typeLineLength)
+    (wBoolOff, wBoolHeight) = (
+        mTypeOff+mTypeHeight, 
+        mTypeOff+mTypeHeight+offsets[1]
+    )
+    (kBoolOff, kBoolHeight) = (
+        mTypeOff+mTypeHeight+offsets[1], 
+        mTypeOff+mTypeHeight+offsets[2]
+    )
+    ax.vlines(
+        ANGLES, mTypeOff, mTypeOff+mTypeHeight, 
+        colors=[mTypeColors[i] for i in playerHistory['match type']],
+        zorder=-5, lw=lw
+    )
+    # Win ---------------------------------------------------------------------
+    ax.vlines(
+        ANGLES, wBoolOff, wBoolHeight, 
+        colors=[winColors[i] for i in playerHistory['winBool']],
+        zorder=-5, lw=lw
+    )
+    # KO ----------------------------------------------------------------------
+    winKO = []
+    for wko in list(zip(playerHistory['winBool'], playerHistory['ko'])):
+        if wko[-1]:
+            if wko[0]:
+                winKO.append(colorsKO[0])
+            else:
+                winKO.append(colorsKO[1])
+        else:
+            winKO.append(colorsKO[2])
+    ax.vlines(
+        ANGLES, kBoolOff, kBoolHeight, 
+        lw=lw, colors=winKO, zorder=-5
+    )
+    ax.set_rscale('symlog')
+    return (fig, ax)
+
+
+def plotIrisStats(
+        playerHistory, figAx,
+        binSize=1, binMax=20, innerOffset=2, meanStat=True, barWidth=0.1,
+        pstats=('kill', 'death', 'assist', 'special', 'ink'),
+        colorBarEdge='#00000033', linewidthEdge=0.1,
+        colorMean='#00000099', linewidthMean=0.5,
+        INKSTATS_STYLE = {
+            'kill': {
+                'color': '#1A1AAEDD', 'range': (0, 15),
+                'scaler': lambda x: np.interp(x, [0, 0.125, 0.25], [0, .50, 1]),
+                'range': (0, 15)
+            },
+            'death': {
+                'color': '#CD2D7EDD', 'range': (0, 15),
+                'scaler': lambda x: np.interp(x, [0, 0.125, 0.25], [0, .50, 1]),
+                'range': (0, 15)
+            },
+            'assist': {
+                'color': '#801AB3DD', 'range': (0, 10),
+                'scaler': lambda x: np.interp(x, [0, 0.250, 0.65], [0, .50, 1]),
+                
+            },
+            'special': {
+                'color': '#1FAFE8DD', 'range': (0, 10),
+                'scaler': lambda x: np.interp(x, [0, 0.250, 0.65], [0, .50, 1]),
+            },
+            'ink': {
+                'color': '#35BA49DD', 'range': (0, 20),
+                'scaler': lambda x: np.interp(x, [0, 0.100, 0.20], [0, .50, 1]),
+            }
+        }
+    ):
+    (fig, ax) = figAx
+    playerHistory['ink'] = playerHistory['paint']/100
+    statsHists = {
+        i: stats.calcBinnedFrequencies(
+            np.array(playerHistory[i]), 0, binMax, 
+            binSize=binSize, normalized=True
+        )
+        for i in pstats
+    }
+    # Vspan for stats -------------------------------------------------------------
+    binsNum = statsHists['kill'].shape[0]
+    (dHeight, rWidth) = (barWidth, 2*math.pi/binsNum)
+    statsNames = list(pstats)
+    # Iterate through stats
+    for (ix, stat) in enumerate(statsNames):
+        # Iterate through bins
+        (clr, sca) = (
+            mcolors.ColorConverter().to_rgba(INKSTATS_STYLE[stat]['color']),
+            INKSTATS_STYLE[stat]['scaler']
+        )
+        bins = statsHists[stat]
+        for (jx, h) in enumerate(range(binsNum)):
+            alpha = sca(bins[jx])
+            ax.add_patch(
+                Rectangle(
+                    (-jx*rWidth, innerOffset-ix*dHeight), -rWidth, -dHeight,
+                    facecolor=(clr[0], clr[1], clr[2], alpha),
+                    edgecolor=colorBarEdge, lw=linewidthEdge
+                )
+            )
+            ax.bar(0, 1).remove()
+    # Quantiles ---------------------------------------------------------------
+    statQNT = {s: np.quantile(playerHistory[s], [0.25, 0.50, 0.75]) for s in pstats}
+    statMNS = {s: np.mean(playerHistory[s]) for s in pstats}
+    rSca = 0.15
+    for (ix, stat) in enumerate(statsNames):
+        if meanStat:
+            rPos = np.interp(statMNS[stat], [0, binMax], [2*np.pi, 0])
+            ax.vlines(
+                rPos, 
+                innerOffset-(ix)*dHeight-rSca*dHeight, 
+                innerOffset-(1+ix)*dHeight+rSca*dHeight,  
+                lw=linewidthMean, colors=colorMean
+            )
+        else:
+            rPos = [
+                np.interp(x, [0, binMax], [2*np.pi, 0])-rWidth/2
+                for x in statQNT[stat]
+            ]
+            ax.vlines(
+                rPos[1], 
+                innerOffset-(ix)*dHeight-rSca*dHeight, 
+                innerOffset-(1+ix)*dHeight+rSca*dHeight,  
+                lw=linewidthMean, colors=colorMean
+            )
+            ax.vlines(
+                [rPos[0], rPos[2]], 
+                innerOffset-(ix)*dHeight-rSca*dHeight, 
+                innerOffset-(1+ix)*dHeight+rSca*dHeight,  
+                lw=linewidthMean*0.25, colors=colorMean
+            )
+    return ((fig, ax), statQNT, statMNS)
+
+
+def plotIrisAxes(
+        figAx, innerOffset=2, statsNum=5, yRange=(0, 100), 
+        barWidth=0.1, frameColor="#00000000", rangeKD=(0, 40), lw=0.25, 
+        innerGuides=(0, 6, 1), innerGuidesColor="#00000088",
+        outerGuides=(0, 50, 10), outerGuidesColor="#00000088"
+    ):
+    (fig, ax) = figAx
+    ax.vlines(
+        [0], innerOffset-barWidth*statsNum, innerOffset+rangeKD[1], 
+        lw=lw, color='#000000CC',
+        zorder=10
+    )
+    circleAngles = np.linspace(0, 2*np.pi, 200)
+    for r in range(*innerGuides):
+        ax.plot(
+            circleAngles, np.repeat(r+innerOffset, 200), 
+            color=innerGuidesColor, lw=0.1,
+            zorder=10
+        )
+    ax.plot(
+        circleAngles, np.repeat(innerOffset-barWidth*5, 200), 
+        color='#000000FF', lw=lw, # ls='-.', 
+        zorder=10
+    )
+    ax.set_theta_offset(np.pi/2)
+    ax.set_xticks([])
+    ax.set_xticklabels([])
+    ax.set_yticklabels([])
+    yTicks = [0+innerOffset] + list(np.arange(
+        outerGuides[0]+innerOffset, outerGuides[1]+innerOffset, outerGuides[2]
+    ))
+    ax.set_yticks(yTicks)
+    ax.yaxis.grid(True, color=outerGuidesColor, ls='-', lw=0.2, zorder=10)
+    ax.spines["start"].set_color("none")
+    ax.spines["polar"].set_color(frameColor)
+    ax.set_ylim(yRange[0], yRange[1])
+    return (fig, ax)
+
+
+def plotIrisHistory(
+        playerHistory, figAx=None, 
+        kassist=True, paint=True, innerOffset=2, clockwise=True,
+        colorsKD=('#4E4EDDCC', '#CD2D7ECC'), colorP='#6A1EC111',
+        rangeKD=(0, 40), rangeP=(0, 3500),
+    ):
+    # Generate (fig, ax) if needed --------------------------------------------
+    if figAx is None:
+        (fig, ax) = plt.subplots(
+            figsize=(10, 10), subplot_kw={"projection": "polar"}
+        )
+    else:
+        (fig, ax) = figAx
+    # Plot kill/death/paint bars ----------------------------------------------
+    ((fig, ax), kdRatio) = plotIrisKDP(
+            playerHistory, figAx, 
+            kassist=kassist, paint=paint, 
+            clockwise=clockwise, innerOffset=innerOffset,
+            colorsKD=colorsKD, colorP=colorP,
+            rangeKD=rangeKD, rangeP=rangeP,
+            lw=0.25
+        )
+    # Return figAx ------------------------------------------------------------
+    return (fig, ax)
```

### Comparing `SplatStats-1.5.0/SplatStats/plotsAux.py` & `SplatStats-1.5.3/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/plotsTeam.py` & `SplatStats-1.5.3/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/statInkConstants.py` & `SplatStats-1.5.3/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/statInkPlots.py` & `SplatStats-1.5.3/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/statInkStats.py` & `SplatStats-1.5.3/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/SplatStats/stats.py` & `SplatStats-1.5.3/SplatStats/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -343,8 +343,18 @@
     for i in myList:
         if i == elem:
             size += 1
             if size > max_size:
                 max_size = size
         else:
             size = 0
-    return max_size
+    return max_size
+
+
+def statSummaries(playerHistory, stat, summaryFuns=(np.sum, np.mean)):
+    return [fun(playerHistory[stat]) for fun in summaryFuns]
+
+
+def statPerMinute(playerHistory, stat, summaryFun=None):
+    statPM = (playerHistory[stat]/(playerHistory['duration']/60))
+    stpm = summaryFun(statPM) if summaryFun else statPM
+    return stpm
```

### Comparing `SplatStats-1.5.0/SplatStats.egg-info/PKG-INFO` & `SplatStats-1.5.3/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.5.0
+Version: 1.5.3
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.5.0/SplatStats.egg-info/SOURCES.txt` & `SplatStats-1.5.3/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.0/setup.py` & `SplatStats-1.5.3/setup.py`

 * *Files identical despite different names*

