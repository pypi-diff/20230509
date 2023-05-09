# Comparing `tmp/misura-1.5.3.tar.gz` & `tmp/misura-1.5.4.tar.gz`

## Comparing `misura-1.5.3.tar` & `misura-1.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.3/.gitattributes
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 misura-1.5.3/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 misura-1.5.3/docs/docs.md
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 misura-1.5.3/src/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/__main__.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/exceptions.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/globals.py
--rw-r--r--   0        0        0    23447 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/quantities.py
--rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/tables.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.3/src/misura/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.3/LICENSE
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 misura-1.5.3/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 misura-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.4/.gitattributes
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 misura-1.5.4/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 misura-1.5.4/docs/docs.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 misura-1.5.4/src/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/__main__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/exceptions.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/globals.py
+-rw-r--r--   0        0        0    24681 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/quantities.py
+-rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/tables.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.4/src/misura/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.4/LICENSE
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 misura-1.5.4/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 misura-1.5.4/PKG-INFO
```

### Comparing `misura-1.5.3/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.5.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/.github/workflows/python-publish.yml` & `misura-1.5.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/docs/docs.md` & `misura-1.5.4/docs/docs.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - [Units of measure](#units-of-measure)
 	- [Defaults](#defaults)
 	- [User defined units of measure](#user-defined-units-of-measure)
 - [Conversions, unpacking and packing](#conversions-unpacking-and-packing)
 	- [Conversion](#conversion)
 	- [Unpacking](#unpacking)
 	- [Packing](#packing)
+	- [Shortcuts](#shortcuts)
 - [Global options](#global-options)
 - [Exceptions](#exceptions)
 - [Examples](#examples)
 
 ## Introduction
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
@@ -198,38 +199,56 @@
 The function `convert` takes a `quantity` object, converted, a string, `targets`, and two flags: `partial` and `un_pack`.
 
 - `qnt: quantity` is the quantity that needs to be converted.
 - `targets: str` is the string of target units, the units that need to be matched after conversion.
 - `partial: bool` whether or not the conversion should be partial, e.g. `"m s-1" -> "km s-1"`.
 - `un_pack: bool` whether or not to (un)pack derived units during conversion.
 
-### unpacking
+### Unpacking
 
 ```python
 misura.unpack(qnt: quantity, targets: str = "") -> quantity
 ```
 
 The function `unpack` takes a `quantity` object, qnt and an optional string, `targets`.
 
 - `qnt: quantity` is the quantity that needs to be converted.
 - `targets: str = ""` is the string of target units, the derived units that need to be unpacked. If empty, it unpacks every derived unit.
 
-### packing
+### Packing
 
 ```python
 misura.pack(qnt: quantity, targets: str, full: bool = False) -> quantity
 ```
 
 The function `pack` takes a `quantity` object, qnt, two strings, `targets` and `ignore`, and a flag, `full`.
 
 - `qnt: quantity` is the quantity that needs to be converted.
 - `targets: str` is the string of target units, the derived units that need to be matched.
 - `ignore: str = ""` Due to the fact that `pack` works by first unpacking the units, some units can be manually ignored to enhance the final result.
 - `full: bool = False` whether or not to fully pack a unit.
 
+### Shortcuts
+
+The following `quantities.quantity` methods should serve as shortcuts to the `convert`, `unpack` and `pack` functions:
+
+``` python
+class quantity:
+	...
+
+    def cto(self, targets: str, partial: bool = False, un_pack: bool = True) -> quantity:  # Convert to.
+        return convert(self, targets, partial, un_pack)
+
+    def uto(self, targets: str = "") -> quantity:  # Unpack to.
+        return unpack(self, targets)
+
+    def pto(self, targets: str, ignore: str = "", full: bool = False) -> quantity:  # Pack to.
+        return pack(self, targets, ignore, full)
+```
+
 Take a look at these [examples](#conversions-unpacking-and-packing-1).
 
 ## Global options
 
 [Go back to ToC](#table-of-contents)
 
 **misura** implements the following global options:
```

### Comparing `misura-1.5.3/src/test.py` & `misura-1.5.4/src/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
 num0 = quantity(5, "m2")
 num1 = quantity(67, "km")
 num2 = quantity(12, "A s")
 num3 = quantity(1, "C mW")
 num4 = quantity(900, "J")
 num5 = quantity(15, "H TT")
-num6 = quantity(12, "m2 s-2")
+num6 = quantity(12, "km2 s-2")
 num7 = quantity(3, "kg km2")
 num8 = quantity(13, "J")
 num9 = quantity(0.9, "mN km")
 num10 = quantity(3, "N m T")
 num11 = quantity(12, "kbnn")
 num12 = quantity(2, "kg", 0.5)
 num13 = quantity(0.7, "m3", 0.15)
 num14 = quantity(3, "", 1)
 
 # Dimensions.
-print(num0.dimension())
+print(num10.dimension())
 
 # Math.
 print(num0**0.5)
 print(7 - num14)
 print(2**num14)
 
 # Logical.
@@ -34,15 +34,15 @@
 print(num0**0.5 < num1)
 print(num0 < 0.02 * num1**2)
 print(num1 == num2)
 print(num1 != num2)
 
 # Conversions.
 print(num0**0.5 + num1)
-print(convert(num0, "dm2"))
+print(num0.cto("dm2"), num0)  # num0 does not change.
 print(convert(num1, "m"))
 print(convert(num2, "mA", partial=True))
 
 # Unpacking.
 print(unpack(num3))
 print(unpack(num4**3))
 print(unpack(num5, "T"))
```

### Comparing `misura-1.5.3/src/misura/__main__.py` & `misura-1.5.4/src/misura/__main__.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/src/misura/exceptions.py` & `misura-1.5.4/src/misura/exceptions.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/src/misura/quantities.py` & `misura-1.5.4/src/misura/quantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     QuantityError,
     ConversionError,
     UnpackError,
     PackError,
     UncertaintyComparisonError,
 )
 from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
-from .utilities import dictFromUnit, unitFromDict, checkIter, uAll, uAny
+from .utilities import checkIter, uAll, uAny
+from .utilities import unitFromDict as ufd
+from .utilities import dictFromUnit as dfu
 from .globals import style, logic
 
 
 class quantity:
     """
     misura's quantity class.
     """
@@ -46,15 +48,15 @@
         self.value: any = value
         self.uncertainty = uncertainty
 
         table: dict = getBase()
         table.update(getDerived())
 
         # From unit: str to self.units: dict.
-        self.units: dict = dictFromUnit(unit)
+        self.units: dict = dfu(unit)
 
         # Checks whether the unit can be converted with the available units.
         self.convertible: bool = all(
             [any([unit in table[family] for family in table]) for unit in self.units]
         )
 
         # Define quantity's dimentsionality based on self.units.
@@ -111,15 +113,15 @@
 
             if style.quantityHighlighting:
                 return Style.BRIGHT + fraction + Style.RESET_ALL if numerator else ""
 
             return "[" + fraction + "]" if numerator else ""
 
         # {"m": 1, "s": -1} -> "m s-1".
-        return unitFromDict(self.units)
+        return ufd(self.units)
 
     def dimension(self) -> str:
         """
         Returns a readable version of the quantity's dimension.
         """
 
         if not len(self.dimensions):
@@ -144,16 +146,16 @@
 
         # Numerator without exponent
         numeratorWOE = [getFamily(ut) for ut in uts if uts[ut] > 0 and uts[ut] == 1]
 
         # Denominator without exponent
         denominatorWOE = [getFamily(ut) for ut in uts if uts[ut] < 0 and uts[ut] == 1]
 
-        numerator = " ".join(sorted(numeratorWE + numeratorWOE))
-        denominator = " ".join(sorted(denominatorWE + denominatorWOE))
+        numerator = " * ".join(sorted(numeratorWE + numeratorWOE))
+        denominator = " * ".join(sorted(denominatorWE + denominatorWOE))
 
         if not numerator and denominator:
             numerator = "1"
 
         fraction = numerator + " / " + denominator if denominator else numerator
 
         return "[" + fraction + "]" if numerator else ""
@@ -334,15 +336,15 @@
 
         for unit in other.units:
             if unit not in newUnits:
                 newUnits[unit] = other.units[unit]
 
         return quantity(
             self.value * other.value,
-            unitFromDict(newUnits),
+            ufd(newUnits),
             sqrt(
                 (other.value * self.uncertainty) ** 2
                 + (self.value * other.uncertainty) ** 2
             ),
         )
 
     def __rmul__(self, other: any) -> any:
@@ -366,15 +368,15 @@
 
         for unit in other.units:
             if unit not in newUnits:
                 newUnits[unit] = -other.units[unit]
 
         return quantity(
             self.value / other.value,
-            unitFromDict(newUnits),
+            ufd(newUnits),
             sqrt(
                 (self.uncertainty / other.value) ** 2
                 + (self.value * other.uncertainty / (other.value**2)) ** 2
             ),
         )
 
     def __floordiv__(self, other: any) -> quantity:
@@ -399,15 +401,15 @@
         newUnits = self.units.copy()
 
         for unit in newUnits:
             newUnits[unit] *= other
 
         return quantity(
             self.value**other,
-            unitFromDict(newUnits),
+            ufd(newUnits),
             abs(other) * (self.value ** (other - 1)) * self.uncertainty,
         )
 
     def __rpow__(self, other: any) -> quantity:
         if isinstance(other, quantity):
             raise QuantityError(other, self, "**")
 
@@ -524,14 +526,29 @@
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "!=")
 
         return self.value != other.value or self.unit() != other.unit()
 
+    # SHORTCUTS
+
+    def cto(
+        self, targets: str, partial: bool = False, un_pack: bool = True
+    ) -> quantity:  # Convert to.
+        return convert(self, targets, partial, un_pack)
+
+    def uto(self, targets: str = "") -> quantity:  # Unpack to.
+        return unpack(self, targets)
+
+    def pto(
+        self, targets: str, ignore: str = "", full: bool = False
+    ) -> quantity:  # Pack to.
+        return pack(self, targets, ignore, full)
+
 
 # CONVERSION, UNPACKING AND PACKING
 
 
 # Conversion function.
 def convert(
     qnt: quantity, targets: str, partial: bool = False, un_pack: bool = True
@@ -547,32 +564,59 @@
         raise ConversionError(qnt, targets)
 
     # Check dimension.
     if not partial:
         if unpack(qnt).dimension() != unpack(quantity(1, targets)).dimension():
             raise ConversionError(qnt, targets)
 
-    # Automatic (un)packing, version 1.
+    # Automatic (un)packing, version 2.
     if un_pack and not partial:
-        try:
-            # Tries to pack qnt.
-            return convert(pack(qnt, targets), targets, un_pack=False)
+        # Tries to pack qnt.
+        target = quantity(1, targets)
+        packUnits = {ut: target.units[ut] for ut in target.units if ut not in qnt.units}
+        ignoreUnits = {ut: qnt.units[ut] for ut in qnt.units if ut not in target.units}
+
+        for tr in range(3):
+            try:
+                if tr == 0:
+                    # First try: uses ignore and full packing.
+                    return convert(
+                        pack(qnt, ufd(packUnits), ignore=ufd(ignoreUnits), full=True),
+                        targets,
+                        un_pack=False,
+                    )
+
+                if tr == 1:
+                    # Second try: uses ignore.
+                    return convert(
+                        pack(qnt, ufd(packUnits), ignore=ufd(ignoreUnits)),
+                        targets,
+                        un_pack=False,
+                    )
+
+                elif tr == 2:
+                    # Third try: does not use ignore.
+                    return convert(
+                        pack(qnt, ufd(packUnits)),
+                        targets,
+                        un_pack=False,
+                    )
 
-        except (PackError, ConversionError):
-            pass
+            except (PackError, ConversionError):
+                pass
 
         # Completely unpacks units.
         return convert(
             unpack(qnt),
-            unpack(quantity(1, targets)).unit(),
+            unpack(target).unit(),
             un_pack=False,
         )
 
     factor: float = 1.0
-    tUnits: dict = dictFromUnit(targets)  # Target units.
+    tUnits: dict = dfu(targets)  # Target units.
 
     pTargets: dict = dict()  # Partial targets.
 
     table: dict = getBase()
     table.update(getDerived())
 
     for unit in qnt.units.keys():
@@ -610,17 +654,15 @@
         # Partial conversion.
         elif partial:
             pTargets[unit] = qnt.units[unit]
 
     return (
         quantity(qnt.value * factor, targets, qnt.uncertainty * factor)
         if not partial
-        else quantity(
-            qnt.value * factor, unitFromDict(pTargets), qnt.uncertainty * factor
-        )
+        else quantity(qnt.value * factor, ufd(pTargets), qnt.uncertainty * factor)
     )
 
 
 # Unpacking function.
 def unpack(qnt: quantity, targets: str = "") -> quantity:
     """
     Unpacking function; unpacks the passed targets units form the quantity object.
@@ -635,15 +677,15 @@
         targets = " ".join(
             [unit for unit in qnt.units if getFamily(unit) in derivedTable]
         )
 
         if targets == "":
             return qnt
 
-    for target in dictFromUnit(targets):
+    for target in dfu(targets):
         # Checks target.
         if getFamily(target) not in [getFamily(unit) for unit in qnt.units]:
             raise UnpackError(qnt, target)
 
         cTarget = getRep(getFamily(target))  # Conversion target.
         cTargetPower = [  # Conversion target's power.
             qnt.units[unit]
@@ -664,17 +706,17 @@
         )
 
         # Units that werent't involved in the previous conversion.
         newUnits = {key: qnt.units[key] for key in qnt.units if key != cTarget}
 
         # Uncertainty should not vary on packing.
         uncertainty = qnt.uncertainty
-        qnt = (
-            quantity(qnt.value, unitFromDict(newUnits)) if len(newUnits) else qnt.value
-        ) * (quantity(1, unpackTable[cTarget]) ** qnt.units[cTarget])
+        qnt = (quantity(qnt.value, ufd(newUnits)) if len(newUnits) else qnt.value) * (
+            quantity(1, unpackTable[cTarget]) ** qnt.units[cTarget]
+        )
         qnt.uncertainty = uncertainty
 
     return qnt
 
 
 # Packing function.
 def pack(qnt: quantity, targets: str, ignore: str = "", full: bool = False) -> quantity:
@@ -699,50 +741,44 @@
             for unit in unitsTable[getFamily(unit)]
             if unitsTable[getFamily(unit)][unit] == 1
         ].pop()
         qnt = convert(qnt, cTarget + str(qnt.units[unit]), partial=True, un_pack=False)
 
     # Unpack only relevant units.
     if ignore:
-        for ignored in dictFromUnit(ignore):
+        for ignored in dfu(ignore):
             if getFamily(ignored) not in [getFamily(unit) for unit in qnt.units]:
                 raise PackError(qnt, targets, ignore)
 
     qnt = (
         quantity(
             qnt.value,
-            unitFromDict(
-                {
-                    unit: qnt.units[unit]
-                    for unit in qnt.units
-                    if unit in dictFromUnit(ignore)
-                }
-            ),
+            ufd({unit: qnt.units[unit] for unit in qnt.units if unit in dfu(ignore)}),
         )
         * unpack(
             quantity(
                 1,
-                unitFromDict(
+                ufd(
                     {
                         unit: qnt.units[unit]
                         for unit in qnt.units
-                        if unit not in dictFromUnit(ignore)
+                        if unit not in dfu(ignore)
                     }
                 ),
             )
         )
         if ignore
         else unpack(qnt)
     )
 
-    for target in dictFromUnit(targets):
+    for target in dfu(targets):
         if target not in packTable:
             continue
 
-        targetUnits = dictFromUnit(packTable[target])
+        targetUnits = dfu(packTable[target])
 
         # Packing powers.
         powers = {
             # Updated from // to / to account for fractional powers.
             qnt.units[targetUnit] / targetUnits[targetUnit]
             for targetUnit in targetUnits
             if targetUnit in qnt.units
@@ -763,13 +799,11 @@
                     raise PackError(qnt, targets, full=True)
 
             if min(powers) < max(powers) or max(powers) < 0:
                 raise PackError(qnt, targets, full=True)
 
         # Uncertainty should not vary on packing.
         uncertainty = qnt.uncertainty
-        qnt *= (quantity(1, target) / quantity(1, unitFromDict(targetUnits))) ** max(
-            powers
-        )
+        qnt *= (quantity(1, target) / quantity(1, ufd(targetUnits))) ** max(powers)
         qnt.uncertainty = uncertainty
 
     return qnt
```

### Comparing `misura-1.5.3/src/misura/tables.py` & `misura-1.5.4/src/misura/tables.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/src/misura/utilities.py` & `misura-1.5.4/src/misura/utilities.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/LICENSE` & `misura-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/README.md` & `misura-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.3/pyproject.toml` & `misura-1.5.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.5.3"
+version = "1.5.4"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `misura-1.5.3/PKG-INFO` & `misura-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

