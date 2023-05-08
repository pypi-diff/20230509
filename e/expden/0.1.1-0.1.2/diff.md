# Comparing `tmp/expden-0.1.1.tar.gz` & `tmp/expden-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expden-0.1.1.tar", max compression
+gzip compressed data, was "expden-0.1.2.tar", max compression
```

## Comparing `expden-0.1.1.tar` & `expden-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2022-11-18 17:49:16.374386 expden-0.1.1/LICENSE
--rw-r--r--   0        0        0     3611 2023-05-04 17:00:07.722817 expden-0.1.1/README.md
--rw-r--r--   0        0        0       38 2023-05-08 22:10:15.700254 expden-0.1.1/expden/__init__.py
--rw-r--r--   0        0        0     2843 2023-05-08 22:00:27.181289 expden-0.1.1/expden/core.py
--rw-r--r--   0        0        0      509 2023-05-08 22:19:17.924480 expden-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4232 1970-01-01 00:00:00.000000 expden-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-11-18 17:49:16.374386 expden-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4249 2023-05-08 22:32:01.931774 expden-0.1.2/README.md
+-rw-r--r--   0        0        0       38 2023-05-08 22:10:15.700254 expden-0.1.2/expden/__init__.py
+-rw-r--r--   0        0        0     2843 2023-05-08 22:00:27.181289 expden-0.1.2/expden/core.py
+-rw-r--r--   0        0        0      486 2023-05-08 22:32:24.834221 expden-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 expden-0.1.2/PKG-INFO
```

### Comparing `expden-0.1.1/LICENSE` & `expden-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `expden-0.1.1/README.md` & `expden-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,28 @@
-
-# ☢️ WORK IN PROGRESS ❗️
-
 # About
 
 `expden` is a library that provides functions to calculate the 
 experienced density, using a modern stack of GIS libraries in Python.
 
+### Basic Usage
+
+To calculate experienced density you just need a raster and a vector file.
+Important!
+
+```python
+import rioxarray
+import geopandas
+import expden as xp
+
+grid = rioxarray.open_rasterio(r"my_raster.tiff")
+vector = geopandas.read_file("my_vector")
+expden_vector = xp.experienced_density(raster=grid, vector=vector, radius=10)
+expden_vector.to_file("exp.geojson")
+```
+
 #### What is Experienced Density?
 
 As described by [Diego Puga](https://diegopuga.org/papers/Duranton_Puga_JEP_2020.pdf):
 
 
 _"Population or employment density is often used as a summary statistic to describe the spatial concentration of economic activity. In this context, density is commonly defined as the number of individuals per unit geographic area. Such "naive density" is easy to calculate. However, it may not appropriately reflect the density actually faced by the individual or firm at hand. One problem is that economic units are traditionally defined as aggregates of administrative units: for example, us metropolitan areas are defined based on counties. However, if a metro area includes some counties with substantial rural portions, such calculation will understate the density experienced by most economic actors. In particular, the match between urban and county boundaries is systematically looser for younger and less dense metropolitan areas in the West. De la Roca and Puga (2017) and and Henderson, Kriticos, and Nigmatulina (2020) have proposed measuring "experienced density" by counting population within a given radius around each individual. Such experienced density, in addition to dealing with the uneven tightness of area boundaries, captures better how close the typical individual is to other people when population is unevenly distributed. To give an illustrative example at the level of countries, where boundaries are given, the United States has nearly nine times the population of Canada with a slightly smaller surface area, so its naive density is ten times higher. And yet walking around cities and towns in both countries, one likely perceives similar concentrations of people nearby."_
 
@@ -28,23 +41,33 @@
 instead of within K kilometres of the average person.
 
 You can use rasters of different nature. For example, rasters with data on pollution or particulate matter.
 Go and see the docs for more!
 
 # Installation and Requirements
 
-For the installation of the package, you need a `Python >= 3.9.16` version. 
+For the installation of the package, you need a `Python >= 3.9.16` version. I recommend using an isolated virtual environment. 
 Please, take into account that you may need to install other GIS libraries in your system, such as GDAL or PROJ4.
 
-To install the latest stable version of the library, please use `pip:
+To install the latest stable version of the library, please use `pip`:
 
 ```
 pip install expden
 ```
 
+The main dependencies of the project include `geopandas`, `xarray-spatial`, `rioxarray` and `geocube`. 
+
+# TO DO List
+
+- [x] First working version
+- [ ] Add documentation
+- [ ] Add examples
+- [ ] Parallel version of the main funcionality
+
+
 # References
 
 This library abstracts the functionality needed to perform the experienced density calculations that 
 you can see in the economic academic literature. Some references:
 
 De la Roca, Jorge and Diego Puga. 2017. Learning by 
 working in big cities. Review of Economic Studies 84(1):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `expden-0.1.1/expden/core.py` & `expden-0.1.2/expden/core.py`

 * *Files identical despite different names*

### Comparing `expden-0.1.1/PKG-INFO` & `expden-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 Metadata-Version: 2.1
 Name: expden
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to compute the experienced density
 License: MIT
 Author: Nico Forteza 
 Author-email: nicoforteza@gmail.com
 Maintainer: Nico Forteza 
 Maintainer-email: nicoforteza@gmail.com
 Requires-Python: ==3.9.16
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: geocube (==0.4.0)
 Requires-Dist: geopandas (==0.12.1)
 Requires-Dist: numba (==0.56.4)
-Requires-Dist: rasterstats (==0.17.0)
 Requires-Dist: rioxarray (==0.13.1)
 Requires-Dist: xarray-spatial (==0.3.5)
 Description-Content-Type: text/markdown
 
-
-# ☢️ WORK IN PROGRESS ❗️
-
 # About
 
 `expden` is a library that provides functions to calculate the 
 experienced density, using a modern stack of GIS libraries in Python.
 
+### Basic Usage
+
+To calculate experienced density you just need a raster and a vector file.
+Important!
+
+```python
+import rioxarray
+import geopandas
+import expden as xp
+
+grid = rioxarray.open_rasterio(r"my_raster.tiff")
+vector = geopandas.read_file("my_vector")
+expden_vector = xp.experienced_density(raster=grid, vector=vector, radius=10)
+expden_vector.to_file("exp.geojson")
+```
+
 #### What is Experienced Density?
 
 As described by [Diego Puga](https://diegopuga.org/papers/Duranton_Puga_JEP_2020.pdf):
 
 
 _"Population or employment density is often used as a summary statistic to describe the spatial concentration of economic activity. In this context, density is commonly defined as the number of individuals per unit geographic area. Such "naive density" is easy to calculate. However, it may not appropriately reflect the density actually faced by the individual or firm at hand. One problem is that economic units are traditionally defined as aggregates of administrative units: for example, us metropolitan areas are defined based on counties. However, if a metro area includes some counties with substantial rural portions, such calculation will understate the density experienced by most economic actors. In particular, the match between urban and county boundaries is systematically looser for younger and less dense metropolitan areas in the West. De la Roca and Puga (2017) and and Henderson, Kriticos, and Nigmatulina (2020) have proposed measuring "experienced density" by counting population within a given radius around each individual. Such experienced density, in addition to dealing with the uneven tightness of area boundaries, captures better how close the typical individual is to other people when population is unevenly distributed. To give an illustrative example at the level of countries, where boundaries are given, the United States has nearly nine times the population of Canada with a slightly smaller surface area, so its naive density is ten times higher. And yet walking around cities and towns in both countries, one likely perceives similar concentrations of people nearby."_
 
@@ -48,23 +60,33 @@
 instead of within K kilometres of the average person.
 
 You can use rasters of different nature. For example, rasters with data on pollution or particulate matter.
 Go and see the docs for more!
 
 # Installation and Requirements
 
-For the installation of the package, you need a `Python >= 3.9.16` version. 
+For the installation of the package, you need a `Python >= 3.9.16` version. I recommend using an isolated virtual environment. 
 Please, take into account that you may need to install other GIS libraries in your system, such as GDAL or PROJ4.
 
-To install the latest stable version of the library, please use `pip:
+To install the latest stable version of the library, please use `pip`:
 
 ```
 pip install expden
 ```
 
+The main dependencies of the project include `geopandas`, `xarray-spatial`, `rioxarray` and `geocube`. 
+
+# TO DO List
+
+- [x] First working version
+- [ ] Add documentation
+- [ ] Add examples
+- [ ] Parallel version of the main funcionality
+
+
 # References
 
 This library abstracts the functionality needed to perform the experienced density calculations that 
 you can see in the economic academic literature. Some references:
 
 De la Roca, Jorge and Diego Puga. 2017. Learning by 
 working in big cities. Review of Economic Studies 84(1):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

