# Comparing `tmp/simfire-1.4.33.tar.gz` & `tmp/simfire-1.4.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfire-1.4.33.tar", max compression
+gzip compressed data, was "simfire-1.4.34.tar", max compression
```

## Comparing `simfire-1.4.33.tar` & `simfire-1.4.34.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    10789 2023-04-28 04:45:12.821836 simfire-1.4.33/LICENSE
--rw-r--r--   0        0        0     2688 2023-04-28 04:45:12.821836 simfire-1.4.33/README.md
--rw-r--r--   0        0        0     1852 2023-04-28 04:45:13.021838 simfire-1.4.33/pyproject.toml
--rw-r--r--   0        0        0     1111 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/__init__.py
--rw-r--r--   0        0        0    10646 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/enums.py
--rw-r--r--   0        0        0       37 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/__init__.py
--rw-r--r--   0        0        0      874 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/_tests/__init__.py
--rw-r--r--   0        0        0    15523 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/_tests/test_game.py
--rw-r--r--   0        0        0     9928 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/_tests/test_sprites.py
--rw-r--r--   0        0        0    14937 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/game.py
--rw-r--r--   0        0        0     1318 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/image.py
--rw-r--r--   0        0        0      379 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/_tests/__init__.py
--rw-r--r--   0        0        0    18385 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/_tests/test_fire.py
--rw-r--r--   0        0        0     8301 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/_tests/test_mitigation.py
--rw-r--r--   0        0        0    29762 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/fire.py
--rw-r--r--   0        0        0     7321 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/managers/mitigation.py
--rw-r--r--   0        0        0    15972 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/game/sprites.py
--rw-r--r--   0        0        0       49 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/_tests/__init__.py
--rw-r--r--   0        0        0    14392 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/_tests/test_simulation.py
--rw-r--r--   0        0        0    37791 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/sim/simulation.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/__init__.py
--rw-r--r--   0        0        0     2378 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_config.py
--rw-r--r--   0        0        0     1925 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config.yml
--rw-r--r--   0        0        0       47 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_bad.yml
--rw-r--r--   0        0        0     1874 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
--rw-r--r--   0        0        0     1876 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_gaussian.yml
--rw-r--r--   0        0        0     1851 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
--rw-r--r--   0        0        0     4693 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_graph.py
--rw-r--r--   0        0        0    17172 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_layers.py
--rw-r--r--   0        0        0      622 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_log.py
--rw-r--r--   0        0        0     2537 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_terrain.py
--rw-r--r--   0        0        0     1472 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/_tests/test_units.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/assets/__init__.py
--rw-r--r--   0        0        0     1854 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/assets/fireline_logo.png
--rw-r--r--   0        0        0    38450 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/config.py
--rw-r--r--   0        0        0      499 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/decorators.py
--rw-r--r--   0        0        0     4153 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/generate_cfd_wind_layer.py
--rw-r--r--   0        0        0    10189 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/graph.py
--rw-r--r--   0        0        0    51105 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/layers.py
--rw-r--r--   0        0        0     2030 2023-04-28 04:45:13.021838 simfire-1.4.33/simfire/utils/log.py
--rw-r--r--   0        0        0   143776 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
--rw-r--r--   0        0        0   143776 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
--rw-r--r--   0        0        0     2248 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/terrain.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/textures/__init__.py
--rw-r--r--   0        0        0   204702 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/textures/terrain.jpg
--rw-r--r--   0        0        0     2555 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/utils/units.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_cfd_wind.py
--rw-r--r--   0        0        0     2423 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_elevation_functions.py
--rw-r--r--   0        0        0     2821 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_rothermel.py
--rw-r--r--   0        0        0     1466 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/_tests/test_wind.py
--rw-r--r--   0        0        0     3703 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/elevation_functions.py
--rw-r--r--   0        0        0     1054 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/fuel_array_functions.py
--rw-r--r--   0        0        0     2306 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/parameters.py
--rw-r--r--   0        0        0     2083 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/presets.py
--rw-r--r--   0        0        0     4306 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/rothermel.py
--rw-r--r--   0        0        0        0 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/__init__.py
--rw-r--r--   0        0        0     8781 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/cfd_wind.py
--rw-r--r--   0        0        0     3132 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/perlin_wind.py
--rw-r--r--   0        0        0     6578 2023-04-28 04:45:13.025838 simfire-1.4.33/simfire/world/wind_mechanics/wind_controller.py
--rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 simfire-1.4.33/PKG-INFO
+-rw-r--r--   0        0        0    10789 2023-05-09 00:16:40.286229 simfire-1.4.34/LICENSE
+-rw-r--r--   0        0        0     2688 2023-05-09 00:16:40.286229 simfire-1.4.34/README.md
+-rw-r--r--   0        0        0     1852 2023-05-09 00:16:40.466230 simfire-1.4.34/pyproject.toml
+-rw-r--r--   0        0        0     1111 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/__init__.py
+-rw-r--r--   0        0        0    10729 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/enums.py
+-rw-r--r--   0        0        0       37 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/_tests/__init__.py
+-rw-r--r--   0        0        0    15523 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/_tests/test_game.py
+-rw-r--r--   0        0        0     9928 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/_tests/test_sprites.py
+-rw-r--r--   0        0        0    14937 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/game.py
+-rw-r--r--   0        0        0     1318 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/image.py
+-rw-r--r--   0        0        0      379 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/managers/_tests/__init__.py
+-rw-r--r--   0        0        0    18385 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/managers/_tests/test_fire.py
+-rw-r--r--   0        0        0     8301 2023-05-09 00:16:40.466230 simfire-1.4.34/simfire/game/managers/_tests/test_mitigation.py
+-rw-r--r--   0        0        0    29762 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/game/managers/fire.py
+-rw-r--r--   0        0        0     7321 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/game/managers/mitigation.py
+-rw-r--r--   0        0        0    15972 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/game/sprites.py
+-rw-r--r--   0        0        0       49 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/sim/_tests/__init__.py
+-rw-r--r--   0        0        0    14392 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/sim/_tests/test_simulation.py
+-rw-r--r--   0        0        0    37815 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/sim/simulation.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/__init__.py
+-rw-r--r--   0        0        0     2771 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_config.py
+-rw-r--r--   0        0        0     1925 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_configs/test_config.yml
+-rw-r--r--   0        0        0       47 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_bad.yml
+-rw-r--r--   0        0        0     1874 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
+-rw-r--r--   0        0        0     1876 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_gaussian.yml
+-rw-r--r--   0        0        0     1851 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
+-rw-r--r--   0        0        0     4693 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_graph.py
+-rw-r--r--   0        0        0    17172 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_layers.py
+-rw-r--r--   0        0        0      622 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_log.py
+-rw-r--r--   0        0        0     4495 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_terrain.py
+-rw-r--r--   0        0        0     1472 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/_tests/test_units.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/assets/__init__.py
+-rw-r--r--   0        0        0     1854 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/assets/fireline_logo.png
+-rw-r--r--   0        0        0    38910 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/config.py
+-rw-r--r--   0        0        0      499 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/decorators.py
+-rw-r--r--   0        0        0     4153 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/generate_cfd_wind_layer.py
+-rw-r--r--   0        0        0    10189 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/graph.py
+-rw-r--r--   0        0        0    51105 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/layers.py
+-rw-r--r--   0        0        0     2030 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/log.py
+-rw-r--r--   0        0        0   143776 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
+-rw-r--r--   0        0        0   143776 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
+-rw-r--r--   0        0        0     3647 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/terrain.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/textures/__init__.py
+-rw-r--r--   0        0        0   204702 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/textures/terrain.jpg
+-rw-r--r--   0        0        0     2555 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/utils/units.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/_tests/__init__.py
+-rw-r--r--   0        0        0     2184 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/_tests/test_cfd_wind.py
+-rw-r--r--   0        0        0     2423 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/_tests/test_elevation_functions.py
+-rw-r--r--   0        0        0     2821 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/_tests/test_rothermel.py
+-rw-r--r--   0        0        0     1466 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/_tests/test_wind.py
+-rw-r--r--   0        0        0     3703 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/elevation_functions.py
+-rw-r--r--   0        0        0     1054 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/fuel_array_functions.py
+-rw-r--r--   0        0        0     2306 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/parameters.py
+-rw-r--r--   0        0        0     2083 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/presets.py
+-rw-r--r--   0        0        0     4306 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/rothermel.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/wind_mechanics/__init__.py
+-rw-r--r--   0        0        0     8781 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/wind_mechanics/cfd_wind.py
+-rw-r--r--   0        0        0     3132 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/wind_mechanics/perlin_wind.py
+-rw-r--r--   0        0        0     6578 2023-05-09 00:16:40.470231 simfire-1.4.34/simfire/world/wind_mechanics/wind_controller.py
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 simfire-1.4.34/PKG-INFO
```

### Comparing `simfire-1.4.33/LICENSE` & `simfire-1.4.34/LICENSE`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/README.md` & `simfire-1.4.34/README.md`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/pyproject.toml` & `simfire-1.4.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simfire"
-version = "1.4.33"
+version = "1.4.34"
 description = "Fire simulator built in Python"
 authors = ["Tim Welsh <twelsh@mitre.org>", "Marissa Dotter <mdotter@mitre.org>",
            "Michael Doyle <mdoyle@mitre.org>", "Dhanuj Gandikota <dgandikota@mitre.org>",
            "Chris Kempis <ckempis@mitre.org>", "Lauren Schambach <lschambach@mitre.org>",
            "Alex Tapley <atapley@mitre.org>", "Michael Threet <mthreet@mitre.org>"]
 readme = "README.md"
 include = ["simfire/utils/textures/terrain.jpg", "simfire/utils/assets/fireline_logo.png"]
```

### Comparing `simfire-1.4.33/simfire/__init__.py` & `simfire-1.4.34/simfire/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/enums.py` & `simfire-1.4.34/simfire/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,19 +123,22 @@
         W_0_MIN: Oven-dry Fuel Load (lb/ft^2) minimum.
         W_0_MAX: Oven-dry Fuel Load (lb/ft^2) maximum.
         DELTA: Fuel bed depth (ft) min and max.
         M_X: Dead fuel moisture of extinction min and max.
         SIGMA: Surface-area-to-volume ratio (ft^2/ft^3) min and max.
     """
 
-    W_0_MIN: float = 0.2
-    W_0_MAX: float = 0.6
-    DELTA: float = 6.000
-    M_X: float = 0.2000
-    SIGMA: int = 1739
+    W_0_MIN: float = 0.0
+    W_0_MAX: float = 1.0
+    DELTA_MIN: float = 0.2
+    DELTA_MAX: float = 6.0
+    M_X_MIN: float = 0.15
+    M_X_MAX: float = 1.0
+    SIGMA_MIN: int = 1
+    SIGMA_MAX: int = 3500
 
 
 @dataclass
 class ElevationConstants:
     """
     Constants to be used in the file and can be imported for reference.
```

### Comparing `simfire-1.4.33/simfire/game/_tests/__init__.py` & `simfire-1.4.34/simfire/game/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/_tests/test_game.py` & `simfire-1.4.34/simfire/game/_tests/test_game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/_tests/test_sprites.py` & `simfire-1.4.34/simfire/game/_tests/test_sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/game.py` & `simfire-1.4.34/simfire/game/game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/image.py` & `simfire-1.4.34/simfire/game/image.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/managers/_tests/test_fire.py` & `simfire-1.4.34/simfire/game/managers/_tests/test_fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/managers/_tests/test_mitigation.py` & `simfire-1.4.34/simfire/game/managers/_tests/test_mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/managers/fire.py` & `simfire-1.4.34/simfire/game/managers/fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/managers/mitigation.py` & `simfire-1.4.34/simfire/game/managers/mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/game/sprites.py` & `simfire-1.4.34/simfire/game/sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/sim/_tests/test_simulation.py` & `simfire-1.4.34/simfire/sim/_tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/sim/simulation.py` & `simfire-1.4.34/simfire/sim/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,17 +298,17 @@
         Returns:
             The dictionary of observation space bounds containing NumPy arrays.
         """
         bounds = {}
         if True:
             fuel_bounds = {
                 "w_0": {"min": FuelConstants.W_0_MIN, "max": FuelConstants.W_0_MAX},
-                "sigma": {"min": FuelConstants.SIGMA, "max": FuelConstants.SIGMA},
-                "delta": {"min": FuelConstants.DELTA, "max": FuelConstants.DELTA},
-                "M_x": {"min": FuelConstants.M_X, "max": FuelConstants.M_X},
+                "sigma": {"min": FuelConstants.SIGMA_MAX, "max": FuelConstants.SIGMA_MAX},
+                "delta": {"min": FuelConstants.DELTA_MAX, "max": FuelConstants.DELTA_MAX},
+                "M_x": {"min": FuelConstants.M_X_MAX, "max": FuelConstants.M_X_MAX},
             }
             bounds.update(fuel_bounds)
         else:
             log.error("Fuel layer type not yet supported")
             raise NotImplementedError
 
         elevation_bounds = {
```

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_config.py` & `simfire-1.4.34/simfire/utils/_tests/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 class ConfigTest(unittest.TestCase):
     def setUp(self) -> None:
         self.yaml = Path("./simfire/utils/_tests/test_configs/test_config.yml")
         self.cfg = Config(self.yaml)
         with open(self.yaml, "r") as f:
             self.true_yaml_data = yaml.safe_load(f)
 
+        self.config_dict = Config(config_dict=self.true_yaml_data)
+
     def test_reset_terrain(self) -> None:
         """
         Test resetting the seed and coordinates for the terrain topography
         and fuel layers.
         """
         # test_config.yml has a seed of 1111
         new_topo_seed = 1234
@@ -42,14 +44,24 @@
         self.assertEqual(
             new_fuel_seed,
             cfg_seed,
             msg=f"The assigned seed of {cfg_seed} does "
             f"not match the test seed of {new_topo_seed}",
         )
 
+    def test_dict_argument(self) -> None:
+        """
+        Test using the dictionary as an argument to the Config class
+        """
+        self.assertDictEqual(
+            self.true_yaml_data,
+            self.config_dict.yaml_data,
+            msg="The dictionary argument does not match the YAML argument",
+        )
+
     def test_reset_wind_function(self) -> None:
         """
         Test resetting the seed for the wind function and returning a different map
         """
         pass
 
     def test_save(self) -> None:
```

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config.yml` & `simfire-1.4.34/simfire/utils/_tests/test_configs/test_config.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_flat_simple.yml` & `simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_flat_simple.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_gaussian.yml` & `simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_gaussian.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml` & `simfire-1.4.34/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_graph.py` & `simfire-1.4.34/simfire/utils/_tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_layers.py` & `simfire-1.4.34/simfire/utils/_tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_log.py` & `simfire-1.4.34/simfire/utils/_tests/test_log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/_tests/test_units.py` & `simfire-1.4.34/simfire/utils/_tests/test_units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/assets/fireline_logo.png` & `simfire-1.4.34/simfire/utils/assets/fireline_logo.png`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/config.py` & `simfire-1.4.34/simfire/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,19 +208,30 @@
     direction: np.ndarray
     speed_function: Optional[FunctionalConfig] = None
     direction_function: Optional[FunctionalConfig] = None
 
 
 @dataclasses.dataclass
 class Config:
-    def __init__(self, path: Union[str, Path], cfd_precompute: bool = False) -> None:
-        if isinstance(path, str):
-            path = Path(path)
+    def __init__(
+        self,
+        path: Optional[Union[str, Path]] = None,
+        config_dict: Optional[Dict[str, Any]] = None,
+        cfd_precompute: bool = False,
+    ) -> None:
+        if path is not None:
+            if isinstance(path, str):
+                path = Path(path)
         self.path = path
-        self.yaml_data = self._load_yaml()
+        if config_dict is None and path is not None:
+            self.yaml_data = self._load_yaml()
+        elif config_dict is not None and path is None:
+            self.yaml_data = config_dict
+        else:
+            raise ValueError("Either a path or a config dictionary must be specified.")
 
         # Save the original screen size in case the simulation changes from
         # operational to functional
         self.original_screen_size = self.yaml_data["area"]["screen_size"]
 
         self.lat_long_box, self.historical_layer = self._make_lat_long_box()
 
@@ -241,21 +252,22 @@
         """
         Loads the YAML file specified in self.path and returns the data as a dictionary.
 
         Returns:
             The YAML data as a dictionary
         """
         try:
-            with open(self.path, "r") as f:
-                try:
-                    yaml_data = yaml.safe_load(f)
-                except ParserError:
-                    message = f"Error parsing YAML file at {self.path}"
-                    log.error(message)
-                    raise ConfigError(message)
+            if self.path is not None:
+                with open(self.path, "r") as f:
+                    try:
+                        yaml_data = yaml.safe_load(f)
+                    except ParserError:
+                        message = f"Error parsing YAML file at {self.path}"
+                        log.error(message)
+                        raise ConfigError(message)
         except FileNotFoundError:
             message = f"Error opening YAML file at {self.path}. Does it exist?"
             log.error(message)
             raise ConfigError(message)
         return yaml_data
 
     def _make_lat_long_box(
```

### Comparing `simfire-1.4.33/simfire/utils/generate_cfd_wind_layer.py` & `simfire-1.4.34/simfire/utils/generate_cfd_wind_layer.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/graph.py` & `simfire-1.4.34/simfire/utils/graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/layers.py` & `simfire-1.4.34/simfire/utils/layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/log.py` & `simfire-1.4.34/simfire/utils/log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy` & `simfire-1.4.34/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy` & `simfire-1.4.34/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/terrain.py` & `simfire-1.4.34/simfire/utils/terrain.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,32 +38,83 @@
     """
     np.random.seed(seed)
     # Update the test for this function if this range is changed in the future
     w_0 = np.random.uniform(FuelConstants.W_0_MIN, FuelConstants.W_0_MAX)
     return w_0
 
 
+def delta_seed(seed: Union[int, None]) -> float:
+    """
+    Create a `w_0` between `0.2` and `0.6` based on an initial `seed` parameter
+
+    Arguments:
+        seed: Initial seed.
+
+    Returns:
+        The oven-dry fuel load value of the fuel.
+    """
+    np.random.seed(seed)
+    # Update the test for this function if this range is changed in the future
+    delta = np.random.uniform(FuelConstants.DELTA_MIN, FuelConstants.DELTA_MAX)
+    return delta
+
+
+def m_x_seed(seed: Union[int, None]) -> float:
+    """
+    Create a `w_0` between `0.2` and `0.6` based on an initial `seed` parameter
+
+    Arguments:
+        seed: Initial seed.
+
+    Returns:
+        The oven-dry fuel load value of the fuel.
+    """
+    np.random.seed(seed)
+    # Update the test for this function if this range is changed in the future
+    m_x = np.random.uniform(FuelConstants.M_X_MIN, FuelConstants.M_X_MAX)
+    return m_x
+
+
+def sigma_seed(seed: Union[int, None]) -> float:
+    """
+    Create a `w_0` between `0.2` and `0.6` based on an initial `seed` parameter
+
+    Arguments:
+        seed: Initial seed.
+
+    Returns:
+        The oven-dry fuel load value of the fuel.
+    """
+    np.random.seed(seed)
+    # Update the test for this function if this range is changed in the future
+    sigma = np.random.uniform(FuelConstants.SIGMA_MIN, FuelConstants.SIGMA_MAX)
+    return sigma
+
+
 def chaparral(seed: Union[int, None] = None) -> Fuel:
     """
     Create a chaparral fuel object using an optional input seed
 
     The seed only affects the input to `w_0`, the oven-dry fuel load value.
 
     Arguments:
         seed: Initial seed.
 
     Returns:
         A fuel with randomized `w_0`, `delta == 6.0`, `M_x == 0.2`, and `sigma == 1739`.
     """
     w_0 = w_0_seed(seed)
+    delta = delta_seed(seed)
+    m_x = m_x_seed(seed)
+    sigma = sigma_seed(seed)
     return Fuel(
         w_0=w_0,
-        delta=FuelConstants.DELTA,
-        M_x=FuelConstants.M_X,
-        sigma=FuelConstants.SIGMA,
+        delta=delta,
+        M_x=m_x,
+        sigma=sigma,
     )
 
 
 def fuel(seed: Optional[int] = None) -> Tuple[float, float]:
     """
     Functionailty to use a random seed to define a center point.
     To be used with operational data layers
```

### Comparing `simfire-1.4.33/simfire/utils/textures/terrain.jpg` & `simfire-1.4.34/simfire/utils/textures/terrain.jpg`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/utils/units.py` & `simfire-1.4.34/simfire/utils/units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/_tests/test_cfd_wind.py` & `simfire-1.4.34/simfire/world/_tests/test_cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/_tests/test_elevation_functions.py` & `simfire-1.4.34/simfire/world/_tests/test_elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/_tests/test_rothermel.py` & `simfire-1.4.34/simfire/world/_tests/test_rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/_tests/test_wind.py` & `simfire-1.4.34/simfire/world/_tests/test_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/elevation_functions.py` & `simfire-1.4.34/simfire/world/elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/fuel_array_functions.py` & `simfire-1.4.34/simfire/world/fuel_array_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/parameters.py` & `simfire-1.4.34/simfire/world/parameters.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/presets.py` & `simfire-1.4.34/simfire/world/presets.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/rothermel.py` & `simfire-1.4.34/simfire/world/rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/wind_mechanics/cfd_wind.py` & `simfire-1.4.34/simfire/world/wind_mechanics/cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/wind_mechanics/perlin_wind.py` & `simfire-1.4.34/simfire/world/wind_mechanics/perlin_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/simfire/world/wind_mechanics/wind_controller.py` & `simfire-1.4.34/simfire/world/wind_mechanics/wind_controller.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.33/PKG-INFO` & `simfire-1.4.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfire
-Version: 1.4.33
+Version: 1.4.34
 Summary: Fire simulator built in Python
 Home-page: https://gitlab.mitre.org/fireline/simfire
 Keywords: python,reinforcement learning,simulation,fire
 Author: Tim Welsh
 Author-email: twelsh@mitre.org
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
```

