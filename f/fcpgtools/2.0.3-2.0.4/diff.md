# Comparing `tmp/fcpgtools-2.0.3.tar.gz` & `tmp/fcpgtools-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcpgtools-2.0.3.tar", max compression
+gzip compressed data, was "fcpgtools-2.0.4.tar", max compression
```

## Comparing `fcpgtools-2.0.3.tar` & `fcpgtools-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1696 2022-09-01 20:26:09.281027 fcpgtools-2.0.3/LICENSE.md
--rw-r--r--   0        0        0     2258 2023-04-07 14:39:47.388061 fcpgtools-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     6674 2023-01-23 19:54:56.786067 fcpgtools-2.0.3/README.md
--rw-r--r--   0        0        0     1894 2023-04-07 14:39:54.952539 fcpgtools-2.0.3/src/fcpgtools/__init__.py
--rw-r--r--   0        0        0     3196 2023-02-22 16:21:06.167802 fcpgtools-2.0.3/src/fcpgtools/custom_types.py
--rw-r--r--   0        0        0      179 2023-02-22 16:24:49.962581 fcpgtools-2.0.3/src/fcpgtools/terrainengine/__init__.py
--rw-r--r--   0        0        0     1814 2023-02-22 18:49:40.438268 fcpgtools-2.0.3/src/fcpgtools/terrainengine/engine_validator.py
--rw-r--r--   0        0        0     7242 2023-02-22 16:37:48.129686 fcpgtools-2.0.3/src/fcpgtools/terrainengine/protocols.py
--rw-r--r--   0        0        0     9630 2023-02-22 16:30:19.959412 fcpgtools-2.0.3/src/fcpgtools/terrainengine/pysheds_engine.py
--rw-r--r--   0        0        0    28395 2023-02-22 16:33:17.723687 fcpgtools-2.0.3/src/fcpgtools/terrainengine/taudem_engine.py
--rw-r--r--   0        0        0    46951 2023-02-22 18:39:16.906699 fcpgtools-2.0.3/src/fcpgtools/tools.py
--rw-r--r--   0        0        0    85241 2023-02-22 16:17:10.163008 fcpgtools-2.0.3/src/fcpgtools/tools_deprecated.py
--rw-r--r--   0        0        0    15904 2023-04-07 14:37:49.682745 fcpgtools-2.0.3/src/fcpgtools/utilities.py
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 fcpgtools-2.0.3/setup.py
--rw-r--r--   0        0        0     8234 1970-01-01 00:00:00.000000 fcpgtools-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1696 2022-09-01 20:26:09.281027 fcpgtools-2.0.4/LICENSE.md
+-rw-r--r--   0        0        0     2258 2023-05-09 21:15:41.002977 fcpgtools-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6876 2023-05-09 21:33:22.969735 fcpgtools-2.0.4/README.md
+-rw-r--r--   0        0        0     1894 2023-05-09 21:15:41.046653 fcpgtools-2.0.4/src/fcpgtools/__init__.py
+-rw-r--r--   0        0        0     3196 2023-02-22 16:21:06.167802 fcpgtools-2.0.4/src/fcpgtools/custom_types.py
+-rw-r--r--   0        0        0      179 2023-02-22 16:24:49.962581 fcpgtools-2.0.4/src/fcpgtools/terrainengine/__init__.py
+-rw-r--r--   0        0        0     1814 2023-02-22 18:49:40.438268 fcpgtools-2.0.4/src/fcpgtools/terrainengine/engine_validator.py
+-rw-r--r--   0        0        0     7242 2023-02-22 16:37:48.129686 fcpgtools-2.0.4/src/fcpgtools/terrainengine/protocols.py
+-rw-r--r--   0        0        0     9630 2023-02-22 16:30:19.959412 fcpgtools-2.0.4/src/fcpgtools/terrainengine/pysheds_engine.py
+-rw-r--r--   0        0        0    28420 2023-05-09 21:12:43.701514 fcpgtools-2.0.4/src/fcpgtools/terrainengine/taudem_engine.py
+-rw-r--r--   0        0        0    46935 2023-05-09 21:33:22.985374 fcpgtools-2.0.4/src/fcpgtools/tools.py
+-rw-r--r--   0        0        0    85241 2023-02-22 16:17:10.163008 fcpgtools-2.0.4/src/fcpgtools/tools_deprecated.py
+-rw-r--r--   0        0        0    15904 2023-04-20 19:58:09.858113 fcpgtools-2.0.4/src/fcpgtools/utilities.py
+-rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 fcpgtools-2.0.4/setup.py
+-rw-r--r--   0        0        0     8434 1970-01-01 00:00:00.000000 fcpgtools-2.0.4/PKG-INFO
```

### Comparing `fcpgtools-2.0.3/LICENSE.md` & `fcpgtools-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/pyproject.toml` & `fcpgtools-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 
 # base attributes
 name = "fcpgtools"
-version = "2.0.3"
+version = "2.0.4"
 description = "Tools to create Flow-Conditioned Parameter Grids (FCPGs) from Flow Direction Rasters (FDRs) and arbitrary rasterized parameter data."
 authors = [
     "Theodore Barnhart <tbarnhart@usgs.gov>", 
     "Xavier R Nogueira <xrnogueira@limno.com>", 
     "Seth Siefken <ssiefken@usgs.gov>", 
     "August Raleigh Schultz <arschultz@usgs.gov>", 
     "Anthony Aufdenkampe <aaufdenkampe@limno.com>",
```

### Comparing `fcpgtools-2.0.3/README.md` & `fcpgtools-2.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Flow-Conditioned Parameter Grid (FCPG) Tools Documentation
 ===============================================================
 
 
-**For detailed documentation please reference our [ReadTheDocs site](https://usgs.github.io/water-fcpg-tools/build/html/index.html)!** 
+**For detailed documentation please reference our [ReadTheDocs site](https://fcpgtools.readthedocs.io/en/latest/)!** 
+
+Note that the most recent version of this repository is available on [GitLab](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools). While mirrored on GitHub, the repos can get out of sync.
 
 Please log any issues or feature requests using [this form](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/issues/new?issuable_template=bug).
 
 # Getting Started
 ## Installation
 `FCPGtools` can be installed from [`PyPI`](https://pypi.org/project/fcpgtools/) into a virtual environment containing [`GDAL`](https://anaconda.org/conda-forge/gdal), and for full functionality, [`TauDEM`](https://anaconda.org/conda-forge/taudem) as well.
 
@@ -46,37 +48,37 @@
 path_to_fdr = r'YOUR/PATH/HERE/fdr.tif'
 
 flow_accumulation_grid = fcpgtools.accumulate_flow(
     d8_fdr=path_to_fdr,
 ) -> xarray.DataArray
 ```
 
-Please refer to our documentation's [Cookbook](https://usgs.github.io/water-fcpg-tools/cookbook.html) page for more intricate examples of usage.
+Please refer to our documentation's [Cookbook](https://fcpgtools.readthedocs.io/en/latest/cookbook.html) page for more intricate examples of usage.
 
 # Citation
 * **Version 2.0** was released in January, 2023.
     * Barnhart, T.B., Nogueira, X.R., Siefken, S.A., Schultz, A.R., Aufenkampe, A., Tomasula, P., 2023, Flow-Conditioned Parameter Grid Tools Version 2.0.
 * **Version 1.1** was released in September, 2022.
 * **Version 1.0** (IP-112996) was approved on September 3, 2020.
     * Barnhart, T.B., Sando, R., Siefken, S.A., McCarthy, P.M., and Rea, A.H., 2020, Flow-Conditioned Parameter Grid Tools: U.S. Geological Survey Software Release, DOI: https://doi.org/10.5066/P9W8UZ47.
 
 # Migrating from Version 1.0
-Version 2.0 of `FCPGtools` is a ground-up refactor and rebuild of Version 1.0. Backwards compatibility is broken, and many work-flows have been significantly streamlined. We strongly suggest that any users accustomed to Version 1.0 reference our [updated documentation site](https://usgs.github.io/water-fcpg-tools/index.html).
+Version 2.0 of `FCPGtools` is a ground-up refactor and rebuild of Version 1.0. Backwards compatibility is broken, and many work-flows have been significantly streamlined. We strongly suggest that any users accustomed to Version 1.0 reference our [updated documentation site](https://fcpgtools.readthedocs.io/en/latest/index.html).
 
 **A non-exhaustive list of key updates is below:**
 * All functions output an in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object, allowing for functions to be strung together into performance oriented pipelines.
     * [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects have a variety of powerful features and optimizations. For more information please reference the library's [documentation](https://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html).
     * Rasters can still be saved to a local GeoTIFF file by providing a valid `.tif` path to `param:out_path`.
 * All functions can now accept either local string paths, local [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html) objects, or in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects.
 * Multi-band parameter grids are now supported!
-    * Example: Passing a 12-month precipitation raster (where each month is a raster band) into [`fcpgtools.accumulate_parameter()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_parameter) will output a 12-band [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object.
+    * Example: Passing a 12-month precipitation raster (where each month is a raster band) into [`fcpgtools.accumulate_parameter()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_parameter) will output a 12-band [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object.
 * Flow Direction Raster format conversion (i.e. ESRI -> TauDEM) is now automated behind-the-scenes.
 * Support for multiple "terrain engines" gives users optionality and increases dependency deprecation resiliancy. 
     * Where necessary users can set `param:engine` to [`taudem`](https://hydrology.usu.edu/taudem/taudem5/) (default) or [`pysheds`](https://github.com/mdbartos/pysheds).
-    * Note that the `pysheds` terrain engine is signifcantly more performant, however it currently only supports [`accumulate_flow()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_flow) and [`accumulate_parameter()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_parameter).
+    * Note that the `pysheds` terrain engine is signifcantly more performant, however it currently only supports [`accumulate_flow()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_flow) and [`accumulate_parameter()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_parameter).
 
 **Please reference our markdown [`refactored_names`](examples/refactored_names.md) document for a complete mapping of Version 1.1 to Version 2.0 function names.**
 
 
 ## Disclaimers
 Any use of trade, firm, or product names is for descriptive purposes only and does not imply endorsement by the U.S. Government.
```

### Comparing `fcpgtools-2.0.3/src/fcpgtools/__init__.py` & `fcpgtools-2.0.4/src/fcpgtools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 machine learning, and physical hydrologic modeling.
 
 For more information and use examples see our documentation: 
 https://usgs.github.io/water-fcpg-tools/build/html/index.html
 
 """
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 from fcpgtools.tools import (
     accumulate_flow,
     accumulate_parameter,
     adjust_parameter_raster,
     align_raster,
     binarize_categorical_raster,
```

### Comparing `fcpgtools-2.0.3/src/fcpgtools/custom_types.py` & `fcpgtools-2.0.4/src/fcpgtools/custom_types.py`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/src/fcpgtools/terrainengine/engine_validator.py` & `fcpgtools-2.0.4/src/fcpgtools/terrainengine/engine_validator.py`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/src/fcpgtools/terrainengine/protocols.py` & `fcpgtools-2.0.4/src/fcpgtools/terrainengine/protocols.py`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/src/fcpgtools/terrainengine/pysheds_engine.py` & `fcpgtools-2.0.4/src/fcpgtools/terrainengine/pysheds_engine.py`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/src/fcpgtools/terrainengine/taudem_engine.py` & `fcpgtools-2.0.4/src/fcpgtools/terrainengine/taudem_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     @staticmethod
     def _taudem_prepper(
         in_raster: Raster,
     ) -> str:
         """Converts an input raster into a TauDEM compatible path string.  Creates a temp file if necessary."""
         if isinstance(in_raster, xr.DataArray):
             temp_path = Path(
-                tempfile.TemporaryFile(
+                tempfile.NamedTemporaryFile(
                     dir=Path.cwd(),
                     prefix='taudem_temp_input',
                     suffix='.tif',
                 ).name
             )
             tools.save_raster(
                 in_raster,
@@ -169,15 +169,15 @@
                     -1,
                 )
             weight_path = TauDEMEngine._taudem_prepper(weights)
             wg = '-wg '
 
         if out_path is None:
             out_path = Path(
-                tempfile.TemporaryFile(
+                tempfile.NamedTemporaryFile(
                     dir=Path.cwd(),
                     prefix='fac_temp',
                     suffix='.tif',
                 ).name
             )
         elif isinstance(out_path, str):
             out_path = Path(out_path)
@@ -358,15 +358,15 @@
         fac_raster = fac_raster.fillna(0)
         fac_raster = fac_raster.rio.write_nodata(0)
         fac_raster = fac_raster.astype('int')
         fac_path = TauDEMEngine._taudem_prepper(fac_raster)
 
         if out_path is None:
             out_path = Path(
-                tempfile.TemporaryFile(
+                tempfile.NamedTemporaryFile(
                     dir=Path.cwd(),
                     prefix='distance_to_stream_temp',
                     suffix='.tif',
                 ).name
             )
         elif isinstance(out_path, str):
             out_path = Path(out_path)
@@ -435,15 +435,15 @@
     ) -> xr.DataArray:
         """Back end function that makes the command line call for TauDEM:D8FlowPathExtremeUp"""
 
         parameter_raster_path = TauDEMEngine._taudem_prepper(parameter_raster)
 
         # make temporary output path
         out_path = Path(
-            tempfile.TemporaryFile(
+            tempfile.NamedTemporaryFile(
                 dir=Path.cwd(),
                 prefix='ext_upslope_temp',
                 suffix='.tif',
             ).name
         )
 
         taudem_dict = {
@@ -589,15 +589,15 @@
         **kwargs,
     ) -> xr.DataArray:
 
         weights_path = TauDEMEngine._taudem_prepper(weights)
 
         # make temporary output path
         out_path = Path(
-            tempfile.TemporaryFile(
+            tempfile.NamedTemporaryFile(
                 dir=Path.cwd(),
                 prefix='decay_accum_temp',
                 suffix='.tif',
             ).name
         )
 
         # build the input dictionary
```

### Comparing `fcpgtools-2.0.3/src/fcpgtools/tools.py` & `fcpgtools-2.0.4/src/fcpgtools/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 This file contains the user-facing tools imported when one imports fcpgtools.
 All functions can accept inputs either as in memory objects 
 (i.e. xarray.DataArray + geopandas.GeoDataFrame) or string/pathlib.Path inputs.
 Additionally, many functions have a out_path parameter that allows outputs to 
 be saved to a path in addition to the function returning an in-memory object.
 
 See function specific documentation here:
-https://usgs.github.io/water-fcpg-tools/build/html/functions.html
+https://fcpgtools.readthedocs.io/en/latest/functions.html
 
 See examples of use here:
-https://usgs.github.io/water-fcpg-tools/build/html/cookbook.html
+https://fcpgtools.readthedocs.io/en/latest/cookbook.html
 """
 from typing import Union, Dict, List, Tuple, Optional
 import warnings
 from pathlib import Path
 import xarray as xr
 import rioxarray as rio
 import numpy as np
```

### Comparing `fcpgtools-2.0.3/src/fcpgtools/tools_deprecated.py` & `fcpgtools-2.0.4/src/fcpgtools/tools_deprecated.py`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/src/fcpgtools/utilities.py` & `fcpgtools-2.0.4/src/fcpgtools/utilities.py`

 * *Files identical despite different names*

### Comparing `fcpgtools-2.0.3/setup.py` & `fcpgtools-2.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'pysheds>=0.3.3,<0.4.0',
  'rasterio>=1.3.4,<2.0.0',
  'rioxarray>=0.13.3,<0.14.0',
  'xarray>=2023.1.0,<2024.0.0']
 
 setup_kwargs = {
     'name': 'fcpgtools',
-    'version': '2.0.3',
+    'version': '2.0.4',
     'description': 'Tools to create Flow-Conditioned Parameter Grids (FCPGs) from Flow Direction Rasters (FDRs) and arbitrary rasterized parameter data.',
-    'long_description': 'Flow-Conditioned Parameter Grid (FCPG) Tools Documentation\n===============================================================\n\n\n**For detailed documentation please reference our [ReadTheDocs site](https://usgs.github.io/water-fcpg-tools/build/html/index.html)!** \n\nPlease log any issues or feature requests using [this form](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/issues/new?issuable_template=bug).\n\n# Getting Started\n## Installation\n`FCPGtools` can be installed from [`PyPI`](https://pypi.org/project/fcpgtools/) into a virtual environment containing [`GDAL`](https://anaconda.org/conda-forge/gdal), and for full functionality, [`TauDEM`](https://anaconda.org/conda-forge/taudem) as well.\n\n**We strongly encourage the following installation workflow:**\n\n1. Install the Anaconda Python Distribution or Miniconda\n    * [Anaconda Individual Edition](https://www.anaconda.com/products/distribution) - includes `conda`, a complete Python (and R) data science stack, and the helpful Anaconda Navigator GUI.\n    * A lighter-weight alternative is to [install Miniconda](https://docs.conda.io/en/latest/miniconda.html).\n2. Use the `conda` command line to clone our lightweight `fcpgtools_base` virtual environment that contains non-Python dependencies from the [`environment.yml`](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/environment.yml) file available in our repo. Either clone the repo, or just download the .yml file locally, and run the following commands:\n\n    ```\n    conda env create -f {PATH}/environment.yml\n    ```\n    * **Note:** We also provide a more robust [`environment_dev.yml`](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/environment_dev.yml) virtual environment for developers containing all libraries relevant to making contributions as well as running our [example notebooks](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/examples).\n3. Activate the `fcpgtools_base` environment, and pip install `fcpgtools`.\n    ```\n    pip install fcpgtools\n    ```\n4. (optional) pip install optional libraries required to run our demo notebook ([`examples/v2_fcpgtools_demo.ipynb`](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/examples/v2_fcpgtools_demo.ipynb)), and to leverage in-line function completion/type-hints.\n    ```\n    pip install jupyterlab\n    pip install ipympl\n    pip install python-lsp-server\n    pip install jupyterlab-lsp\n    pip install pydaymet\n    ```\n\n\n\n## Using FCPGtools\nVersion 2.0 of `FCPGtools` has a "flat" architecture, meaning all functions can be accessed by importing the main `fcpgtools` module as shown in a simple example below:\n\n```python\n# creating an flow accumulation raster from a Flow Direction Raster (FDR)\nimport fcpgtools\n\npath_to_fdr = r\'YOUR/PATH/HERE/fdr.tif\'\n\nflow_accumulation_grid = fcpgtools.accumulate_flow(\n    d8_fdr=path_to_fdr,\n) -> xarray.DataArray\n```\n\nPlease refer to our documentation\'s [Cookbook](https://usgs.github.io/water-fcpg-tools/cookbook.html) page for more intricate examples of usage.\n\n# Citation\n* **Version 2.0** was released in January, 2023.\n    * Barnhart, T.B., Nogueira, X.R., Siefken, S.A., Schultz, A.R., Aufenkampe, A., Tomasula, P., 2023, Flow-Conditioned Parameter Grid Tools Version 2.0.\n* **Version 1.1** was released in September, 2022.\n* **Version 1.0** (IP-112996) was approved on September 3, 2020.\n    * Barnhart, T.B., Sando, R., Siefken, S.A., McCarthy, P.M., and Rea, A.H., 2020, Flow-Conditioned Parameter Grid Tools: U.S. Geological Survey Software Release, DOI: https://doi.org/10.5066/P9W8UZ47.\n\n# Migrating from Version 1.0\nVersion 2.0 of `FCPGtools` is a ground-up refactor and rebuild of Version 1.0. Backwards compatibility is broken, and many work-flows have been significantly streamlined. We strongly suggest that any users accustomed to Version 1.0 reference our [updated documentation site](https://usgs.github.io/water-fcpg-tools/index.html).\n\n**A non-exhaustive list of key updates is below:**\n* All functions output an in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object, allowing for functions to be strung together into performance oriented pipelines.\n    * [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects have a variety of powerful features and optimizations. For more information please reference the library\'s [documentation](https://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html).\n    * Rasters can still be saved to a local GeoTIFF file by providing a valid `.tif` path to `param:out_path`.\n* All functions can now accept either local string paths, local [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html) objects, or in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects.\n* Multi-band parameter grids are now supported!\n    * Example: Passing a 12-month precipitation raster (where each month is a raster band) into [`fcpgtools.accumulate_parameter()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_parameter) will output a 12-band [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object.\n* Flow Direction Raster format conversion (i.e. ESRI -> TauDEM) is now automated behind-the-scenes.\n* Support for multiple "terrain engines" gives users optionality and increases dependency deprecation resiliancy. \n    * Where necessary users can set `param:engine` to [`taudem`](https://hydrology.usu.edu/taudem/taudem5/) (default) or [`pysheds`](https://github.com/mdbartos/pysheds).\n    * Note that the `pysheds` terrain engine is signifcantly more performant, however it currently only supports [`accumulate_flow()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_flow) and [`accumulate_parameter()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_parameter).\n\n**Please reference our markdown [`refactored_names`](examples/refactored_names.md) document for a complete mapping of Version 1.1 to Version 2.0 function names.**\n\n\n## Disclaimers\nAny use of trade, firm, or product names is for descriptive purposes only and does not imply endorsement by the U.S. Government.\n\nPlease see [DISCLAIMER.md](DISCLAIMER.md) in the project repository.\n\n## License\nPlease see [LICENSE.md](LICENSE.md) in the project repository.\n',
+    'long_description': 'Flow-Conditioned Parameter Grid (FCPG) Tools Documentation\n===============================================================\n\n\n**For detailed documentation please reference our [ReadTheDocs site](https://fcpgtools.readthedocs.io/en/latest/)!** \n\nNote that the most recent version of this repository is available on [GitLab](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools). While mirrored on GitHub, the repos can get out of sync.\n\nPlease log any issues or feature requests using [this form](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/issues/new?issuable_template=bug).\n\n# Getting Started\n## Installation\n`FCPGtools` can be installed from [`PyPI`](https://pypi.org/project/fcpgtools/) into a virtual environment containing [`GDAL`](https://anaconda.org/conda-forge/gdal), and for full functionality, [`TauDEM`](https://anaconda.org/conda-forge/taudem) as well.\n\n**We strongly encourage the following installation workflow:**\n\n1. Install the Anaconda Python Distribution or Miniconda\n    * [Anaconda Individual Edition](https://www.anaconda.com/products/distribution) - includes `conda`, a complete Python (and R) data science stack, and the helpful Anaconda Navigator GUI.\n    * A lighter-weight alternative is to [install Miniconda](https://docs.conda.io/en/latest/miniconda.html).\n2. Use the `conda` command line to clone our lightweight `fcpgtools_base` virtual environment that contains non-Python dependencies from the [`environment.yml`](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/environment.yml) file available in our repo. Either clone the repo, or just download the .yml file locally, and run the following commands:\n\n    ```\n    conda env create -f {PATH}/environment.yml\n    ```\n    * **Note:** We also provide a more robust [`environment_dev.yml`](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/environment_dev.yml) virtual environment for developers containing all libraries relevant to making contributions as well as running our [example notebooks](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/examples).\n3. Activate the `fcpgtools_base` environment, and pip install `fcpgtools`.\n    ```\n    pip install fcpgtools\n    ```\n4. (optional) pip install optional libraries required to run our demo notebook ([`examples/v2_fcpgtools_demo.ipynb`](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/blob/master/examples/v2_fcpgtools_demo.ipynb)), and to leverage in-line function completion/type-hints.\n    ```\n    pip install jupyterlab\n    pip install ipympl\n    pip install python-lsp-server\n    pip install jupyterlab-lsp\n    pip install pydaymet\n    ```\n\n\n\n## Using FCPGtools\nVersion 2.0 of `FCPGtools` has a "flat" architecture, meaning all functions can be accessed by importing the main `fcpgtools` module as shown in a simple example below:\n\n```python\n# creating an flow accumulation raster from a Flow Direction Raster (FDR)\nimport fcpgtools\n\npath_to_fdr = r\'YOUR/PATH/HERE/fdr.tif\'\n\nflow_accumulation_grid = fcpgtools.accumulate_flow(\n    d8_fdr=path_to_fdr,\n) -> xarray.DataArray\n```\n\nPlease refer to our documentation\'s [Cookbook](https://fcpgtools.readthedocs.io/en/latest/cookbook.html) page for more intricate examples of usage.\n\n# Citation\n* **Version 2.0** was released in January, 2023.\n    * Barnhart, T.B., Nogueira, X.R., Siefken, S.A., Schultz, A.R., Aufenkampe, A., Tomasula, P., 2023, Flow-Conditioned Parameter Grid Tools Version 2.0.\n* **Version 1.1** was released in September, 2022.\n* **Version 1.0** (IP-112996) was approved on September 3, 2020.\n    * Barnhart, T.B., Sando, R., Siefken, S.A., McCarthy, P.M., and Rea, A.H., 2020, Flow-Conditioned Parameter Grid Tools: U.S. Geological Survey Software Release, DOI: https://doi.org/10.5066/P9W8UZ47.\n\n# Migrating from Version 1.0\nVersion 2.0 of `FCPGtools` is a ground-up refactor and rebuild of Version 1.0. Backwards compatibility is broken, and many work-flows have been significantly streamlined. We strongly suggest that any users accustomed to Version 1.0 reference our [updated documentation site](https://fcpgtools.readthedocs.io/en/latest/index.html).\n\n**A non-exhaustive list of key updates is below:**\n* All functions output an in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object, allowing for functions to be strung together into performance oriented pipelines.\n    * [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects have a variety of powerful features and optimizations. For more information please reference the library\'s [documentation](https://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html).\n    * Rasters can still be saved to a local GeoTIFF file by providing a valid `.tif` path to `param:out_path`.\n* All functions can now accept either local string paths, local [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html) objects, or in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects.\n* Multi-band parameter grids are now supported!\n    * Example: Passing a 12-month precipitation raster (where each month is a raster band) into [`fcpgtools.accumulate_parameter()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_parameter) will output a 12-band [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object.\n* Flow Direction Raster format conversion (i.e. ESRI -> TauDEM) is now automated behind-the-scenes.\n* Support for multiple "terrain engines" gives users optionality and increases dependency deprecation resiliancy. \n    * Where necessary users can set `param:engine` to [`taudem`](https://hydrology.usu.edu/taudem/taudem5/) (default) or [`pysheds`](https://github.com/mdbartos/pysheds).\n    * Note that the `pysheds` terrain engine is signifcantly more performant, however it currently only supports [`accumulate_flow()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_flow) and [`accumulate_parameter()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_parameter).\n\n**Please reference our markdown [`refactored_names`](examples/refactored_names.md) document for a complete mapping of Version 1.1 to Version 2.0 function names.**\n\n\n## Disclaimers\nAny use of trade, firm, or product names is for descriptive purposes only and does not imply endorsement by the U.S. Government.\n\nPlease see [DISCLAIMER.md](DISCLAIMER.md) in the project repository.\n\n## License\nPlease see [LICENSE.md](LICENSE.md) in the project repository.\n',
     'author': 'Theodore Barnhart',
     'author_email': 'tbarnhart@usgs.gov',
     'maintainer': 'Xavier R Nogueira',
     'maintainer_email': 'xrnogueira@limno.com',
     'url': 'https://usgs.github.io/water-fcpg-tools/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `fcpgtools-2.0.3/PKG-INFO` & `fcpgtools-2.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcpgtools
-Version: 2.0.3
+Version: 2.0.4
 Summary: Tools to create Flow-Conditioned Parameter Grids (FCPGs) from Flow Direction Rasters (FDRs) and arbitrary rasterized parameter data.
 Home-page: https://usgs.github.io/water-fcpg-tools/
 Keywords: hydrology,terrain,machine-learning,raster,flow-statistics
 Author: Theodore Barnhart
 Author-email: tbarnhart@usgs.gov
 Maintainer: Xavier R Nogueira
 Maintainer-email: xrnogueira@limno.com
@@ -34,15 +34,17 @@
 Project-URL: Repository, https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools
 Description-Content-Type: text/markdown
 
 Flow-Conditioned Parameter Grid (FCPG) Tools Documentation
 ===============================================================
 
 
-**For detailed documentation please reference our [ReadTheDocs site](https://usgs.github.io/water-fcpg-tools/build/html/index.html)!** 
+**For detailed documentation please reference our [ReadTheDocs site](https://fcpgtools.readthedocs.io/en/latest/)!** 
+
+Note that the most recent version of this repository is available on [GitLab](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools). While mirrored on GitHub, the repos can get out of sync.
 
 Please log any issues or feature requests using [this form](https://code.usgs.gov/StreamStats/data-preparation/cpg/FCPGtools/-/issues/new?issuable_template=bug).
 
 # Getting Started
 ## Installation
 `FCPGtools` can be installed from [`PyPI`](https://pypi.org/project/fcpgtools/) into a virtual environment containing [`GDAL`](https://anaconda.org/conda-forge/gdal), and for full functionality, [`TauDEM`](https://anaconda.org/conda-forge/taudem) as well.
 
@@ -82,37 +84,37 @@
 path_to_fdr = r'YOUR/PATH/HERE/fdr.tif'
 
 flow_accumulation_grid = fcpgtools.accumulate_flow(
     d8_fdr=path_to_fdr,
 ) -> xarray.DataArray
 ```
 
-Please refer to our documentation's [Cookbook](https://usgs.github.io/water-fcpg-tools/cookbook.html) page for more intricate examples of usage.
+Please refer to our documentation's [Cookbook](https://fcpgtools.readthedocs.io/en/latest/cookbook.html) page for more intricate examples of usage.
 
 # Citation
 * **Version 2.0** was released in January, 2023.
     * Barnhart, T.B., Nogueira, X.R., Siefken, S.A., Schultz, A.R., Aufenkampe, A., Tomasula, P., 2023, Flow-Conditioned Parameter Grid Tools Version 2.0.
 * **Version 1.1** was released in September, 2022.
 * **Version 1.0** (IP-112996) was approved on September 3, 2020.
     * Barnhart, T.B., Sando, R., Siefken, S.A., McCarthy, P.M., and Rea, A.H., 2020, Flow-Conditioned Parameter Grid Tools: U.S. Geological Survey Software Release, DOI: https://doi.org/10.5066/P9W8UZ47.
 
 # Migrating from Version 1.0
-Version 2.0 of `FCPGtools` is a ground-up refactor and rebuild of Version 1.0. Backwards compatibility is broken, and many work-flows have been significantly streamlined. We strongly suggest that any users accustomed to Version 1.0 reference our [updated documentation site](https://usgs.github.io/water-fcpg-tools/index.html).
+Version 2.0 of `FCPGtools` is a ground-up refactor and rebuild of Version 1.0. Backwards compatibility is broken, and many work-flows have been significantly streamlined. We strongly suggest that any users accustomed to Version 1.0 reference our [updated documentation site](https://fcpgtools.readthedocs.io/en/latest/index.html).
 
 **A non-exhaustive list of key updates is below:**
 * All functions output an in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object, allowing for functions to be strung together into performance oriented pipelines.
     * [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects have a variety of powerful features and optimizations. For more information please reference the library's [documentation](https://docs.xarray.dev/en/stable/getting-started-guide/why-xarray.html).
     * Rasters can still be saved to a local GeoTIFF file by providing a valid `.tif` path to `param:out_path`.
 * All functions can now accept either local string paths, local [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html) objects, or in-memory [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) objects.
 * Multi-band parameter grids are now supported!
-    * Example: Passing a 12-month precipitation raster (where each month is a raster band) into [`fcpgtools.accumulate_parameter()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_parameter) will output a 12-band [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object.
+    * Example: Passing a 12-month precipitation raster (where each month is a raster band) into [`fcpgtools.accumulate_parameter()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_parameter) will output a 12-band [`xarray.DataArray`](https://docs.xarray.dev/en/stable/generated/xarray.DataArray.html#xarray.DataArray) object.
 * Flow Direction Raster format conversion (i.e. ESRI -> TauDEM) is now automated behind-the-scenes.
 * Support for multiple "terrain engines" gives users optionality and increases dependency deprecation resiliancy. 
     * Where necessary users can set `param:engine` to [`taudem`](https://hydrology.usu.edu/taudem/taudem5/) (default) or [`pysheds`](https://github.com/mdbartos/pysheds).
-    * Note that the `pysheds` terrain engine is signifcantly more performant, however it currently only supports [`accumulate_flow()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_flow) and [`accumulate_parameter()`](https://usgs.github.io/water-fcpg-tools/functions.html#fcpgtools.tools.accumulate_parameter).
+    * Note that the `pysheds` terrain engine is signifcantly more performant, however it currently only supports [`accumulate_flow()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_flow) and [`accumulate_parameter()`](https://fcpgtools.readthedocs.io/en/latest/functions.html#fcpgtools.tools.accumulate_parameter).
 
 **Please reference our markdown [`refactored_names`](examples/refactored_names.md) document for a complete mapping of Version 1.1 to Version 2.0 function names.**
 
 
 ## Disclaimers
 Any use of trade, firm, or product names is for descriptive purposes only and does not imply endorsement by the U.S. Government.
```

