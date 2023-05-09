# Comparing `tmp/misura-1.5.4.tar.gz` & `tmp/misura-1.5.5.tar.gz`

## Comparing `misura-1.5.4.tar` & `misura-1.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.4/.gitattributes
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 misura-1.5.4/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 misura-1.5.4/docs/docs.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 misura-1.5.4/src/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/__main__.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/exceptions.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/globals.py
--rw-r--r--   0        0        0    24681 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/quantities.py
--rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/tables.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.4/LICENSE
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 misura-1.5.4/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 misura-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.5/.gitattributes
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 misura-1.5.5/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 misura-1.5.5/docs/docs.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 misura-1.5.5/src/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/__main__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/exceptions.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/globals.py
+-rw-r--r--   0        0        0    24403 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/quantities.py
+-rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/tables.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 misura-1.5.5/src/misura/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.5/LICENSE
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 misura-1.5.5/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 misura-1.5.5/PKG-INFO
```

### Comparing `misura-1.5.4/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.5.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/.github/workflows/python-publish.yml` & `misura-1.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/docs/docs.md` & `misura-1.5.5/docs/docs.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/src/test.py` & `misura-1.5.5/src/test.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/src/misura/__main__.py` & `misura-1.5.5/src/misura/__main__.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/src/misura/exceptions.py` & `misura-1.5.5/src/misura/exceptions.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/src/misura/quantities.py` & `misura-1.5.5/src/misura/quantities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quantities.
 from __future__ import annotations
 
 from colorama import Style
 from math import sqrt, log
 
 from .exceptions import (
-    UnitError,
+    InitError,
     QuantityError,
     ConversionError,
     UnpackError,
     PackError,
     UncertaintyComparisonError,
 )
 from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
@@ -31,23 +31,23 @@
         - value: Can be anything that can be somewhat treated as a number.
         - unit: A properly formatted string including all the units with their exponents. e.g. "m s-1".
         - uncertainty: Value's uncertainty.
         """
 
         try:
             assert isinstance(unit, str)
-            assert uAll(uncertainty >= 0) if uAny(uncertainty) else True
+            assert uAll(uncertainty >= 0)
             assert (
                 (checkIter(value) == checkIter(uncertainty))
                 if uAny(uncertainty)
                 else True
             )
 
         except AssertionError:
-            raise UnitError(value, unit, uncertainty)  # Needs a better exception.
+            raise InitError(value, unit, uncertainty)
 
         self.value: any = value
         self.uncertainty = uncertainty
 
         table: dict = getBase()
         table.update(getDerived())
 
@@ -72,66 +72,63 @@
 
         'print = True' makes the output fancier.
         """
 
         if not len(self.units):
             return ""
 
-        # Fancy version.
-        if print:
-            # {"m": 1, "s": -1} -> "[m / s]".
+        uts: dict = self.units.copy()
+        # ut: short for unit.
 
-            uts = self.units.copy()
-            # ut: short for unit.
+        if not print:
+            # Plain version.
+            # {"m": 1, "s": -1} -> "m s-1".
+            return ufd(self.units)
 
-            # Numerator with exponent
-            numeratorWE = [
-                "{}({})".format(ut, uts[ut])
-                for ut in uts
-                if uts[ut] > 0 and uts[ut] != 1
-            ]
+        # Fancy version.
+        # {"m": 1, "s": -1} -> "[m / s]".
 
-            # Denominator with exponent
-            denominatorWE = [
-                "{}({})".format(ut, -uts[ut])
-                for ut in uts
-                if uts[ut] < 0 and uts[ut] != 1
-            ]
+        # Numerator with exponent
+        numeratorWE = [
+            "{}({})".format(ut, uts[ut]) for ut in uts if uts[ut] > 0 and uts[ut] != 1
+        ]
 
-            # Numerator without exponent
-            numeratorWOE = [ut for ut in uts if uts[ut] > 0 and uts[ut] == 1]
+        # Denominator with exponent
+        denominatorWE = [
+            "{}({})".format(ut, -uts[ut]) for ut in uts if uts[ut] < 0 and uts[ut] != 1
+        ]
 
-            # Denominator without exponent
-            denominatorWOE = [ut for ut in uts if uts[ut] < 0 and uts[ut] == 1]
+        # Numerator without exponent
+        numeratorWOE = [ut for ut in uts if uts[ut] > 0 and uts[ut] == 1]
 
-            numerator = " ".join(sorted(numeratorWE + numeratorWOE))
-            denominator = " ".join(sorted(denominatorWE + denominatorWOE))
+        # Denominator without exponent
+        denominatorWOE = [ut for ut in uts if uts[ut] < 0 and uts[ut] == 1]
 
-            if not numerator and denominator:
-                numerator = "1"
+        numerator = " ".join(sorted(numeratorWE + numeratorWOE))
+        denominator = " ".join(sorted(denominatorWE + denominatorWOE))
 
-            fraction = numerator + " / " + denominator if denominator else numerator
+        if not numerator and denominator:
+            numerator = "1"
 
-            if style.quantityHighlighting:
-                return Style.BRIGHT + fraction + Style.RESET_ALL if numerator else ""
+        fraction = numerator + " / " + denominator if denominator else numerator
 
-            return "[" + fraction + "]" if numerator else ""
+        if style.quantityHighlighting:
+            return Style.BRIGHT + fraction + Style.RESET_ALL if numerator else ""
 
-        # {"m": 1, "s": -1} -> "m s-1".
-        return ufd(self.units)
+        return "[" + fraction + "]" if numerator else ""
 
     def dimension(self) -> str:
         """
         Returns a readable version of the quantity's dimension.
         """
 
         if not len(self.dimensions):
             return ""
 
-        uts = self.units.copy()
+        uts: dict = self.units.copy()
         # ut: short for unit.
 
         # Numerator with exponent
         numeratorWE = [
             "{}({})".format(getFamily(ut), uts[ut])
             for ut in uts
             if uts[ut] > 0 and uts[ut] != 1
@@ -159,30 +156,26 @@
         fraction = numerator + " / " + denominator if denominator else numerator
 
         return "[" + fraction + "]" if numerator else ""
 
     # STRINGS.
 
     def __str__(self) -> str:
-        from .globals import style
-
         pm = style.quantityPlusMinus
         unit = self.unit(print=True)
         uncert = self.uncertainty
 
         return "{}{}{}".format(
             self.value, "{}{} ".format(pm, uncert) if uAny(uncert) else " ", unit
         )
 
     def __repr__(self) -> str:
         return str(self)
 
     def __format__(self, string) -> str:  # Unit highlighting works for print only.
-        from .globals import style
-
         pm = style.quantityPlusMinus
         unit = self.unit(print=True)
         uncert = self.uncertainty
 
         # This works best with print.
         return (
             self.value.__format__(string)
@@ -669,22 +662,19 @@
 
     'targets = ""' completely unpacks the quantity.
     """
 
     unpackTable: dict = getDerivedUnpacking()
     derivedTable: dict = getDerived()
 
-    if targets == "":  # Unpacks all derived units.
+    if not targets:  # Unpacks all derived units.
         targets = " ".join(
             [unit for unit in qnt.units if getFamily(unit) in derivedTable]
         )
 
-        if targets == "":
-            return qnt
-
     for target in dfu(targets):
         # Checks target.
         if getFamily(target) not in [getFamily(unit) for unit in qnt.units]:
             raise UnpackError(qnt, target)
 
         cTarget = getRep(getFamily(target))  # Conversion target.
         cTargetPower = [  # Conversion target's power.
@@ -745,36 +735,30 @@
 
     # Unpack only relevant units.
     if ignore:
         for ignored in dfu(ignore):
             if getFamily(ignored) not in [getFamily(unit) for unit in qnt.units]:
                 raise PackError(qnt, targets, ignore)
 
-    qnt = (
-        quantity(
-            qnt.value,
-            ufd({unit: qnt.units[unit] for unit in qnt.units if unit in dfu(ignore)}),
-        )
-        * unpack(
-            quantity(
-                1,
-                ufd(
-                    {
-                        unit: qnt.units[unit]
-                        for unit in qnt.units
-                        if unit not in dfu(ignore)
-                    }
-                ),
-            )
-        )
-        if ignore
-        else unpack(qnt)
-    )
+        val = qnt.value
+        uts: dict = qnt.units.copy()
+        # ut: short for unit.
+
+        # Does not completely unpack the quantity qnt but unpacks the non-ignored units
+        # and then merges them with the ignored ones.
+        ignored = quantity(val, ufd({ut: uts[ut] for ut in uts if ut in dfu(ignore)}))
+        packed = quantity(1, ufd({ut: uts[ut] for ut in uts if ut not in dfu(ignore)}))
+
+        qnt = ignored * unpack(packed)
+
+    else:
+        qnt = unpack(qnt)
 
     for target in dfu(targets):
+        # Ignores non-packable units.
         if target not in packTable:
             continue
 
         targetUnits = dfu(packTable[target])
 
         # Packing powers.
         powers = {
@@ -785,16 +769,15 @@
         }
 
         if not len(powers):
             raise PackError(qnt, targets)
 
         # Full packing is a stricter form of packing which
         # requires that "no other units are produced from the packing process".
-        if full:
-            # Packability check.
+        if full:  # Full-packability check.
             for targetUnit in targetUnits:
                 if targetUnit not in qnt.units:
                     raise PackError(qnt, targets, full=True)
 
                 if qnt.units[targetUnit] % targetUnits[targetUnit]:
                     raise PackError(qnt, targets, full=True)
```

### Comparing `misura-1.5.4/src/misura/tables.py` & `misura-1.5.5/src/misura/tables.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/src/misura/utilities.py` & `misura-1.5.5/src/misura/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
     """
     Returns the dictionary of units from a properly formatted string.
     """
 
     units = dict()
 
+    if not unit:
+        return units
+
     for sym in unit.split(" "):
         candidate = findall(r"-?\d+\.?\d*", sym)
 
         if len(candidate) == 1:
             power = candidate[0]
 
         elif len(candidate) > 1:
```

### Comparing `misura-1.5.4/LICENSE` & `misura-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/README.md` & `misura-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.4/pyproject.toml` & `misura-1.5.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `misura-1.5.4/PKG-INFO` & `misura-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

