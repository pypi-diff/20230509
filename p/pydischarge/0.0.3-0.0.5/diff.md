# Comparing `tmp/pydischarge-0.0.3.tar.gz` & `tmp/pydischarge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydischarge-0.0.3.tar", last modified: Tue May  9 16:34:02 2023, max compression
+gzip compressed data, was "pydischarge-0.0.5.tar", last modified: Tue May  9 17:49:13 2023, max compression
```

## Comparing `pydischarge-0.0.3.tar` & `pydischarge-0.0.5.tar`

### file list

```diff
@@ -1,153 +1,441 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.191518 pydischarge-0.0.3/
--rw-rw-rw-   0        0        0       38 2023-05-09 16:05:10.000000 pydischarge-0.0.3/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.763519 pydischarge-0.0.3/.github/
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.835518 pydischarge-0.0.3/.github/workflows/
--rw-rw-rw-   0        0        0     5314 2023-05-09 16:05:10.000000 pydischarge-0.0.3/.github/workflows/conda.yml
--rw-rw-rw-   0        0        0     3051 2023-05-09 16:05:10.000000 pydischarge-0.0.3/.github/workflows/dependencies.yml
--rw-rw-rw-   0        0        0     3300 2023-05-09 16:09:20.000000 pydischarge-0.0.3/.github/workflows/dist.yml
--rw-rw-rw-   0        0        0      737 2023-05-09 16:09:53.000000 pydischarge-0.0.3/.github/workflows/documentation.yml
--rw-rw-rw-   0        0        0     1481 2023-05-02 15:35:55.000000 pydischarge-0.0.3/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      805 2023-05-09 16:05:10.000000 pydischarge-0.0.3/.gitignore
--rw-rw-rw-   0        0        0      142 2023-05-09 16:05:10.000000 pydischarge-0.0.3/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     4736 2023-05-09 16:05:10.000000 pydischarge-0.0.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35821 2023-05-02 15:35:55.000000 pydischarge-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      195 2023-05-09 16:05:10.000000 pydischarge-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3513 2023-05-09 16:34:02.190515 pydischarge-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2071 2023-05-09 16:05:10.000000 pydischarge-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.862518 pydischarge-0.0.3/docs/
--rw-rw-rw-   0        0        0      825 2023-05-09 16:20:07.000000 pydischarge-0.0.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.868517 pydischarge-0.0.3/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.871515 pydischarge-0.0.3/docs/_static/css/
--rw-rw-rw-   0        0        0     1366 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/_static/css/gwpy-sphinx.css
--rw-rw-rw-   0        0        0   174729 2023-05-09 13:06:08.000000 pydischarge-0.0.3/docs/_static/favicon.png
--rw-rw-rw-   0        0        0    15166 2023-05-02 15:35:55.000000 pydischarge-0.0.3/docs/_static/gwpy_white_24.png
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.769519 pydischarge-0.0.3/docs/_templates/
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.873518 pydischarge-0.0.3/docs/_templates/autoclass/
--rw-rw-rw-   0        0        0      915 2023-05-02 15:35:55.000000 pydischarge-0.0.3/docs/_templates/autoclass/class.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.882517 pydischarge-0.0.3/docs/_templates/autosummary/
--rw-rw-rw-   0        0        0      180 2023-05-02 15:35:55.000000 pydischarge-0.0.3/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0        0        0     1210 2023-05-02 15:35:55.000000 pydischarge-0.0.3/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0        0        0      744 2023-05-02 15:35:55.000000 pydischarge-0.0.3/docs/_templates/autosummary/module.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.885518 pydischarge-0.0.3/docs/astro/
--rw-rw-rw-   0        0        0      797 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/astro/index.rst
--rw-rw-rw-   0        0        0     2812 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/citing.rst.in
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.891518 pydischarge-0.0.3/docs/cli/
--rw-rw-rw-   0        0        0     5555 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/cli/examples.ini
--rw-rw-rw-   0        0        0     3036 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/cli/index.rst
--rw-rw-rw-   0        0        0    14000 2023-05-09 16:21:30.000000 pydischarge-0.0.3/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.894518 pydischarge-0.0.3/docs/detector/
--rw-rw-rw-   0        0        0     3372 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/detector/channel.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.897517 pydischarge-0.0.3/docs/dev/
--rw-rw-rw-   0        0        0     4047 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/dev/release.rst
--rw-rw-rw-   0        0        0     1690 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/env.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.775516 pydischarge-0.0.3/docs/examples/
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.901518 pydischarge-0.0.3/docs/examples/table/
--rw-rw-rw-   0        0        0       68 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.913517 pydischarge-0.0.3/docs/external/
--rw-rw-rw-   0        0        0     1206 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/external/framecpp.rst
--rw-rw-rw-   0        0        0     1034 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/external/framel.rst
--rw-rw-rw-   0        0        0     3310 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/external/lalsuite.rst
--rw-rw-rw-   0        0        0     1058 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/external/nds2.rst
--rw-rw-rw-   0        0        0     2730 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/index.rst
--rw-rw-rw-   0        0        0     1440 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/install.rst
--rw-rw-rw-   0        0        0     2825 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/overview.rst
--rw-rw-rw-   0        0        0    67943 2023-05-09 13:03:59.000000 pydischarge-0.0.3/docs/pdpy-docs-logo.png
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.937518 pydischarge-0.0.3/docs/plot/
--rw-rw-rw-   0        0        0     2751 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/colorbars.rst
--rw-rw-rw-   0        0        0     3201 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/colors.rst
--rw-rw-rw-   0        0        0      820 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/filter.rst
--rw-rw-rw-   0        0        0     2646 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/gps.rst
--rw-rw-rw-   0        0        0     3324 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/index.rst
--rw-rw-rw-   0        0        0     1943 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/legend.rst
--rw-rw-rw-   0        0        0     1441 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/plot/log.rst
--rw-rw-rw-   0        0        0     5080 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/references.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.951516 pydischarge-0.0.3/docs/segments/
--rw-rw-rw-   0        0        0     1577 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/segments/dqsegdb.rst
--rw-rw-rw-   0        0        0     7113 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/segments/index.rst
--rw-rw-rw-   0        0        0     7013 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/segments/io.rst
--rw-rw-rw-   0        0        0     2191 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/segments/thresholding.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.956519 pydischarge-0.0.3/docs/signal/
--rw-rw-rw-   0        0        0     4678 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/signal/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.958516 pydischarge-0.0.3/docs/spectrogram/
--rw-rw-rw-   0        0        0     3988 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/spectrogram/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.969519 pydischarge-0.0.3/docs/spectrum/
--rw-rw-rw-   0        0        0      559 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/spectrum/filtering.rst
--rw-rw-rw-   0        0        0     3931 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/spectrum/index.rst
--rw-rw-rw-   0        0        0     5204 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/spectrum/io.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.993516 pydischarge-0.0.3/docs/table/
--rw-rw-rw-   0        0        0       65 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-rw-rw-   0        0        0     7597 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/filter.rst
--rw-rw-rw-   0        0        0     1013 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/histogram.rst
--rw-rw-rw-   0        0        0     1610 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/index.rst
--rw-rw-rw-   0        0        0    31631 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/io.rst
--rw-rw-rw-   0        0        0     1851 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/plot.rst
--rw-rw-rw-   0        0        0     2242 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/table/rate.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:01.996517 pydischarge-0.0.3/docs/time/
--rw-rw-rw-   0        0        0     1183 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/time/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.017519 pydischarge-0.0.3/docs/timeseries/
--rw-rw-rw-   0        0        0    12005 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/timeseries/datafind.rst
--rw-rw-rw-   0        0        0     2889 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/timeseries/index.rst
--rw-rw-rw-   0        0        0    11214 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/timeseries/io.rst
--rw-rw-rw-   0        0        0     2860 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/timeseries/opendata.rst
--rw-rw-rw-   0        0        0     3206 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/timeseries/plot.rst
--rw-rw-rw-   0        0        0     8769 2023-05-09 16:05:10.000000 pydischarge-0.0.3/docs/timeseries/statevector.rst
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.020517 pydischarge-0.0.3/examples/
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.047517 pydischarge-0.0.3/examples/frequencyseries/
--rw-rw-rw-   0        0        0     2699 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/coherence.py
--rw-rw-rw-   0        0        0     2203 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/hoff.py
--rw-rw-rw-   0        0        0      282 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/index.rst
--rw-rw-rw-   0        0        0     2719 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/inject.py
--rw-rw-rw-   0        0        0     2966 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/percentiles.py
--rw-rw-rw-   0        0        0     2935 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/rayleigh.py
--rw-rw-rw-   0        0        0     2336 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/transfer_function.py
--rw-rw-rw-   0        0        0     2757 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/frequencyseries/variance.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.059520 pydischarge-0.0.3/examples/miscellaneous/
--rw-rw-rw-   0        0        0      236 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/miscellaneous/index.rst
--rw-rw-rw-   0        0        0     3502 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/miscellaneous/open-data-spectrogram.py
--rw-rw-rw-   0        0        0     2463 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/miscellaneous/range-spectrogram.py
--rw-rw-rw-   0        0        0     2603 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/miscellaneous/range-timeseries.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.065517 pydischarge-0.0.3/examples/segments/
--rw-rw-rw-   0        0        0      176 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/segments/index.rst
--rw-rw-rw-   0        0        0     2527 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/segments/open-data.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.074517 pydischarge-0.0.3/examples/signal/
--rw-rw-rw-   0        0        0     5913 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/signal/gw150914.py
--rw-rw-rw-   0        0        0      198 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/signal/index.rst
--rw-rw-rw-   0        0        0     3279 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/signal/qscan.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.095519 pydischarge-0.0.3/examples/spectrogram/
--rw-rw-rw-   0        0        0     2517 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/spectrogram/coherence.py
--rw-rw-rw-   0        0        0      231 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/spectrogram/index.rst
--rw-rw-rw-   0        0        0     2768 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/spectrogram/plot.py
--rw-rw-rw-   0        0        0     2746 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/spectrogram/ratio.py
--rw-rw-rw-   0        0        0     2240 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/spectrogram/rayleigh.py
--rw-rw-rw-   0        0        0     3007 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/spectrogram/spectrogram2.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.117519 pydischarge-0.0.3/examples/table/
--rw-rw-rw-   0        0        0       65 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-rw-rw-   0        0        0     1695 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/histogram.py
--rw-rw-rw-   0        0        0      220 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/index.rst
--rw-rw-rw-   0        0        0     2431 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/rate.py
--rw-rw-rw-   0        0        0     2564 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/rate_binned.py
--rw-rw-rw-   0        0        0     2133 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/scatter.py
--rw-rw-rw-   0        0        0     2386 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/table/tiles.py
--rw-rw-rw-   0        0        0     3923 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/test_examples.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.148518 pydischarge-0.0.3/examples/timeseries/
--rw-rw-rw-   0        0        0     2693 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/blrms.py
--rw-rw-rw-   0        0        0     4356 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/correlate.py
--rw-rw-rw-   0        0        0     2946 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/filter.py
--rw-rw-rw-   0        0        0      272 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/index.rst
--rw-rw-rw-   0        0        0     2761 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/inject.py
--rw-rw-rw-   0        0        0     2594 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/public.py
--rw-rw-rw-   0        0        0     3960 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/pycbc-snr.py
--rw-rw-rw-   0        0        0     2718 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/qscan.py
--rw-rw-rw-   0        0        0     2309 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/statevector.py
--rw-rw-rw-   0        0        0     2586 2023-05-09 16:05:10.000000 pydischarge-0.0.3/examples/timeseries/whiten.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.156516 pydischarge-0.0.3/pydischarge/
--rw-rw-rw-   0        0        0      164 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:34:02.188516 pydischarge-0.0.3/pydischarge.egg-info/
--rw-rw-rw-   0        0        0     3513 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3218 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      793 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-09 16:34:01.000000 pydischarge-0.0.3/pydischarge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5154 2023-05-09 16:05:10.000000 pydischarge-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 16:34:02.192518 pydischarge-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.255703 pydischarge-0.0.5/
+-rw-rw-rw-   0        0        0      578 2023-05-09 17:16:48.000000 pydischarge-0.0.5/.codeclimate.yml
+-rw-rw-rw-   0        0        0      519 2023-05-09 17:09:20.000000 pydischarge-0.0.5/.codecov.yml
+-rw-rw-rw-   0        0        0      520 2023-05-09 17:16:48.000000 pydischarge-0.0.5/.flake8
+-rw-rw-rw-   0        0        0       38 2023-05-09 17:16:48.000000 pydischarge-0.0.5/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.207558 pydischarge-0.0.5/.github/
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.398597 pydischarge-0.0.5/.github/workflows/
+-rw-rw-rw-   0        0        0     5314 2023-05-09 17:16:50.000000 pydischarge-0.0.5/.github/workflows/conda.yml
+-rw-rw-rw-   0        0        0     3051 2023-05-09 17:16:50.000000 pydischarge-0.0.5/.github/workflows/dependencies.yml
+-rw-rw-rw-   0        0        0     3300 2023-05-09 17:16:50.000000 pydischarge-0.0.5/.github/workflows/dist.yml
+-rw-rw-rw-   0        0        0      748 2023-05-09 17:47:39.000000 pydischarge-0.0.5/.github/workflows/documentation.yaml
+-rw-rw-rw-   0        0        0     1481 2023-05-09 17:09:20.000000 pydischarge-0.0.5/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      797 2023-05-09 17:16:48.000000 pydischarge-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0       47 2023-05-09 17:09:20.000000 pydischarge-0.0.5/.pep8speaks.yml
+-rw-rw-rw-   0        0        0      142 2023-05-09 17:15:30.000000 pydischarge-0.0.5/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     4736 2023-05-09 17:16:48.000000 pydischarge-0.0.5/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35821 2023-05-09 17:09:20.000000 pydischarge-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-05-09 17:16:48.000000 pydischarge-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3458 2023-05-09 17:49:13.254701 pydischarge-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2030 2023-05-09 17:16:48.000000 pydischarge-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.435557 pydischarge-0.0.5/docs/
+-rw-rw-rw-   0        0        0      825 2023-05-09 17:16:49.000000 pydischarge-0.0.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.439557 pydischarge-0.0.5/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.441559 pydischarge-0.0.5/docs/_static/css/
+-rw-rw-rw-   0        0        0     1366 2023-05-09 17:15:34.000000 pydischarge-0.0.5/docs/_static/css/pydischarge-sphinx.css
+-rw-rw-rw-   0        0        0    19634 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/_static/favicon.png
+-rw-rw-rw-   0        0        0    15166 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/_static/pydischarge_white_24.png
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.216560 pydischarge-0.0.5/docs/_templates/
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.450557 pydischarge-0.0.5/docs/_templates/autoclass/
+-rw-rw-rw-   0        0        0      915 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/_templates/autoclass/class.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.463557 pydischarge-0.0.5/docs/_templates/autosummary/
+-rw-rw-rw-   0        0        0      180 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/_templates/autosummary/base.rst
+-rw-rw-rw-   0        0        0     1210 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/_templates/autosummary/class.rst
+-rw-rw-rw-   0        0        0      744 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/_templates/autosummary/module.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.466556 pydischarge-0.0.5/docs/astro/
+-rw-rw-rw-   0        0        0      797 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/astro/index.rst
+-rw-rw-rw-   0        0        0     2812 2023-05-09 17:16:49.000000 pydischarge-0.0.5/docs/citing.rst.in
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.479558 pydischarge-0.0.5/docs/cli/
+-rw-rw-rw-   0        0        0     5555 2023-05-09 17:16:50.000000 pydischarge-0.0.5/docs/cli/examples.ini
+-rw-rw-rw-   0        0        0     3036 2023-05-09 17:16:50.000000 pydischarge-0.0.5/docs/cli/index.rst
+-rw-rw-rw-   0        0        0    14056 2023-05-09 17:24:42.000000 pydischarge-0.0.5/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.482558 pydischarge-0.0.5/docs/detector/
+-rw-rw-rw-   0        0        0     3372 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/detector/channel.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.484557 pydischarge-0.0.5/docs/dev/
+-rw-rw-rw-   0        0        0     4026 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/dev/release.rst
+-rw-rw-rw-   0        0        0     1718 2023-05-09 17:24:10.000000 pydischarge-0.0.5/docs/env.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.225566 pydischarge-0.0.5/docs/examples/
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.486561 pydischarge-0.0.5/docs/examples/table/
+-rw-rw-rw-   0        0        0       68 2023-05-09 17:16:50.000000 pydischarge-0.0.5/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.496556 pydischarge-0.0.5/docs/external/
+-rw-rw-rw-   0        0        0     1206 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/external/framecpp.rst
+-rw-rw-rw-   0        0        0     1034 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/external/framel.rst
+-rw-rw-rw-   0        0        0     3310 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/external/lalsuite.rst
+-rw-rw-rw-   0        0        0     1058 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/external/nds2.rst
+-rw-rw-rw-   0        0        0     2730 2023-05-09 17:16:49.000000 pydischarge-0.0.5/docs/index.rst
+-rw-rw-rw-   0        0        0     1440 2023-05-09 17:24:37.000000 pydischarge-0.0.5/docs/install.rst
+-rw-rw-rw-   0        0        0     2825 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/overview.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.513558 pydischarge-0.0.5/docs/plot/
+-rw-rw-rw-   0        0        0     2751 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/plot/colorbars.rst
+-rw-rw-rw-   0        0        0     3201 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/plot/colors.rst
+-rw-rw-rw-   0        0        0      820 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/plot/filter.rst
+-rw-rw-rw-   0        0        0     2646 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/plot/gps.rst
+-rw-rw-rw-   0        0        0     3324 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/plot/index.rst
+-rw-rw-rw-   0        0        0     1943 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/plot/legend.rst
+-rw-rw-rw-   0        0        0     1441 2023-05-09 17:16:50.000000 pydischarge-0.0.5/docs/plot/log.rst
+-rw-rw-rw-   0        0        0    52297 2023-05-09 17:09:20.000000 pydischarge-0.0.5/docs/pydischarge-docs-logo.png
+-rw-rw-rw-   0        0        0     5073 2023-05-09 17:16:49.000000 pydischarge-0.0.5/docs/references.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.522556 pydischarge-0.0.5/docs/segments/
+-rw-rw-rw-   0        0        0     1577 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/segments/dqsegdb.rst
+-rw-rw-rw-   0        0        0     7113 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/segments/index.rst
+-rw-rw-rw-   0        0        0     7013 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/segments/io.rst
+-rw-rw-rw-   0        0        0     2191 2023-05-09 17:16:50.000000 pydischarge-0.0.5/docs/segments/thresholding.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.524559 pydischarge-0.0.5/docs/signal/
+-rw-rw-rw-   0        0        0     4678 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/signal/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.529559 pydischarge-0.0.5/docs/spectrogram/
+-rw-rw-rw-   0        0        0     3988 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/spectrogram/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.536557 pydischarge-0.0.5/docs/spectrum/
+-rw-rw-rw-   0        0        0      559 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/spectrum/filtering.rst
+-rw-rw-rw-   0        0        0     3931 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/spectrum/index.rst
+-rw-rw-rw-   0        0        0     5204 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/spectrum/io.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.604558 pydischarge-0.0.5/docs/table/
+-rw-rw-rw-   0        0        0       65 2023-05-09 17:16:49.000000 pydischarge-0.0.5/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-rw-rw-   0        0        0     7597 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/table/filter.rst
+-rw-rw-rw-   0        0        0     1013 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/table/histogram.rst
+-rw-rw-rw-   0        0        0     1610 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/table/index.rst
+-rw-rw-rw-   0        0        0    31631 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/table/io.rst
+-rw-rw-rw-   0        0        0     1851 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/table/plot.rst
+-rw-rw-rw-   0        0        0     2242 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/table/rate.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.606556 pydischarge-0.0.5/docs/time/
+-rw-rw-rw-   0        0        0     1183 2023-05-09 17:17:14.000000 pydischarge-0.0.5/docs/time/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.625560 pydischarge-0.0.5/docs/timeseries/
+-rw-rw-rw-   0        0        0    12005 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/timeseries/datafind.rst
+-rw-rw-rw-   0        0        0     2889 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/timeseries/index.rst
+-rw-rw-rw-   0        0        0    11207 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/timeseries/io.rst
+-rw-rw-rw-   0        0        0     2860 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/timeseries/opendata.rst
+-rw-rw-rw-   0        0        0     3206 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/timeseries/plot.rst
+-rw-rw-rw-   0        0        0     8769 2023-05-09 17:17:13.000000 pydischarge-0.0.5/docs/timeseries/statevector.rst
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.628558 pydischarge-0.0.5/examples/
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.682557 pydischarge-0.0.5/examples/frequencyseries/
+-rw-rw-rw-   0        0        0     2699 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/coherence.py
+-rw-rw-rw-   0        0        0     2203 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/hoff.py
+-rw-rw-rw-   0        0        0      282 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/index.rst
+-rw-rw-rw-   0        0        0     2719 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/inject.py
+-rw-rw-rw-   0        0        0     2966 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/percentiles.py
+-rw-rw-rw-   0        0        0     2935 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/rayleigh.py
+-rw-rw-rw-   0        0        0     2336 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/transfer_function.py
+-rw-rw-rw-   0        0        0     2757 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/frequencyseries/variance.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.693557 pydischarge-0.0.5/examples/miscellaneous/
+-rw-rw-rw-   0        0        0      236 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/miscellaneous/index.rst
+-rw-rw-rw-   0        0        0     3502 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/miscellaneous/open-data-spectrogram.py
+-rw-rw-rw-   0        0        0     2463 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/miscellaneous/range-spectrogram.py
+-rw-rw-rw-   0        0        0     2603 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/miscellaneous/range-timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.699163 pydischarge-0.0.5/examples/segments/
+-rw-rw-rw-   0        0        0      176 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/segments/index.rst
+-rw-rw-rw-   0        0        0     2527 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/segments/open-data.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.718644 pydischarge-0.0.5/examples/signal/
+-rw-rw-rw-   0        0        0     5913 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/signal/gw150914.py
+-rw-rw-rw-   0        0        0      198 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/signal/index.rst
+-rw-rw-rw-   0        0        0     3279 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/signal/qscan.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.738865 pydischarge-0.0.5/examples/spectrogram/
+-rw-rw-rw-   0        0        0     2517 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/spectrogram/coherence.py
+-rw-rw-rw-   0        0        0      231 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/spectrogram/index.rst
+-rw-rw-rw-   0        0        0     2768 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/spectrogram/plot.py
+-rw-rw-rw-   0        0        0     2746 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/spectrogram/ratio.py
+-rw-rw-rw-   0        0        0     2240 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/spectrogram/rayleigh.py
+-rw-rw-rw-   0        0        0     3007 2023-05-09 17:16:49.000000 pydischarge-0.0.5/examples/spectrogram/spectrogram2.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.760865 pydischarge-0.0.5/examples/table/
+-rw-rw-rw-   0        0        0       65 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-rw-rw-   0        0        0     1695 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/histogram.py
+-rw-rw-rw-   0        0        0      220 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/index.rst
+-rw-rw-rw-   0        0        0     2431 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/rate.py
+-rw-rw-rw-   0        0        0     2564 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/rate_binned.py
+-rw-rw-rw-   0        0        0     2133 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/scatter.py
+-rw-rw-rw-   0        0        0     2386 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/table/tiles.py
+-rw-rw-rw-   0        0        0     3923 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.789324 pydischarge-0.0.5/examples/timeseries/
+-rw-rw-rw-   0        0        0     2693 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/blrms.py
+-rw-rw-rw-   0        0        0     4356 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/correlate.py
+-rw-rw-rw-   0        0        0     2946 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/filter.py
+-rw-rw-rw-   0        0        0      272 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/index.rst
+-rw-rw-rw-   0        0        0     2761 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/inject.py
+-rw-rw-rw-   0        0        0     2594 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/public.py
+-rw-rw-rw-   0        0        0     3960 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/pycbc-snr.py
+-rw-rw-rw-   0        0        0     2718 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/qscan.py
+-rw-rw-rw-   0        0        0     2309 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/statevector.py
+-rw-rw-rw-   0        0        0     2586 2023-05-09 17:16:48.000000 pydischarge-0.0.5/examples/timeseries/whiten.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.798322 pydischarge-0.0.5/pydischarge/
+-rw-rw-rw-   0        0        0     1623 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-05-09 17:49:10.000000 pydischarge-0.0.5/pydischarge/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.862325 pydischarge-0.0.5/pydischarge/astro/
+-rw-rw-rw-   0        0        0     2051 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/astro/__init__.py
+-rw-rw-rw-   0        0        0    25906 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/astro/range.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.868323 pydischarge-0.0.5/pydischarge/astro/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/astro/tests/__init__.py
+-rw-rw-rw-   0        0        0     6325 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/astro/tests/test_range.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.904323 pydischarge-0.0.5/pydischarge/cli/
+-rw-rw-rw-   0        0        0     1505 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/__init__.py
+-rw-rw-rw-   0        0        0    36334 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/cliproduct.py
+-rw-rw-rw-   0        0        0     4207 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/coherence.py
+-rw-rw-rw-   0        0        0     3482 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/coherencegram.py
+-rw-rw-rw-   0        0        0     9432 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/qtransform.py
+-rw-rw-rw-   0        0        0     7370 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/spectrogram.py
+-rw-rw-rw-   0        0        0     5098 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/spectrum.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.939323 pydischarge-0.0.5/pydischarge/cli/tests/
+-rw-rw-rw-   0        0        0      799 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/__init__.py
+-rw-rw-rw-   0        0        0    11211 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/base.py
+-rw-rw-rw-   0        0        0     1427 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_coherence.py
+-rw-rw-rw-   0        0        0     1660 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_coherencegram.py
+-rw-rw-rw-   0        0        0     1866 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_pydischarge_plot.py
+-rw-rw-rw-   0        0        0     3026 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_qtransform.py
+-rw-rw-rw-   0        0        0     1591 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_spectrogram.py
+-rw-rw-rw-   0        0        0     1494 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_spectrum.py
+-rw-rw-rw-   0        0        0     1350 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_timeseries.py
+-rw-rw-rw-   0        0        0     2092 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/cli/tests/test_transferfunction.py
+-rw-rw-rw-   0        0        0     4141 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/timeseries.py
+-rw-rw-rw-   0        0        0    10108 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/cli/transferfunction.py
+-rw-rw-rw-   0        0        0     1737 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.947322 pydischarge-0.0.5/pydischarge/detector/
+-rw-rw-rw-   0        0        0     2365 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/__init__.py
+-rw-rw-rw-   0        0        0    27830 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/channel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.957322 pydischarge-0.0.5/pydischarge/detector/io/
+-rw-rw-rw-   0        0        0     1093 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/detector/io/__init__.py
+-rw-rw-rw-   0        0        0     3338 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/io/cis.py
+-rw-rw-rw-   0        0        0     5902 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/io/clf.py
+-rw-rw-rw-   0        0        0     6159 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/detector/io/omega.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.974322 pydischarge-0.0.5/pydischarge/detector/tests/
+-rw-rw-rw-   0        0        0      804 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/tests/__init__.py
+-rw-rw-rw-   0        0        0    19115 2023-05-09 17:24:11.000000 pydischarge-0.0.5/pydischarge/detector/tests/test_channel.py
+-rw-rw-rw-   0        0        0     2664 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/tests/test_units.py
+-rw-rw-rw-   0        0        0     7382 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/detector/units.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.998322 pydischarge-0.0.5/pydischarge/frequencyseries/
+-rw-rw-rw-   0        0        0     1052 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/frequencyseries/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/_fdcommon.py
+-rw-rw-rw-   0        0        0    14844 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/frequencyseries.py
+-rw-rw-rw-   0        0        0    12357 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/hist.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.009323 pydischarge-0.0.5/pydischarge/frequencyseries/io/
+-rw-rw-rw-   0        0        0      970 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/io/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/io/ascii.py
+-rw-rw-rw-   0        0        0     1092 2023-05-09 17:15:33.000000 pydischarge-0.0.5/pydischarge/frequencyseries/io/hdf5.py
+-rw-rw-rw-   0        0        0     1214 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/io/ligolw.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.020323 pydischarge-0.0.5/pydischarge/frequencyseries/tests/
+-rw-rw-rw-   0        0        0      811 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/frequencyseries/tests/__init__.py
+-rw-rw-rw-   0        0        0    11385 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/frequencyseries/tests/test_frequencyseries.py
+-rw-rw-rw-   0        0        0     4162 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/frequencyseries/tests/test_hist.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.112323 pydischarge-0.0.5/pydischarge/io/
+-rw-rw-rw-   0        0        0      881 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/io/__init__.py
+-rw-rw-rw-   0        0        0     4394 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/io/_framecpp.py
+-rw-rw-rw-   0        0        0    15275 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/cache.py
+-rw-rw-rw-   0        0        0    19137 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/datafind.py
+-rw-rw-rw-   0        0        0     8751 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/ffldatafind.py
+-rw-rw-rw-   0        0        0    19783 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/gwf.py
+-rw-rw-rw-   0        0        0     5461 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/io/hdf5.py
+-rw-rw-rw-   0        0        0     7184 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/kerberos.py
+-rw-rw-rw-   0        0        0    22961 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/ligolw.py
+-rw-rw-rw-   0        0        0     4277 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/mp.py
+-rw-rw-rw-   0        0        0    20037 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/nds2.py
+-rw-rw-rw-   0        0        0     3651 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/io/registry.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.138323 pydischarge-0.0.5/pydischarge/io/tests/
+-rw-rw-rw-   0        0        0      798 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/__init__.py
+-rw-rw-rw-   0        0        0     8955 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_cache.py
+-rw-rw-rw-   0        0        0    11022 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_datafind.py
+-rw-rw-rw-   0        0        0     6581 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_ffldatafind.py
+-rw-rw-rw-   0        0        0     4399 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_gwf.py
+-rw-rw-rw-   0        0        0     6827 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_kerberos.py
+-rw-rw-rw-   0        0        0    11073 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_ligolw.py
+-rw-rw-rw-   0        0        0     3440 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_mp.py
+-rw-rw-rw-   0        0        0    12794 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_nds2.py
+-rw-rw-rw-   0        0        0     4157 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/tests/test_utils.py
+-rw-rw-rw-   0        0        0     7625 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/io/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.248323 pydischarge-0.0.5/pydischarge/plot/
+-rw-rw-rw-   0        0        0     1733 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/plot/__init__.py
+-rw-rw-rw-   0        0        0    23909 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/axes.py
+-rw-rw-rw-   0        0        0     9059 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/bode.py
+-rw-rw-rw-   0        0        0     7290 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/plot/colorbar.py
+-rw-rw-rw-   0        0        0     3545 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/plot/colors.py
+-rw-rw-rw-   0        0        0    17263 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/plot/gps.py
+-rw-rw-rw-   0        0        0     1723 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/legend.py
+-rw-rw-rw-   0        0        0     5222 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/plot/log.py
+-rw-rw-rw-   0        0        0    22499 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/plot.py
+-rw-rw-rw-   0        0        0     5121 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/plot/rc.py
+-rw-rw-rw-   0        0        0    17597 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/segments.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.295325 pydischarge-0.0.5/pydischarge/plot/tests/
+-rw-rw-rw-   0        0        0      795 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/__init__.py
+-rw-rw-rw-   0        0        0    11913 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_axes.py
+-rw-rw-rw-   0        0        0     3474 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_bode.py
+-rw-rw-rw-   0        0        0     1979 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_colors.py
+-rw-rw-rw-   0        0        0     5690 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_gps.py
+-rw-rw-rw-   0        0        0     2802 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_log.py
+-rw-rw-rw-   0        0        0     4562 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_plot.py
+-rw-rw-rw-   0        0        0     1329 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_rc.py
+-rw-rw-rw-   0        0        0     5636 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_segments.py
+-rw-rw-rw-   0        0        0     2483 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_tex.py
+-rw-rw-rw-   0        0        0     1367 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_text.py
+-rw-rw-rw-   0        0        0     1708 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/test_utils.py
+-rw-rw-rw-   0        0        0     2031 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tests/utils.py
+-rw-rw-rw-   0        0        0     5000 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/plot/tex.py
+-rw-rw-rw-   0        0        0     2092 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/plot/text.py
+-rw-rw-rw-   0        0        0     1451 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/plot/units.py
+-rw-rw-rw-   0        0        0     1758 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/plot/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.305324 pydischarge-0.0.5/pydischarge/segments/
+-rw-rw-rw-   0        0        0     1259 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/segments/__init__.py
+-rw-rw-rw-   0        0        0    54360 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/flag.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.382324 pydischarge-0.0.5/pydischarge/segments/io/
+-rw-rw-rw-   0        0        0     1069 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/io/__init__.py
+-rw-rw-rw-   0        0        0    11429 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/segments/io/hdf5.py
+-rw-rw-rw-   0        0        0     3168 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/segments/io/json.py
+-rw-rw-rw-   0        0        0     5096 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/io/ligolw.py
+-rw-rw-rw-   0        0        0     5207 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/io/segwizard.py
+-rw-rw-rw-   0        0        0     9348 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/segments.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.402323 pydischarge-0.0.5/pydischarge/segments/tests/
+-rw-rw-rw-   0        0        0      804 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/tests/__init__.py
+-rw-rw-rw-   0        0        0    30642 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/segments/tests/test_flag.py
+-rw-rw-rw-   0        0        0     5564 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/segments/tests/test_segments.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.417323 pydischarge-0.0.5/pydischarge/signal/
+-rw-rw-rw-   0        0        0     1033 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/fft.py
+-rw-rw-rw-   0        0        0    21073 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/filter_design.py
+-rw-rw-rw-   0        0        0    25296 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/qtransform.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.448323 pydischarge-0.0.5/pydischarge/signal/spectral/
+-rw-rw-rw-   0        0        0     1938 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/spectral/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_lal.py
+-rw-rw-rw-   0        0        0     1932 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_median_mean.py
+-rw-rw-rw-   0        0        0     3752 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_pycbc.py
+-rw-rw-rw-   0        0        0     2456 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_registry.py
+-rw-rw-rw-   0        0        0     6797 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_scipy.py
+-rw-rw-rw-   0        0        0    14757 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_ui.py
+-rw-rw-rw-   0        0        0     1751 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/signal/spectral/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.482324 pydischarge-0.0.5/pydischarge/signal/tests/
+-rw-rw-rw-   0        0        0      802 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/__init__.py
+-rw-rw-rw-   0        0        0     4539 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_filter_design.py
+-rw-rw-rw-   0        0        0     4170 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_qtransform.py
+-rw-rw-rw-   0        0        0     3684 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_lal.py
+-rw-rw-rw-   0        0        0     2314 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_median_mean.py
+-rw-rw-rw-   0        0        0     2346 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_pycbc.py
+-rw-rw-rw-   0        0        0     1537 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_registry.py
+-rw-rw-rw-   0        0        0     1961 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_scipy.py
+-rw-rw-rw-   0        0        0     3203 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_ui.py
+-rw-rw-rw-   0        0        0     1532 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_spectral_utils.py
+-rw-rw-rw-   0        0        0     2859 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/tests/test_window.py
+-rw-rw-rw-   0        0        0     6179 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/signal/window.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.506323 pydischarge-0.0.5/pydischarge/spectrogram/
+-rw-rw-rw-   0        0        0      973 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/spectrogram/__init__.py
+-rw-rw-rw-   0        0        0     5972 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/spectrogram/coherence.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.512322 pydischarge-0.0.5/pydischarge/spectrogram/io/
+-rw-rw-rw-   0        0        0      900 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/spectrogram/io/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/spectrogram/io/hdf5.py
+-rw-rw-rw-   0        0        0    22994 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/spectrogram/spectrogram.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.518324 pydischarge-0.0.5/pydischarge/spectrogram/tests/
+-rw-rw-rw-   0        0        0      807 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/spectrogram/tests/__init__.py
+-rw-rw-rw-   0        0        0     6830 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/spectrogram/tests/test_spectrogram.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.550324 pydischarge-0.0.5/pydischarge/table/
+-rw-rw-rw-   0        0        0     1494 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/__init__.py
+-rw-rw-rw-   0        0        0     8211 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/filter.py
+-rw-rw-rw-   0        0        0     2768 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/filters.py
+-rw-rw-rw-   0        0        0     8467 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/gravityspy.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.633323 pydischarge-0.0.5/pydischarge/table/io/
+-rw-rw-rw-   0        0        0     1635 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/__init__.py
+-rw-rw-rw-   0        0        0     3965 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/table/io/cwb.py
+-rw-rw-rw-   0        0        0     4864 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/fetch.py
+-rw-rw-rw-   0        0        0     4833 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/gravityspy.py
+-rw-rw-rw-   0        0        0     8693 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/io/gstlal.py
+-rw-rw-rw-   0        0        0     5645 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/io/gwf.py
+-rw-rw-rw-   0        0        0     5391 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/table/io/hacr.py
+-rw-rw-rw-   0        0        0    14039 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/io/ligolw.py
+-rw-rw-rw-   0        0        0     4625 2023-05-09 17:15:32.000000 pydischarge-0.0.5/pydischarge/table/io/losc.py
+-rw-rw-rw-   0        0        0     2726 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/omega.py
+-rw-rw-rw-   0        0        0     1400 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/omicron.py
+-rw-rw-rw-   0        0        0     9239 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/io/pycbc.py
+-rw-rw-rw-   0        0        0     3463 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/root.py
+-rw-rw-rw-   0        0        0     4008 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/io/snax.py
+-rw-rw-rw-   0        0        0     3195 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/sql.py
+-rw-rw-rw-   0        0        0     3335 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/table/io/utils.py
+-rw-rw-rw-   0        0        0    27321 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.652323 pydischarge-0.0.5/pydischarge/table/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/tests/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/tests/test_gravityspy.py
+-rw-rw-rw-   0        0        0     8230 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/tests/test_io_gstlal.py
+-rw-rw-rw-   0        0        0     2986 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/tests/test_io_ligolw.py
+-rw-rw-rw-   0        0        0     8666 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/tests/test_io_pycbc.py
+-rw-rw-rw-   0        0        0    31317 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/table/tests/test_table.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.681323 pydischarge-0.0.5/pydischarge/testing/
+-rw-rw-rw-   0        0        0      800 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.714324 pydischarge-0.0.5/pydischarge/testing/data/
+-rw-rw-rw-   0        0        0    58124 2023-05-09 17:09:21.000000 pydischarge-0.0.5/pydischarge/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-rw-rw-   0        0        0   377295 2023-05-09 17:09:21.000000 pydischarge-0.0.5/pydischarge/testing/data/HLV-HW100916-968654552-1.gwf
+-rw-rw-rw-   0        0        0   382679 2023-05-09 17:09:21.000000 pydischarge-0.0.5/pydischarge/testing/data/HLV-HW100916-968654552-1.hdf
+-rw-rw-rw-   0        0        0       63 2023-05-09 17:09:21.000000 pydischarge-0.0.5/pydischarge/testing/data/X1-PYDISCHARGE_TEST_SEGMENTS-0-10.txt
+-rw-rw-rw-   0        0        0      564 2023-05-09 17:09:21.000000 pydischarge-0.0.5/pydischarge/testing/data/X1-PYDISCHARGE_TEST_SEGMENTS-0-10.xml.gz
+-rw-rw-rw-   0        0        0     2921 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/testing/errors.py
+-rw-rw-rw-   0        0        0     3949 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/testing/fixtures.py
+-rw-rw-rw-   0        0        0     1595 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/testing/marks.py
+-rw-rw-rw-   0        0        0     4299 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/testing/mocks.py
+-rw-rw-rw-   0        0        0    12211 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/testing/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.736325 pydischarge-0.0.5/pydischarge/time/
+-rw-rw-rw-   0        0        0     1897 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/time/__init__.py
+-rw-rw-rw-   0        0        0     2387 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/time/__main__.py
+-rw-rw-rw-   0        0        0     9344 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/time/_tconvert.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.753323 pydischarge-0.0.5/pydischarge/time/tests/
+-rw-rw-rw-   0        0        0      800 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/time/tests/__init__.py
+-rw-rw-rw-   0        0        0     1452 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/time/tests/test_main.py
+-rw-rw-rw-   0        0        0     6007 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/time/tests/test_time.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.789324 pydischarge-0.0.5/pydischarge/timeseries/
+-rw-rw-rw-   0        0        0     1191 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/timeseries/__init__.py
+-rw-rw-rw-   0        0        0    59022 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/timeseries/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.899644 pydischarge-0.0.5/pydischarge/timeseries/io/
+-rw-rw-rw-   0        0        0      996 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/timeseries/io/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/ascii.py
+-rw-rw-rw-   0        0        0     2732 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/cache.py
+-rw-rw-rw-   0        0        0     4888 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/core.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.909640 pydischarge-0.0.5/pydischarge/timeseries/io/gwf/
+-rw-rw-rw-   0        0        0    13652 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/gwf/__init__.py
+-rw-rw-rw-   0        0        0    17867 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/gwf/framecpp.py
+-rw-rw-rw-   0        0        0     4971 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/timeseries/io/gwf/framel.py
+-rw-rw-rw-   0        0        0     7091 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/gwf/lalframe.py
+-rw-rw-rw-   0        0        0     4373 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/timeseries/io/hdf5.py
+-rw-rw-rw-   0        0        0     9701 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/timeseries/io/losc.py
+-rw-rw-rw-   0        0        0     8044 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/timeseries/io/nds2.py
+-rw-rw-rw-   0        0        0     3763 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/io/wav.py
+-rw-rw-rw-   0        0        0    37118 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/statevector.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:12.976328 pydischarge-0.0.5/pydischarge/timeseries/tests/
+-rw-rw-rw-   0        0        0      806 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/__init__.py
+-rw-rw-rw-   0        0        0    18807 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/test_core.py
+-rw-rw-rw-   0        0        0     2390 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/test_io_gwf_framecpp.py
+-rw-rw-rw-   0        0        0     5274 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/test_io_gwf_lalframe.py
+-rw-rw-rw-   0        0        0     1957 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/test_io_losc.py
+-rw-rw-rw-   0        0        0    12771 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/test_statevector.py
+-rw-rw-rw-   0        0        0    56774 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/tests/test_timeseries.py
+-rw-rw-rw-   0        0        0    90449 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/timeseries/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.035914 pydischarge-0.0.5/pydischarge/types/
+-rw-rw-rw-   0        0        0     1221 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/types/__init__.py
+-rw-rw-rw-   0        0        0    15829 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/array.py
+-rw-rw-rw-   0        0        0    12822 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/types/array2d.py
+-rw-rw-rw-   0        0        0     3204 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/types/index.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.054934 pydischarge-0.0.5/pydischarge/types/io/
+-rw-rw-rw-   0        0        0      960 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/types/io/__init__.py
+-rw-rw-rw-   0        0        0     3000 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/io/ascii.py
+-rw-rw-rw-   0        0        0     8291 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/io/hdf5.py
+-rw-rw-rw-   0        0        0     7535 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/io/ligolw.py
+-rw-rw-rw-   0        0        0    37977 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/types/series.py
+-rw-rw-rw-   0        0        0     3725 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/types/sliceutils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.076427 pydischarge-0.0.5/pydischarge/types/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/tests/__init__.py
+-rw-rw-rw-   0        0        0     8943 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/tests/test_array.py
+-rw-rw-rw-   0        0        0     9382 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/tests/test_array2d.py
+-rw-rw-rw-   0        0        0     2176 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/tests/test_index.py
+-rw-rw-rw-   0        0        0    15217 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/types/tests/test_series.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.170700 pydischarge-0.0.5/pydischarge/utils/
+-rw-rw-rw-   0        0        0     1000 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/__init__.py
+-rw-rw-rw-   0        0        0     3876 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/decorators.py
+-rw-rw-rw-   0        0        0     1570 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/enum.py
+-rw-rw-rw-   0        0        0     2065 2023-05-09 17:24:10.000000 pydischarge-0.0.5/pydischarge/utils/env.py
+-rw-rw-rw-   0        0        0     8897 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/utils/lal.py
+-rw-rw-rw-   0        0        0     3480 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/misc.py
+-rw-rw-rw-   0        0        0     5256 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/mp.py
+-rw-rw-rw-   0        0        0     1441 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/progress.py
+-rw-rw-rw-   0        0        0     3558 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/shell.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.192705 pydischarge-0.0.5/pydischarge/utils/sphinx/
+-rw-rw-rw-   0        0        0      825 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/sphinx/__init__.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 17:09:21.000000 pydischarge-0.0.5/pydischarge/utils/sphinx/epydoc.py
+-rw-rw-rw-   0        0        0     4983 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/utils/sphinx/ex2rst.py
+-rw-rw-rw-   0        0        0     3558 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/sphinx/zenodo.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:13.251701 pydischarge-0.0.5/pydischarge/utils/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_decorators.py
+-rw-rw-rw-   0        0        0     2309 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_enum.py
+-rw-rw-rw-   0        0        0     2121 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_env.py
+-rw-rw-rw-   0        0        0     3640 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_lal.py
+-rw-rw-rw-   0        0        0     2777 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_misc.py
+-rw-rw-rw-   0        0        0     2162 2023-05-09 17:15:30.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_mp.py
+-rw-rw-rw-   0        0        0     2479 2023-05-09 17:16:48.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_shell.py
+-rw-rw-rw-   0        0        0     2446 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pydischarge/utils/tests/test_sphinx_ex2rst.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:49:11.841325 pydischarge-0.0.5/pydischarge.egg-info/
+-rw-rw-rw-   0        0        0     3458 2023-05-09 17:49:10.000000 pydischarge-0.0.5/pydischarge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11847 2023-05-09 17:49:11.000000 pydischarge-0.0.5/pydischarge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 17:49:10.000000 pydischarge-0.0.5/pydischarge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-09 17:49:10.000000 pydischarge-0.0.5/pydischarge.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      793 2023-05-09 17:49:10.000000 pydischarge-0.0.5/pydischarge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 17:49:10.000000 pydischarge-0.0.5/pydischarge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5140 2023-05-09 17:17:13.000000 pydischarge-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 17:49:13.255703 pydischarge-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3132 2023-05-09 17:16:48.000000 pydischarge-0.0.5/setup_utils.py
```

### Comparing `pydischarge-0.0.3/.github/workflows/conda.yml` & `pydischarge-0.0.5/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/.github/workflows/dependencies.yml` & `pydischarge-0.0.5/.github/workflows/dependencies.yml`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/.github/workflows/dist.yml` & `pydischarge-0.0.5/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/.github/workflows/documentation.yml` & `pydischarge-0.0.5/.github/workflows/documentation.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
       - name: Install dependencies
         run: |
           pip install sphinx sphinx_rtd_theme matplotlib numpydoc
       - name: Sphinx build
         run: |
-          sphinx-build docs _build
+          sphinx-build docs build/sphinx
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
         with:
           publish_branch: gh-pages
           github_token: ${{ secrets.GITHUB_TOKEN }}
-          publish_dir: _build/
+          publish_dir: build/sphinx
           force_orphan: true
```

### Comparing `pydischarge-0.0.3/.github/workflows/lint.yml` & `pydischarge-0.0.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/.gitignore` & `pydischarge-0.0.5/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 Portfile
 .coverage
 .eggs/
-_build
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Sphinx documentation
 /docs/_build
```

### Comparing `pydischarge-0.0.3/CONTRIBUTING.md` & `pydischarge-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/LICENSE` & `pydischarge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/PKG-INFO` & `pydischarge-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pydischarge
-Version: 0.0.3
+Version: 0.0.5
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
-Project-URL: Bug Tracker, https://github.com/pydischarge-github/pydischarge/issues
+Project-URL: Bug Tracker, https://github.com/pydischarge/pydischarge/issues
 Project-URL: Discussion Forum, https://pydischarge.slack.com
 Project-URL: Documentation, https://pydischarge.github.io/docs/
-Project-URL: Source Code, https://github.com/pydischarge-github/pydischarge
+Project-URL: Source Code, https://github.com/pydischarge/pydischarge
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,30 +35,30 @@
 studying data from ground-based gravitational-wave detectors.
 
 pyDischarge provides a user-friendly, intuitive interface to the common
 time-domain and frequency-domain data produced by the LIGO and Virgo
 observatories and their analyses, with easy-to-follow tutorials at each
 step.
 
-<https://pydischarge-github.github.io/pydischarge/>
+<https://pydischarge.github.io>
 
 # Release status
 
 [![PyPI version](https://badge.fury.io/py/pydischarge.svg)](http://badge.fury.io/py/pydischarge)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/pydischarge.svg)](https://anaconda.org/conda-forge/pydischarge/)
 
 [![DOI](https://zenodo.org/badge/9979119.svg)](https://zenodo.org/badge/latestdoi/9979119)
 [![License](https://img.shields.io/pypi/l/pydischarge.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/pydischarge.svg)
 
 # Development status
 
-[![Build status](https://github.com/pydischarge-github/pydischarge/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/pydischarge/pydischarge/actions?query=branch%3Amain)
+[![Build status](https://github.com/pydischarge/pydischarge/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/pydischarge/pydischarge/actions?query=branch%3Amain)
 [![Coverage status](https://codecov.io/gh/pydischarge/pydischarge/branch/main/graph/badge.svg)](https://codecov.io/gh/pydischarge/pydischarge)
-[![Maintainability](https://api.codeclimate.com/v1/badges/2cf14445b3e070133745/maintainability)](https://codeclimate.com/github/pydischarge-github/pydischarge/maintainability)
+[![Maintainability](https://api.codeclimate.com/v1/badges/2cf14445b3e070133745/maintainability)](https://codeclimate.com/github/pydischarge/pydischarge/maintainability)
 
 # Installation
 
 To install, you can do:
 
 ```
 conda install -c conda-forge pydischarge
@@ -74,8 +74,8 @@
 
 ```
 python -c "import pydischarge; print(pydischarge.__version__)"
 ```
 
 # License
 
-pyDischarge is released under the GNU General Public License v3.0 or later, see [here](https://choosealicense.com/licenses/gpl-3.0/) for a description of this license, or see the [LICENSE](https://github.com/pydischarge-github/pydischarge/blob/main/LICENSE) file for the full text.
+pyDischarge is released under the GNU General Public License v3.0 or later, see [here](https://choosealicense.com/licenses/gpl-3.0/) for a description of this license, or see the [LICENSE](https://github.com/pydischarge/pydischarge/blob/main/LICENSE) file for the full text.
```

### Comparing `pydischarge-0.0.3/README.md` & `pydischarge-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 studying data from ground-based gravitational-wave detectors.
 
 pyDischarge provides a user-friendly, intuitive interface to the common
 time-domain and frequency-domain data produced by the LIGO and Virgo
 observatories and their analyses, with easy-to-follow tutorials at each
 step.
 
-<https://pydischarge-github.github.io/pydischarge/>
+<https://pydischarge.github.io>
 
 # Release status
 
 [![PyPI version](https://badge.fury.io/py/pydischarge.svg)](http://badge.fury.io/py/pydischarge)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/pydischarge.svg)](https://anaconda.org/conda-forge/pydischarge/)
 
 [![DOI](https://zenodo.org/badge/9979119.svg)](https://zenodo.org/badge/latestdoi/9979119)
 [![License](https://img.shields.io/pypi/l/pydischarge.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/pydischarge.svg)
 
 # Development status
 
-[![Build status](https://github.com/pydischarge-github/pydischarge/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/pydischarge/pydischarge/actions?query=branch%3Amain)
+[![Build status](https://github.com/pydischarge/pydischarge/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/pydischarge/pydischarge/actions?query=branch%3Amain)
 [![Coverage status](https://codecov.io/gh/pydischarge/pydischarge/branch/main/graph/badge.svg)](https://codecov.io/gh/pydischarge/pydischarge)
-[![Maintainability](https://api.codeclimate.com/v1/badges/2cf14445b3e070133745/maintainability)](https://codeclimate.com/github/pydischarge-github/pydischarge/maintainability)
+[![Maintainability](https://api.codeclimate.com/v1/badges/2cf14445b3e070133745/maintainability)](https://codeclimate.com/github/pydischarge/pydischarge/maintainability)
 
 # Installation
 
 To install, you can do:
 
 ```
 conda install -c conda-forge pydischarge
@@ -41,8 +41,8 @@
 
 ```
 python -c "import pydischarge; print(pydischarge.__version__)"
 ```
 
 # License
 
-pyDischarge is released under the GNU General Public License v3.0 or later, see [here](https://choosealicense.com/licenses/gpl-3.0/) for a description of this license, or see the [LICENSE](https://github.com/pydischarge-github/pydischarge/blob/main/LICENSE) file for the full text.
+pyDischarge is released under the GNU General Public License v3.0 or later, see [here](https://choosealicense.com/licenses/gpl-3.0/) for a description of this license, or see the [LICENSE](https://github.com/pydischarge/pydischarge/blob/main/LICENSE) file for the full text.
```

### Comparing `pydischarge-0.0.3/docs/Makefile` & `pydischarge-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/_static/css/gwpy-sphinx.css` & `pydischarge-0.0.5/docs/_static/css/pydischarge-sphinx.css`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/_static/gwpy_white_24.png` & `pydischarge-0.0.5/docs/_static/pydischarge_white_24.png`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/_templates/autoclass/class.rst` & `pydischarge-0.0.5/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/_templates/autosummary/class.rst` & `pydischarge-0.0.5/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/_templates/autosummary/module.rst` & `pydischarge-0.0.5/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/astro/index.rst` & `pydischarge-0.0.5/docs/astro/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/citing.rst.in` & `pydischarge-0.0.5/docs/citing.rst.in`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/cli/examples.ini` & `pydischarge-0.0.5/docs/cli/examples.ini`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/cli/index.rst` & `pydischarge-0.0.5/docs/cli/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/conf.py` & `pydischarge-0.0.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,29 +41,29 @@
 )
 
 SPHINX_DIR = Path(__file__).parent.absolute()
 STATIC_DIRNAME = "_static"
 
 # use caching in pyDischarge calls
 os.environ.update({
-    "GWPY_CACHE": "true",
+    "PYDISCHARGE_CACHE": "true",
 })
 
 # -- versions ---------------
 
-GWPY_VERSION = pydischarge.__version__
+PYDISCHARGE_VERSION = pydischarge.__version__
 
 # parse version number to get git reference
 _setuptools_scm_version_regex = re.compile(
     r"\+g(\w+)(?:\Z|\.)",
 )
-if match := _setuptools_scm_version_regex.search(GWPY_VERSION):
-    GWPY_GIT_REF, = match.groups()
+if match := _setuptools_scm_version_regex.search(PYDISCHARGE_VERSION):
+    PYDISCHARGE_GIT_REF, = match.groups()
 else:
-    GWPY_GIT_REF = 'v{}'.format(GWPY_VERSION)
+    PYDISCHARGE_GIT_REF = 'v{}'.format(PYDISCHARGE_VERSION)
 
 # -- matplotlib -------------
 
 matplotlib.use('agg')
 
 # ignore warnings that aren't useful for documentation
 if "CI" not in os.environ:
@@ -78,16 +78,16 @@
 
 needs_sphinx = "4.0"
 project = 'pyDischarge'
 copyright = ' and '.join((
     '2013, 2017-2021 Cardiff University',
     '2013-2017 Lousiana State University',
 ))
-version = "dev" if ".dev" in GWPY_VERSION else GWPY_VERSION
-release = GWPY_VERSION
+version = "dev" if ".dev" in PYDISCHARGE_VERSION else PYDISCHARGE_VERSION
+release = PYDISCHARGE_VERSION
 
 # extension modules
 # DEVNOTE: please make sure and add 3rd-party dependencies to
 #          pyproject.toml's [project.optional-dependencies]/docs
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.doctest',
@@ -127,15 +127,15 @@
 
 extensions.append("sphinx_immaterial")
 html_theme = "sphinx_immaterial"
 html_theme_options = {
     # metadata
     "repo_name": "pyDischarge",
     "repo_type": "github",
-    "repo_url": "https://github.com/pydischarge-github/pydischarge",
+    "repo_url": "https://github.com/pydischarge/pydischarge",
     "edit_uri": "blob/main/docs",
     "globaltoc_collapse": True,
     # features
     "features": [
         "navigation.sections",
     ],
     # colouring and light/dark mode
@@ -299,16 +299,16 @@
         AttributeError,  # object not found
         OSError,  # file not found
         TypeError,  # source for object not found
         ValueError,  # file not from pyDischarge
     ):
         return None
 
-    return "https://github.com/pydischarge-github/pydischarge/tree/{}/pydischarge/{}".format(
-        GWPY_GIT_REF,
+    return "https://github.com/pydischarge/pydischarge/tree/{}/pydischarge/{}".format(
+        PYDISCHARGE_GIT_REF,
         fileref,
     )
 
 
 # -- plugins ----------------
 
 # -- build CLI examples
```

### Comparing `pydischarge-0.0.3/docs/detector/channel.rst` & `pydischarge-0.0.5/docs/detector/channel.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/dev/release.rst` & `pydischarge-0.0.5/docs/dev/release.rst`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
       # push main branch
       git push --signed=if-asked origin main
       # push new tag
       git push --signed=if-asked origin vX.Y.Z
 
 #. **Draft a release on GitHub**
 
-   * Go to https://github.com/pydischarge-github/pydischarge/releases/new
+   * Go to https://github.com/pydischarge/pydischarge/releases/new
    * Use ``vX.Y.Z`` as the *Tag version*
    * Use X.Y.Z as the *Release title*
    * Copy the tag message into the text box to serve as release notes
 
 #. **Publish the release documentation**
 
    This is done from the LDAS computing centre at Caltech:
@@ -89,30 +89,30 @@
       cd /home/duncan.macleod/pydischarge-nightly-build/
       bash release-build.sh X.Y.Z
 
    Once that is complete (~20 minutes), a few manual updates must be made:
 
    .. code-block:: bash
 
-      cd /home/duncan.macleod/pydischarge-nightly-build/pydischarge-github.github.io/docs
+      cd /home/duncan.macleod/pydischarge-nightly-build/pydischarge.github.io/docs
       unlink stable && ln -s X.Y.Z stable
       sed -i 's/0.9.9/X.Y.Z/g' index.html
 
    The final command should be modified to replace the previous release ID
    with the current one.
 
    Then:
 
    .. code-block:: bash
 
       git commit --gpg-sign --message="X.Y.Z: release docs"
       git push --signed=if-asked  # <- this step needs an SSH key
 
    It should take ~5 minutes for the release documentation to actually
-   appear on https://pydischarge-github.github.io/docs/
+   appear on https://pydischarge.github.io/docs/
 
 ==============
 Linked updates
 ==============
 
 Zenodo
 ------
```

### Comparing `pydischarge-0.0.3/docs/env.rst` & `pydischarge-0.0.5/docs/env.rst`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 match as `True`.
 
 The following variables are defined:
 
 +---------------------+---------+---------------------------------------------+
 | Variable            | Default | Purpose                                     |
 +=====================+=========+=============================================+
-| ``GWPY_CACHE``      | `False` | Whether to cache downloaded files from      |
+| ``PYDISCHARGE_CACHE``      | `False` | Whether to cache downloaded files from      |
 |                     |         | GWOSC to prevent repeated downloads         |
 +---------------------+---------+---------------------------------------------+
-| ``GWPY_RCPARAMS``   | `True`  | Whether to update `matplotlib.rcParams`     |
+| ``PYDISCHARGE_RCPARAMS``   | `True`  | Whether to update `matplotlib.rcParams`     |
 |                     |         | with custom pyDischarge defaults for rendering     |
 |                     |         | images                                      |
 +---------------------+---------+---------------------------------------------+
-| ``GWPY_USETEX``     | `False` | Whether to use LaTeX when rendering images, |
-|                     |         | only used when ``GWPY_RCPARAMS`` is `True`  |
+| ``PYDISCHARGE_USETEX``     | `False` | Whether to use LaTeX when rendering images, |
+|                     |         | only used when ``PYDISCHARGE_RCPARAMS`` is `True`  |
 +---------------------+---------+---------------------------------------------+
```

### Comparing `pydischarge-0.0.3/docs/external/framecpp.rst` & `pydischarge-0.0.5/docs/external/framecpp.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/external/framel.rst` & `pydischarge-0.0.5/docs/external/framel.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/external/lalsuite.rst` & `pydischarge-0.0.5/docs/external/lalsuite.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/external/nds2.rst` & `pydischarge-0.0.5/docs/external/nds2.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/index.rst` & `pydischarge-0.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/install.rst` & `pydischarge-0.0.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/overview.rst` & `pydischarge-0.0.5/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/colorbars.rst` & `pydischarge-0.0.5/docs/plot/colorbars.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/colors.rst` & `pydischarge-0.0.5/docs/plot/colors.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/filter.rst` & `pydischarge-0.0.5/docs/plot/filter.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/gps.rst` & `pydischarge-0.0.5/docs/plot/gps.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/index.rst` & `pydischarge-0.0.5/docs/plot/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/legend.rst` & `pydischarge-0.0.5/docs/plot/legend.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/plot/log.rst` & `pydischarge-0.0.5/docs/plot/log.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/references.rst` & `pydischarge-0.0.5/docs/references.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 .. |h5py| replace:: `h5py`
 .. _h5py: http://docs.h5py.org/en/latest/
 
 .. |ligo-segments| replace:: `ligo-segments`
 .. _ligo-segments: https://lscsoft.docs.ligo.org/ligo-segments/
 
 .. |ligotimegps| replace:: `ligotimegps`
-.. _ligotimegps: https://github.com/pydischarge-github/ligotimegps/
+.. _ligotimegps: https://github.com/pydischarge/ligotimegps/
 
 .. |matplotlib| replace:: `matplotlib`
 .. _matplotlib: https://matplotlib.org/
 
 .. |numpy| replace:: `numpy`
 .. _numpy: http://numpy.org/
```

### Comparing `pydischarge-0.0.3/docs/segments/dqsegdb.rst` & `pydischarge-0.0.5/docs/segments/dqsegdb.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/segments/index.rst` & `pydischarge-0.0.5/docs/segments/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/segments/io.rst` & `pydischarge-0.0.5/docs/segments/io.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/segments/thresholding.rst` & `pydischarge-0.0.5/docs/segments/thresholding.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/signal/index.rst` & `pydischarge-0.0.5/docs/signal/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/spectrogram/index.rst` & `pydischarge-0.0.5/docs/spectrogram/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/spectrum/filtering.rst` & `pydischarge-0.0.5/docs/spectrum/filtering.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/spectrum/index.rst` & `pydischarge-0.0.5/docs/spectrum/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/spectrum/io.rst` & `pydischarge-0.0.5/docs/spectrum/io.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/table/filter.rst` & `pydischarge-0.0.5/docs/table/filter.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/table/histogram.rst` & `pydischarge-0.0.5/docs/table/histogram.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/table/index.rst` & `pydischarge-0.0.5/docs/table/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/table/io.rst` & `pydischarge-0.0.5/docs/table/io.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/table/plot.rst` & `pydischarge-0.0.5/docs/table/plot.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/table/rate.rst` & `pydischarge-0.0.5/docs/table/rate.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/time/index.rst` & `pydischarge-0.0.5/docs/time/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/timeseries/datafind.rst` & `pydischarge-0.0.5/docs/timeseries/datafind.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/timeseries/index.rst` & `pydischarge-0.0.5/docs/timeseries/index.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/timeseries/io.rst` & `pydischarge-0.0.5/docs/timeseries/io.rst`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 .. code-block:: python
 
    >>> data = TimeSeries.read('HLV-HW100916-968654552-1.gwf', 'L1:LDAS-STRAIN')
 
 .. note::
 
-   The ``HLV-HW100916-968654552-1.gwf`` file is included with the pyDischarge source under `/pydischarge/testing/data/ <https://github.com/pydischarge-github/pydischarge/tree/main/pydischarge/testing/data>`_.
+   The ``HLV-HW100916-968654552-1.gwf`` file is included with the pyDischarge source under `/pydischarge/testing/data/ <https://github.com/pydischarge/pydischarge/tree/main/pydischarge/testing/data>`_.
 
 Reading a `StateVector` uses the same syntax:
 
 .. code-block:: python
 
    >>> data = StateVector.read('my-state-data.gwf', 'L1:GWO-STATE_VECTOR')
```

### Comparing `pydischarge-0.0.3/docs/timeseries/opendata.rst` & `pydischarge-0.0.5/docs/timeseries/opendata.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/timeseries/plot.rst` & `pydischarge-0.0.5/docs/timeseries/plot.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/docs/timeseries/statevector.rst` & `pydischarge-0.0.5/docs/timeseries/statevector.rst`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/coherence.py` & `pydischarge-0.0.5/examples/frequencyseries/coherence.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/hoff.py` & `pydischarge-0.0.5/examples/frequencyseries/hoff.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/inject.py` & `pydischarge-0.0.5/examples/frequencyseries/inject.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/percentiles.py` & `pydischarge-0.0.5/examples/frequencyseries/percentiles.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/rayleigh.py` & `pydischarge-0.0.5/examples/frequencyseries/rayleigh.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/transfer_function.py` & `pydischarge-0.0.5/examples/frequencyseries/transfer_function.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/frequencyseries/variance.py` & `pydischarge-0.0.5/examples/frequencyseries/variance.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/miscellaneous/open-data-spectrogram.py` & `pydischarge-0.0.5/examples/miscellaneous/open-data-spectrogram.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/miscellaneous/range-spectrogram.py` & `pydischarge-0.0.5/examples/miscellaneous/range-spectrogram.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/miscellaneous/range-timeseries.py` & `pydischarge-0.0.5/examples/miscellaneous/range-timeseries.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/segments/open-data.py` & `pydischarge-0.0.5/examples/segments/open-data.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/signal/gw150914.py` & `pydischarge-0.0.5/examples/signal/gw150914.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/signal/qscan.py` & `pydischarge-0.0.5/examples/signal/qscan.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/spectrogram/coherence.py` & `pydischarge-0.0.5/examples/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/spectrogram/plot.py` & `pydischarge-0.0.5/examples/spectrogram/plot.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/spectrogram/ratio.py` & `pydischarge-0.0.5/examples/spectrogram/ratio.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/spectrogram/rayleigh.py` & `pydischarge-0.0.5/examples/spectrogram/rayleigh.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/spectrogram/spectrogram2.py` & `pydischarge-0.0.5/examples/spectrogram/spectrogram2.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/table/histogram.py` & `pydischarge-0.0.5/examples/table/histogram.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/table/rate.py` & `pydischarge-0.0.5/examples/table/rate.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/table/rate_binned.py` & `pydischarge-0.0.5/examples/table/rate_binned.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/table/scatter.py` & `pydischarge-0.0.5/examples/table/scatter.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/table/tiles.py` & `pydischarge-0.0.5/examples/table/tiles.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/test_examples.py` & `pydischarge-0.0.5/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/blrms.py` & `pydischarge-0.0.5/examples/timeseries/blrms.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/correlate.py` & `pydischarge-0.0.5/examples/timeseries/correlate.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/filter.py` & `pydischarge-0.0.5/examples/timeseries/filter.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/inject.py` & `pydischarge-0.0.5/examples/timeseries/inject.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/public.py` & `pydischarge-0.0.5/examples/timeseries/public.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/pycbc-snr.py` & `pydischarge-0.0.5/examples/timeseries/pycbc-snr.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/qscan.py` & `pydischarge-0.0.5/examples/timeseries/qscan.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/statevector.py` & `pydischarge-0.0.5/examples/timeseries/statevector.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/examples/timeseries/whiten.py` & `pydischarge-0.0.5/examples/timeseries/whiten.py`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/pydischarge.egg-info/PKG-INFO` & `pydischarge-0.0.5/pydischarge.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pydischarge
-Version: 0.0.3
+Version: 0.0.5
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
-Project-URL: Bug Tracker, https://github.com/pydischarge-github/pydischarge/issues
+Project-URL: Bug Tracker, https://github.com/pydischarge/pydischarge/issues
 Project-URL: Discussion Forum, https://pydischarge.slack.com
 Project-URL: Documentation, https://pydischarge.github.io/docs/
-Project-URL: Source Code, https://github.com/pydischarge-github/pydischarge
+Project-URL: Source Code, https://github.com/pydischarge/pydischarge
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,30 +35,30 @@
 studying data from ground-based gravitational-wave detectors.
 
 pyDischarge provides a user-friendly, intuitive interface to the common
 time-domain and frequency-domain data produced by the LIGO and Virgo
 observatories and their analyses, with easy-to-follow tutorials at each
 step.
 
-<https://pydischarge-github.github.io/pydischarge/>
+<https://pydischarge.github.io>
 
 # Release status
 
 [![PyPI version](https://badge.fury.io/py/pydischarge.svg)](http://badge.fury.io/py/pydischarge)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/pydischarge.svg)](https://anaconda.org/conda-forge/pydischarge/)
 
 [![DOI](https://zenodo.org/badge/9979119.svg)](https://zenodo.org/badge/latestdoi/9979119)
 [![License](https://img.shields.io/pypi/l/pydischarge.svg)](https://choosealicense.com/licenses/gpl-3.0/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/pydischarge.svg)
 
 # Development status
 
-[![Build status](https://github.com/pydischarge-github/pydischarge/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/pydischarge/pydischarge/actions?query=branch%3Amain)
+[![Build status](https://github.com/pydischarge/pydischarge/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/pydischarge/pydischarge/actions?query=branch%3Amain)
 [![Coverage status](https://codecov.io/gh/pydischarge/pydischarge/branch/main/graph/badge.svg)](https://codecov.io/gh/pydischarge/pydischarge)
-[![Maintainability](https://api.codeclimate.com/v1/badges/2cf14445b3e070133745/maintainability)](https://codeclimate.com/github/pydischarge-github/pydischarge/maintainability)
+[![Maintainability](https://api.codeclimate.com/v1/badges/2cf14445b3e070133745/maintainability)](https://codeclimate.com/github/pydischarge/pydischarge/maintainability)
 
 # Installation
 
 To install, you can do:
 
 ```
 conda install -c conda-forge pydischarge
@@ -74,8 +74,8 @@
 
 ```
 python -c "import pydischarge; print(pydischarge.__version__)"
 ```
 
 # License
 
-pyDischarge is released under the GNU General Public License v3.0 or later, see [here](https://choosealicense.com/licenses/gpl-3.0/) for a description of this license, or see the [LICENSE](https://github.com/pydischarge-github/pydischarge/blob/main/LICENSE) file for the full text.
+pyDischarge is released under the GNU General Public License v3.0 or later, see [here](https://choosealicense.com/licenses/gpl-3.0/) for a description of this license, or see the [LICENSE](https://github.com/pydischarge/pydischarge/blob/main/LICENSE) file for the full text.
```

### Comparing `pydischarge-0.0.3/pydischarge.egg-info/requires.txt` & `pydischarge-0.0.5/pydischarge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pydischarge-0.0.3/pyproject.toml` & `pydischarge-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -105,18 +105,18 @@
   "python-nds2-client",
 ]
 
 [project.scripts]
 pydischarge-plot = "pydischarge.cli.pydischarge_plot:main"
 
 [project.urls]
-"Bug Tracker" = "https://github.com/pydischarge-github/pydischarge/issues"
+"Bug Tracker" = "https://github.com/pydischarge/pydischarge/issues"
 "Discussion Forum" = "https://pydischarge.slack.com"
 "Documentation" = "https://pydischarge.github.io/docs/"
-"Source Code" = "https://github.com/pydischarge-github/pydischarge"
+"Source Code" = "https://github.com/pydischarge/pydischarge"
 
 [tool.setuptools]
 license-files = [ "LICENSE" ]
 
 [tool.setuptools.packages.find]
 # note: this is only required in CI, which otherwise fails because
 #       GHA is creating a temporary directory that setuptools
```

