# Comparing `tmp/module_qc_analysis_tools-1.3.1rc6.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc7.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc6.tar` & `module_qc_analysis_tools-1.3.1rc7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    26971 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    35037 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/LICENSE
--rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/README.md
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/pyproject.toml
--rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    26971 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/LICENSE
+-rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/README.md
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/pyproject.toml
+-rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc7/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc6/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/tbump.toml` & `module_qc_analysis_tools-1.3.1rc7/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3622 0a0a  t = "1.3.1rc6"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3722 0a0a  t = "1.3.1rc7"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3620 e286 9220 7b6e 6577  .3.1rc6 ... {new
+00000150: 2e33 2e31 7263 3720 e286 9220 7b6e 6577  .3.1rc7 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/LP_MODE.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/TUNING.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/classification.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc7/src/module_qc_analysis_tools/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,20 @@
                 len_x = len(self.qcdataframe[required_keyword])
                 self.var_x = required_keyword
                 first_keyword = False
             if self.qcdataframe.get_x(required_keyword) is True:
                 len_x = len(self.qcdataframe[required_keyword])
                 self.var_x = required_keyword
 
+        if len_x == 0:
+            log.error(
+                bcolors.ERROR + "The input is empty! Please check." + bcolors.ENDC
+            )
+            raise LengthMismatchError()
+
         for required_keyword in self.required_keywords:
             if len_x != len(self.qcdataframe[required_keyword]):
                 log.error(
                     bcolors.ERROR
                     + f"The length of {required_keyword} is not equal to {self.var_x}!"
                     + bcolors.ENDC
                 )
```

### Comparing `module_qc_analysis_tools-1.3.1rc6/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/.gitignore` & `module_qc_analysis_tools-1.3.1rc7/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/LICENSE` & `module_qc_analysis_tools-1.3.1rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/README.md` & `module_qc_analysis_tools-1.3.1rc7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc6
+# module-qc-analysis-tools v1.3.1rc7
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -69,15 +69,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc6
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc7
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-1.3.1rc6/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc6/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc6
+Version: 1.3.1rc7
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc6
+# module-qc-analysis-tools v1.3.1rc7
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -109,15 +109,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc6
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc7
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

