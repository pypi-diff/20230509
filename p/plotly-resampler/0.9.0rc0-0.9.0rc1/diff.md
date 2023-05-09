# Comparing `tmp/plotly_resampler-0.9.0rc0.tar.gz` & `tmp/plotly_resampler-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.9.0rc0.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.0rc1.tar", max compression
```

## Comparing `plotly_resampler-0.9.0rc0.tar` & `plotly_resampler-0.9.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1115 2023-04-24 11:55:40.176114 plotly_resampler-0.9.0rc0/LICENSE
--rw-r--r--   0        0        0     9540 2023-04-24 11:55:40.176114 plotly_resampler-0.9.0rc0/README.md
--rw-r--r--   0        0        0      853 2023-04-24 11:56:28.830431 plotly_resampler-0.9.0rc0/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      796 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     7281 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    14446 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0     3048 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/gap_handler_interface.py
--rw-r--r--   0        0        0     3116 2023-04-24 11:55:40.180114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/gap_handlers.py
--rw-r--r--   0        0        0     7889 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/plotly_aggregator_parser.py
--rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    23717 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    58683 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13669 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     5376 2023-04-24 11:55:40.184114 plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc0/plotly_resampler/registering.py
--rw-r--r--   0        0        0     3035 2023-04-24 11:56:14.754918 plotly_resampler-0.9.0rc0/pyproject.toml
--rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-05-03 12:32:58.928306 plotly_resampler-0.9.0rc1/LICENSE
+-rw-r--r--   0        0        0     9540 2023-05-09 09:35:41.332034 plotly_resampler-0.9.0rc1/README.md
+-rw-r--r--   0        0        0      853 2023-05-09 09:36:29.006385 plotly_resampler-0.9.0rc1/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     6934 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    11877 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3048 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3179 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     7933 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    23690 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    61202 2023-05-09 09:35:41.356033 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13669 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     5376 2023-05-07 09:13:04.096399 plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc1/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     2857 2023-05-09 09:36:04.819222 plotly_resampler-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    11486 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc1/PKG-INFO
```

### Comparing `plotly_resampler-0.9.0rc0/LICENSE` & `plotly_resampler-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc0/README.md` & `plotly_resampler-0.9.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
   organization={IEEE}
 }
 ```
 
 ## Future work 🔨
 
 - [x] Support `.add_traces()` (currently only `.add_trace` is supported)
-- [ ] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
+- [x] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
 - [x] Integrate with [tsdownsample](https://github.com/predict-idlab/tsdownsample) :racehorse:
 
 <br>
 
 ---
 
 <p align="center">
```

#### html2text {}

```diff
@@ -95,13 +95,13 @@
 further with the developers, see issue [#49](https://github.com/predict-idlab/
 plotly-resampler/issues/49). ## Cite Paper (preprint): https://arxiv.org/abs/
 2206.08703 ```bibtex @inproceedings{van2022plotly, title={Plotly-resampler:
 Effective visual analytics for large time series}, author={Van Der Donckt,
 Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
 booktitle={2022 IEEE Visualization and Visual Analytics (VIS)}, pages={21--25},
 year={2022}, organization={IEEE} } ``` ## Future work ð¨ - [x] Support
-`.add_traces()` (currently only `.add_trace` is supported) - [ ] Support
+`.add_traces()` (currently only `.add_trace` is supported) - [x] Support
 `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/
 plotly-resampler/pull/148) - [x] Integrate with [tsdownsample](https://
 github.com/predict-idlab/tsdownsample) :racehorse:
 ---
         ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/__init__.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.9.0rc0"
+__version__ = "0.9.0rc1"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
     "MinMaxLTTB",
     "LTTB",
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/aggregation_interface.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregation_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,38 +10,32 @@
 
 import numpy as np
 
 
 class AbstractAggregator(ABC):
     def __init__(
         self,
-        interleave_gaps: bool = True,
         x_dtype_regex_list: Optional[List[str]] = None,
         y_dtype_regex_list: Optional[List[str]] = None,
         **downsample_kwargs,
     ):
         """Constructor of AbstractSeriesAggregator.
 
         Parameters
         ----------
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. An x-range based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
         x_dtype_regex_list: List[str], optional
             List containing the regex matching the supported datatypes for the x array,
             by default None.
         y_dtype_regex_list: List[str], optional
             List containing the regex matching the supported datatypes for the y array,
             by default None.
         downsample_kwargs: dict
             Additional kwargs passed to the downsample method.
 
         """
-        self.interleave_gaps = interleave_gaps
         self.x_dtype_regex_list = x_dtype_regex_list
         self.y_dtype_regex_list = y_dtype_regex_list
         self.downsample_kwargs = downsample_kwargs
 
     @staticmethod
     def _check_n_out(n_out: int) -> None:
         """Check if the n_out is valid."""
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/aggregators.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/aggregators.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,26 +71,16 @@
         >>> s_cat = s.astype(cat_type)
     * `LTTB` has no downsample kwargs, as it cannot be paralellized. Instead, you can
       use the :class:`MinMaxLTTB <MinMaxLTTB>` downsampler, which performs
       minmax preselection (in parallel if configured so), followed by LTTB.
 
     """
 
-    def __init__(self, interleave_gaps: bool = True):
-        """
-        Parameters
-        ----------
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. A quantile-based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
-
-        """
+    def __init__(self):
         super().__init__(
-            interleave_gaps,
             y_dtype_regex_list=[rf"{dtype}\d*" for dtype in ("float", "int", "uint")]
             + ["category", "bool"],
         )
         self.downsampler = LTTBDownsampler()
 
     def _arg_downsample(
         self,
@@ -116,28 +106,18 @@
 
     .. note::
         This method is implemented in Python (leveraging numpy for vecotrization), but
         is **significantly slower than the MinMaxAggregator** (which is implemented in
         the tsdownsample toolkit in Rust). |br|
         As such, this class does not support any downsample kwargs.
 
-    """
-
-    def __init__(self, interleave_gaps: bool = True):
-        """
-        Parameters
-        ----------
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. A quantile-based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
+    .. note::
+        This downsampler supports all dtypes.
 
-        """
-        # this downsampler supports all dtypes
-        super().__init__(interleave_gaps)
+    """
 
     def _arg_downsample(
         self,
         x: np.ndarray | None,
         y: np.ndarray,
         n_out: int,
     ) -> np.ndarray:
@@ -182,29 +162,25 @@
         This method is rather efficient when scaling to large data sizes and can be used
         as a data-reduction step before feeding it to the :class:`LTTB <LTTB>`
         algorithm, as :class:`MinMaxLTTB <MinMaxLTTB>` does with the
         :class:`MinMaxOverlapAggregator <MinMaxOverlapAggregator>`.
 
     """
 
-    def __init__(self, interleave_gaps: bool = True, **downsample_kwargs):
+    def __init__(self, **downsample_kwargs):
         """
         Parameters
         ----------
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. A quantile-based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
         **downsample_kwargs
             Keyword arguments passed to the :class:`MinMaxDownsampler`.
             - The `parallel` argument is set to False by default.
 
         """
         # this downsampler supports all dtypes
-        super().__init__(interleave_gaps, **downsample_kwargs)
+        super().__init__(**downsample_kwargs)
         self.downsampler = MinMaxDownsampler()
 
     def _arg_downsample(
         self,
         x: np.ndarray | None,
         y: np.ndarray,
         n_out: int,
@@ -223,79 +199,57 @@
     points to enhance computational efficiency.
 
     Inventors: Jonas & Jeroen Van Der Donckt - 2022
 
     Paper: pending
     """
 
-    def __init__(
-        self, interleave_gaps: bool = True, minmax_ratio: int = 4, **downsample_kwargs
-    ):
+    def __init__(self, minmax_ratio: int = 4, **downsample_kwargs):
         """
         Parameters
         ----------
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. A quantile-based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
         minmax_ratio: int, optional
             The ratio between the number of data points in the MinMax-prefetching and
             the number of data points that will be outputted by LTTB. By default, 4.
         **downsample_kwargs
             Keyword arguments passed to the :class:`MinMaxLTTBDownsampler`.
             - The `parallel` argument is set to False by default.
-            - The `minmax_ratio` argument is set to 30 by default, whic was empirically
+            - The `minmax_ratio` argument is set to 4 by default, which was empirically
               proven to be a good default.
 
         """
-        self.lttb = LTTBDownsampler()
         self.minmaxlttb = MinMaxLTTBDownsampler()
         self.minmax_ratio = minmax_ratio
 
         super().__init__(
-            interleave_gaps,
             y_dtype_regex_list=[rf"{dtype}\d*" for dtype in ("float", "int", "uint")]
             + ["category", "bool"],
             **downsample_kwargs,
         )
 
     def _arg_downsample(
         self,
         x: np.ndarray | None,
         y: np.ndarray,
         n_out: int,
     ) -> np.ndarray:
-        # when n to n_out ratio is below the threshold, use the LTTB downsampler
-        if y.shape[0] / n_out < (20 * self.minmax_ratio):
-            return self.lttb.downsample(
-                *_to_tsdownsample_args(x, y), n_out=n_out, **self.downsample_kwargs
-            )
         return self.minmaxlttb.downsample(
             *_to_tsdownsample_args(x, y),
             n_out=n_out,
             minmax_ratio=self.minmax_ratio,
             **self.downsample_kwargs,
         )
 
 
 class EveryNthPoint(DataPointSelector):
-    """Naive (but fast) aggregator method which returns every N'th point."""
+    """Naive (but fast) aggregator method which returns every N'th point.
 
-    def __init__(self, interleave_gaps: bool = True):
-        """
-        Parameters
-        ----------
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. A quantile-based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
-
-        """
-        # this downsampler supports all dtypes
-        super().__init__(interleave_gaps)
+    .. note::
+        This downsampler supports all dtypes.
+    """
 
     def _arg_downsample(
         self,
         x: np.ndarray | None,
         y: np.ndarray,
         n_out: int,
     ) -> np.ndarray:
@@ -317,37 +271,27 @@
         data types.
 
     """
 
     def __init__(
         self,
         aggregation_func,
-        interleave_gaps: bool = True,
         x_dtype_regex_list=None,
         y_dtype_regex_list=None,
         **downsample_kwargs,
     ):
         """
         Parameters
         ----------
         aggregation_func: Callable
             The aggregation function which will be applied on each pin.
-        interleave_gaps: bool, optional
-            Whether None values should be added when there are gaps / irregularly
-            sampled data. A quantile-based approach is used to determine the gaps /
-            irregularly sampled data. By default, True.
 
         """
         self.aggregation_func = aggregation_func
-        super().__init__(
-            interleave_gaps,
-            x_dtype_regex_list=x_dtype_regex_list,
-            y_dtype_regex_list=y_dtype_regex_list,
-            **downsample_kwargs,
-        )
+        super().__init__(x_dtype_regex_list, y_dtype_regex_list, **downsample_kwargs)
 
     def _aggregate(
         self,
         x: np.ndarray | None,
         y: np.ndarray,
         n_out: int,
     ) -> Tuple[np.ndarray, np.ndarray]:
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/gap_handler_interface.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handler_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/gap_handlers.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/gap_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,11 +74,12 @@
             A boolean mask indicating the indices where there are gaps. If there are no
             gaps, None is returned.
 
         """
         med_diff, x_diff = self._calc_med_diff(x_agg)
 
         # TODO: this 4 was revealed to me in a dream, but it seems to work well
-        gap_mask = x_diff > 4 * med_diff
+        # After some consideration, we altered this to a 4.1
+        gap_mask = x_diff > 4.1 * med_diff
         if not any(gap_mask):
             return
         return gap_mask
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/aggregation/plotly_aggregator_parser.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/aggregation/plotly_aggregator_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 import pandas as pd
 import pytz
 
 from .aggregation_interface import DataAggregator, DataPointSelector
 from .gap_handler_interface import AbstractGapHandler
+from .gap_handlers import NoGapHandler
 
 
 class PlotlyAggregatorParser:
     @staticmethod
     def parse_hf_data(
         hf_data: np.ndarray | pd.Categorical | pd.Series | pd.Index,
     ) -> np.ndarray | pd.Categorical:
@@ -156,25 +157,25 @@
                 + f"DataAggregator or a DataPointSelector, got {type(downsampler)}"
             )
 
         # TODO check for trace mode (markers, lines, etc.) and only perform the
         # gap insertion methodology when the mode is lines.
         # if trace.get("connectgaps") != True and
         if (
-            not downsampler.interleave_gaps
+            isinstance(gap_handler, NoGapHandler)
             # rangeIndex | datetimeIndex with freq -> equally spaced x; so no gaps
             or isinstance(hf_trace_data["x"], pd.RangeIndex)
             or (
                 isinstance(hf_trace_data["x"], pd.DatetimeIndex)
                 and hf_trace_data["x"].freq is not None
             )
         ):
             return agg_x, agg_y, indices
 
-        # Interleave the gaps`
+        # Interleave the gaps
         # View the data as an int64 when we have a DatetimeIndex
         # We only want to detect gaps, so we only want to compare values.
         agg_x_parsed = PlotlyAggregatorParser.parse_hf_data(agg_x)
         xdt = agg_x_parsed.dtype
         if np.issubdtype(xdt, np.timedelta64) or np.issubdtype(xdt, np.datetime64):
             agg_x_parsed = agg_x_parsed.view("int64")
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,19 +238,19 @@
             .. note::
                 * This can be overridden within the :func:`add_trace` method.
                 * If a trace withholds fewer datapoints than this parameter,
                   the data will *not* be aggregated.
         default_downsampler: AbstractAggregator, optional
             An instance which implements the AbstractAggregator interface and
             will be used as default downsampler, by default ``MinMaxLTTB`` with
-            _interleave_gaps_ set to True. ``MinMaxLTTB`` is a heuristic to the LTTB
-            algorithm that uses pre-selection of min-max values (default 4 per bin) to
-            speed up LTTB (as now only 4 values per bin should be compared). This
-            min-max ratio of 4 can be changed by initializing ``MinMaxLTTB`` with a
-            different value for the ``minmax_ratio`` parameter. \n
+            ``MinMaxLTTB`` is a heuristic to the LTTB algorithm that uses pre-selection
+            of min-max values (default 4 per bin) to speed up LTTB (as now only 4 values
+            per bin are considered by LTTB). This min-max ratio of 4 can be changed by
+            initializing ``MinMaxLTTB`` with a different value for the ``minmax_ratio``
+            parameter. \n
             .. note:: This can be overridden within the :func:`add_trace` method.
         default_gap_handler: AbstractGapHandler, optional
             An instance which implements the AbstractGapHandler interface and
             will be used as default gap handler, by default ``MedDiffGapHandler``.
             ``MedDiffGapHandler`` will determine gaps by first calculating the median
             aggregated x difference and then thresholding the aggregated x delta on a
             multiple of this median difference.  \n
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 
 from ..aggregation import AbstractAggregator, MedDiffGapHandler, MinMaxLTTB
 from ..aggregation.aggregation_interface import DataPointSelector
 from ..aggregation.gap_handler_interface import AbstractGapHandler
 from ..aggregation.plotly_aggregator_parser import PlotlyAggregatorParser
 from .utils import round_number_str, round_td_str
 
-_hf_data_container = namedtuple("DataContainer", ["x", "y", "text", "hovertext"])
+# A high-frequency data container
+# NOTE: the attributes must all be valid trace attributes, with attribute levels
+# separated by an '_' (e.g., 'marker_color' is valid) as the
+# `_hf_data_container._asdict()` function is used in
+#  `AbstractFigureAggregator._construct_hf_data_dict`.
+_hf_data_container = namedtuple(
+    "DataContainer", ["x", "y", "text", "hovertext", "marker_size", "marker_color"]
+)
 
 
 class AbstractFigureAggregator(BaseFigure, ABC):
     """Abstract interface for data aggregation functionality for plotly figures."""
 
     _high_frequency_traces = ["scatter", "scattergl"]
 
@@ -71,16 +78,15 @@
             by default 1000.\n
             .. note::
                 * This can be overridden within the :func:`add_trace` method.
                 * If a trace withholds fewer datapoints than this parameter,
                   the data will *not* be aggregated.
         default_downsampler: AbstractAggregator
             An instance which implements the AbstractSeriesDownsampler interface and
-            will be used as default downsampler, by default ``EfficientLTTB`` with
-            _interleave_gaps_ set to True. \n
+            will be used as default downsampler, by default ``MinMaxLTTB``. \n
             .. note:: This can be overridden within the :func:`add_trace` method.
         default_gap_handler: GapHandler
             An instance which implements the AbstractGapHandler interface and will be
             used as default gap handler, by default ``MedDiffGapHandler``. \n
             .. note:: This can be overridden within the :func:`add_trace` method.
         resampled_trace_prefix_suffix: str, optional
             A tuple which contains the ``prefix`` and ``suffix``, respectively, which
@@ -352,22 +358,30 @@
         # NOTE: this can be removed once orjson supports f16
         trace["x"] = self._parse_dtype_orjson(agg_x)
         trace["y"] = self._parse_dtype_orjson(agg_y)
         trace["name"] = self._parse_trace_name(
             hf_trace_data, end_idx - start_idx, agg_x
         )
 
+        def _nest_dict_rec(k: str, v: any, out: dict) -> None:
+            """Recursively nest a dict based on the key whose '_' indicates level."""
+            k, *rest = k.split("_", 1)
+            if rest:
+                _nest_dict_rec(rest[0], v, out.setdefault(k, {}))
+            else:
+                out[k] = v
+
         # Check if (hover)text also needs to be downsampled
-        for k in ["text", "hovertext"]:
+        for k in ["text", "hovertext", "marker_size", "marker_color"]:
             k_val = hf_trace_data.get(k)
             if isinstance(k_val, (np.ndarray, pd.Series)):
                 assert isinstance(
                     hf_trace_data["downsampler"], DataPointSelector
                 ), "Only DataPointSelector can downsample non-data trace array props."
-                trace[k] = k_val[start_idx + indices]
+                _nest_dict_rec(k, k_val[start_idx + indices], trace)
             elif k_val is not None:
                 trace[k] = k_val
 
         return trace
 
     def _check_update_figure_dict(
         self,
@@ -532,14 +546,16 @@
     def _parse_get_trace_props(
         self,
         trace: BaseTraceType,
         hf_x: Iterable = None,
         hf_y: Iterable = None,
         hf_text: Iterable = None,
         hf_hovertext: Iterable = None,
+        hf_marker_size: Iterable = None,
+        hf_marker_color: Iterable = None,
         check_nans: bool = True,
     ) -> _hf_data_container:
         """Parse and capture the possibly high-frequency trace-props in a datacontainer.
 
         Parameters
         ----------
         trace : BaseTraceType
@@ -598,14 +614,34 @@
             hf_hovertext
             if hf_hovertext is not None
             else trace["hovertext"]
             if hasattr(trace, "hovertext") and trace["hovertext"] is not None
             else None
         )
 
+        hf_marker_size = (
+            trace["marker"]["size"]
+            if (
+                hf_marker_size is None
+                and hasattr(trace, "marker")
+                and "size" in trace["marker"]
+            )
+            else hf_marker_size
+        )
+
+        hf_marker_color = (
+            trace["marker"]["color"]
+            if (
+                hf_marker_color is None
+                and hasattr(trace, "marker")
+                and "color" in trace["marker"]
+            )
+            else hf_marker_color
+        )
+
         if trace["type"].lower() in self._high_frequency_traces:
             if hf_x is None:  # if no data as x or hf_x is passed
                 if hf_y.ndim != 0:  # if hf_y is an array
                     hf_x = pd.RangeIndex(0, len(hf_y))  # np.arange(len(hf_y))
                 else:  # if no data as y or hf_y is passed
                     hf_x = np.asarray(None)
 
@@ -684,16 +720,23 @@
                 trace["y"] = hf_y
 
             if hasattr(trace, "text"):
                 trace["text"] = hf_text
 
             if hasattr(trace, "hovertext"):
                 trace["hovertext"] = hf_hovertext
+            if hasattr(trace, "marker"):
+                if hasattr(trace.marker, "size"):
+                    trace.marker.size = hf_marker_size
+                if hasattr(trace.marker, "color"):
+                    trace.marker.color = hf_marker_color
 
-        return _hf_data_container(hf_x, hf_y, hf_text, hf_hovertext)
+        return _hf_data_container(
+            hf_x, hf_y, hf_text, hf_hovertext, hf_marker_size, hf_marker_color
+        )
 
     def _construct_hf_data_dict(
         self,
         dc: _hf_data_container,
         trace: BaseTraceType,
         downsampler: AbstractAggregator | None,
         gap_handler: AbstractGapHandler | None,
@@ -797,14 +840,16 @@
         gap_handler: AbstractGapHandler = None,
         limit_to_view: bool = False,
         # Use these if you want some speedups (and are working with really large data)
         hf_x: Iterable = None,
         hf_y: Iterable = None,
         hf_text: Union[str, Iterable] = None,
         hf_hovertext: Union[str, Iterable] = None,
+        hf_marker_size: Union[str, Iterable] = None,
+        hf_marker_color: Union[str, Iterable] = None,
         check_nans: bool = True,
         **trace_kwargs,
     ):
         """Add a trace to the figure.
 
         Parameters
         ----------
@@ -847,14 +892,20 @@
             trace its data.
         hf_text: Iterable, optional
             The original high frequency text. If set, this has priority over the trace
             its ``text`` argument.
         hf_hovertext: Iterable, optional
             The original high frequency hovertext. If set, this has priority over the
             trace its ```hovertext`` argument.
+        hf_marker_size: Iterable, optional
+            The original high frequency marker size. If set, this has priority over the
+            trace its ``marker.size`` argument.
+        hf_marker_color: Iterable, optional
+            The original high frequency marker color. If set, this has priority over the
+            trace its ``marker.color`` argument.
         check_nans: boolean, optional
             If set to True, the trace's data will be checked for NaNs - which will be
             removed. By default True.
             As this is a costly operation, it is recommended to set this parameter to
             False if you are sure that your data does not contain NaNs (or when the
             downsampler can handle NaNs, e.g., EveryNthPoint). This should considerably
             speed up the graph construction time.
@@ -926,15 +977,22 @@
         # key for comparison. If the trace already has a UUID, we will keep it.
         uuid_str = str(uuid4()) if trace.uid is None else trace.uid
         trace.uid = uuid_str
 
         # construct the hf_data_container
         # TODO in future version -> maybe regex on kwargs which start with `hf_`
         dc = self._parse_get_trace_props(
-            trace, hf_x, hf_y, hf_text, hf_hovertext, check_nans
+            trace,
+            hf_x,
+            hf_y,
+            hf_text,
+            hf_hovertext,
+            hf_marker_size,
+            hf_marker_color,
+            check_nans,
         )
 
         # These traces will determine the autoscale its RANGE!
         #   -> so also store when `limit_to_view` is set.
         if trace["type"].lower() in self._high_frequency_traces:
             n_samples = len(dc.x)
             if n_samples > max_out_s or limit_to_view:
@@ -952,14 +1010,16 @@
 
                 # Before we update the trace, we create a new pointer to that trace in
                 # which the downsampled data will be stored. This way, the original
                 # data of the trace to this `add_trace` method will not be altered.
                 # We copy (by reference) all the non-data properties of the trace in
                 # the new trace.
                 trace = trace._props  # convert the trace into a dict
+                # NOTE: there is no need to store `marker` property here.
+                # If needed, it will be added  to `trace` via `check_update_trace_data`
                 trace = {
                     k: trace[k] for k in set(trace.keys()).difference(set(dc._fields))
                 }
 
                 # NOTE:
                 # If all the raw data needs to be sent to the javascript, and the trace
                 # is high-frequency, this would take significant time!
@@ -967,20 +1027,20 @@
                 trace = self._check_update_trace_data(trace)
                 assert trace is not None
                 return super(AbstractFigureAggregator, self).add_traces(
                     [trace], **self._add_trace_to_add_traces_kwargs(trace_kwargs)
                 )
             else:
                 self._print(f"[i] NOT resampling {trace['name']} - len={n_samples}")
-                for k in dc._fields:
-                    setattr(trace, k, getattr(dc, k))
+                trace._process_kwargs(**{k: getattr(dc, k) for k in dc._fields})
                 return super(AbstractFigureAggregator, self).add_traces(
                     [trace], **self._add_trace_to_add_traces_kwargs(trace_kwargs)
                 )
-        return super(AbstractFigureAggregator, self).add_traces(
+
+        return super(self._figure_class, self).add_traces(
             [trace], **self._add_trace_to_add_traces_kwargs(trace_kwargs)
         )
 
     def add_traces(
         self,
         data: List[BaseTraceType | dict] | BaseTraceType | Dict,
         max_n_samples: None | List[int] | int = None,
@@ -1181,15 +1241,18 @@
         """
         self._clear_figure()
         self.__init__(
             figure=figure,
             convert_existing_traces=convert_existing_traces,
             default_n_shown_samples=self._global_n_shown_samples,
             default_downsampler=self._global_downsampler,
+            default_gap_handler=self._global_gap_handler,
             resampled_trace_prefix_suffix=(self._prefix, self._suffix),
+            show_mean_aggregation_size=self._show_mean_aggregation_size,
+            verbose=self._print_verbose,
         )
 
     def _parse_relayout(self, relayout_dict: dict) -> dict:
         """Update the relayout object so that the autorange will be set to None when
         there are xy-matches.
 
         Parameters
@@ -1296,15 +1359,15 @@
             return dash.no_update
 
         # -------------------- construct callback data --------------------------
         # 1. Create the layout data for the front-end
         layout_traces_list: List[dict] = [relayout_data]
 
         # 2. Create the additional trace data for the frond-end
-        relevant_keys = list(_hf_data_container._fields) + ["name"]
+        relevant_keys = list(_hf_data_container._fields) + ["name", "marker"]
         # Note that only updated trace-data will be sent to the client
         for idx in updated_trace_indices:
             trace = current_graph["data"][idx]
             # TODO: check if we can reduce even more
             trace_reduced = {k: trace[k] for k in relevant_keys if k in trace}
 
             # Store the index into the corresponding to-be-sent trace-data so
@@ -1352,14 +1415,15 @@
             "_hf_data",
             "_global_n_shown_samples",
             "_print_verbose",
             "_show_mean_aggregation_size",
             "_prefix",
             "_suffix",
             "_global_downsampler",
+            "_global_gap_handler",
         ]
 
     def __reduce__(self):
         """Overwrite the reduce method (which is used to support deep copying and
         pickling).
 
         Note
```

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/figure_resampler/utils.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc0/plotly_resampler/registering.py` & `plotly_resampler-0.9.0rc1/plotly_resampler/registering.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc0/pyproject.toml` & `plotly_resampler-0.9.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.9.0rc0"
+version = "0.9.0rc1"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
 documentation = "https://predict-idlab.github.io/plotly-resampler"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
@@ -64,37 +64,28 @@
 pyarrow = "^10.0"
 Sphinx = "^4.4.0"
 pydata-sphinx-theme = "^0.13.3"
 sphinx-autodoc-typehints = "^1.17.0"
 ipywidgets = "^7.7.1"
 memory-profiler = "^0.60.0"
 line-profiler = "^4.0"
-ruff = "^0.0.173"
+ruff = "^0.0.262"
 black = "^22.6.0"
-isort = "^5.10.1"
 pytest-lazy-fixture = "^0.6.3"
 # yep = "^0.4"  # c code profiling
 
 # Linting
 [tool.ruff]
+select = ["E", "F", "I"]
 line-length = 88
 ignore = ["E501"] # Never enforce `E501` (line length violations).
 [tool.ruff.per-file-ignores]
 "tests/test_registering.py" = ["F401", "F811"]
 "tests/test_serialization.py" = ["F401", "F811"]
 
 # Formatting
 [tool.black]
 line-length = 88
 
-# Sort imports
-[tool.isort]
-line_length = 88
-known_first_party = ["plotly_resampler"]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `plotly_resampler-0.9.0rc0/PKG-INFO` & `plotly_resampler-0.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotly-resampler
-Version: 0.9.0rc0
+Version: 0.9.0rc1
 Summary: Visualizing large time series with plotly
 Home-page: https://github.com/predict-idlab/plotly-resampler
 License: MIT
 Keywords: time-series,visualization,resampling,plotly,plotly-dash
 Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -197,15 +197,15 @@
   organization={IEEE}
 }
 ```
 
 ## Future work 🔨
 
 - [x] Support `.add_traces()` (currently only `.add_trace` is supported)
-- [ ] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
+- [x] Support `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/plotly-resampler/pull/148)
 - [x] Integrate with [tsdownsample](https://github.com/predict-idlab/tsdownsample) :racehorse:
 
 <br>
 
 ---
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc0 Summary:
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc1 Summary:
 Visualizing large time series with plotly Home-page: https://github.com/
 predict-idlab/plotly-resampler License: MIT Keywords: time-
 series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
@@ -122,13 +122,13 @@
 further with the developers, see issue [#49](https://github.com/predict-idlab/
 plotly-resampler/issues/49). ## Cite Paper (preprint): https://arxiv.org/abs/
 2206.08703 ```bibtex @inproceedings{van2022plotly, title={Plotly-resampler:
 Effective visual analytics for large time series}, author={Van Der Donckt,
 Jonas and Van Der Donckt, Jeroen and Deprost, Emiel and Van Hoecke, Sofie},
 booktitle={2022 IEEE Visualization and Visual Analytics (VIS)}, pages={21--25},
 year={2022}, organization={IEEE} } ``` ## Future work ð¨ - [x] Support
-`.add_traces()` (currently only `.add_trace` is supported) - [ ] Support
+`.add_traces()` (currently only `.add_trace` is supported) - [x] Support
 `hf_color` and `hf_markersize`, see [#148](https://github.com/predict-idlab/
 plotly-resampler/pull/148) - [x] Integrate with [tsdownsample](https://
 github.com/predict-idlab/tsdownsample) :racehorse:
 ---
         ð¤ Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost
```

