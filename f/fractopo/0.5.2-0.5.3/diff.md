# Comparing `tmp/fractopo-0.5.2.tar.gz` & `tmp/fractopo-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractopo-0.5.2.tar", max compression
+gzip compressed data, was "fractopo-0.5.3.tar", max compression
```

## Comparing `fractopo-0.5.2.tar` & `fractopo-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     9241 2023-01-16 08:26:40.626522 fractopo-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     1062 2023-01-16 08:26:40.626522 fractopo-0.5.2/LICENSE.md
--rw-r--r--   0        0        0    17261 2023-01-16 08:26:40.626522 fractopo-0.5.2/README.rst
--rw-r--r--   0        0        0      615 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/__init__.py
--rw-r--r--   0        0        0       99 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/__main__.py
--rw-r--r--   0        0        0      157 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/__init__.py
--rw-r--r--   0        0        0     6025 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/anisotropy.py
--rw-r--r--   0        0        0    10031 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/azimuth.py
--rwxr-xr-x   0        0        0    12212 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/contour_grid.py
--rw-r--r--   0        0        0    38899 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/length_distributions.py
--rw-r--r--   0        0        0    12781 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/line_data.py
--rw-r--r--   0        0        0    11620 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/multi_network.py
--rw-r--r--   0        0        0    49397 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/network.py
--rw-r--r--   0        0        0    30203 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/parameters.py
--rw-r--r--   0        0        0     8431 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/random_sampling.py
--rw-r--r--   0        0        0    19138 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/relationships.py
--rw-r--r--   0        0        0     9713 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/analysis/subsampling.py
--rw-r--r--   0        0        0    38887 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/branches_and_nodes.py
--rw-r--r--   0        0        0    14885 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/cli.py
--rw-r--r--   0        0        0     9873 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/fractopo_utils.py
--rw-r--r--   0        0        0    64569 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/general.py
--rw-r--r--   0        0        0       47 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/tval/__init__.py
--rw-r--r--   0        0        0     4952 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/tval/proximal_traces.py
--rw-r--r--   0        0        0    13453 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/tval/trace_validation.py
--rw-r--r--   0        0        0     9141 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/tval/trace_validation_utils.py
--rw-r--r--   0        0        0    22651 2023-01-16 08:26:40.654521 fractopo-0.5.2/fractopo/tval/trace_validators.py
--rw-r--r--   0        0        0     4183 2023-01-16 08:26:40.662521 fractopo-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    19162 1970-01-01 00:00:00.000000 fractopo-0.5.2/setup.py
--rw-r--r--   0        0        0    19409 1970-01-01 00:00:00.000000 fractopo-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10512 2023-05-09 13:36:02.379897 fractopo-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1062 2022-08-09 06:47:39.850606 fractopo-0.5.3/LICENSE.md
+-rw-r--r--   0        0        0    17836 2023-04-27 05:19:53.007651 fractopo-0.5.3/README.rst
+-rw-r--r--   0        0        0      450 2023-05-09 13:36:02.379897 fractopo-0.5.3/fractopo/__init__.py
+-rw-r--r--   0        0        0       99 2022-12-19 11:21:09.472974 fractopo-0.5.3/fractopo/__main__.py
+-rw-r--r--   0        0        0      157 2022-08-09 06:47:39.860606 fractopo-0.5.3/fractopo/analysis/__init__.py
+-rw-r--r--   0        0        0     6025 2022-12-19 11:21:09.472974 fractopo-0.5.3/fractopo/analysis/anisotropy.py
+-rw-r--r--   0        0        0    10031 2023-01-03 07:14:10.186524 fractopo-0.5.3/fractopo/analysis/azimuth.py
+-rwxr-xr-x   0        0        0    12212 2022-12-19 11:21:09.472974 fractopo-0.5.3/fractopo/analysis/contour_grid.py
+-rw-r--r--   0        0        0    39477 2023-04-19 11:13:49.901023 fractopo-0.5.3/fractopo/analysis/length_distributions.py
+-rw-r--r--   0        0        0    12858 2023-04-19 11:13:49.901023 fractopo-0.5.3/fractopo/analysis/line_data.py
+-rw-r--r--   0        0        0    11618 2023-02-06 08:21:48.478737 fractopo-0.5.3/fractopo/analysis/multi_network.py
+-rw-r--r--   0        0        0    50843 2023-04-19 11:13:49.901023 fractopo-0.5.3/fractopo/analysis/network.py
+-rw-r--r--   0        0        0    30407 2023-04-19 11:13:49.901023 fractopo-0.5.3/fractopo/analysis/parameters.py
+-rw-r--r--   0        0        0     8431 2022-12-19 11:21:09.482974 fractopo-0.5.3/fractopo/analysis/random_sampling.py
+-rw-r--r--   0        0        0    19587 2023-04-19 11:13:49.901023 fractopo-0.5.3/fractopo/analysis/relationships.py
+-rw-r--r--   0        0        0     9712 2023-02-06 08:21:48.478737 fractopo-0.5.3/fractopo/analysis/subsampling.py
+-rw-r--r--   0        0        0    39804 2023-04-19 11:13:49.901023 fractopo-0.5.3/fractopo/branches_and_nodes.py
+-rw-r--r--   0        0        0    15376 2023-04-27 05:19:53.007651 fractopo-0.5.3/fractopo/cli.py
+-rw-r--r--   0        0        0     9852 2023-01-19 11:13:09.859786 fractopo-0.5.3/fractopo/fractopo_utils.py
+-rw-r--r--   0        0        0    67295 2023-04-27 05:19:53.007651 fractopo-0.5.3/fractopo/general.py
+-rw-r--r--   0        0        0       47 2022-08-09 06:47:39.870606 fractopo-0.5.3/fractopo/tval/__init__.py
+-rw-r--r--   0        0        0     4952 2022-12-15 09:18:57.208755 fractopo-0.5.3/fractopo/tval/proximal_traces.py
+-rw-r--r--   0        0        0    14034 2023-04-27 05:19:53.007651 fractopo-0.5.3/fractopo/tval/trace_validation.py
+-rw-r--r--   0        0        0     9348 2023-04-12 15:33:20.703350 fractopo-0.5.3/fractopo/tval/trace_validation_utils.py
+-rw-r--r--   0        0        0    22650 2023-02-06 08:21:48.478737 fractopo-0.5.3/fractopo/tval/trace_validators.py
+-rw-r--r--   0        0        0     4174 2023-05-09 13:36:02.379897 fractopo-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    19749 1970-01-01 00:00:00.000000 fractopo-0.5.3/setup.py
+-rw-r--r--   0        0        0    20013 1970-01-01 00:00:00.000000 fractopo-0.5.3/PKG-INFO
```

### Comparing `fractopo-0.5.2/CHANGELOG.md` & `fractopo-0.5.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,45 @@
 # Changelog
 
+## v0.5.3 (2023-05-09)
+
+### New Features
+
+-   A basic input geometry check is done before starting `tracevalidate` and
+    `network` command-line invocations as suggested in
+    <https://github.com/nialov/fractopo/issues/36>.
+
+-   `joblib` cache settings can be set from environment
+    variables.
+
+### Fixes
+
+-   (branches_and_nodes): Fixed `angle_to_point` by setting distance
+    and similarity checks to more reasonable accuracy.
+
+-   (general): Now crs is added before merging geodataframes in
+    `dissolve_multi_part_traces`
+
+-   (length_distribution): Handle empty arrays in in `powerlaw.Fit`
+    invocations by returning `None` instead of a `Fit` instance.
+
+-   (analysis): Length plot ticks are set explicitly in `setup_ax_for_ld` to
+    avoid differences between Python package versions
+    (<https://github.com/nialov/fractopo/issues/25>).
+
+-   Z-coordinates are now *handled* across `fractopo` i.e. they do not raise
+    errors. However, they are not guaranteed to be kept in results such as
+    validated traces. Reported in
+    <https://github.com/nialov/fractopo/issues/21>.
+
+-   (analysis): Removed function signatures with mutable default arguments.
+
+Full set of changes:
+[`v0.5.2...v0.5.3`](https://github.com/nialov/fractopo/compare/v0.5.2...v0.5.3)
+
 ## v0.5.2 (2023-01-16)
 
 ### New Features
 
 -   Add `plain` keyword argument to output less visualized rose and
     length plots.
```

### Comparing `fractopo-0.5.2/LICENSE.md` & `fractopo-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fractopo-0.5.2/README.rst` & `fractopo-0.5.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 
 |Documentation Status| |PyPI Status| |CI Test| |Conda Test| |Coverage| |Binder| |Zenodo|
 
 ``fractopo`` is a Python library/application that contains tools for
 validating and analysing lineament and fracture trace maps (fracture
 networks). It is targeted at structural geologists working on the
 characterization of bedrock fractures from outcrops and through remote
-sensing. As it is a Python library, the use of ``fractopo`` requires
-prior (Python) programming knowledge.
+sensing. ``fractopo`` is available as a Python library and through a
+command-line interface. As a Python library, the use of ``fractopo``
+requires prior (Python) programming knowledge. However, if used through
+the command-line, using ``fractopo`` only requires general knowledge of
+command-line interfaces in your operating system of choice.
 
 -  `Full Documentation is hosted on Read the Docs
    <https://fractopo.readthedocs.io/en/latest/index.html#full-documentation>`__
 
 .. figure:: https://git.io/JBRuK
    :alt: Overview of fractopo
 
@@ -28,18 +31,14 @@
 
 Installation
 ------------
 
 ``pip`` and ``poetry`` installation only supported for ``linux`` -based
 operating systems. For Windows and MacOS install using `(ana)conda <#conda>`__.
 
-For ``pip`` and ``poetry``: Omit ``--dev`` or ``[dev]`` for regular
-installation. Keep if you want to test/develop or otherwise install all
-development Python dependencies.
-
 conda
 ~~~~~
 
 -  Only (supported) installation method for ``Windows`` and ``MacOS``!
 
 .. code:: bash
 
@@ -55,33 +54,25 @@
 The module is on `PyPI <https://www.pypi.org>`__.
 
 .. code:: bash
 
    # Non-development installation
    pip install fractopo
 
-Or locally for development:
-
-.. code:: bash
-
-   git clone https://github.com/nialov/fractopo
-   cd fractopo
-   # Omit [dev] from end if you do not want installation for development
-   pip install --editable .[dev]
-
 poetry
 ~~~~~~
 
 For usage:
 
 .. code:: bash
 
    poetry add fractopo
 
-For development:
+For development, only ``poetry`` installation of ``fractopo`` is
+supported:
 
 .. code:: bash
 
    git clone https://github.com/nialov/fractopo
    cd fractopo
    poetry install
 
@@ -167,18 +158,19 @@
 
 Trace validation
 ~~~~~~~~~~~~~~~~
 
 Trace data must be validated using ``fractopo`` validation functionality
 before analysis. The topological analysis of lineament & fracture traces
 implemented in ``fractopo`` will not tolerate uncertainty related to the
-topological abutting and snapping relationships between traces.
-Therefore the trace validation is recommended before all analysis using
-``Network``. Trace and target area data can be validated for further
-analysis with a ``Validation`` object.
+topological abutting and snapping relationships between traces. See `the
+documentation <https://fractopo.readthedocs.io/en/latest/validation/errors.html>`__
+for further info on validation error types. Trace validation is
+recommended before all analysis using ``Network``. Trace and target area
+data can be validated for further analysis with a ``Validation`` object:
 
 .. code:: python
 
    from fractopo import Validation
 
    validation = Validation(
        trace_data,
@@ -186,35 +178,33 @@
        name="mytraces",
        allow_fix=True,
    )
 
    # Validation is done explicitly with `run_validation` method
    validated_trace_data = validation.run_validation()
 
-Trace validation is also accessible as a command-line script,
-``fractopo tracevalidate`` which is more straightforward to use than through
-Python calls. Note that all subcommands of ``fractopo`` are available by
-appending them after ``fractopo``.
+Trace validation is also accessible through the ``fractopo``
+command-line interface, ``fractopo tracevalidate`` which is more
+straightforward to use than through Python calls. Note that all
+subcommands of ``fractopo`` are available by appending them after
+``fractopo``.
 
 ``tracevalidate`` always requires the target area that delineates trace
 data.
 
 .. code:: bash
 
-   # Get full up-to-date script help
-
+   # Get full up-to-date command-line interface help
    fractopo tracevalidate --help
 
    # Basic usage example:
-
    fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\
       --output /path/to/validated_trace_data.shp
 
    # Or with automatic saving to validated/ directory
-
    fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\
       --summary
 
 Geometric and topological trace network analysis
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``fractopo`` can be used to extract lineament & fracture size,
@@ -235,15 +225,18 @@
        area_data,
        # Give the Network a name!
        name="mynetwork",
        # Specify whether to determine topological branches and nodes
        # (Required for almost all analysis)
        determine_branches_nodes=True,
        # Specify the snapping distance threshold to define when traces are
-       # snapped to each other
+       # snapped to each other. The unit is the same as the one in the
+       # coordinate system the trace and area data are in.
+       # In default values, fractopo assumes a metric unit and using metric units
+       # is heavily recommended.
        snap_threshold=0.001,
        # If the target area used in digitization is a circle, the knowledge can
        # be used in some analysis
        circular_target_area=True,
        # Analysis on traces can be done for the full inputted dataset or the
        # traces can be cropped to the target area before analysis (cropping
        # recommended)
@@ -254,19 +247,20 @@
    # e.g.,
    network.branch_counts
    network.node_counts
 
    # Plotting is done by plot_ -prefixed methods
    network.plot_trace_lengths()
 
-Network analysis is also available as a command-line script but using the
-Python interface (e.g. ``jupyter lab``, ``ipython``) is recommended when
-analysing ``Networks`` to have access to all available analysis and plotting
-methods. The command-line entrypoint is **opinionated** in what outputs it
-produces. Brief example of command-line entrypoint:
+Network analysis is also available through the ``fractopo`` command-line
+interface but using the Python interface (e.g. ``jupyter lab``,
+``ipython``) is recommended when analysing ``Networks`` to have access
+to all available analysis and plotting methods. The command-line
+entrypoint is **opinionated** in what outputs it produces. Brief example
+of command-line entrypoint:
 
 .. code:: bash
 
    fractopo network /path/to/trace_data.shp /path/to/area_data.shp\
       --name mynetwork
 
    # Use --help to see all up-to-date arguments and help
@@ -358,17 +352,21 @@
 
    -  Plots used in my Thesis were done with an older version of the
       same code used for this plugin.
 
 Development
 -----------
 
--  **Breaking changes are possible and expected.**
+-  The package interfaces are nearing stability and breaking changes in
+   code should for the most part be included in the ``CHANGELOG.md``
+   after 25.4.2023. However, this is not guaranteed until the version
+   reaches v1.0.0. The interfaces of ``Network`` and ``Validation`` can
+   be expected to be the most stable.
 
--  For general contributing guidelines, see `CONTRIBUTING.rst </CONTRIBUTING>`__
+-  For general contributing guidelines, see `CONTRIBUTING.rst </CONTRIBUTING.rst>`__
 
 Development dependencies for ``fractopo`` include:
 
 -  ``poetry``
 
    -  Used to handle Python package dependencies.
```

### Comparing `fractopo-0.5.2/fractopo/analysis/anisotropy.py` & `fractopo-0.5.3/fractopo/analysis/anisotropy.py`

 * *Files identical despite different names*

### Comparing `fractopo-0.5.2/fractopo/analysis/azimuth.py` & `fractopo-0.5.3/fractopo/analysis/azimuth.py`

 * *Files identical despite different names*

### Comparing `fractopo-0.5.2/fractopo/analysis/contour_grid.py` & `fractopo-0.5.3/fractopo/analysis/contour_grid.py`

 * *Files identical despite different names*

### Comparing `fractopo-0.5.2/fractopo/analysis/length_distributions.py` & `fractopo-0.5.3/fractopo/analysis/length_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Wrap powerlaw.Fit for the singular purpose of silencing output.
 
     Silences output both to stdout and stderr.
     """
 
     def __init__(
         self,
-        data,
+        data: np.ndarray,
         discrete=False,
         xmin=None,
         xmax=None,
         verbose=True,
         fit_method="Likelihood",
         estimate_discrete=True,
         discrete_approximation="round",
@@ -165,15 +165,15 @@
             + (" High filter proportion!" if high_filtered else "")
         )
 
         # Set preprocessed lengths back into lengths attribute
         self.lengths = filtered_lengths
 
     @property
-    def automatic_fit(self) -> powerlaw.Fit:
+    def automatic_fit(self) -> Optional[powerlaw.Fit]:
         """
         Get automatic powerlaw Fit.
         """
         if self._automatic_fit is None:
             self._automatic_fit = determine_fit(length_array=self.lengths)
         return self._automatic_fit
 
@@ -279,24 +279,21 @@
             full_length_array_all,
             full_ccm_array_normed_all,
             cut_offs,
         ) = ([], [], [], [], [])
 
         # Iterate over distributions
         for idx, distribution in enumerate(self.distributions):
-
             # Default cut_off is a static value to reduce errors
             # due to very low decimal numbers
             cut_off = general.MINIMUM_LINE_LENGTH
             if automatic_cut_offs:
-
                 # Use automatic cut off determined by powerlaw
                 cut_off = distribution.automatic_fit.xmin
             elif self.cut_offs is not None:
-
                 # Use manual cut offs given as inputs
                 cut_off = self.cut_offs[idx]
 
             assert isinstance(cut_off, float)
 
             # Resolve the lengths and ccm
             (
@@ -465,18 +462,26 @@
             proportions_of_data=proportions,
         )
 
 
 @general.JOBLIB_CACHE.cache
 def determine_fit(
     length_array: np.ndarray, cut_off: Optional[float] = None
-) -> powerlaw.Fit:
+) -> Optional[powerlaw.Fit]:
     """
     Determine powerlaw (along other) length distribution fits for given data.
     """
+    if len(length_array) == 0:
+        return None
+    length_array_max = length_array.max()
+    if cut_off is not None and cut_off >= length_array_max:
+        raise ValueError(
+            f"Expected lower cut_off ({cut_off}) "
+            f"than max of length_array ({length_array_max})."
+        )
     fit = (
         # Use cut-off if it is given
         SilentFit(length_array, xmin=cut_off, verbose=False)
         # Otherwise powerlaw determines it automatically using the data
         if cut_off is not None
         else SilentFit(length_array, verbose=False)
     )
@@ -543,45 +548,43 @@
     use_probability_density_function: bool,
     cut_off: Optional[float] = None,
     fit: Optional[powerlaw.Fit] = None,
     fig: Optional[Figure] = None,
     ax: Optional[Axes] = None,
     fits_to_plot: Tuple[Dist, ...] = (Dist.EXPONENTIAL, Dist.LOGNORMAL, Dist.POWERLAW),
     plain: bool = False,
-) -> Tuple[powerlaw.Fit, Figure, Axes]:
+) -> Tuple[Optional[powerlaw.Fit], Figure, Axes]:
     """
     Plot length distribution and `powerlaw` fits.
 
     If a powerlaw.Fit is not given it will be automatically determined (using
     the optionally given cut_off).
     """
-    if fit is None:
-        # Determine powerlaw, exponential, lognormal fits
-        fit = determine_fit(length_array, cut_off)
-
     if fig is None:
         if ax is None:
             # Create figure, ax
             fig, ax = plt.subplots(figsize=(7, 7))
         else:
             fig_maybe = ax.get_figure()
             assert isinstance(fig_maybe, Figure)
             fig = fig_maybe
 
     assert isinstance(fig, Figure)
     assert isinstance(ax, Axes)
     assert ax is not None
-    assert fit is not None
 
-    if len(length_array) == 0:
-        log.error(
-            "Empty length array passed into plot_distribution_fits. "
-            "Fit and plot will be invalid."
+    if fit is None:
+        # Determine powerlaw, exponential, lognormal fits
+        fit = determine_fit(length_array, cut_off)
+
+    if fit is None:
+        log.warning(
+            f"No length data for plotting with label {label}. Returning fit as None."
         )
-        return fit, fig, ax
+        return None, fig, ax
 
     # Get the x, y data from fit
     # y values are either the complementary cumulative distribution function
     # or the probability density function
     # Depends on use_probability_density_function boolean
     cut_off_is_lower = fit.xmin < length_array.min()
     if not use_probability_density_function:
@@ -717,15 +720,21 @@
         prop={"size": "xx-large"},
         framealpha=0.6,
         facecolor="white",
         # fontsize=40,
     )
 
     # Setup legend line widths larger
-    for lh in lgnd.legendHandles:
+    # TODO: This can be cleaned to use legend_handles only when matplotlib min
+    # version is high enough
+    legend_handles = getattr(lgnd, "legend_handles", None)
+    legend_handles = (
+        legend_handles if legend_handles is not None else lgnd.legendHandles
+    )
+    for lh in legend_handles:
         # lh._sizes = [750]
         lh.set_linewidth(3)
 
 
 def setup_ax_for_ld(
     ax: Axes,
     using_branches: bool,
@@ -764,19 +773,26 @@
     ax.set_ylabel(
         f"{prefix}{function_name} {ccm_unit}",
         # prefix + function_name + ccm_unit,
         **font_props,
     ) if not plain else None
 
     # Setup x and y axis ticks and their labels
-    # plt.xticks(color="black", fontsize="x-large")
-    # plt.yticks(color="black", fontsize="x-large")
-    # plt.tick_params(axis="both", width=1.2)
-    ax.set_xticks(ax.get_xticks(), color="black", fontsize="x-large")
-    ax.set_yticks(ax.get_yticks(), color="black", fontsize="x-large")
+    ax.xaxis.set_ticks(
+        ticks=ax.xaxis.get_ticklocs(),
+        labels=ax.xaxis.get_ticklabels(),
+        color="black",
+        fontsize="x-large",
+    )
+    ax.yaxis.set_ticks(
+        ticks=ax.yaxis.get_ticklocs(),
+        labels=ax.yaxis.get_ticklabels(),
+        color="black",
+        fontsize="x-large",
+    )
     ax.tick_params(axis="both", width=1.2)
 
     # Setup legend
     setup_length_dist_legend(ax=ax) if not plain else None
 
     # Setup grid
     ax.grid(zorder=-10, color="black", alpha=0.25)
@@ -1100,21 +1116,19 @@
 
 def _optimize_cut_offs(
     cut_offs: np.ndarray,
     distributions: List[LengthDistribution],
     fitter: Callable[[np.ndarray, np.ndarray], Tuple[float, float]],
     scorer: Callable[[np.ndarray, np.ndarray], float],
 ) -> Tuple[Polyfit, List[float]]:
-
     # Each length and associated ccm must be collected
     cut_length_arrays, cut_ccm_arrays, proportions = [], [], []
 
     # Iterate over given distributions and cut-offs
     for dist, cut_off in zip(distributions, cut_offs):
-
         # Use LengthDistribution.apply_cut_off to get truncated and normalized
         # length and ccm data
         cut_lengths, cut_ccm = dist.generate_distributions(cut_off=cut_off)
         cut_off_proportion = len(cut_lengths) / len(dist.lengths)
         cut_length_arrays.append(cut_lengths)
         cut_ccm_arrays.append(cut_ccm)
         proportions.append(cut_off_proportion)
@@ -1201,15 +1215,14 @@
     """
     # use powerlaw.Fit to determine ccm
     lengths, ccm = SilentFit(data=lengths, xmin=general.MINIMUM_LINE_LENGTH).ccdf(
         original_data=True
     )
 
     if area_value is not None:
-
         # Normalize with area
         ccm = ccm / area_value
 
     return lengths, ccm
 
 
 def apply_cut_off(
```

### Comparing `fractopo-0.5.2/fractopo/analysis/line_data.py` & `fractopo-0.5.3/fractopo/analysis/line_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Trace and branch data analysis with LineData class abstraction.
 """
 import logging
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Tuple
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import powerlaw
 from matplotlib.axes import Axes
@@ -60,15 +60,15 @@
 
     azimuth_set_ranges: SetRangeTuple
     azimuth_set_names: Tuple[str, ...]
 
     length_set_ranges: SetRangeTuple = ()
     length_set_names: Tuple[str, ...] = ()
 
-    area_boundary_intersects: np.ndarray = np.array([])
+    area_boundary_intersects: np.ndarray = field(default_factory=lambda: np.array([]))
 
     _automatic_fit: Optional[powerlaw.Fit] = None
 
     def __getattr__(self, __name: str) -> Any:
         """
         Overwrite __getattr__ to warn about accessing _line_gdf.
         """
@@ -224,15 +224,15 @@
         Get dictionary of length set counts.
         """
         return parameters.determine_set_counts(
             self.length_set_names, self.length_set_array
         )
 
     @property
-    def automatic_fit(self) -> powerlaw.Fit:
+    def automatic_fit(self) -> Optional[powerlaw.Fit]:
         """
         Get automatic powerlaw Fit.
         """
         if self._automatic_fit is None:
             self._automatic_fit = length_distributions.determine_fit(self.length_array)
         return self._automatic_fit
 
@@ -256,15 +256,15 @@
     @property
     def geometry(self) -> gpd.GeoSeries:
         """
         Get line geometries.
         """
         return self._line_gdf.geometry
 
-    def determine_manual_fit(self, cut_off: float) -> powerlaw.Fit:
+    def determine_manual_fit(self, cut_off: float) -> Optional[powerlaw.Fit]:
         """
         Get manually determined Fit with set cut off.
         """
         return length_distributions.determine_fit(self.length_array, cut_off=cut_off)
 
     def describe_fit(
         self, label: Optional[str] = None, cut_off: Optional[float] = None
@@ -283,15 +283,15 @@
 
     def plot_lengths(
         self,
         label: str,
         use_probability_density_function: bool,
         fit: Optional[powerlaw.Fit] = None,
         plain: bool = False,
-    ) -> Tuple[powerlaw.Fit, Figure, Axes]:
+    ) -> Tuple[Optional[powerlaw.Fit], Figure, Axes]:
         """
         Plot length data with powerlaw fit.
         """
         return length_distributions.plot_distribution_fits(
             self.length_array,
             label=label,
             fit=self.automatic_fit if fit is None else fit,
@@ -360,24 +360,23 @@
             ]
             for azimuth_set_name in self.azimuth_set_names
         }
 
     def plot_azimuth_set_lengths(
         self,
         use_probability_density_function: bool = False,
-    ) -> Tuple[List[powerlaw.Fit], List[Figure], List[Axes]]:
+    ) -> Tuple[List[Optional[powerlaw.Fit]], List[Figure], List[Axes]]:
         """
         Plot azimuth set length distributions with fits.
         """
         # Collect fits and plots
         fits, figs, axes = [], [], []
 
         # Iterate over azimuth set names and corresponding length arrays
         for azimuth_set_name, set_lengths in self.azimuth_set_length_arrays.items():
-
             # Create plot for each set length array
             fit, fig, ax = length_distributions.plot_distribution_fits(
                 set_lengths,
                 label=azimuth_set_name,
                 using_branches=self.using_branches,
                 use_probability_density_function=use_probability_density_function,
             )
```

### Comparing `fractopo-0.5.2/fractopo/analysis/multi_network.py` & `fractopo-0.5.3/fractopo/analysis/multi_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,25 +84,23 @@
         # Collect (set-wise) length distributions for all networks
         distributions: Dict[
             str, Dict[str, length_distributions.LengthDistribution]
         ] = dict()
 
         # Iterate over the networks
         for network in self.networks:
-
             # Name is either the network name or if categorizing by set,
             # the set name
             # Only one LengthDistribution is collected if not using the set,
             # otherwise an amount equal to the amount of azimuth sets
             names = [network.name] if not using_azimuth_sets else set_names
 
             # Collect length distributions (for each set)
             network_distributions = dict()
             for name in names:
-
                 # Label the LengthDistribution with either just network name
                 # or with the name and the azimuth set
                 azimuth_set = name if using_azimuth_sets else None
 
                 # # Use network name or set name as key in second dictionary
                 network_distributions[name] = (
                     network.branch_length_distribution(azimuth_set=azimuth_set)
```

### Comparing `fractopo-0.5.2/fractopo/analysis/network.py` & `fractopo-0.5.3/fractopo/analysis/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Analyse and plot trace map data with Network.
 """
 import logging
 from dataclasses import dataclass, field
 from functools import wraps
 from pathlib import Path
+from textwrap import dedent
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import geopandas as gpd
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import powerlaw
@@ -49,20 +50,22 @@
     EE_branch,
     Number,
     Param,
     SetRangeTuple,
     assign_branch_and_node_colors,
     bool_arrays_sum,
     calc_circle_radius,
+    check_for_z_coordinates,
     crop_to_target_areas,
     determine_boundary_intersecting_lines,
     focus_plot_to_bounds,
     numpy_to_python_type,
     pygeos_spatial_index,
     raise_determination_error,
+    remove_z_coordinates_from_geodata,
     sanitize_name,
     save_fig,
     spatial_index_intersection,
     total_bounds,
     write_geodata,
     write_geodataframe,
 )
@@ -173,20 +176,23 @@
 
     # Branch length
     branch_length_set_names: Tuple[str, ...] = ()
     branch_length_set_ranges: SetRangeTuple = ()
 
     # Branches and nodes
     # ==================
-    branch_gdf: gpd.GeoDataFrame = gpd.GeoDataFrame()
-    node_gdf: gpd.GeoDataFrame = gpd.GeoDataFrame()
+    branch_gdf: gpd.GeoDataFrame = field(default_factory=lambda: gpd.GeoDataFrame())
+    node_gdf: gpd.GeoDataFrame = field(default_factory=lambda: gpd.GeoDataFrame())
 
-    censoring_area: gpd.GeoDataFrame = gpd.GeoDataFrame()
+    censoring_area: gpd.GeoDataFrame = field(default_factory=lambda: gpd.GeoDataFrame())
 
+    # Misc
+    # ==================
     cache_results: bool = True
+    remove_z_coordinates_from_inputs: bool = True
 
     # Private caching attributes
     # ==========================
     _anisotropy: Optional[Tuple[np.ndarray, np.ndarray]] = field(
         default=None, repr=False
     )
     _parameters: Optional[Dict[str, float]] = field(default=None, repr=False)
@@ -239,14 +245,40 @@
                     "Traces must be truncated to the target area"
                     " to perform circular area trace weighting. "
                     "\n(To fix: pass truncate_traces=True.)"
                 )
         # Copy geodataframes instead of using pointers
         # Traces
         self.trace_gdf = self.trace_gdf.copy()
+        has_z_coordinates = check_for_z_coordinates(geodata=self.trace_gdf)
+        if has_z_coordinates:
+            log.warning(
+                dedent(
+                    """
+                Traces inputted into Network contain Z-coordinates.
+                They might not be correct in output geometries
+                and might cause unexpected errors.
+                """
+                ).strip()
+            )
+            if self.remove_z_coordinates_from_inputs:
+                log.warning(
+                    dedent(
+                        """
+                    Z-coordinates will be removed from the input traces and
+                    subsuquently from all outputs because Network input
+                    remove_z_coordinates_from_geodata is True.
+                    """
+                    ).strip()
+                )
+                trace_gdf_without_z_coords = remove_z_coordinates_from_geodata(
+                    geodata=self.trace_gdf
+                )
+                assert isinstance(trace_gdf_without_z_coords, gpd.GeoDataFrame)
+                self.trace_gdf = trace_gdf_without_z_coords
         # Area
         self.area_gdf = self.area_gdf.copy()
         # Branches
         self.branch_gdf = self.branch_gdf.copy()
         # Branches
         self.node_gdf = self.node_gdf.copy()
 
@@ -689,17 +721,15 @@
         -  1 == One intersection
         -  2 == Two intersections
 
         Does not discriminate between which target area (if multiple) the trace
         intersects. Intersection detection based on snap_threshold.
         """
         if self._trace_intersects_target_area_boundary is None:
-
             if self.circular_target_area:
-
                 (
                     intersecting_lines,
                     cuts_through_lines,
                 ) = determine_boundary_intersecting_lines(
                     line_gdf=self.trace_gdf,
                     area_gdf=self.area_gdf,
                     snap_threshold=self.snap_threshold,
@@ -792,28 +822,28 @@
         point_list = self.area_gdf.representative_point().to_list()
         assert isinstance(point_list, list)
         assert all(isinstance(point, Point) for point in point_list)
         return point_list
 
     def trace_lengths_powerlaw_fit(
         self, cut_off: Optional[float] = None
-    ) -> powerlaw.Fit:
+    ) -> Optional[powerlaw.Fit]:
         """
         Determine powerlaw fit for trace lengths.
         """
         return (
             self.trace_data.automatic_fit
             if cut_off is None
             else self.trace_data.determine_manual_fit(cut_off=cut_off)
         )
 
     @requires_topology
     def branch_lengths_powerlaw_fit(
         self, cut_off: Optional[float] = None
-    ) -> powerlaw.Fit:
+    ) -> Optional[powerlaw.Fit]:
         """
         Determine powerlaw fit for branch lengths.
         """
         return (
             self.branch_data.automatic_fit
             if cut_off is None
             else self.branch_data.determine_manual_fit(cut_off=cut_off)
@@ -875,15 +905,15 @@
     @requires_topology
     def plot_branch_lengths(
         self,
         label: Optional[str] = None,
         fit: Optional[powerlaw.Fit] = None,
         use_probability_density_function: bool = False,
         plain: bool = False,
-    ) -> Tuple[powerlaw.Fit, Figure, Axes]:  # type: ignore
+    ) -> Tuple[Optional[powerlaw.Fit], Figure, Axes]:  # type: ignore
         """
         Plot branch length distribution with `powerlaw` fits.
         """
         if label is None:
             label = self.name
         return self.branch_data.plot_lengths(
             label=label,
@@ -1069,24 +1099,24 @@
         """
         if label is None:
             label = self.name
         return self.branch_data.plot_length_set_count(label=label)
 
     def plot_trace_azimuth_set_lengths(
         self,
-    ) -> Tuple[List[powerlaw.Fit], List[Figure], List[Axes]]:
+    ) -> Tuple[List[Optional[powerlaw.Fit]], List[Figure], List[Axes]]:
         """
         Plot trace azimuth set lengths with fits.
         """
         return self.trace_data.plot_azimuth_set_lengths()
 
     @requires_topology
     def plot_branch_azimuth_set_lengths(
         self,
-    ) -> Tuple[List[powerlaw.Fit], List[Figure], List[Axes]]:
+    ) -> Tuple[List[Optional[powerlaw.Fit]], List[Figure], List[Axes]]:
         """
         Plot branch azimuth set lengths with fits.
         """
         return self.branch_data.plot_azimuth_set_lengths()
 
     def contour_grid(
         self,
@@ -1228,15 +1258,14 @@
         errors.
         """
         for topo_name, topo_type, gdf in zip(
             (branches_name, nodes_name),
             ("branches", "nodes"),
             (self.branch_gdf, self.node_gdf),
         ):
-
             topo_path = output_dir_path / (
                 f"{self.name}_{topo_type}.geojson" if topo_name is None else topo_name
             )
             write_geodata(gdf=gdf, path=topo_path, allow_list_column_transform=False)
             log.info(
                 "Wrote topological data to disk.",
                 extra=dict(
```

### Comparing `fractopo-0.5.2/fractopo/analysis/parameters.py` & `fractopo-0.5.3/fractopo/analysis/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,22 +184,20 @@
     # Initialize ternary plot
     fig, ax = plt.subplots(figsize=(6.5, 5.1))
     fig, tax = ternary.figure(ax=ax, scale=scale)
 
     # If only one set of counts is give, we are only plotting a single ternary
     # point
     if len(counts_list) == 1:
-
         # Call plotter with single point
         plotter(counts=counts_list[0], label=labels[0], tax=tax, color=colors[0])
 
         # Decorate plot
         decorator(ax, tax, counts=counts_list[0])
     else:
-
         # Gather points from tuples of counts
         points = [
             counts_to_point(counts=count, scale=100, is_nodes=is_nodes)
             for count in counts_list
         ]
 
         # Filter to X,Y,I or CC,CI,II using get_counts_func
@@ -293,18 +291,15 @@
 
 def counts_to_point(
     counts: Dict[str, int], is_nodes: bool, scale: int = 100
 ) -> Optional[Tuple[float, float, float]]:
     """
     Create ternary point from node_counts.
 
-    The order is important:
-
-      -  For nodes: X, I, Y.
-      -  For branches: CC, II, CI.
+    The order is important: for nodes: X, I, Y and for branches: CC, II, CI.
     """
     if is_nodes:
         # xcount, ycount, icount = _get_xyi_counts(node_counts)
         point_counts = _get_xyi_counts(counts)
     else:
         # cc_count, ci_count, ii_count = _get_branch_class_counts(branch_counts)
         point_counts = _get_branch_class_counts(counts)
@@ -352,15 +347,17 @@
         color = "black"
     # xcount, ycount, icount = _get_xyi_counts(node_counts)
     point = counts_to_point(counts, scale=100, is_nodes=True)
     if point is not None:
         # plot_ternary_point(tax=tax, point=point, marker="o", label=label, color=color)
         # Add shadow to point
         tax.scatter(
-            points=[point], **ternary_point_kwargs(marker="o", s=35), color="black"
+            points=[point],
+            **ternary_point_kwargs(marker="o", s=35),
+            color="black",
         )
         tax.scatter(
             points=[point], **ternary_point_kwargs(marker="o"), label=label, color=color
         )
     tax.legend(
         loc="upper center",
         bbox_to_anchor=(0.5, -0.15),
@@ -638,25 +635,31 @@
     prop = dict(boxstyle="square", facecolor="linen", alpha=1, pad=0.45)
 
     columns_to_plot = [
         param for param in Param if param.value.name in topology_parameters_list[0]
     ]
     figs, axes = [], []
 
-    for column in columns_to_plot:
-        # Figure size setup
-        # TODO: width higher, MAYBE lower bar_width
+    width = 6 + 1 * len(topology_parameters_list) / 6
+    bar_width = 0.6 * len(topology_parameters_list) / 6
 
-        width = 6 + 1 * len(topology_parameters_list) / 6
-        bar_width = 0.6 * len(topology_parameters_list) / 6
+    topology_concat = pd.DataFrame(topology_parameters_list)
+    topology_concat["label"] = labels
+    topology_concat.label = topology_concat.label.astype("category")
 
+    for column in columns_to_plot:
         fig, ax = plt.subplots(figsize=(width, 5.5))
-        topology_concat = pd.DataFrame(topology_parameters_list)
-        topology_concat["label"] = labels
-        topology_concat.label = topology_concat.label.astype("category")
+
+        if all(np.isnan(topology_concat[column.value.name])):
+            figs.append(fig)
+            axes.append(ax)
+            continue
+
+        # Figure size setup
+        # TODO: width higher, MAYBE lower bar_width
 
         # Trying to have sensible widths for bars:
         topology_concat.plot.bar(
             x="label",
             y=column.value.name,
             color=colors,
             zorder=5,
@@ -679,15 +682,17 @@
             fontsize="xx-large",
             bbox=prop,
             transform=ax.transAxes,
             zorder=-10,
         )
         legend = ax.legend()
         legend.remove()
-        if column.value.plot_as_log:
+        if column.value.plot_as_log and not all(
+            topology_concat[column.value.name] <= 0
+        ):
             ax.set_yscale("log")
         fig.subplots_adjust(top=0.85, bottom=0.25, left=0.2)
         locs, xtick_labels = plt.xticks()
         # xtick_labels = ["\n".join(wrap(label.get_text(), 6)) for label in xtick_labels]
         xtick_labels = [fill(label.get_text(), 6) for label in xtick_labels]
         plt.yticks(fontsize="xx-large", color="black")
         plt.xticks(locs, labels, fontsize="xx-large", color="black")
```

### Comparing `fractopo-0.5.2/fractopo/analysis/random_sampling.py` & `fractopo-0.5.3/fractopo/analysis/random_sampling.py`

 * *Files identical despite different names*

### Comparing `fractopo-0.5.2/fractopo/analysis/relationships.py` & `fractopo-0.5.3/fractopo/analysis/relationships.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 from matplotlib.ticker import MaxNLocator
 from shapely import prepared
-from shapely.geometry import LineString, Point
-from shapely.strtree import STRtree
+from shapely.geometry import LineString, MultiPoint, Point
 
 from fractopo.general import (
     X_node,
     Y_node,
     get_trace_endpoints,
     prepare_geometry_traces,
 )
@@ -85,16 +84,16 @@
 
     assert len(node_series_xy) == len(node_types_xy)
 
     if len(set_names) < 2:
         raise ValueError("Expected more than one set to be defined.")
 
     set_combinations = combinations(set_names, 2)
+    additions = []
     for first_set, second_set in set_combinations:
-
         trace_series_two_sets: Tuple[gpd.GeoSeries, gpd.GeoSeries] = (
             trace_series.loc[set_array == first_set],  # type: ignore
             trace_series.loc[set_array == second_set],  # type: ignore
         )
 
         if any(series.shape[0] == 0 for series in trace_series_two_sets):
             log.warning("Expected first_set and second_set to both contain traces.")
@@ -121,15 +120,15 @@
         )
         intersect_series = intersectframe.groupby(["nodeclass", "sets"]).size()
 
         x_count = 0
         y_count = 0
         y_reverse_count = 0
 
-        for item in list(intersect_series.iteritems()):
+        for item in list(intersect_series.items()):
             value = item[1]
             if item[0][0] == X_node:
                 x_count = value
             elif item[0][0] == Y_node:
                 if item[0][1] == (
                     first_set,
                     second_set,
@@ -154,16 +153,18 @@
             "name": label,
             "sets": (first_set, second_set),
             "x": x_count,
             "y": y_count,
             "y-reverse": y_reverse_count,
             "error-count": len(intersectframe.loc[intersectframe.error]),
         }
+        additions.append(addition)
 
-        relations_df = relations_df.append(addition, ignore_index=True)
+    additions_df = pd.DataFrame(additions)
+    relations_df = pd.concat([relations_df, additions_df], ignore_index=True)
     return relations_df
 
 
 def determine_nodes_intersecting_sets(
     trace_series_two_sets: Tuple[gpd.GeoSeries, gpd.GeoSeries],
     set_names_two_sets: Tuple[str, str],
     node_series_xy: gpd.GeoSeries,
@@ -265,17 +266,19 @@
     second_set_prep = prepare_geometry_traces(trace_series_second_set)
     # Creates a rtree from all start- and endpoints of set 1
     # Used in deducting in which set a trace abuts (Y-node)
     first_set_points = list(
         chain(*list(trace_series_first_set.geometry.apply(get_trace_endpoints).values))
     )
     assert all(isinstance(p, Point) for p in first_set_points)
-    first_setpointtree = STRtree(first_set_points)
+    # first_setpointtree = STRtree(first_set_points)
+    first_setpointtree = prepared.prep(MultiPoint(first_set_points))
     node: Point
     node_class: str
+    additions = []
     for node, node_class in zip(node_series_xy_intersects, node_types_xy_intersects):
         assert isinstance(node, Point)
         assert isinstance(node_class, str)
         # for idx, row in intersecting_nodes_frame.iterrows():
         # node = row.geometry
         # c = row.c
 
@@ -306,30 +309,33 @@
             # addition gets overwritten if there are no errors
             addition = {
                 "node": node,
                 "nodeclass": node_class,
                 "sets": set_names_two_sets,
                 "error": True,
             }  # DEBUGGING
+        additions.append(addition)
 
-        intersectframe = intersectframe.append(
-            addition, ignore_index=True
-        )  # Append frame with result
+    additions_df = pd.DataFrame(additions)
+    intersectframe = pd.concat([intersectframe, additions_df], ignore_index=True)
+    # intersectframe = intersectframe.append(
+    #     addition, ignore_index=True
+    # )  # Append frame with result
 
     return intersectframe
 
 
 def determine_intersect(
     node: Point,
     node_class: str,
     l1: bool,
     l2: bool,
     first_set: str,
     second_set: str,
-    first_setpointtree: STRtree,
+    first_setpointtree: prepared.PreparedGeometry,
     buffer_value: float,
 ) -> Dict[str, Union[Point, str, Tuple[str, str], bool]]:
     """
     Determine what intersection the node represents.
 
     TODO: R0912: Too many branches.
     """
@@ -365,16 +371,17 @@
             )
 
     # ALL Y NODE RELATIONS
     elif node_class == "Y":
         if (l1 is True) and (l2 is True):  # It's an y-node between sets
             # p1 == length of list of nodes from first_set traces
             # that intersect with X- or Y-node
-            p1 = len(first_setpointtree.query(node.buffer(buffer_value)))
-            if p1 != 0:  # set 1 ends in set 2
+            # p1 = len(first_setpointtree.query(node.buffer(buffer_value)))
+            p1 = first_setpointtree.intersects(node.buffer(buffer_value))
+            if p1:  # set 1 ends in set 2
                 sets = (first_set, second_set)
             else:  # set 2 ends in set 1
                 sets = (second_set, first_set)
             addition = {
                 "node": node,
                 "nodeclass": node_class,
                 "sets": sets,
@@ -484,16 +491,18 @@
 
                 ax.set_ylim(0, 1.6 * max([row["x"], row["y"], row["y-reverse"]]))
 
                 ax.grid(zorder=-10, color="black", alpha=0.5)
 
                 xticks = [0.3, 0.6]
                 xticklabels = ["X", "Y"]
-                ax.set_xticks(xticks)
-                ax.set_xticklabels(xticklabels)
+                ax.xaxis.set_ticks(
+                    ticks=xticks,
+                    labels=xticklabels,
+                )
 
                 xticklabels_texts = ax.get_xticklabels()
 
                 for xtick in xticklabels_texts:
                     xtick.set_fontweight("bold")
                     xtick.set_fontsize(12)
```

### Comparing `fractopo-0.5.2/fractopo/analysis/subsampling.py` & `fractopo-0.5.3/fractopo/analysis/subsampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,14 @@
     )
 
     # Collect the Series that are chosen
     chosen: general.ParameterListType = []
 
     # Iterate over the DataFrameGroupBy dataframe groups
     for idx, group in enumerate(grouped.values()):
-
         # Skip if not chosen base circle previously
         if idx not in which_idxs:
             continue
 
         chosen_dict = choose_sample_from_group(group=group)
         chosen.append(chosen_dict)
```

### Comparing `fractopo-0.5.2/fractopo/branches_and_nodes.py` & `fractopo-0.5.3/fractopo/branches_and_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import math
 from itertools import chain, compress
 from typing import Dict, List, Optional, Tuple, Union
 
 import geopandas as gpd
 import numpy as np
-import pandas as pd
 from geopandas.sindex import PyGEOSSTRTreeIndex
 from shapely.geometry import (
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
@@ -36,22 +35,24 @@
     EE_branch,
     Error_branch,
     I_node,
     IE_branch,
     II_branch,
     X_node,
     Y_node,
+    check_for_z_coordinates,
     crop_to_target_areas,
     geom_bounds,
     get_trace_coord_points,
     get_trace_endpoints,
     line_intersection_to_points,
     numpy_to_python_type,
     point_to_point_unit_vector,
     pygeos_spatial_index,
+    remove_z_coordinates_from_geodata,
     spatial_index_intersection,
 )
 
 log = logging.getLogger(__name__)
 
 UNARY_ERROR_SIZE_THRESHOLD = 100
 
@@ -199,15 +200,15 @@
 
     """
     if (
         point.intersects(nearest_point)
         or point.intersects(comparison_point)
         or nearest_point.intersects(comparison_point)
     ):
-        raise ValueError("Points in angle_to_point intersect.")
+        raise ValueError("Expected points in angle_to_point not to intersect.")
 
     unit_vector_1 = point_to_point_unit_vector(point=nearest_point, other_point=point)
     unit_vector_2 = point_to_point_unit_vector(
         point=nearest_point, other_point=comparison_point
     )
     dot_product = np.dot(unit_vector_1, unit_vector_2)
     if dot_product > 1 or dot_product < -1:
@@ -264,38 +265,40 @@
     assert isinstance(trace, LineString)
     assert isinstance(point, Point)
     if trace.has_z:
         log.warning("Trace contains z-coordinates. These will be lost.")
     if point.has_z:
         log.warning("Point contains z-coordinates. These will be lost.")
 
-    if any(point.intersects(Point(xy)) for xy in trace.coords):
+    if any(point.intersects(Point(xy)) for xy in list(trace.coords)):
         log.error(
             "Point already matches a coordinate point in trace.\n"
             f"point: {point.wkt}, trace: {trace.wkt}\n"
             "Returning original trace without changes."
         )
         return trace
     trace_point_dists = [
         (idx, trace_point, trace_point.distance(point))
-        for idx, trace_point in enumerate([Point(c) for c in trace.coords])
+        for idx, trace_point in enumerate([Point(c) for c in list(trace.coords)])
     ]
     trace_point_dists = sorted(trace_point_dists, key=lambda vals: vals[2])
     nearest_point = trace_point_dists[0][1]
     nearest_point_idx = trace_point_dists[0][0]
 
     # Determine if to insert or modify trace
     idx, insert = determine_insert_approach(
         nearest_point_idx, trace_point_dists, snap_threshold, point, nearest_point
     )
 
     t_coords = list(trace.coords)
     if not insert:
         t_coords.pop(idx)
-    t_coords.insert(idx, tuple(*point.coords))
+    t_coords.insert(idx, (point.x, point.y)) if not point.has_z else t_coords.insert(
+        idx, (point.x, point.y, point.z)
+    )
     # Closest points might not actually be the points which in between the
     # point is added. Have to use project and interpolate (?)
     # print(t_coords)
     new_trace = LineString(t_coords)
     # print(new_trace.wkt)
     assert new_trace.intersects(point)
     assert isinstance(new_trace, LineString)
@@ -320,24 +323,34 @@
     if nearest_point_idx == 0:
         # It is the first node of linestring
         idx = nearest_point_idx + 1
     elif nearest_point_idx == max(vals[0] for vals in trace_point_dists):
         # It is the last node of linestring
         idx = nearest_point_idx
     else:
-
-        if nearest_point.distance(point) < snap_threshold:
+        nearest_point_distance_to_point = nearest_point.distance(point)
+        if (
+            nearest_point_distance_to_point < snap_threshold
+            or nearest_point.wkt == point.wkt
+            or np.isnan(nearest_point_distance_to_point)
+        ):
             # Replace instead of insert
             insert = False
             idx = nearest_point_idx
         else:
-
             # It is in the middle of the linestring
             points_on_either_side = [
-                (vals, angle_to_point(point, nearest_point, vals[1]))
+                (
+                    vals,
+                    angle_to_point(
+                        point=point,
+                        nearest_point=nearest_point,
+                        comparison_point=vals[1],
+                    ),
+                )
                 for vals in trace_point_dists
                 if vals[0] in (nearest_point_idx - 1, nearest_point_idx + 1)
             ]
 
             points_on_either_side = sorted(
                 points_on_either_side, key=lambda vals: vals[1]
             )
@@ -380,19 +393,18 @@
     >>> additional_snapping_func(trace, idx, additional_snapping).wkt
     'LINESTRING (0 0, 1 0, 2 0, 3 0)'
 
     """
     indexes_to_fix, points_to_add = zip(*additional_snapping)
     if idx not in indexes_to_fix:
         return trace
-    df = pd.DataFrame(
-        {"indexes_to_fix": indexes_to_fix, "points_to_add": points_to_add}
-    )
-    df = df.loc[df["indexes_to_fix"] == idx]
-    for p in df["points_to_add"].values:
+
+    is_idx = np.array(indexes_to_fix) == idx
+    filtered_points = compress(points_to_add, is_idx)
+    for p in filtered_points:
         trace = insert_point_to_linestring(trace, p, snap_threshold=0.001)
     assert isinstance(trace, LineString)
     return trace
 
 
 def snap_traces(
     traces: List[LineString],
@@ -677,15 +689,14 @@
         coord_points = get_trace_coord_points(trace_to_snap_to)[1:-1]
         if len(coord_points) == 0:
             # Cannot snap trace to any point as there are only endpoints
             continue
 
         # Check both trace endpoints
         for endpoint in trace_endpoints:
-
             # Check for already existing snap
             if any(endpoint.intersects(coord_point) for coord_point in coord_points):
                 # Already snapped
                 continue
 
             # Get distances between endpoint in coord_points
             distances: List[float] = [
@@ -749,15 +760,15 @@
     """
     Filter out traces that are not unique.
     """
     assert isinstance(traces, gpd.GeoSeries)
     traces_set = set()
     idxs_to_keep = []
     for idx, geom in enumerate(traces.geometry.values):
-        assert isinstance(geom, LineString)
+        assert isinstance(geom, LineString), geom
 
         # Use a less strict coordinate precision when finding duplicates
         geom_wkt = dumps(geom, rounding_precision=int(-math.log10(snap_threshold)))
         if geom_wkt in traces_set:
             continue
         traces_set.add(geom_wkt)
         idxs_to_keep.append(idx)
@@ -807,15 +818,14 @@
         if len(normal_full_union.geoms) > trace_count and isinstance(
             normal_full_union, MultiLineString
         ):
             return normal_full_union
 
     # Debugging, fail safely
     if size_threshold < UNARY_ERROR_SIZE_THRESHOLD:
-
         log.critical(
             "Expected size_threshold to be higher than 100. Union might be impossible."
         )
 
     # How many parts
     div = int(np.ceil(trace_count / size_threshold))
 
@@ -865,15 +875,14 @@
     Conduct safer_unary_union in parts.
     """
     # Collect partly done unary_unions to part_unions list
     part_unions = []
 
     # Iterate over list of split trace GeoSeries
     for part in split_traces:
-
         # Do unary_union to part
         part_union = part.unary_union
 
         # Do naive check for if unary_union is successful
         if (
             not isinstance(part_union, MultiLineString)
             or len(part_union.geoms) < part.shape[0]
@@ -934,14 +943,23 @@
             len_areas=len(areas),
             snap_threshold=snap_threshold,
             already_clipped=already_clipped,
             allowed_loops=allowed_loops,
         ),
     )
     traces_geosrs: gpd.GeoSeries = traces.geometry
+    if check_for_z_coordinates(geodata=traces_geosrs):
+        log.info(
+            "Removing z-coordinates from trace data before branch and node determination."
+        )
+        traces_without_z_coords = remove_z_coordinates_from_geodata(
+            geodata=traces_geosrs
+        )
+        assert isinstance(traces_without_z_coords, gpd.GeoSeries)
+        traces_geosrs = traces_without_z_coords
 
     # Filter out traces that are not unique by wkt
     # unary_union will fail to take them into account any way
     traces_geosrs = filter_non_unique_traces(
         traces_geosrs, snap_threshold=snap_threshold
     )
 
@@ -952,15 +970,17 @@
         poly
         for poly in areas_geosrs.geometry.values
         if isinstance(poly, (Polygon, MultiPolygon))
     ]
 
     # Collect into lists
     traces_list = [
-        trace for trace in traces.geometry.values if isinstance(trace, LineString)
+        trace
+        for trace in traces_geosrs.geometry.values
+        if isinstance(trace, LineString)
     ]
 
     # Snapping occurs multiple times due to possible side effects of each snap
     loops = 0
     traces_list, any_changes_applied = snap_traces(
         traces_list, snap_threshold, areas=areas_list
     )
@@ -1016,15 +1036,14 @@
     branches = gpd.GeoSeries(
         [b for b in branches_all if b.length > snap_threshold * 1.01],
         crs=traces_geosrs.crs,
     )
 
     # Report and error possibly unary_union failure
     if len(branches_all) < len(traces_geosrs):
-
         # unary_union can fail with too large datasets
         log.critical(
             "Expected more branches than traces. Possible unary_union failure."
         )
 
     # Determine nodes and identities
     nodes, node_identities = node_identities_from_branches(
@@ -1182,15 +1201,14 @@
     # Get spatial index
     endpoints_spatial_index = pygeos_spatial_index(all_endpoints_geoseries)
 
     # Collect resolved nodes
     collected_nodes: Dict[str, Tuple[Point, str]] = dict()
 
     for idx, endpoint in enumerate(all_endpoints):
-
         # Do not resolve nodes that have already been resolved
         if endpoint.wkt in collected_nodes:
             continue
 
         # Determine node identity
         identity = node_identity(
             endpoint=endpoint,
```

### Comparing `fractopo-0.5.2/fractopo/cli.py` & `fractopo-0.5.3/fractopo/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from typer import Typer
 
 from fractopo import __version__
 from fractopo.analysis.network import Network
-from fractopo.general import read_geofile, save_fig
+from fractopo.general import check_for_wrong_geometries, read_geofile, save_fig
 from fractopo.tval.trace_validation import Validation
 from fractopo.tval.trace_validators import SharpCornerValidator, TargetAreaSnapValidator
 
 log = logging.getLogger(__name__)
 
 # Initialize typer command-line app object
 APP = Typer()
@@ -65,27 +65,32 @@
             exists=exists, file_okay=True, dir_okay=False, resolve_path=True, **kwargs
         ),
         nargs=1,
     )
     return path_arguments
 
 
+def _check_for_wrong_geometries_cli(traces: gpd.GeoDataFrame, area: gpd.GeoDataFrame):
+    try:
+        check_for_wrong_geometries(traces=traces, area=area)
+    except TypeError:
+        CONSOLE.print(
+            Text.assemble(
+                "Check that traces and target area arguments are passed in"
+                " the correct order in the command-line (Check with --help)."
+            )
+        )
+        raise
+
+
 def describe_results(
     validated: gpd.GeoDataFrame, error_column: str, console: Console = CONSOLE
 ):
     """
     Describe validation results to stdout.
-
-    E.g.
-
-    >>> gdf = gpd.GeoDataFrame({"VALIDATION_ERRORS": [("V NODE",)]})
-    >>> describe_results(gdf, "VALIDATION_ERRORS")
-    Out of 1 traces, 1 were invalid.
-    There were 1 error types. These were:
-    V NODE
     """
     error_count = sum(len(val) != 0 for val in validated[error_column].values)
     error_types = {
         c for c in chain(*validated[error_column].to_list()) if isinstance(c, str)
     }
     trace_count = validated.shape[0]
     count_string = f"Out of {trace_count} traces, {error_count} were invalid."
@@ -93,29 +98,30 @@
     type_color = "yellow"
     for error_type in error_types:
         type_string += error_type + "\n"
         if SharpCornerValidator.ERROR not in error_type:
             type_color = "bold red"
     count_color = "bold red" if error_count / trace_count > 0.05 else "yellow"
     console.print(Text.assemble((count_string, count_color)))
-    console.print(Text.assemble((type_string, type_color)))
+    if len(error_types) > 0:
+        console.print(Text.assemble((type_string, type_color)))
 
 
-def make_output_dir(trace_path: Path) -> Path:
+def make_output_dir(base_path: Path) -> Path:
     """
     Make timestamped output dir.
     """
     localtime = time.localtime()
     tm_min = localtime.tm_min
     hour = localtime.tm_hour
     day = localtime.tm_mday
     month = localtime.tm_mon
     year = localtime.tm_year
     timestr = "_".join(map(str, [day, month, year, hour, tm_min]))
-    output_dir = trace_path.parent / f"validated_{timestr}"
+    output_dir = base_path / f"validated_{timestr}"
     if not output_dir.exists():
         output_dir.mkdir()
     return output_dir
 
 
 def rich_table_from_parameters(parameters: Dict[str, float]) -> Table:
     """
@@ -162,15 +168,18 @@
         resolve_path=True,
         help=AREA_FILE_HELP,
     ),
     allow_fix: bool = typer.Option(
         True,
         "--allow-fix",
         "--fix",
-        help="Allow the direct modification of trace file to fix errors.",
+        help=(
+            "Enable the direct modification of output trace file to fix errors. "
+            "Input files will not be modified unless specified as the --output target."
+        ),
     ),
     summary: bool = typer.Option(True, help="Print summary of validation results."),
     snap_threshold: float = typer.Option(
         0.001,
         help="Distance threshold used to estimate whether e.g. a trace abuts another.",
     ),
     output: Optional[Path] = typer.Option(
@@ -193,14 +202,15 @@
     traces: gpd.GeoDataFrame = read_geofile(trace_file)
     areas: gpd.GeoDataFrame = read_geofile(area_file)
     if not all(isinstance(val, gpd.GeoDataFrame) for val in (traces, areas)):
         raise TypeError(
             "Expected trace and area files to be readable as GeoDataFrames."
         )
 
+    _check_for_wrong_geometries_cli(traces=traces, area=areas)
     log.info(f"Validating traces: {trace_file} area: {area_file}.")
     # Get input crs
     input_crs = traces.crs
 
     # Validate
     validation = Validation(
         traces,
@@ -230,25 +240,21 @@
     # Get input driver to use as save driver
     with fiona.open(trace_file) as open_trace_file:
         assert open_trace_file is not None
         save_driver = open_trace_file.driver
 
     # Resolve output if not explicitly given
     if output is None:
-        output_dir = make_output_dir(trace_file)
-        output_path = (
-            trace_file.parent
-            / output_dir
-            / f"{trace_file.stem}_validated{trace_file.suffix}"
-        )
+        output_dir = make_output_dir(Path(".")).resolve()
+        output_path = output_dir / f"{trace_file.stem}_validated{trace_file.suffix}"
         CONSOLE.print(
             Text.assemble(
                 (
-                    f"Generated output directory at {output_dir}"
-                    f"\nwhere validated output will be saved at {output_path}.",
+                    f"Generated output directory at {output_dir} "
+                    f"where validated output will be saved in file {output_path.name}.",
                     "blue",
                 )
             )
         )
     else:
         output_path = output
 
@@ -312,18 +318,21 @@
     network_name = name if name is not None else area_file.stem
 
     CONSOLE.print(
         Text.assemble(
             "Performing network analysis of ", (network_name, "bold green"), "."
         )
     )
+    traces = gpd.read_file(trace_file)
+    areas = gpd.read_file(area_file)
+    _check_for_wrong_geometries_cli(traces=traces, area=areas)
 
     network = Network(
-        trace_gdf=read_geofile(trace_file),
-        area_gdf=read_geofile(area_file),
+        trace_gdf=traces,
+        area_gdf=areas,
         snap_threshold=snap_threshold,
         determine_branches_nodes=determine_branches_nodes,
         name=network_name,
         circular_target_area=circular_target_area,
         truncate_traces=truncate_traces,
         censoring_area=read_geofile(censoring_area)
         if censoring_area is not None
```

### Comparing `fractopo-0.5.2/fractopo/fractopo_utils.py` & `fractopo-0.5.3/fractopo/fractopo_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,17 @@
     @staticmethod
     def conditional_linemerge(
         first: LineString, second: LineString, tolerance: float, buffer_value: float
     ) -> Union[None, LineString]:
         """
         Conditionally merge two LineStrings (first and second).
 
-        Merge occurs if:
-            1. Their endpoints are within buffer_value of each other.
-            2. Their total orientations are within tolerance (degrees) of each
-               other.
+        Merge occurs if 1) their endpoints are within buffer_value of each
+        other and 2) their total orientations are within tolerance (degrees) of
+        each other.
 
         Merges by joining their coordinates. The endpoint
         (that is within buffer_value of endpoint of first) of the second
         LineString is trimmed from the resulting coordinates.
 
         E.g. with merging:
```

### Comparing `fractopo-0.5.2/fractopo/general.py` & `fractopo-0.5.3/fractopo/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import pygeos
 import sklearn.metrics as sklm
 from geopandas.sindex import PyGEOSSTRTreeIndex
 from joblib import Memory
 from matplotlib import patheffects as path_effects
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
-from shapely import prepared
+from shapely import prepared, wkb
 from shapely.affinity import scale
 from shapely.geometry import (
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
@@ -92,19 +92,23 @@
 PointTuple = Tuple[float, float]
 Number = Union[float, int]
 ParameterValuesType = Dict[str, Union[float, int, str]]
 ParameterListType = List[ParameterValuesType]
 
 MINIMUM_LINE_LENGTH = 1e-18
 
-DEFAULT_FRACTOPO_CACHE_PATH = Path(".fractopo_cache")
+DEFAULT_FRACTOPO_CACHE_PATH = Path(".cache/fractopo")
 
 JOBLIB_CACHE = Memory(
-    DEFAULT_FRACTOPO_CACHE_PATH,
-    verbose=int(os.environ.get("JOBLIB_CACHE_VERBOSITY", 0)),
+    os.environ.get("FRACTOPO_CACHE_PATH", DEFAULT_FRACTOPO_CACHE_PATH)
+    # Disk caching is disabled in pytest execution by setting an environment
+    # variable FRACTOPO_DISABLE_CACHE to a non-zero string (i.e. "1") However,
+    # it can be enabled even in tests by setting FRACTOPO_DISABLE_CACHE to 0
+    if os.environ.get("FRACTOPO_DISABLE_CACHE") in (None, "0") else None,
+    verbose=int(os.environ.get("FRACTOPO_JOBLIB_CACHE_VERBOSITY", 0)),
 )
 
 
 @dataclass
 class ProcessResult:
 
     """
@@ -736,15 +740,14 @@
     # spatial_index = traces.geometry.sindex
     try:
         spatial_index = pygeos_spatial_index(traces.geometry)
     except TypeError:
         spatial_index = None
     for idx, geom in enumerate(traces.geometry.values):
         if not isinstance(geom, LineString):
-
             # Intersections and endpoints are not defined for
             # MultiLineStrings
             intersect_nodes.append(())
             endpoint_nodes.append(())
             continue
 
         # Get trace candidates for intersection
@@ -811,26 +814,24 @@
     p_to_keep = [True] * len(inter)
 
     # Iterate over the trace candidates
     for trace_candidate in trace_candidates.geometry.values:
         candidate_endpoints = get_trace_endpoints(trace_candidate)
         for ce in candidate_endpoints:
             for ge in geom_endpoints:
-
                 # First check: is the candidate endpoint close to the geom endpoint
                 candidate_endpoint_is_close_to_geom_endpoint = np.isclose(
                     ce.distance(ge), 0, atol=1e-4
                 )
                 # If not, keep it in `inter`
                 if not candidate_endpoint_is_close_to_geom_endpoint:
                     continue
 
                 # Enumerate over the valid intersection points
                 for idx, p in enumerate(inter):
-
                     # If the current valid intersection point is already set
                     # for removal, continue the loop to the next
                     if not p_to_keep[idx]:
                         continue
                     # Second check: is the `geom` LineString endpoint close to
                     # the intersection point `p`. If yes, mark the intersection
                     # point for removal from `interl`
@@ -983,15 +984,14 @@
         # current trace by using the idx.
         other_nodes_geoseries: gpd.GeoSeries = flattened_nodes_geoseries.loc[
             [idx_reference != idx for idx_reference in flattened_idx_reference]
         ]
 
         # Iterate over the actual Points of the current trace
         for _, point in enumerate(points):
-
             # Get node candidates from spatial index
             node_candidates_idx = spatial_index_intersection(
                 nodes_geoseries_sindex,
                 geom_bounds(
                     safe_buffer(
                         point, snap_threshold * snap_threshold_error_multiplier * 10
                     )
@@ -1378,15 +1378,17 @@
         for new_geom in as_linestrings:
             # Do not modify mls_traces inplace
             new_row = row.copy()
             new_row[GEOMETRY_COLUMN] = new_geom
             dissolved_rows.append(new_row)
 
     # Merge with ls_traces
-    dissolved_traces = pd.concat([ls_traces, gpd.GeoDataFrame(dissolved_rows)])
+    dissolved_rows_gdf = gpd.GeoDataFrame(dissolved_rows, crs=ls_traces.crs)
+    assert ls_traces.crs == dissolved_rows_gdf.crs
+    dissolved_traces = pd.concat([ls_traces, dissolved_rows_gdf])
     assert isinstance(dissolved_traces, gpd.GeoDataFrame)
 
     if not all(isinstance(val, LineString) for val in dissolved_traces.geometry.values):
         raise TypeError("Expected all LineStrings in dissolved_traces.")
     return dissolved_traces
 
 
@@ -1530,14 +1532,18 @@
     """
     Get total bounds of geodataset.
 
     >>> geodata = gpd.GeoSeries([Point(-10, 10), Point(10, 10)])
     >>> total_bounds(geodata)
     (-10.0, 10.0, 10.0, 10.0)
     """
+    if geodata.empty or all(
+        geom is None or geom.is_empty for geom in geodata.geometry.values
+    ):
+        return tuple([np.nan] * 4)
     bounds = geodata.total_bounds
     if not len(bounds) == 4:
         raise ValueError(
             f"Expected total_bounds to return an array of length 4: {bounds}."
         )
     return bounds[0], bounds[1], bounds[2], bounds[3]
 
@@ -1735,21 +1741,24 @@
     Create unit vector from point to other point.
 
     >>> point = Point(0, 0)
     >>> other_point = Point(1, 1)
     >>> point_to_point_unit_vector(point, other_point)
     array([0.70710678, 0.70710678])
     """
-    x1, y1 = tuple(*point.coords)
-    x2, y2 = tuple(*other_point.coords)
+    x1, y1 = point.x, point.y
+    x2, y2 = other_point.x, other_point.y
     if any(np.isnan([x1, y1, x2, y2])):
-        raise ValueError(
-            f"Expected no nan values in point_to_point_unit_vector: {x1, y1, x2, y2}"
-        )
+        raise ValueError(f"Expected no nan values: {x1, y1, x2, y2}")
     vector = np.array([x2 - x1, y2 - y1])
+    if np.isclose(point.distance(other_point), 0.0, rtol=1e-15, atol=1e-15):
+        logging.info(
+            "Cannot compute unit vector between points due to close approximity."
+        )
+        return np.array([np.nan, np.nan])
     normed_vector = vector / np.linalg.norm(vector)
     assert isinstance(normed_vector, np.ndarray)
     return normed_vector
 
 
 def raise_determination_error(
     attribute: str,
@@ -1785,41 +1794,37 @@
     Returns result as a list where the error is appended when execution fails.
     """
     # Collect results into a list
     collect_results: List[ProcessResult] = []
 
     # multiprocessing!
     with ProcessPoolExecutor() as executor:
-
         keyword_arguments = list(keyword_arguments) * (repeats + 1)
 
         # Iterate over invalids. submit as tasks
         futures = {
             executor.submit(function_to_call, keyword_arg): keyword_arg
             for keyword_arg in keyword_arguments
         }
 
         # Collect all tasks as they complete
         # Will not be in same order as submitted
         for future in as_completed(futures):
-
             identifier = arguments_identifier(futures[future])
             # If execution critically fails it will be caught and logged
             try:
-
                 # Get result from Future
                 # This will throw an error (if it happened in process)
                 result = future.result()
 
                 # Collect result
                 collect_results.append(
                     ProcessResult(identifier=identifier, result=result, error=False)
                 )
             except Exception as exc:
-
                 # Catch and log critical failures
                 log.error(f"Process exception with {futures[future]}:\n\n" f"{exc}")
                 collect_results.append(
                     ProcessResult(identifier=identifier, error=True, result=exc)
                 )
     return collect_results
 
@@ -2014,15 +2019,14 @@
     non_dupl_columns = remove_duplicate_caseinsensitive_columns(geodataframe.columns)
     fid_col = "fid"
     for column in geodataframe.columns:
         if column not in non_dupl_columns:
             # print(f"Dropping column: {column}")
             geodataframe.drop(columns=[column], inplace=True)
         if column.lower() == fid_col:
-
             # Remove fid columns
             # print(f"Dropping column: {column} due to case-insensitive match to fid.")
             geodataframe.drop(columns=[column], inplace=True)
     error_base = "Failed to write {} as {}."
     try:
         geodataframe.to_file(results_dir / f"{name}.gpkg", driver="GPKG")
     except Exception:
@@ -2035,12 +2039,64 @@
         shp_dir = results_dir / f"{name}_as_shp"
         shp_dir.mkdir(exist_ok=False)
         geodataframe.to_file(shp_dir / f"{name}.shp")
     except Exception:
         log.error(error_base.format(name, "ESRI Shapefile"), exc_info=True)
 
 
+def check_for_z_coordinates(geodata: Union[gpd.GeoDataFrame, gpd.GeoSeries]) -> bool:
+    """
+    Check if geopandas data contains Z-coordinates.
+    """
+    return any(geom.has_z for geom in geodata.geometry.values if hasattr(geom, "has_z"))
+
+
+def remove_z_coordinates_from_geodata(
+    geodata: Union[gpd.GeoDataFrame, gpd.GeoSeries]
+) -> Union[gpd.GeoDataFrame, gpd.GeoSeries]:
+    """
+    Remove Z-coordinates from geometries in geopandasgeodata.
+    """
+    geodata_without_z = geodata.copy()
+    geodata_without_z_geometries = geodata_without_z.geometry.apply(
+        remove_z_coordinates
+    )
+    if isinstance(geodata_without_z, gpd.GeoDataFrame):
+        geodata_without_z["geometry"] = geodata_without_z_geometries
+    else:
+        geodata_without_z = geodata_without_z_geometries
+
+    assert isinstance(geodata_without_z, (gpd.GeoDataFrame, gpd.GeoSeries))
+    return geodata_without_z
+
+
+def remove_z_coordinates(geometry: Union[BaseGeometry, BaseMultipartGeometry]) -> Any:
+    """
+    Remove z-coordinates from a geometry.
+
+    A ``shapely`` geometry should be provided. Output will always be the same
+    type of geometry with the z-coordinates removed.
+
+    :param geometry: Shapely geometry
+    :return: Shapely geometry with the same geometry type
+    """
+    return wkb.loads(wkb.dumps(geometry, output_dimension=2))
+
+
 def sanitize_name(name: str) -> str:
     """
     Return only alphanumeric parts of name string.
     """
     return "".join(filter(str.isalnum, name))
+
+
+def check_for_wrong_geometries(traces: gpd.GeoDataFrame, area: gpd.GeoDataFrame):
+    """
+    Check that traces are line geometries and area contains area geometries.
+    """
+    accepted_line_types = (LineString, MultiLineString)
+    accepted_area_types = (Polygon, MultiPolygon)
+    for name, geoms, accepted_types in zip(
+        ("traces", "area"), (traces, area), (accepted_line_types, accepted_area_types)
+    ):
+        if not all(isinstance(geom, accepted_types) for geom in geoms.geometry.values):
+            raise TypeError(f"Expected {name} to contain only any of {accepted_types}.")
```

### Comparing `fractopo-0.5.2/fractopo/tval/proximal_traces.py` & `fractopo-0.5.3/fractopo/tval/proximal_traces.py`

 * *Files identical despite different names*

### Comparing `fractopo-0.5.2/fractopo/tval/trace_validation.py` & `fractopo-0.5.3/fractopo/tval/trace_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,27 @@
 
 Create Validation objects from traces and their target areas to validate
 the traces for further analysis (``fractopo.analysis.network.Network``).
 """
 import logging
 from dataclasses import dataclass
 from itertools import chain
+from textwrap import dedent
 from typing import Any, List, Optional, Set, Tuple
 
 import geopandas as gpd
 from geopandas.sindex import PyGEOSSTRTreeIndex
 from shapely.geometry import LineString, MultiLineString, Point
 
-from fractopo.general import determine_general_nodes, is_empty_area
+from fractopo.general import (
+    check_for_z_coordinates,
+    determine_general_nodes,
+    is_empty_area,
+    remove_z_coordinates_from_geodata,
+)
 from fractopo.tval import trace_validators
 from fractopo.tval.trace_validation_utils import determine_trace_candidates
 from fractopo.tval.trace_validators import (
     ALL_VALIDATORS,
     MAJOR_ERRORS,
     MAJOR_VALIDATORS,
     VALIDATION_REQUIRES_NODES,
@@ -70,17 +76,29 @@
 
         self.ERROR_COLUMN_TRUNC = (
             self.ERROR_COLUMN[0:10]
             if len(self.ERROR_COLUMN) > 9
             else self.ERROR_COLUMN[0 : len(self.ERROR_COLUMN)]
         )
 
-        # Validate trace and area inputs
-        # for geom in self.area.geometry.values:
-        #     if not isinstance(geom, Polygon)
+        if check_for_z_coordinates(geodata=self.traces):
+            log.warning(
+                dedent(
+                    """
+                Traces inputted into Validation contain Z-coordinates. They
+                will be removed from the input traces and subsuquently from all
+                outputs.
+                """
+                ).strip()
+            )
+            traces_with_removed_z = remove_z_coordinates_from_geodata(
+                geodata=self.traces
+            )
+            assert isinstance(traces_with_removed_z, gpd.GeoDataFrame)
+            self.traces = traces_with_removed_z
 
     def set_general_nodes(self):
         """
         Set _intersect_nodes and _endpoint_nodes attributes.
         """
         self._intersect_nodes, self._endpoint_nodes = determine_general_nodes(
             self.traces
@@ -204,28 +222,26 @@
             log.error(f"No traces within target area with name: {self.name}.")
             empty_gdf: gpd.GeoDataFrame = self.traces.copy()
             return empty_gdf
 
         all_errors: List[List[str]] = []
         all_geoms: List[LineString] = []
         for idx, geom in enumerate(self.traces.geometry.values):
-
             # Collect errors from each validator for each geom
             current_errors: List[str] = []
 
             # If geom contains validation error that will cause issues in later
             # validation -> ignore the geom and break out of validation loop
             # for current geom.
             ignore_geom: bool = False
             trace_candidates: Optional[gpd.GeoSeries] = None
 
             # validation loop
             for validator in validators:
                 if ignore_geom:
-
                     # Break out of validation loop. See above comments
                     break
 
                 if isinstance(geom, LineString) and not geom.is_empty:
                     # Some conditionals to avoid try-except loop
                     # trace candidates that are nearby to geom based on spatial index
                     trace_candidates = (
```

### Comparing `fractopo-0.5.2/fractopo/tval/trace_validation_utils.py` & `fractopo-0.5.3/fractopo/tval/trace_validation_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,16 +77,24 @@
 
     # Iterate over list of LineStrings
     for ls in mls_geoms:
         all_segments.extend(
             segmentize_linestring(ls, snap_threshold * overlap_detection_multiplier)
         )
     for start, end in all_segments:
-        if within_bounds(*start, min_x, min_y, max_x, max_y) and within_bounds(
-            *end, min_x, min_y, max_x, max_y
+        if within_bounds(
+            x=start[0], y=start[1], min_x=min_x, min_y=min_y, max_x=max_x, max_y=max_y
+        ) and within_bounds(
+            x=end[0],
+            y=end[1],
+            min_x=min_x,
+            min_y=min_y,
+            max_x=max_x,
+            max_y=max_y
+            # *end, min_x, min_y, max_x, max_y
         ):
             ls = LineString([start, end])
             if ls.length > snap_threshold * overlap_detection_multiplier and ls.within(
                 buffered_linestring
             ):
                 return True
     return False
```

### Comparing `fractopo-0.5.2/fractopo/tval/trace_validators.py` & `fractopo-0.5.3/fractopo/tval/trace_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,14 @@
 
         """
         if len(trace_candidates) == 0:
             return True
 
         endpoints = get_trace_endpoints(geom)
         for endpoint in endpoints:
-
             # Check that if endpoint is well snapped to one trace another trace
             # won't have chance to cause a validation error (false positive).
             if any(trace_candidates.distance(endpoint) < snap_threshold):
                 continue
             trace: LineString
             for trace in trace_candidates.geometry.values:
                 if (
```

### Comparing `fractopo-0.5.2/pyproject.toml` & `fractopo-0.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractopo"
-version = "0.5.2"
+version = "0.5.3"
 description = "Fracture Network Analysis"
 authors = ["nialov <nikolasovaskainen@gmail.com>"]
 readme = "README.rst"
 license = "MIT"
 # Make sure hyphens/underscores are correct in urls
 homepage = "https://github.com/nialov/fractopo"
 repository = "https://github.com/nialov/fractopo"
@@ -35,15 +35,15 @@
 
 # Changes here should be kept in sync with ./environment.yml
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click = "*"
 geopandas = ">=0.11.1,<1.0.0"
 joblib = ">=1.2.0,<2.0.0"
-matplotlib = "*"
+matplotlib = ">=3.5.3,<4.0.0"
 numpy = "*"
 pandas = ">=1.3,<2.0.0"
 powerlaw = "*"
 pygeos = ">=0.13.0,<1.0.0"
 python-ternary = "*"
 rich = ">=11.0.0"
 scikit-learn = "*"
@@ -85,15 +85,15 @@
 json5 = "*"
 jupyterlab = "*"
 nbstripout = "^0.6.1"
 nox = "*"
 pre-commit = "*"
 pyinstrument = "*"
 pytest = "*"
-pytest-regressions = "==2.2.0"
+pytest-regressions = ">=2.2.0,<3.0.0"
 toml = "*"
 
 [tool.poetry.extras]
 coverage = ["coverage", "coverage-badge"]
 docs = [
     "sphinx",
     "sphinx-rtd-theme",
@@ -122,33 +122,34 @@
 addopts = "--doctest-modules"
 doctest_optionflags =[
     "NUMBER",
     "NORMALIZE_WHITESPACE",
     ]
 
 filterwarnings =[
-    "ignore:invalid value encountered in true_divide:RuntimeWarning",
-    "ignore:The Shapely GEOS version :UserWarning",
-    "ignore:invalid value encountered in double_scalars:RuntimeWarning",
-    "ignore:Mean of empty slice:RuntimeWarning",
-    "ignore:Degrees of freedom :RuntimeWarning",
-    "ignore:divide by zero encountered in double_scalars:RuntimeWarning",
-    "ignore:This method will be removed in future versions:DeprecationWarning",
-    "ignore:The default dtype for empty Series will be:DeprecationWarning",
-    "ignore:All-NaN slice encountered:RuntimeWarning",
+    "error",
+    "ignore:The Shapely:UserWarning:geopandas",
+    "ignore:The shapely GEOS version:UserWarning:pygeos",
+    "ignore:No data for colormapping provided:UserWarning",
+    "ignore:invalid value encountered in divide:RuntimeWarning:powerlaw",
+    "ignore:divide by zero encountered in divide:RuntimeWarning:powerlaw",
+    "ignore:The behavior of :FutureWarning",
+    "ignore:In a future version, :FutureWarning",
+    "ignore:invalid value encountered in intersection:RuntimeWarning:pygeos",
+    "ignore:More than 20 figures have been opened:RuntimeWarning",
     ]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 src_paths = ["fractopo", "tests"]
 
 [tool.pylint.master]
 fail-under = "9.5"
-ignore = [".fractopo_cache", "examples"]
+ignore = ["examples"]
 
 [tool.pylint.report]
 output-format = "text"
 
 [tool.pylint.messages_control]
 max-line-length = 100
 disable = [
```

### Comparing `fractopo-0.5.2/setup.py` & `fractopo-0.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click',
  'geopandas>=0.11.1,<1.0.0',
  'joblib>=1.2.0,<2.0.0',
- 'matplotlib',
+ 'matplotlib>=3.5.3,<4.0.0',
  'numpy',
  'pandas>=1.3,<2.0.0',
  'powerlaw',
  'pygeos>=0.13.0,<1.0.0',
  'python-ternary',
  'rich>=11.0.0',
  'scikit-learn',
@@ -36,17 +36,17 @@
  'typecheck': ['mypy']}
 
 entry_points = \
 {'console_scripts': ['fractopo = fractopo.__main__:APP']}
 
 setup_kwargs = {
     'name': 'fractopo',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'Fracture Network Analysis',
-    'long_description': 'fractopo\n========\n\n|Documentation Status| |PyPI Status| |CI Test| |Conda Test| |Coverage| |Binder| |Zenodo|\n\n``fractopo`` is a Python library/application that contains tools for\nvalidating and analysing lineament and fracture trace maps (fracture\nnetworks). It is targeted at structural geologists working on the\ncharacterization of bedrock fractures from outcrops and through remote\nsensing. As it is a Python library, the use of ``fractopo`` requires\nprior (Python) programming knowledge.\n\n-  `Full Documentation is hosted on Read the Docs\n   <https://fractopo.readthedocs.io/en/latest/index.html#full-documentation>`__\n\n.. figure:: https://git.io/JBRuK\n   :alt: Overview of fractopo\n\n   Overview of fractopo\n\n.. figure:: /docs_src/imgs/fractopo-visualizations.png\n   :alt: Data visualization\n\n   Visualisation of ``fractopo`` data. ``fractopo`` analyses the trace\n   data that can e.g. be digitized from drone orthophotographs\n   (=fractures) or from digital elevation models (=lineaments). The\n   displayed branches and nodes are extracted with ``fractopo``.\n\nInstallation\n------------\n\n``pip`` and ``poetry`` installation only supported for ``linux`` -based\noperating systems. For Windows and MacOS install using `(ana)conda <#conda>`__.\n\nFor ``pip`` and ``poetry``: Omit ``--dev`` or ``[dev]`` for regular\ninstallation. Keep if you want to test/develop or otherwise install all\ndevelopment Python dependencies.\n\nconda\n~~~~~\n\n-  Only (supported) installation method for ``Windows`` and ``MacOS``!\n\n.. code:: bash\n\n   # Create new environment for fractopo (recommended but optional)\n   conda env create fractopo-env\n   conda activate fractopo-env\n   # Available on conda-forge channel\n   conda install -c conda-forge fractopo\n\npip\n~~~\n\nThe module is on `PyPI <https://www.pypi.org>`__.\n\n.. code:: bash\n\n   # Non-development installation\n   pip install fractopo\n\nOr locally for development:\n\n.. code:: bash\n\n   git clone https://github.com/nialov/fractopo\n   cd fractopo\n   # Omit [dev] from end if you do not want installation for development\n   pip install --editable .[dev]\n\npoetry\n~~~~~~\n\nFor usage:\n\n.. code:: bash\n\n   poetry add fractopo\n\nFor development:\n\n.. code:: bash\n\n   git clone https://github.com/nialov/fractopo\n   cd fractopo\n   poetry install\n\nUsage\n-----\n\n``fractopo`` has two main use cases:\n\n1. Validation of lineament & fracture trace data\n2. Analysis of lineament & fracture trace data\n\nValidation is done to make sure the data is valid for the analysis and\nis crucial as analysis cannot take into account different kinds of\ngeometric and topological inconsistencies between the traces.\nCapabilities and associated guides are inexhaustively listed in the\ntable below.\n\n========================================================  ======================\nFunctionality                                             Tutorial/Guide/Example\n========================================================  ======================\nValidation of trace data                                  `Validation 1`_; `Validation 2`_\nVisualize trace map data                                  `Visualizing`_\nTopological branches and nodes                            `Network`_; `Topological`_\nTrace and branch length distributions                     `Length-distributions`_\nOrientation rose plots                                    `Orientation 1`_; `Orientation 2`_\nPlot topological ternary node and branch proportions      `Proportions`_\nCross-cutting and abutting relationships                  `Relationships 1`_; `Relationships 2`_;\nGeometric and topological fracture network parameters     `Parameters`_\nContour grids of fracture network parameters              `Contour-grids`_\nMulti-scale length distributions                          `Multi-scale`_\n========================================================  ======================\n\n.. _Validation 1:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_validation_1.html\n.. _Validation 2:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_validation_2.html\n.. _Visualizing:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Visualizing-trace-map-data\n.. _Network:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Network\n.. _Topological:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_branches_and_nodes.html#sphx-glr-auto-examples-plot-branches-and-nodes-py\n.. _Length-distributions:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Length-distributions\n.. _Orientation 1:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Rose-plots\n.. _Orientation 2:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_rose_plot.html#sphx-glr-auto-examples-plot-rose-plot-py\n.. _Proportions:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Node-and-branch-proportions\n.. _Relationships 1:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Crosscutting-and-abutting-relationships\n.. _Relationships 2:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_azimuth_set_relationships.html#sphx-glr-auto-examples-plot-azimuth-set-relationships-py\n.. _Parameters:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Numerical-Fracture-Network-Characterization-Parameters\n.. _Contour-grids:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Contour-Grids\n.. _Multi-scale:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_multi_scale_networks.html#sphx-glr-auto-examples-plot-multi-scale-networks-py\n\nFor a short tutorial on use of ``fractopo`` continue reading:\n\nInput data\n~~~~~~~~~~\n\nReading and writing spatial filetypes is done in ``geopandas`` and you\nshould see ``geopandas`` documentation for more advanced read-write use\ncases:\n\n-  https://geopandas.org/\n\nSimple example with trace and area data in GeoPackages:\n\n.. code:: python\n\n   import geopandas as gpd\n\n   # Trace data is in a file `traces.gpkg` in current working directory\n   # Area data is in a file `areas.gpkg` in current working directory\n   trace_data = gpd.read_file("traces.gpkg")\n   area_data = gpd.read_file("areas.gpkg")\n\nTrace validation\n~~~~~~~~~~~~~~~~\n\nTrace data must be validated using ``fractopo`` validation functionality\nbefore analysis. The topological analysis of lineament & fracture traces\nimplemented in ``fractopo`` will not tolerate uncertainty related to the\ntopological abutting and snapping relationships between traces.\nTherefore the trace validation is recommended before all analysis using\n``Network``. Trace and target area data can be validated for further\nanalysis with a ``Validation`` object.\n\n.. code:: python\n\n   from fractopo import Validation\n\n   validation = Validation(\n       trace_data,\n       area_data,\n       name="mytraces",\n       allow_fix=True,\n   )\n\n   # Validation is done explicitly with `run_validation` method\n   validated_trace_data = validation.run_validation()\n\nTrace validation is also accessible as a command-line script,\n``fractopo tracevalidate`` which is more straightforward to use than through\nPython calls. Note that all subcommands of ``fractopo`` are available by\nappending them after ``fractopo``.\n\n``tracevalidate`` always requires the target area that delineates trace\ndata.\n\n.. code:: bash\n\n   # Get full up-to-date script help\n\n   fractopo tracevalidate --help\n\n   # Basic usage example:\n\n   fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\\\n      --output /path/to/validated_trace_data.shp\n\n   # Or with automatic saving to validated/ directory\n\n   fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\\\n      --summary\n\nGeometric and topological trace network analysis\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n``fractopo`` can be used to extract lineament & fracture size,\nabundance and topological parameters from two-dimensional lineament and\nfracture trace, branch and node data.\n\nTrace and target area data (``GeoDataFrames``) are passed into a\n``Network`` object which has properties and functions for returning and\nvisualizing different parameters and attributes of trace data.\n\n.. code:: python\n\n   from fractopo import Network\n\n   # Initialize Network object and determine the topological branches and nodes\n   network = Network(\n       trace_data,\n       area_data,\n       # Give the Network a name!\n       name="mynetwork",\n       # Specify whether to determine topological branches and nodes\n       # (Required for almost all analysis)\n       determine_branches_nodes=True,\n       # Specify the snapping distance threshold to define when traces are\n       # snapped to each other\n       snap_threshold=0.001,\n       # If the target area used in digitization is a circle, the knowledge can\n       # be used in some analysis\n       circular_target_area=True,\n       # Analysis on traces can be done for the full inputted dataset or the\n       # traces can be cropped to the target area before analysis (cropping\n       # recommended)\n       truncate_traces=True,\n   )\n\n   # Properties are easily accessible\n   # e.g.,\n   network.branch_counts\n   network.node_counts\n\n   # Plotting is done by plot_ -prefixed methods\n   network.plot_trace_lengths()\n\nNetwork analysis is also available as a command-line script but using the\nPython interface (e.g. ``jupyter lab``, ``ipython``) is recommended when\nanalysing ``Networks`` to have access to all available analysis and plotting\nmethods. The command-line entrypoint is **opinionated** in what outputs it\nproduces. Brief example of command-line entrypoint:\n\n.. code:: bash\n\n   fractopo network /path/to/trace_data.shp /path/to/area_data.shp\\\n      --name mynetwork\n\n   # Use --help to see all up-to-date arguments and help\n   fractopo network --help\n\n.. figure:: /docs_src/imgs/fractopo_workflow_visualisation.jpg\n   :alt: Data analysis workflow visualisation for fracture trace data.\n\n   Data analysis workflow visualisation for fracture trace data\n   (``KB11``). A. Target area for trace digitisation. B. Digitized\n   traces and target area. C. Orthomosaic used as the base raster from\n   which the traces are digitized from. D. Equal-area length-weighted\n   rose plot of the fracture trace azimuths. E. Length distribution\n   analysis of the trace lengths. F. Determined branches and nodes\n   through topological analysis. G. Cross-cut and abutting relationships\n   between chosen azimuth sets. H. Ternary plot of node (X, Y and I)\n   proportions. I. Ternary plot of branch (C-C, C-I, I-I) proportions.\n\n\nCiting\n------\n\nTo cite this software:\n\n-  The software is introduced in https://doi.org/10.1016/j.jsg.2022.104528 and\n   you can cite that article as a general citation:\n\n.. code:: text\n\n   Ovaskainen, N., Nordbäck, N., Skyttä, P. and Engström, J., 2022. A new\n   subsampling methodology to optimize the characterization of\n   two-dimensional bedrock fracture networks. Journal of Structural Geology,\n   p.104528.\n\n-  To cite a specific version of ``fractopo`` you can use a ``zenodo``\n   provided ``DOI``. E.g. https://doi.org/10.5281/zenodo.5957206 for version\n   ``v0.2.6``. See the ``zenodo`` page of ``fractopo`` for the ``DOI`` of each\n   version: https://doi.org/10.5281/zenodo.5517485\n\nSupport\n-------\n\nFor issues of any kind: please create a GitHub issue here!\nAlternatively, you can contact the main developer by email at\nnikolasovaskainen@gmail.com.\n\nReferences\n----------\n\nFor the scientific background, prior works, definition of traces, branches and\nnodes along with the explanation of the plots and the plotted parameters, you\nare referred to multiple sources:\n\n-  `Sanderson and Nixon,\n   2015 <https://doi.org/10.1016/j.jsg.2015.01.005>`__\n\n   -  Trace and branch size, abundance and topological parameter\n      definitions.\n\n-  `Ovaskainen et al, 2022 <https://doi.org/10.1016/j.jsg.2022.104528>`__\n\n   -  Application of ``fractopo`` for subsampling analysis of fracture networks.\n\n-  `Nyberg et al., 2018 <https://doi.org/10.1130/GES01595.1>`__\n\n   -  A similar package to ``fractopo`` with a ``QGIS`` GUI.\n   -  `NetworkGT GitHub <https://github.com/BjornNyberg/NetworkGT>`__\n\n-  `Sanderson and Peacock,\n   2020 <https://www.sciencedirect.com/science/article/abs/pii/S001282521930594X>`__\n\n   -  Discussion around rose plots and justification for using\n      length-weighted equal-area rose plots.\n\n-  `Alstott et al.\n   2014 <https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0085777>`__\n\n   -  Length distribution modelling using the Python 3 ``powerlaw``\n      package which ``fractopo`` uses\n   -  `powerlaw GitHub <https://github.com/jeffalstott/powerlaw>`__\n\n-  `Bonnet et al.,\n   2001 <https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/1999RG000074>`__\n\n   -  Length distribution modelling review.\n\n-  `My Master’s Thesis, Ovaskainen,\n   2020 <http://urn.fi/URN:NBN:fi-fe202003259211>`__\n\n   -  Plots used in my Thesis were done with an older version of the\n      same code used for this plugin.\n\nDevelopment\n-----------\n\n-  **Breaking changes are possible and expected.**\n\n-  For general contributing guidelines, see `CONTRIBUTING.rst </CONTRIBUTING>`__\n\nDevelopment dependencies for ``fractopo`` include:\n\n-  ``poetry``\n\n   -  Used to handle Python package dependencies.\n\n   .. code:: bash\n\n      # Use poetry run to execute poetry installed cli tools such as invoke,\n      # nox and pytest.\n      poetry run \'<cmd>\'\n\n\n-  ``doit``\n\n   -  A general task executor that is a replacement for a ``Makefile``\n   -  Understands task dependencies and can run tasks in parallel\n      even while running them in the order determined from dependencies\n      between tasks. E.g., requirements.txt is a requirement for running\n      tests and therefore the task creating requirements.txt will always\n      run before the test task.\n\n   .. code:: bash\n\n      # Tasks are defined in dodo.py\n      # To list doit tasks from command line\n      poetry run doit list\n      # To run all tasks in parallel (recommended before pushing and/or\n      # committing)\n      # 8 is the number of cpu cores, change as wanted\n      # -v 0 sets verbosity to very low. (Errors will always still be printed.)\n      poetry run doit -n 8 -v 0\n\n-  ``nox``\n\n   -  ``nox`` is a replacement for ``tox``. Both are made to create\n      reproducible Python environments for testing, making docs locally, etc.\n\n   .. code:: bash\n\n      # To list available nox sessions\n      # Sessions are defined in noxfile.py\n      poetry run nox --list\n\n-  ``copier``\n\n   -  ``copier`` is a project templater. Many Python projects follow a similar\n      framework for testing, creating documentations and overall placement of\n      files and configuration. ``copier`` allows creating a template project\n      (e.g., https://github.com/nialov/nialov-py-template) which can be firstly\n      cloned as the framework for your own package and secondly to pull updates\n      from the template to your already started project.\n\n   .. code:: bash\n\n      # To pull copier update from github/nialov/nialov-py-template\n      poetry run copier update\n\n\n-  ``pytest``\n\n   -  ``pytest`` is a Python test runner. It is used to run defined tests to\n      check that the package executes as expected. The defined tests in\n      ``./tests`` contain many regression tests (done with\n      ``pytest-regressions``) that make it almost impossible\n      to add features to ``fractopo`` that changes the results of functions\n      and methods.\n\n   .. code:: bash\n\n      # To run tests implemented in ./tests directory and as doctests\n      # within project itself:\n      poetry run pytest\n\n\n-  ``coverage``\n\n   .. code:: bash\n\n      # To check coverage of tests\n      # (Implemented as nox session!)\n      poetry run nox --session test_pip\n\n-  ``sphinx``\n\n   -  Creates documentation from files in ``./docs_src``.\n\n   .. code:: bash\n\n      # To create documentation\n      # (Implemented as nox session!)\n      poetry run nox --session docs\n\nBig thanks to all maintainers of the above packages!\n\nLicense\n~~~~~~~\n\nCopyright © 2020-2023, Nikolas Ovaskainen.\n\n-----\n\n\n.. |Documentation Status| image:: https://readthedocs.org/projects/fractopo/badge/?version=latest\n   :target: https://fractopo.readthedocs.io/en/latest/?badge=latest\n.. |PyPI Status| image:: https://img.shields.io/pypi/v/fractopo.svg\n   :target: https://pypi.python.org/pypi/fractopo\n.. |CI Test| image:: https://github.com/nialov/fractopo/workflows/CI/badge.svg\n   :target: https://github.com/nialov/fractopo/actions/workflows/main.yaml?query=branch%3Amaster\n.. |Conda Test| image:: https://github.com/nialov/fractopo/workflows/conda/badge.svg\n   :target: https://github.com/nialov/fractopo/actions/workflows/conda.yaml?query=branch%3Amaster\n.. |Coverage| image:: https://raw.githubusercontent.com/nialov/fractopo/master/docs_src/imgs/coverage.svg\n   :target: https://github.com/nialov/fractopo/blob/master/docs_src/imgs/coverage.svg\n.. |Binder| image:: http://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/nialov/fractopo/HEAD?filepath=docs_src%2Fnotebooks%2Ffractopo_network_1.ipynb\n.. |Zenodo| image:: https://zenodo.org/badge/297451015.svg\n   :target: https://zenodo.org/badge/latestdoi/297451015\n',
+    'long_description': 'fractopo\n========\n\n|Documentation Status| |PyPI Status| |CI Test| |Conda Test| |Coverage| |Binder| |Zenodo|\n\n``fractopo`` is a Python library/application that contains tools for\nvalidating and analysing lineament and fracture trace maps (fracture\nnetworks). It is targeted at structural geologists working on the\ncharacterization of bedrock fractures from outcrops and through remote\nsensing. ``fractopo`` is available as a Python library and through a\ncommand-line interface. As a Python library, the use of ``fractopo``\nrequires prior (Python) programming knowledge. However, if used through\nthe command-line, using ``fractopo`` only requires general knowledge of\ncommand-line interfaces in your operating system of choice.\n\n-  `Full Documentation is hosted on Read the Docs\n   <https://fractopo.readthedocs.io/en/latest/index.html#full-documentation>`__\n\n.. figure:: https://git.io/JBRuK\n   :alt: Overview of fractopo\n\n   Overview of fractopo\n\n.. figure:: /docs_src/imgs/fractopo-visualizations.png\n   :alt: Data visualization\n\n   Visualisation of ``fractopo`` data. ``fractopo`` analyses the trace\n   data that can e.g. be digitized from drone orthophotographs\n   (=fractures) or from digital elevation models (=lineaments). The\n   displayed branches and nodes are extracted with ``fractopo``.\n\nInstallation\n------------\n\n``pip`` and ``poetry`` installation only supported for ``linux`` -based\noperating systems. For Windows and MacOS install using `(ana)conda <#conda>`__.\n\nconda\n~~~~~\n\n-  Only (supported) installation method for ``Windows`` and ``MacOS``!\n\n.. code:: bash\n\n   # Create new environment for fractopo (recommended but optional)\n   conda env create fractopo-env\n   conda activate fractopo-env\n   # Available on conda-forge channel\n   conda install -c conda-forge fractopo\n\npip\n~~~\n\nThe module is on `PyPI <https://www.pypi.org>`__.\n\n.. code:: bash\n\n   # Non-development installation\n   pip install fractopo\n\npoetry\n~~~~~~\n\nFor usage:\n\n.. code:: bash\n\n   poetry add fractopo\n\nFor development, only ``poetry`` installation of ``fractopo`` is\nsupported:\n\n.. code:: bash\n\n   git clone https://github.com/nialov/fractopo\n   cd fractopo\n   poetry install\n\nUsage\n-----\n\n``fractopo`` has two main use cases:\n\n1. Validation of lineament & fracture trace data\n2. Analysis of lineament & fracture trace data\n\nValidation is done to make sure the data is valid for the analysis and\nis crucial as analysis cannot take into account different kinds of\ngeometric and topological inconsistencies between the traces.\nCapabilities and associated guides are inexhaustively listed in the\ntable below.\n\n========================================================  ======================\nFunctionality                                             Tutorial/Guide/Example\n========================================================  ======================\nValidation of trace data                                  `Validation 1`_; `Validation 2`_\nVisualize trace map data                                  `Visualizing`_\nTopological branches and nodes                            `Network`_; `Topological`_\nTrace and branch length distributions                     `Length-distributions`_\nOrientation rose plots                                    `Orientation 1`_; `Orientation 2`_\nPlot topological ternary node and branch proportions      `Proportions`_\nCross-cutting and abutting relationships                  `Relationships 1`_; `Relationships 2`_;\nGeometric and topological fracture network parameters     `Parameters`_\nContour grids of fracture network parameters              `Contour-grids`_\nMulti-scale length distributions                          `Multi-scale`_\n========================================================  ======================\n\n.. _Validation 1:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_validation_1.html\n.. _Validation 2:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_validation_2.html\n.. _Visualizing:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Visualizing-trace-map-data\n.. _Network:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Network\n.. _Topological:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_branches_and_nodes.html#sphx-glr-auto-examples-plot-branches-and-nodes-py\n.. _Length-distributions:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Length-distributions\n.. _Orientation 1:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Rose-plots\n.. _Orientation 2:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_rose_plot.html#sphx-glr-auto-examples-plot-rose-plot-py\n.. _Proportions:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Node-and-branch-proportions\n.. _Relationships 1:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Crosscutting-and-abutting-relationships\n.. _Relationships 2:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_azimuth_set_relationships.html#sphx-glr-auto-examples-plot-azimuth-set-relationships-py\n.. _Parameters:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Numerical-Fracture-Network-Characterization-Parameters\n.. _Contour-grids:\n   https://fractopo.readthedocs.io/en/latest/notebooks/fractopo_network_1.html#Contour-Grids\n.. _Multi-scale:\n   https://fractopo.readthedocs.io/en/latest/auto_examples/plot_multi_scale_networks.html#sphx-glr-auto-examples-plot-multi-scale-networks-py\n\nFor a short tutorial on use of ``fractopo`` continue reading:\n\nInput data\n~~~~~~~~~~\n\nReading and writing spatial filetypes is done in ``geopandas`` and you\nshould see ``geopandas`` documentation for more advanced read-write use\ncases:\n\n-  https://geopandas.org/\n\nSimple example with trace and area data in GeoPackages:\n\n.. code:: python\n\n   import geopandas as gpd\n\n   # Trace data is in a file `traces.gpkg` in current working directory\n   # Area data is in a file `areas.gpkg` in current working directory\n   trace_data = gpd.read_file("traces.gpkg")\n   area_data = gpd.read_file("areas.gpkg")\n\nTrace validation\n~~~~~~~~~~~~~~~~\n\nTrace data must be validated using ``fractopo`` validation functionality\nbefore analysis. The topological analysis of lineament & fracture traces\nimplemented in ``fractopo`` will not tolerate uncertainty related to the\ntopological abutting and snapping relationships between traces. See `the\ndocumentation <https://fractopo.readthedocs.io/en/latest/validation/errors.html>`__\nfor further info on validation error types. Trace validation is\nrecommended before all analysis using ``Network``. Trace and target area\ndata can be validated for further analysis with a ``Validation`` object:\n\n.. code:: python\n\n   from fractopo import Validation\n\n   validation = Validation(\n       trace_data,\n       area_data,\n       name="mytraces",\n       allow_fix=True,\n   )\n\n   # Validation is done explicitly with `run_validation` method\n   validated_trace_data = validation.run_validation()\n\nTrace validation is also accessible through the ``fractopo``\ncommand-line interface, ``fractopo tracevalidate`` which is more\nstraightforward to use than through Python calls. Note that all\nsubcommands of ``fractopo`` are available by appending them after\n``fractopo``.\n\n``tracevalidate`` always requires the target area that delineates trace\ndata.\n\n.. code:: bash\n\n   # Get full up-to-date command-line interface help\n   fractopo tracevalidate --help\n\n   # Basic usage example:\n   fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\\\n      --output /path/to/validated_trace_data.shp\n\n   # Or with automatic saving to validated/ directory\n   fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\\\n      --summary\n\nGeometric and topological trace network analysis\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n``fractopo`` can be used to extract lineament & fracture size,\nabundance and topological parameters from two-dimensional lineament and\nfracture trace, branch and node data.\n\nTrace and target area data (``GeoDataFrames``) are passed into a\n``Network`` object which has properties and functions for returning and\nvisualizing different parameters and attributes of trace data.\n\n.. code:: python\n\n   from fractopo import Network\n\n   # Initialize Network object and determine the topological branches and nodes\n   network = Network(\n       trace_data,\n       area_data,\n       # Give the Network a name!\n       name="mynetwork",\n       # Specify whether to determine topological branches and nodes\n       # (Required for almost all analysis)\n       determine_branches_nodes=True,\n       # Specify the snapping distance threshold to define when traces are\n       # snapped to each other. The unit is the same as the one in the\n       # coordinate system the trace and area data are in.\n       # In default values, fractopo assumes a metric unit and using metric units\n       # is heavily recommended.\n       snap_threshold=0.001,\n       # If the target area used in digitization is a circle, the knowledge can\n       # be used in some analysis\n       circular_target_area=True,\n       # Analysis on traces can be done for the full inputted dataset or the\n       # traces can be cropped to the target area before analysis (cropping\n       # recommended)\n       truncate_traces=True,\n   )\n\n   # Properties are easily accessible\n   # e.g.,\n   network.branch_counts\n   network.node_counts\n\n   # Plotting is done by plot_ -prefixed methods\n   network.plot_trace_lengths()\n\nNetwork analysis is also available through the ``fractopo`` command-line\ninterface but using the Python interface (e.g. ``jupyter lab``,\n``ipython``) is recommended when analysing ``Networks`` to have access\nto all available analysis and plotting methods. The command-line\nentrypoint is **opinionated** in what outputs it produces. Brief example\nof command-line entrypoint:\n\n.. code:: bash\n\n   fractopo network /path/to/trace_data.shp /path/to/area_data.shp\\\n      --name mynetwork\n\n   # Use --help to see all up-to-date arguments and help\n   fractopo network --help\n\n.. figure:: /docs_src/imgs/fractopo_workflow_visualisation.jpg\n   :alt: Data analysis workflow visualisation for fracture trace data.\n\n   Data analysis workflow visualisation for fracture trace data\n   (``KB11``). A. Target area for trace digitisation. B. Digitized\n   traces and target area. C. Orthomosaic used as the base raster from\n   which the traces are digitized from. D. Equal-area length-weighted\n   rose plot of the fracture trace azimuths. E. Length distribution\n   analysis of the trace lengths. F. Determined branches and nodes\n   through topological analysis. G. Cross-cut and abutting relationships\n   between chosen azimuth sets. H. Ternary plot of node (X, Y and I)\n   proportions. I. Ternary plot of branch (C-C, C-I, I-I) proportions.\n\n\nCiting\n------\n\nTo cite this software:\n\n-  The software is introduced in https://doi.org/10.1016/j.jsg.2022.104528 and\n   you can cite that article as a general citation:\n\n.. code:: text\n\n   Ovaskainen, N., Nordbäck, N., Skyttä, P. and Engström, J., 2022. A new\n   subsampling methodology to optimize the characterization of\n   two-dimensional bedrock fracture networks. Journal of Structural Geology,\n   p.104528.\n\n-  To cite a specific version of ``fractopo`` you can use a ``zenodo``\n   provided ``DOI``. E.g. https://doi.org/10.5281/zenodo.5957206 for version\n   ``v0.2.6``. See the ``zenodo`` page of ``fractopo`` for the ``DOI`` of each\n   version: https://doi.org/10.5281/zenodo.5517485\n\nSupport\n-------\n\nFor issues of any kind: please create a GitHub issue here!\nAlternatively, you can contact the main developer by email at\nnikolasovaskainen@gmail.com.\n\nReferences\n----------\n\nFor the scientific background, prior works, definition of traces, branches and\nnodes along with the explanation of the plots and the plotted parameters, you\nare referred to multiple sources:\n\n-  `Sanderson and Nixon,\n   2015 <https://doi.org/10.1016/j.jsg.2015.01.005>`__\n\n   -  Trace and branch size, abundance and topological parameter\n      definitions.\n\n-  `Ovaskainen et al, 2022 <https://doi.org/10.1016/j.jsg.2022.104528>`__\n\n   -  Application of ``fractopo`` for subsampling analysis of fracture networks.\n\n-  `Nyberg et al., 2018 <https://doi.org/10.1130/GES01595.1>`__\n\n   -  A similar package to ``fractopo`` with a ``QGIS`` GUI.\n   -  `NetworkGT GitHub <https://github.com/BjornNyberg/NetworkGT>`__\n\n-  `Sanderson and Peacock,\n   2020 <https://www.sciencedirect.com/science/article/abs/pii/S001282521930594X>`__\n\n   -  Discussion around rose plots and justification for using\n      length-weighted equal-area rose plots.\n\n-  `Alstott et al.\n   2014 <https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0085777>`__\n\n   -  Length distribution modelling using the Python 3 ``powerlaw``\n      package which ``fractopo`` uses\n   -  `powerlaw GitHub <https://github.com/jeffalstott/powerlaw>`__\n\n-  `Bonnet et al.,\n   2001 <https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/1999RG000074>`__\n\n   -  Length distribution modelling review.\n\n-  `My Master’s Thesis, Ovaskainen,\n   2020 <http://urn.fi/URN:NBN:fi-fe202003259211>`__\n\n   -  Plots used in my Thesis were done with an older version of the\n      same code used for this plugin.\n\nDevelopment\n-----------\n\n-  The package interfaces are nearing stability and breaking changes in\n   code should for the most part be included in the ``CHANGELOG.md``\n   after 25.4.2023. However, this is not guaranteed until the version\n   reaches v1.0.0. The interfaces of ``Network`` and ``Validation`` can\n   be expected to be the most stable.\n\n-  For general contributing guidelines, see `CONTRIBUTING.rst </CONTRIBUTING.rst>`__\n\nDevelopment dependencies for ``fractopo`` include:\n\n-  ``poetry``\n\n   -  Used to handle Python package dependencies.\n\n   .. code:: bash\n\n      # Use poetry run to execute poetry installed cli tools such as invoke,\n      # nox and pytest.\n      poetry run \'<cmd>\'\n\n\n-  ``doit``\n\n   -  A general task executor that is a replacement for a ``Makefile``\n   -  Understands task dependencies and can run tasks in parallel\n      even while running them in the order determined from dependencies\n      between tasks. E.g., requirements.txt is a requirement for running\n      tests and therefore the task creating requirements.txt will always\n      run before the test task.\n\n   .. code:: bash\n\n      # Tasks are defined in dodo.py\n      # To list doit tasks from command line\n      poetry run doit list\n      # To run all tasks in parallel (recommended before pushing and/or\n      # committing)\n      # 8 is the number of cpu cores, change as wanted\n      # -v 0 sets verbosity to very low. (Errors will always still be printed.)\n      poetry run doit -n 8 -v 0\n\n-  ``nox``\n\n   -  ``nox`` is a replacement for ``tox``. Both are made to create\n      reproducible Python environments for testing, making docs locally, etc.\n\n   .. code:: bash\n\n      # To list available nox sessions\n      # Sessions are defined in noxfile.py\n      poetry run nox --list\n\n-  ``copier``\n\n   -  ``copier`` is a project templater. Many Python projects follow a similar\n      framework for testing, creating documentations and overall placement of\n      files and configuration. ``copier`` allows creating a template project\n      (e.g., https://github.com/nialov/nialov-py-template) which can be firstly\n      cloned as the framework for your own package and secondly to pull updates\n      from the template to your already started project.\n\n   .. code:: bash\n\n      # To pull copier update from github/nialov/nialov-py-template\n      poetry run copier update\n\n\n-  ``pytest``\n\n   -  ``pytest`` is a Python test runner. It is used to run defined tests to\n      check that the package executes as expected. The defined tests in\n      ``./tests`` contain many regression tests (done with\n      ``pytest-regressions``) that make it almost impossible\n      to add features to ``fractopo`` that changes the results of functions\n      and methods.\n\n   .. code:: bash\n\n      # To run tests implemented in ./tests directory and as doctests\n      # within project itself:\n      poetry run pytest\n\n\n-  ``coverage``\n\n   .. code:: bash\n\n      # To check coverage of tests\n      # (Implemented as nox session!)\n      poetry run nox --session test_pip\n\n-  ``sphinx``\n\n   -  Creates documentation from files in ``./docs_src``.\n\n   .. code:: bash\n\n      # To create documentation\n      # (Implemented as nox session!)\n      poetry run nox --session docs\n\nBig thanks to all maintainers of the above packages!\n\nLicense\n~~~~~~~\n\nCopyright © 2020-2023, Nikolas Ovaskainen.\n\n-----\n\n\n.. |Documentation Status| image:: https://readthedocs.org/projects/fractopo/badge/?version=latest\n   :target: https://fractopo.readthedocs.io/en/latest/?badge=latest\n.. |PyPI Status| image:: https://img.shields.io/pypi/v/fractopo.svg\n   :target: https://pypi.python.org/pypi/fractopo\n.. |CI Test| image:: https://github.com/nialov/fractopo/workflows/CI/badge.svg\n   :target: https://github.com/nialov/fractopo/actions/workflows/main.yaml?query=branch%3Amaster\n.. |Conda Test| image:: https://github.com/nialov/fractopo/workflows/conda/badge.svg\n   :target: https://github.com/nialov/fractopo/actions/workflows/conda.yaml?query=branch%3Amaster\n.. |Coverage| image:: https://raw.githubusercontent.com/nialov/fractopo/master/docs_src/imgs/coverage.svg\n   :target: https://github.com/nialov/fractopo/blob/master/docs_src/imgs/coverage.svg\n.. |Binder| image:: http://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/nialov/fractopo/HEAD?filepath=docs_src%2Fnotebooks%2Ffractopo_network_1.ipynb\n.. |Zenodo| image:: https://zenodo.org/badge/297451015.svg\n   :target: https://zenodo.org/badge/latestdoi/297451015\n',
     'author': 'nialov',
     'author_email': 'nikolasovaskainen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nialov/fractopo',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fractopo-0.5.2/PKG-INFO` & `fractopo-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractopo
-Version: 0.5.2
+Version: 0.5.3
 Summary: Fracture Network Analysis
 Home-page: https://github.com/nialov/fractopo
 License: MIT
 Keywords: data,gis,geology,fracture,topology
 Author: nialov
 Author-email: nikolasovaskainen@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -19,39 +19,39 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: GIS
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: typecheck
 Requires-Dist: click
-Requires-Dist: coverage-badge; extra == "coverage"
-Requires-Dist: coverage; extra == "coverage"
+Requires-Dist: coverage ; extra == "coverage"
+Requires-Dist: coverage-badge ; extra == "coverage"
 Requires-Dist: geopandas (>=0.11.1,<1.0.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
-Requires-Dist: markupsafe; extra == "lint"
-Requires-Dist: matplotlib
-Requires-Dist: mypy; extra == "typecheck"
-Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: markupsafe ; extra == "lint"
+Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
+Requires-Dist: mypy ; extra == "typecheck"
+Requires-Dist: nbsphinx ; extra == "docs"
 Requires-Dist: numpy
 Requires-Dist: pandas (>=1.3,<2.0.0)
 Requires-Dist: powerlaw
 Requires-Dist: pygeos (>=0.13.0,<1.0.0)
-Requires-Dist: pylint; extra == "lint"
+Requires-Dist: pylint ; extra == "lint"
 Requires-Dist: python-ternary
 Requires-Dist: rich (>=11.0.0)
-Requires-Dist: rstcheck; extra == "lint"
+Requires-Dist: rstcheck ; extra == "lint"
 Requires-Dist: scikit-learn
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: seaborn
 Requires-Dist: shapely (>=1.8.0,<2.0.0)
-Requires-Dist: sphinx-autobuild; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx-gallery; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
-Requires-Dist: sphinx; extra == "docs" or extra == "lint"
+Requires-Dist: sphinx ; extra == "docs" or extra == "lint"
+Requires-Dist: sphinx-autobuild ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
+Requires-Dist: sphinx-gallery ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: typer (>=0.4,<1.0.0)
 Project-URL: Bug Tracker, https://github.com/nialov/fractopo/issues
 Project-URL: Documentation, https://fractopo.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/nialov/fractopo
 Description-Content-Type: text/x-rst
 
 fractopo
@@ -59,16 +59,19 @@
 
 |Documentation Status| |PyPI Status| |CI Test| |Conda Test| |Coverage| |Binder| |Zenodo|
 
 ``fractopo`` is a Python library/application that contains tools for
 validating and analysing lineament and fracture trace maps (fracture
 networks). It is targeted at structural geologists working on the
 characterization of bedrock fractures from outcrops and through remote
-sensing. As it is a Python library, the use of ``fractopo`` requires
-prior (Python) programming knowledge.
+sensing. ``fractopo`` is available as a Python library and through a
+command-line interface. As a Python library, the use of ``fractopo``
+requires prior (Python) programming knowledge. However, if used through
+the command-line, using ``fractopo`` only requires general knowledge of
+command-line interfaces in your operating system of choice.
 
 -  `Full Documentation is hosted on Read the Docs
    <https://fractopo.readthedocs.io/en/latest/index.html#full-documentation>`__
 
 .. figure:: https://git.io/JBRuK
    :alt: Overview of fractopo
 
@@ -84,18 +87,14 @@
 
 Installation
 ------------
 
 ``pip`` and ``poetry`` installation only supported for ``linux`` -based
 operating systems. For Windows and MacOS install using `(ana)conda <#conda>`__.
 
-For ``pip`` and ``poetry``: Omit ``--dev`` or ``[dev]`` for regular
-installation. Keep if you want to test/develop or otherwise install all
-development Python dependencies.
-
 conda
 ~~~~~
 
 -  Only (supported) installation method for ``Windows`` and ``MacOS``!
 
 .. code:: bash
 
@@ -111,33 +110,25 @@
 The module is on `PyPI <https://www.pypi.org>`__.
 
 .. code:: bash
 
    # Non-development installation
    pip install fractopo
 
-Or locally for development:
-
-.. code:: bash
-
-   git clone https://github.com/nialov/fractopo
-   cd fractopo
-   # Omit [dev] from end if you do not want installation for development
-   pip install --editable .[dev]
-
 poetry
 ~~~~~~
 
 For usage:
 
 .. code:: bash
 
    poetry add fractopo
 
-For development:
+For development, only ``poetry`` installation of ``fractopo`` is
+supported:
 
 .. code:: bash
 
    git clone https://github.com/nialov/fractopo
    cd fractopo
    poetry install
 
@@ -223,18 +214,19 @@
 
 Trace validation
 ~~~~~~~~~~~~~~~~
 
 Trace data must be validated using ``fractopo`` validation functionality
 before analysis. The topological analysis of lineament & fracture traces
 implemented in ``fractopo`` will not tolerate uncertainty related to the
-topological abutting and snapping relationships between traces.
-Therefore the trace validation is recommended before all analysis using
-``Network``. Trace and target area data can be validated for further
-analysis with a ``Validation`` object.
+topological abutting and snapping relationships between traces. See `the
+documentation <https://fractopo.readthedocs.io/en/latest/validation/errors.html>`__
+for further info on validation error types. Trace validation is
+recommended before all analysis using ``Network``. Trace and target area
+data can be validated for further analysis with a ``Validation`` object:
 
 .. code:: python
 
    from fractopo import Validation
 
    validation = Validation(
        trace_data,
@@ -242,35 +234,33 @@
        name="mytraces",
        allow_fix=True,
    )
 
    # Validation is done explicitly with `run_validation` method
    validated_trace_data = validation.run_validation()
 
-Trace validation is also accessible as a command-line script,
-``fractopo tracevalidate`` which is more straightforward to use than through
-Python calls. Note that all subcommands of ``fractopo`` are available by
-appending them after ``fractopo``.
+Trace validation is also accessible through the ``fractopo``
+command-line interface, ``fractopo tracevalidate`` which is more
+straightforward to use than through Python calls. Note that all
+subcommands of ``fractopo`` are available by appending them after
+``fractopo``.
 
 ``tracevalidate`` always requires the target area that delineates trace
 data.
 
 .. code:: bash
 
-   # Get full up-to-date script help
-
+   # Get full up-to-date command-line interface help
    fractopo tracevalidate --help
 
    # Basic usage example:
-
    fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\
       --output /path/to/validated_trace_data.shp
 
    # Or with automatic saving to validated/ directory
-
    fractopo tracevalidate /path/to/trace_data.shp /path/to/target_area.shp\
       --summary
 
 Geometric and topological trace network analysis
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``fractopo`` can be used to extract lineament & fracture size,
@@ -291,15 +281,18 @@
        area_data,
        # Give the Network a name!
        name="mynetwork",
        # Specify whether to determine topological branches and nodes
        # (Required for almost all analysis)
        determine_branches_nodes=True,
        # Specify the snapping distance threshold to define when traces are
-       # snapped to each other
+       # snapped to each other. The unit is the same as the one in the
+       # coordinate system the trace and area data are in.
+       # In default values, fractopo assumes a metric unit and using metric units
+       # is heavily recommended.
        snap_threshold=0.001,
        # If the target area used in digitization is a circle, the knowledge can
        # be used in some analysis
        circular_target_area=True,
        # Analysis on traces can be done for the full inputted dataset or the
        # traces can be cropped to the target area before analysis (cropping
        # recommended)
@@ -310,19 +303,20 @@
    # e.g.,
    network.branch_counts
    network.node_counts
 
    # Plotting is done by plot_ -prefixed methods
    network.plot_trace_lengths()
 
-Network analysis is also available as a command-line script but using the
-Python interface (e.g. ``jupyter lab``, ``ipython``) is recommended when
-analysing ``Networks`` to have access to all available analysis and plotting
-methods. The command-line entrypoint is **opinionated** in what outputs it
-produces. Brief example of command-line entrypoint:
+Network analysis is also available through the ``fractopo`` command-line
+interface but using the Python interface (e.g. ``jupyter lab``,
+``ipython``) is recommended when analysing ``Networks`` to have access
+to all available analysis and plotting methods. The command-line
+entrypoint is **opinionated** in what outputs it produces. Brief example
+of command-line entrypoint:
 
 .. code:: bash
 
    fractopo network /path/to/trace_data.shp /path/to/area_data.shp\
       --name mynetwork
 
    # Use --help to see all up-to-date arguments and help
@@ -414,17 +408,21 @@
 
    -  Plots used in my Thesis were done with an older version of the
       same code used for this plugin.
 
 Development
 -----------
 
--  **Breaking changes are possible and expected.**
+-  The package interfaces are nearing stability and breaking changes in
+   code should for the most part be included in the ``CHANGELOG.md``
+   after 25.4.2023. However, this is not guaranteed until the version
+   reaches v1.0.0. The interfaces of ``Network`` and ``Validation`` can
+   be expected to be the most stable.
 
--  For general contributing guidelines, see `CONTRIBUTING.rst </CONTRIBUTING>`__
+-  For general contributing guidelines, see `CONTRIBUTING.rst </CONTRIBUTING.rst>`__
 
 Development dependencies for ``fractopo`` include:
 
 -  ``poetry``
 
    -  Used to handle Python package dependencies.
```

